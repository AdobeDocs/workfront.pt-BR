---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: Configurar acesso simples para [!DNL Workfront Proof] usuários
description: Se você tiver o plano Select ou Premium, poderá fornecer o recurso de Logon Único (SSO) que permite usar o nome de usuário e a senha da sua organização existente para acessar o [!DNL Workfront Proof] conta.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 52ac1919-1821-424f-89f8-72865b236e4e
source-git-commit: 007a603ef1df2a02959d7fb623ac784bf5b9cb80
workflow-type: tm+mt
source-wordcount: '1264'
ht-degree: 0%

---

# Configurar acesso simples para [!DNL Workfront Proof] usuários

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro do [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

Se você tiver o plano Select ou Premium, poderá fornecer o recurso de Logon Único (SSO) que permite usar o nome de usuário e a senha da sua organização existente para acessar o [!DNL Workfront Proof] conta.

Isso significa que você irá autenticar em seu próprio sistema de logon, não em relação ao [!DNL Workfront Proof] página de logon.

>[!NOTE]
>
>Você deve ter um subdomínio ou domínio personalizado configurado em [!DNL Workfront Proof] para habilitar o SAML. A configuração de subdomínios personalizados é livre. Consulte [Marcas](https://support.workfront.com/hc/en-us/sections/115000921208-Branding) para obter mais informações.Você pode ler mais sobre domínios totalmente personalizados em nossa [Marcar o [!DNL Workfront Proof] site - avançado](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

## Habilitar SSO em [!DNL Workfront Proof]

A funcionalidade de Logon único pode ser ativada na [!UICONTROL Logon único] guia do seu [!UICONTROL Configurações da conta], e se aplicará a todos os usuários em seu [!DNL Workfront Proof] conta. Consulte [Configurações da conta](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) para obter mais informações.

## ID da entidade

Como um Provedor de serviços, publicamos nossa ID de entidade aqui:

[https://yoursubdomain.proofhq.com/saml/module.php/saml/sp/metadata.php/phq](https://yoursubdomain.proofhq.com/saml/module.php/saml/sp/metadata.php/phq) (onde &quot;yoursubdomain&quot; é o subdomínio de sua conta)

[!DNL Workfront Proof] O requer o endereço de email do usuário como identificador exclusivo, que pode ser passado como um dos seguintes atributos:

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

1. Abra o **[!UICONTROL Logon único]** guia (1).
1. Insira o **URL DO SSO** (2).
Esse é o link para o seu servidor SSO (por exemplo, **https://sso.mycompany.com/opensso**).

1. Insira o **URL de logon** (3).
Este é o URL que será chamado para redirecionar os usuários para o seu provedor de identidade.

1. Este não é um URL real que você digita no navegador, mas um terminal que processará as informações que enviamos para apresentar a tela de login.

Insira o **URL de saída** (4).
Este é o URL ao qual você retornará depois de fazer logoff, por exemplo

**https://www.yourcompany.com/services/logout.asp**

1. Insira o **Impressão digital do certificado** (5).
1. A impressão digital SHA1 do certificado SAML fornecido pelo Provedor de Identidade SAML.
1. Certifique-se de incluir as informações principais definindo isso no Provedor de identidade.
1. Alternar **SSO** para **[!UICONTROL Ativado]** (6).
Quando o SSO estiver habilitado, você e outros usuários da sua conta farão logon usando seu próprio mecanismo de autenticação. Isso significa que quando os usuários acessam o seu [!DNL Workfront Proof] tela de logon da conta (por exemplo, **yourcompany.proofhq.com/login**), eles serão avisados com a janela de transferência para sua própria página de logon de autenticação.

1. (Opcional) Ativar **Provisionar usuários automaticamente** (7).
Quando esta opção estiver habilitada, as contas de usuário serão criadas automaticamente para pessoas que não têm suas próprias [!DNL Workfront Proof] perfis, mas acessarão suas [!DNL Workfront Proof] usando suas credenciais de Logon único. Isso será ativado somente quando o limite do usuário ainda não for atingido em sua conta.

1. Os novos usuários provisionados terão as permissões de perfil de gerente atribuídas por padrão. Se precisar de mais informações, consulte [Perfis de permissões de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

![Enable_SSO_SAML_2.0.png](assets/enable-sso-saml-2.0-350x236.png)

## Ativação do SSO para contas satélite

Quando você tem contas satélite conectadas à sua conta hub, é possível administrá-las a partir do nível da conta hub.

Single Sign-On é um recurso Select e Premium, portanto, o Single Sign-On só pode ser ativado em satélites que estejam nos planos Select e Premium.

1. Clique em **[!UICONTROL Configurações]** > **[!UICONTROL Configurações da conta]** (1).

1. Clique na conta satélite no menu suspenso (2).
1. Abra o **[!UICONTROL Logon único]** guia (3).
1. Comece a editar a configuração de SSO (4).
1. ![Enabling_SSO_Satellite_Account.png](assets/enabling-sso---satellite-account-350x266.png)
Aqui você terá dois métodos (5) de configuração:

1. **Herdado:** SSO com a configuração retirada da sua conta de hub.
Se um usuário acessar [!DNL Workfront Proof] por meio da **página de logon padrão** ([https://www.proofhq.com/login](https://www.proofhq.com/login)) haverá **dois níveis de**: primeiro um usuário é solicitado a fazer logon usando [!DNL Workfront Proof] acessar dados (email e senha); em seguida, o usuário é transferido por meio de uma janela SSO para a página de logon SSO.
Portanto, com o serviço SSO habilitado, recomendamos que você faça o logon por meio do seu próprio [!DNL Workfront Proof] subdomínio/domínio.

   >[!NOTE]
   >
   >Neste momento, quando o Logon único está ativado em sua [!DNL Workfront Proof] conta, você não poderá fazer logon no aplicativo iPhone com essas credenciais.

   1. **Manual** (padrão): SSO com uma configuração diferente (por exemplo, apontar para outro Provedor de identidade).

      >[!NOTE]
      >
      >Se a conta satélite estiver herdando a configuração do SSO da conta hub, a tela de logon será a da conta hub. Quando o usuário da conta satélite digitar os detalhes de logon com SSO nesta página, ele será redirecionado de volta para a conta satélite.

      ![Enabling_SSO_Satellite_Account_2.png](assets/enabling-sso---satellite-account-2-350x224.png)

   1. Clique em **[!UICONTROL Salvar]** (6).

## Configurações de SSO Herdadas de uma Conta Hub

Ao optar por herdar as configurações da sua conta hub, você notará que todos os campos agora são preenchidos com os dados da sua conta hub (7) e que o Logon único é automaticamente Ativado/Desativado(8) como na sua conta principal. Também não há mais links de edição nos campos, pois toda a configuração do SSO para a Conta satélite agora está definida e gerenciada a partir da sua conta hub.

![Satellite_Account_Inherited_SSO.png](assets/satellite-account---inherited-sso-350x99.png)

Na sua conta do hub (9), a variável [!UICONTROL Uso do SSO] mostra que esta configuração é utilizada por contas satélite (10).\
![Hub_Account_SSO.png](assets/hub-account---inherited-sso-350x275.png)

## SSO configurado manualmente

Se a configuração de SSO Manual tiver sido escolhida para uma conta satélite (1), você precisará inserir manualmente os dados para o Single Sign-On.

1. Clique em **[!UICONTROL Configurações]** > **[!UICONTROL Configurações da conta]** (1).

1. Abra o **[!UICONTROL Logon único]** guia.
1. Clique em **[!UICONTROL Editar],** preencha o campo e clique em **[!UICONTROL Salvar]** (2).

1. No **[!UICONTROL SSO]** clique em **[!UICONTROL Ativado]** (3).

![Satellite_Account_Manual_SSO.png](assets/satellite-account---manual-sso-350x280.png)

## Login com SSO

1. Clique em **[!UICONTROL Configurações]** > **[!UICONTROL Configurações da conta]** (1).

1. Abra o **[!UICONTROL Logon único]** guia.
1. Verifique se o seu [!DNL Workfront Proof] domínio/subdomínio (1) estiver configurado e que seus usuários acessem o [!DNL Workfront Proof] conta por meio deste domínio/subdomínio personalizado.
   ![SAML_Subdomain.png](assets/saml-subdomain-350x150.png)
Com o Logon único habilitado, o URL de logon de subdomínio (por exemplo, yourcompany.proofhq.com/login) exibe uma tela de transferência (2) que o direciona diretamente para a página de logon com SSO.
   ![SSO_login_page.png](assets/sso-login-page-350x164.png)

1. Se um usuário acessar [!DNL Workfront Proof] por meio da **página de logon padrão** ([https://www.proofhq.com/login](https://www.proofhq.com/login)) haverá **dois níveis de**. Primeiro, um usuário é solicitado a fazer logon usando [!DNL Workfront Proof] acessar dados (email e senha). Em seguida, o usuário é transferido por meio de uma janela SSO (2) para a página de logon SSO.\
   Portanto, com o serviço SSO habilitado, recomendamos que você faça o logon por meio do seu próprio [!DNL Workfront Proof] subdomínio/domínio.

1. Nesse momento, quando o Logon único está ativado na sua conta do Workfront Proof, você não poderá fazer logon no aplicativo da iPhone com essas credenciais.

## Sobre a adição de um novo usuário

Quando a funcionalidade de Logon único estiver ativada em seu [!DNL Workfront Proof] Os novos usuários não receberão emails de confirmação, pois suas contas serão ativadas automaticamente e estarão prontas para uso.

Do seu [!DNL Workfront Proof] página de login, depois de clicar no link [!UICONTROL Logon] , os usuários são direcionados à sua página de login de SSO e solicitados a digitar suas credenciais de login de login de login único.

>[!IMPORTANT]
>
>Os usuários são identificados por meio de um endereço de email durante o processo de autenticação, o que significa que a conta de email usada para seu logon no SSO deve ser o endereço de email do usuário registrado em sua conta.

## Serviços de Federação do Ative Diretory (AD FS)

O AD FS (Serviços de Federação do Ative Diretory) é um [!DNL Microsoft] componente de software que pode ser instalado nos sistemas operacionais Windows Server para fornecer aos usuários acesso de Logon Único a sistemas e aplicativos localizados além dos limites organizacionais. Para obter mais informações, consulte &quot;Ative Diretory Federation Services&quot; no site da Microsoft Developer Network.

A variável [!DNL Workfront Proof] O sistema oferece suporte ao SAML 2.0 e só é compatível com o AD FS versão 2.0 ou superior.

Consulte [Logon único [!DNL Workfront Proof]: Configuração do AD FS](../../../workfront-proof/wp-acct-admin/account-settings/sso-in-wp-adfs-configuration.md) para obter instruções detalhadas.
