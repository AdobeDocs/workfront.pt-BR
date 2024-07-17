---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: Configurar Logon Único para  [!DNL Workfront Proof]  usuários
description: Se você tiver o plano Select ou Premium, poderá fornecer o recurso de Logon Único (SSO) que permite usar o nome de usuário e a senha da sua organização existente para acessar sua conta  [!DNL Workfront Proof] .
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 52ac1919-1821-424f-89f8-72865b236e4e
source-git-commit: 007a603ef1df2a02959d7fb623ac784bf5b9cb80
workflow-type: tm+mt
source-wordcount: '1225'
ht-degree: 0%

---

# Configurar Logon Único para [!DNL Workfront Proof] usuários

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

Se você tiver o plano Select ou Premium, poderá fornecer o recurso de Logon Único (SSO) que permite usar o nome de usuário e a senha da sua organização existente para acessar sua conta do [!DNL Workfront Proof].

Isso significa que você autenticará em seu próprio sistema de logon, não na página de logon do [!DNL Workfront Proof].

>[!NOTE]
>
>É necessário ter um subdomínio ou domínio personalizado configurado em sua conta do [!DNL Workfront Proof] para habilitar o SAML. A configuração de subdomínios personalizados é livre. Consulte [Identidade Visual](https://support.workfront.com/hc/en-us/sections/115000921208-Branding) para obter mais informações. Você pode ler mais sobre domínios totalmente personalizados em nosso [Marcar o [!DNL Workfront Proof] site - avançado](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

## Habilitando SSO em [!DNL Workfront Proof]

A funcionalidade Logon Único pode ser habilitada na guia [!UICONTROL Logon Único] das [!UICONTROL Configurações de conta] e se aplicará a todos os usuários da sua conta [!DNL Workfront Proof]. Consulte [Configurações da conta](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) para obter mais informações.

## ID da entidade

Como um Provedor de serviços, publicamos nossa ID de entidade aqui:

[https://yoursubdomain.proofhq.com/saml/module.php/saml/sp/metadata.php/phq](https://yoursubdomain.proofhq.com/saml/module.php/saml/sp/metadata.php/phq) (onde &quot;seusubdomínio&quot; é o subdomínio de sua conta)

[!DNL Workfront Proof] exige o endereço de email do usuário como seu identificador exclusivo, que pode ser passado como um dos seguintes atributos:

* urn:mace:dir:attribute-def:emailAddress
* http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress
* http://schemas.xmlsoap.org/claims/EmailAddress
* urn:oid:0.9.2342.19200300.100.1.3
* http://axschema.org/contact/email
* openid.sreg.email
* email
* email
* emailAddress

Para configurar o SSO:

1. Abra a guia **[!UICONTROL Logon Único]** (1).
1. Insira a **URL do SSO** (2).
Este é o link para seu servidor SSO (por exemplo, **https://sso.mycompany.com/opensso**).

1. Insira a **URL de Logon** (3).
Este é o URL que será chamado para redirecionar os usuários para o seu provedor de identidade.

1. Este não é um URL real que você digita no navegador, mas um terminal que processará as informações que enviamos para apresentar a tela de login.

Insira a **URL de logoff** (4).
Este é o URL ao qual você retornará depois de fazer logoff, por exemplo

**https://www.yourcompany.com/services/logout.asp**

1. Insira a **Impressão digital do certificado** (5).
1. A impressão digital SHA1 do certificado SAML fornecido pelo Provedor de Identidade SAML.
1. Certifique-se de incluir as informações principais definindo isso no Provedor de identidade.
1. Alternar **SSO** para **[!UICONTROL Habilitado]** (6).
Quando o SSO estiver habilitado, você e outros usuários da sua conta farão logon usando seu próprio mecanismo de autenticação. Isso significa que quando os usuários acessarem a tela de logon da conta do [!DNL Workfront Proof] (por exemplo, **yourcompany.proofhq.com/login**), será exibida a janela de transferência para a sua própria página de logon de autenticação.

1. (Opcional) Habilitar **Provisionar usuários automaticamente** (7).
Quando esta opção estiver habilitada, as contas de usuário serão criadas automaticamente para pessoas que não têm seus próprios perfis do [!DNL Workfront Proof], mas acessarão sua conta do [!DNL Workfront Proof] usando suas credenciais de Logon Único. Isso será ativado somente quando o limite do usuário ainda não for atingido em sua conta.

1. Os novos usuários provisionados terão as permissões de perfil de gerente atribuídas por padrão. Se precisar de mais informações, consulte [Perfis de Permissões de Prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

![Habilitar_SSO_SAML_2.0.png](assets/enable-sso-saml-2.0-350x236.png)

## Ativação do SSO para contas satélite

Quando você tem contas satélite conectadas à sua conta hub, é possível administrá-las a partir do nível da conta hub.

Single Sign-On é um recurso Select e Premium, portanto, o Single Sign-On só pode ser ativado em satélites que estejam nos planos Select e Premium.

1. Clique em **[!UICONTROL Configurações]** > **[!UICONTROL Configurações de conta]** (1).

1. Clique na conta satélite no menu suspenso (2).
1. Abra a guia **[!UICONTROL Logon Único]** (3).
1. Comece a editar a configuração de SSO (4).
1. ![Enabling_SSO_-_Satellite_Account.png](assets/enabling-sso---satellite-account-350x266.png)
Aqui você terá dois métodos (5) de configuração:

1. **Herdado:** SSO com a configuração retirada da sua conta de hub.
Se um usuário acessar [!DNL Workfront Proof] por meio da **página de logon padrão** ([https://www.proofhq.com/login](https://www.proofhq.com/login)), haverá **dois níveis de autorização**: primeiro, um usuário é solicitado a fazer logon usando os dados de acesso do [!DNL Workfront Proof] (email e senha); em seguida, o usuário é transferido por meio de uma janela SSO para a página de logon SSO.
Portanto, com o serviço SSO habilitado, recomendamos fazer logon por meio de seu próprio subdomínio/domínio [!DNL Workfront Proof].

   >[!NOTE]
   >
   >Neste momento, quando o Logon Único estiver habilitado na sua conta do [!DNL Workfront Proof], você não poderá fazer logon no aplicativo iPhone com essas credenciais.

   1. **Manual** (padrão): SSO com uma configuração diferente (por exemplo, apontando para outro Provedor de Identidade).

      >[!NOTE]
      >
      >Se a conta satélite estiver herdando a configuração do SSO da conta hub, a tela de logon será a da conta hub. Quando o usuário da conta satélite digitar os detalhes de logon com SSO nesta página, ele será redirecionado de volta para a conta satélite.

      ![Enabling_SSO_-_Satellite_Account_2.png](assets/enabling-sso---satellite-account-2-350x224.png)

   1. Clique em **[!UICONTROL Salvar]** (6).

## Configurações de SSO Herdadas de uma Conta Hub

Ao optar por herdar as configurações da sua conta hub, você notará que todos os campos agora são preenchidos com os dados da sua conta hub (7) e que o Logon único é automaticamente Ativado/Desativado(8) como na sua conta principal. Também não há mais links de edição nos campos, pois toda a configuração do SSO para a Conta satélite agora está definida e gerenciada a partir da sua conta hub.

![Conta_Satélite_-_Inherited_SSO.png](assets/satellite-account---inherited-sso-350x99.png)

Na sua conta do hub (9) o campo [!UICONTROL Uso do SSO] mostra que essa configuração está sendo usada por contas satélite (10).\
![Conta_de_Hub_-_Inherited_SSO.png](assets/hub-account---inherited-sso-350x275.png)

## SSO configurado manualmente

Se a configuração de SSO Manual tiver sido escolhida para uma conta satélite (1), você precisará inserir manualmente os dados para o Single Sign-On.

1. Clique em **[!UICONTROL Configurações]** > **[!UICONTROL Configurações de conta]** (1).

1. Abra a guia **[!UICONTROL Logon único]**.
1. Clique em **[!UICONTROL Editar],** para preencher o campo e em **[!UICONTROL Salvar]** (2).

1. Na linha **[!UICONTROL SSO]**, clique em **[!UICONTROL Habilitado]** (3).

![Conta_Satélite_-_Manual_SSO.png](assets/satellite-account---manual-sso-350x280.png)

## Login com SSO

1. Clique em **[!UICONTROL Configurações]** > **[!UICONTROL Configurações de conta]** (1).

1. Abra a guia **[!UICONTROL Logon único]**.
1. Verifique se o domínio/subdomínio do [!DNL Workfront Proof] (1) está configurado e se os usuários acessam a conta do [!DNL Workfront Proof] por meio desse domínio/subdomínio personalizado.
   ![SAML_Subdomain.png](assets/saml-subdomain-350x150.png)
Com o Logon único habilitado, o URL de logon de subdomínio (por exemplo, yourcompany.proofhq.com/login) exibe uma tela de transferência (2) que o direciona diretamente para a página de logon com SSO.
   ![SSO_login_page.png](assets/sso-login-page-350x164.png)

1. Se um usuário acessar [!DNL Workfront Proof] por meio da **página de logon padrão** ([https://www.proofhq.com/login](https://www.proofhq.com/login)), haverá **dois níveis de autorização**. Primeiro, um usuário é solicitado a fazer logon usando os dados de acesso do [!DNL Workfront Proof] (email e senha). Em seguida, o usuário é transferido por meio de uma janela SSO (2) para a página de logon SSO.\
   Portanto, com o serviço SSO habilitado, recomendamos fazer logon por meio de seu próprio subdomínio/domínio [!DNL Workfront Proof].

1. Neste momento, quando o Logon único está ativado na sua conta da Workfront Proof, você não poderá fazer logon no aplicativo da iPhone com essas credenciais.

## Sobre a adição de um novo usuário

Quando a funcionalidade Logon Único estiver habilitada na sua conta do [!DNL Workfront Proof], os novos usuários não receberão emails de confirmação, pois suas contas serão ativadas automaticamente e prontas para uso.

Na página de logon do [!DNL Workfront Proof], depois de clicar no botão [!UICONTROL Logon], os usuários são direcionados para a sua página de logon por SSO e solicitados a inserir suas credenciais de logon único.

>[!IMPORTANT]
>
>Os usuários são identificados por meio de um endereço de email durante o processo de autenticação, o que significa que a conta de email usada para seu logon no SSO deve ser o endereço de email do usuário registrado em sua conta.

## Serviços de Federação do Ative Diretory (AD FS)

O AD FS (Serviços de Federação do Ative Diretory) é um componente de software [!DNL Microsoft] que pode ser instalado em sistemas operacionais Windows Server para fornecer aos usuários acesso de Logon Único a sistemas e aplicativos localizados além dos limites organizacionais. Para obter mais informações, consulte &quot;Ative Diretory Federation Services&quot; no site da Microsoft Developer Network.

O sistema [!DNL Workfront Proof] dá suporte ao SAML 2.0 e só é compatível com o AD FS versão 2.0 ou superior.

Consulte [Logon Único [!DNL Workfront Proof]: Configuração do AD FS](../../../workfront-proof/wp-acct-admin/account-settings/sso-in-wp-adfs-configuration.md) para obter instruções detalhadas.
