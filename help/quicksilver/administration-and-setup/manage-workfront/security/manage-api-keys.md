---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Gerenciar chaves de API
description: Para minimizar as vulnerabilidades de segurança da API, os administradores do Adobe Workfront podem gerenciar as Chaves de API usadas para permitir que os aplicativos acessem o Workfront em nome de um usuário.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 1176d899-0585-430d-87f2-0823bda2f1be
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: aeb471fd63269d30a675e44fe1a47db6141eb9ed
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 17%

---

# Gerenciar chaves de API

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->



>[!IMPORTANT]
>
>A Workfront não recomenda mais o uso das chaves de API ou do ponto de acesso `/login`. Em vez disso, use um dos seguintes métodos de autenticação:
>
>* Autenticação do servidor com JWT
>* Autenticação de usuário com OAuth2
>
>Para obter instruções sobre como configurar esses métodos de autenticação, consulte [Criar aplicativos OAuth2 para integrações do Workfront](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).
>
>Para obter instruções sobre como usar a autenticação de servidor no Workfront, consulte [Configurar e usar os aplicativos OAuth2 personalizados da sua organização usando o fluxo JWT](/help/quicksilver/wf-api/api/oauth-app-jwt-flow.md).
>
>Para obter instruções sobre como usar a autenticação de usuário no Workfront, consulte [Configurar e usar os aplicativos OAuth2 personalizados de sua organização usando o fluxo de código de autorização](/help/quicksilver/wf-api/api/oauth-app-code-token-flow.md).

Para minimizar as vulnerabilidades de segurança da API, os administradores do Adobe Workfront podem gerenciar as Chaves de API usadas para permitir que os aplicativos acessem o Workfront em nome de um usuário.

Você pode redefinir ou remover sua Chave de API do administrador atual, configurar as Chaves de API para expirar e remover as Chaves de API para todos os usuários.

Exemplos de aplicativos que usam a API do Workfront são:

* Integrações de documentos, como Dropbox, Google Drive e Workfront DAM
* aplicativos móveis Workfront

>[!IMPORTANT]
>
>Ao redefinir ou remover uma Chave de API, qualquer aplicativo que use a API do Workfront e seja autenticado no Workfront por meio dessa Chave de API deve ser reconfigurado para recuperar o acesso ao Workfront.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Padrão</p><p>Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Chaves de API do Workfront

Cada usuário no Workfront tem uma chave de API exclusiva. Essa chave é gerada com base no usuário no momento em que o usuário acessa uma integração que aproveita a API do Workfront (como o aplicativo móvel Workfront ou uma integração de documentos).

>[!NOTE]
>
> As chaves de API geradas no ambiente de produção são copiadas para o ambiente de Pré-visualização durante a atualização semanal. Quaisquer chaves de API geradas no ambiente de Pré-visualização serão substituídas pelas chaves de API de produção durante a atualização semanal.

Os administradores do Workfront também têm uma chave de API exclusiva. Quando um aplicativo usa uma chave de API de administrador para acessar o Workfront, ele tem acesso de administrador ao Workfront.

## Gerenciar uma chave de API do administrador

Você pode gerar, redefinir ou remover a Chave de API da conta de usuário administrador.

{{step-1-to-setup}}

1. Clique em **Sistema >** **Informações do Cliente.**
1. (Condicional) Execute uma das seguintes ações:

   Para gerar uma Chave de API: Na seção **Configurações da Chave de API**, clique em **Gerar Chave de API**.

   Ou\
   Para redefinir uma Chave de API: Na seção **Configurações da Chave de API**, clique em **Redefinir** e depois em **Redefinir.**

   Ou

   Para remover a Chave de API: Na seção **Configurações da Chave de API**, clique em **Remover** e depois em **Remover**.

<!--

   Remove me October 2026

## Generate an API Key for Non-Admin Users

You can generate and manage API Keys for users in roles other than Workfront administrator.

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

1. (Conditional) If your organization uses Single Sign-On (SSO) access management, temporarily disable the option requiring SSO authentication.

   {{step-1-to-setup}} 
   
   1. Expand **System**, then click **Single Sign-on (SSO)**. 
   1. In the **Type** field, select the type of SSO your organization uses.
   1. With the type selected, scroll down and clear the **Enable** checkbox. 
      ![Enable SSO](assets/sysadmin-security-sso-disable-31620-350x320.png)  
   1. Click **Save**.


1. In the address bar of a browser, enter the following API call:

   `<domain>`.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&username=**username**&password=**password**&method=PUT

   Replace `<domain>` with your Workfront domain name, and username and password with the user's Workfront credentials.

