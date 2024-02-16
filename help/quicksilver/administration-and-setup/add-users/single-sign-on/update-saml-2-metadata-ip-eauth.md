---
title: Atualizar os metadados do SAML 2.0 no IDP ao usar a autenticação aprimorada
description: Como administrador do Adobe Workfront, você pode integrar o logon único (SSO) da Workfront a qualquer provedor de identidade que ofereça suporte ao protocolo SAML (Security Assertion Markup Language) 2.0.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 55d7d8a8-0dfe-45bc-a23a-47111347e9ca
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 0%

---

# Atualizar os metadados do SAML 2.0 no IDP ao usar a autenticação aprimorada

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Como administrador do Adobe Workfront, você pode integrar o logon único (SSO) da Workfront a qualquer provedor de identidade que ofereça suporte ao protocolo SAML (Security Assertion Markup Language) 2.0.

As seções a seguir descrevem o processo de integração quando sua conta do Workfront é atualizada para a experiência de autenticação aprimorada (ainda não disponível para todas as organizações). Para obter mais informações sobre a experiência de autenticação aprimorada, consulte [Visão geral da autenticação aprimorada](../../../administration-and-setup/manage-workfront/security/get-started-enhanced-authentication.md).

Para obter informações sobre como configurar o SAML antes de migrar para a experiência de autenticação aprimorada, consulte [Atualizar metadados do SAML 2.0 no provedor de identidade](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).


## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>NOTA</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Usar o Okta como seu provedor de identidade

Okta é um exemplo de um provedor de identidade compatível com SAML 2.0. Esta seção descreve como usar o Okta como seu provedor de identidade. Etapas semelhantes seriam necessárias ao configurar outro provedor de identidade que ofereça suporte ao SAML 2.0.

>[!NOTE]
>
>Os usuários são mapeados com base em seus endereços de email. Para fazer logon no Workfront usando o Okta, você deve ter um usuário com o mesmo endereço de email (não diferencia maiúsculas de minúsculas) criado em seu cliente do Workfront.

Complete as seções a seguir para configurar o Okta como seu provedor de identidade na Workfront.

* [Criar um aplicativo Workfront no Okta](#create-a-workfront-app-in-okta)
* [Adicione sua instância do Okta como um provedor de identidade na Workfront](#add-your-okta-instance-as-an-identity-provider-in-workfront)

### Criar um aplicativo Workfront no Okta {#create-a-workfront-app-in-okta}

1. Faça logon no ambiente do Okta.
1. Assegure que **Interface clássica** está selecionada no canto superior esquerdo da interface do Okta.
1. No menu, clique em **Aplicativos** > **Aplicativos**.

1. Clique em **Adicionar aplicativo** e, em seguida, clique em **Criar novo aplicativo**.

1. No **Caixa de diálogo Criar uma Nova Integração de Aplicativos** , selecione **SAML 2.0** e, em seguida, clique em **Criar**.

1. Especifique um nome para o aplicativo Workfront e clique em **Próxima**.
1. Na página Configurações SAML que é exibida, localize as informações necessárias para a página Configurações SAML:

   1. Sem sair da aba do navegador onde a interface do Okta é exibida, abra uma aba ou janela separada do navegador.
   1. Especifique o seguinte URL no navegador:

      `https://[your_customer_subdomain].my.workfront.com/auth/saml2/metadata`

   1. No arquivo XML resultante, identifique os valores de **entityID** e **Localização**.

      ![sso-okta.png](assets/sso-okta.png)

   1. Copie o valor de **entityID** para a área de transferência do sistema. Não feche esta guia do navegador.

1. Volte para a página Configurações SAML que você abriu na Etapa 6.
1. Cole o valor do **entityID** no campo **URI do público-alvo (ID de entidade da controladora)** campo.

1. No arquivo XML de outra guia do navegador, copie o valor do **Localização** campo.
1. Cole o valor do **Localização** no campo **Logon único** **URL** campo.

1. Role para a **Instruções de atributo (opcional)** seção.
1. No **Nome** campo, especificar **email**.

1. No **Valor** campo, especificar **user.email**.

1. (Opcional) Adicione quaisquer valores avançados.
1. Clique em **Próxima**.
1. Selecionar, **Sou um cliente do Okta adicionando um aplicativo interno** e, em seguida, clique em **Concluir**.

### Adicione sua instância do Okta como um provedor de identidade na Workfront {#add-your-okta-instance-as-an-identity-provider-in-workfront}

Este procedimento fornece informações essenciais para configurar o Okta como um provedor de identidade no Workfront. Para obter informações adicionais sobre outros mapeamentos ou opções de configuração, consulte [Configurar o Adobe Workfront com SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

1. Baixe os metadados do provedor de identidade para sua instância do Okta:

   1. Faça logon no ambiente do Okta.
   1. Assegure que **Interface clássica** está selecionada no canto superior esquerdo da interface do Okta.
   1. No menu, clique em **Aplicativos** > **Aplicativos**.

   1. Clique no aplicativo Workfront que você criou, conforme descrito na seção, [Criar um aplicativo Workfront no Okta](#create-a-workfront-app-in-okta)
   1. No **Fazer logon** clique em **Metadados do provedor de identidade**.

      ![idp_okta_metadata.png](assets/idp-okta-metadata.png)

      Os metadados são abertos como XML em uma nova guia do navegador.

   1. Copie o URL exibido no campo URL do navegador.

1. Faça logon no administrador do Workfront as a Workfront.
1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Sistema** > **Logon único (SSO)**.

1. (Condicional) Se você visualizar duas guias, clique na guia **Novos Provedores de SSO** guia.

   ![sso_idp_halflife.png](assets/sso-idp-halflife-350x234.png)

   >[!IMPORTANT]
   >
   >Não exclua suas definições de configuração de SSO existentes na **Provedor de SSO atual** até que sua conta seja atualizada para a experiência de autenticação aprimorada e a nova configuração do SSO seja totalmente funcional.

1. Clique em **Novo Provedor de SSO**.
1. Especifique um nome, como Okta IDP, e especifique uma descrição.
1. No **Preencher campos a partir dos metadados do provedor de identidade** cole o URL que você copiou na Etapa 1 na caixa **URL de metadados** campo.\
   Como alternativa, você pode clicar em **Escolher arquivo** para carregar um arquivo .xml, mas recomendamos que você cole o URL.

1. No **Mapear Atributos de Usuário** seção, no campo **Diretório de Atributo** campo, tipo **email**. (**Endereço de e-mail** já está preenchida na variável **Atributo de usuário do Workfront** campo.)

1. (Opcional) Ativar **Tornar padrão o Provedor de SSO** para enviar usuários não autenticados à tela de logon do provedor de identidade em vez de à tela de logon da Workfront para autenticação. Recomendamos que você ative essa opção somente se todos os usuários no seu sistema acessarem o Workfront por meio do provedor de identidade.
1. Selecione o **Ativar** caixa de seleção Antes de fazer isso, verifique se os usuários em seu sistema estão cientes da nova experiência de logon para garantir que não percam o acesso ao sistema do Workfront.
1. Clique em **Testar conexão**.\
   Você deve ver uma mensagem informando que a conexão foi bem-sucedida.

1. Clique em **Salvar**.

## Uso de outros provedores de identidade

Ao usar provedores de identidade diferentes do Okta (como Ping ou Centrify), você deve fazer upload novamente dos metadados do Workfront para seu provedor de identidade.