1. (Conditional) Enable the option requiring SSO authentication if you disabled it in Step 1.

   {{step-1-to-setup}}
   
   1. Expand **System**, then click **Single Sign-on (SSO)**.
   
   1. Select your SSO method in the **Type** drop down menu.
   1. Check the checkbox requiring SSO authentication.

   -->

## Configurar quando as chaves de API expiram

Você pode configurar as Chaves de API para expirarem para todos os usuários em seu sistema. Quando a chave de API de um usuário expira, o usuário deve se autenticar novamente em qualquer aplicativo que use a API do Workfront para acessar o Workfront. Você pode alterar a frequência com que as Chaves de API expiram. Você também pode configurar se as Chaves de API expiram quando a senha de um usuário expira.

{{step-1-to-setup}}

1. Clique em **Sistema** > **Informações do cliente**.
1. Na área **Configurações da Chave de API**, na lista suspensa **Após a criação**, as **chaves de API expiram em**, selecione o período em que deseja que as chaves de API expirem.

   Ao alterar essa opção, o novo período começa a partir do momento em que você fez a alteração. Por exemplo, se você alterar esta opção de *1 mês* para *6 meses*, as Chaves de API expirarão em 6 meses a partir do momento em que você fizer a alteração.

   Por padrão, as Chaves de API expiram a cada mês.

1. Para configurar as Chaves de API para expirarem no momento em que as senhas dos usuários expirarem, habilite **Remover chave de API quando a senha de um usuário expirar**.

   Por padrão, essa opção não está ativada.

   Para obter informações sobre como configurar senhas de usuário para expirar, consulte [Configurar preferências de segurança do sistema](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

1. Clique em **Salvar**.

## Remover as chaves de API de todos os usuários

Se você estiver preocupado com uma violação de segurança específica em relação ao seu sistema Workfront, poderá remover as Chaves de API simultaneamente para todos os usuários.

>[!IMPORTANT]
>
>Remover as chaves de API de todos os usuários invalida TODAS as chaves de API de todos os usuários do sistema. Essa ação causará falha em todas as suas integrações no Workfront até que você gere uma nova Chave de API no Workfront e atualize todas as suas integrações.

{{step-1-to-setup}}

1. Expanda **Sistema** e clique em **Informações do cliente**.

1. Na área **Configurações da Chave de API**, clique em **Remover todas as chaves de API** e em **Remover** **Tudo**.

<!--

Remove me October 2026

## Restricting API logins with an X.509 certificate

>[!IMPORTANT]
>
>The procedure described in this section applies only to organizations that have not yet been onboarded to the Adobe Business Platform. Logging in to Workfront through the Workfront API is not available if your organization has been onboarded to the Adobe Business Platform.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

Third-party applications can communicate with Workfront through the API. To increase the security of your Workfront site, you can configure Workfront to restrict API login requests by uploading an X.509 certificate to Workfront. Once enabled, all login requests through the API must include a client certificate in addition to username and password.

* [Obtain the X.509 certificate](#obtain-the-x-509-certificate) 
* [Upload the certificate to Workfront](#upload-the-certificate-to-workfront) 
* [Verify API login calls are restricted](#verify-api-login-calls-are-restricted)

### Obtain the X.509 certificate {#obtain-the-x-509-certificate}

Obtain a valid X.509 certificate from a trusted Certificate Authority (such as Verisign), and save it to a temporary location on your workstation. 

### Upload the certificate to Workfront {#upload-the-certificate-to-workfront}

After you have obtained the X.509 certificate from your Certificate Authority, you need to upload it to Workfront.

1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).  

1. Expand **System**, then click **Customer Info**.

1. In the **API Key Settings** area, select **Require X.509 Certificate for API logins**.
1. Click **Change Certificate**.
1. On your workstation, browse to and select the X.509 certificate that you previously downloaded.
1. (Optional) Click **View Details** next to the certificate name to view the following details about the certificate:

   * Subject Common Name
   * Subject Organization
   * Subject Organization Unit
   * Issuer Common Name
   * Issuer Organization
   * Issuer Organization Unit
   * Serial Number
   * Issue Date
   * Expiration Date

1. Click **Save**. 

### Verify API login calls are restricted {#verify-api-login-calls-are-restricted}

Prior to configuring your instance of Workfront to require an X.509 certificate, perform an API request to the `/login` endpoint using valid username and password parameters. You will receive a 200 response that contains a sessionID.

After making the X.509 certificate a requirement via the customer info page in your instance of Workfront, make another login attempt. This time you will receive a 500 error response with the following message: "Untrusted request. Please contact your system administrator and attach certificate."

After confirming that the X.509 certificate is required, perform the same login request with an additional parameter for apiCertificate set to the value of your certificate. If this operation was performed correctly you will receive a 200 response that contains a valid sessionID.

-->
