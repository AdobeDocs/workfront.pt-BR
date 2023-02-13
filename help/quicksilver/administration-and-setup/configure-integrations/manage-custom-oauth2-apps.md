---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: Exibir e gerenciar aplicativos OAuth2 personalizados
description: Como administrador do Adobe Workfront, você pode exibir e gerenciar os aplicativos OAuth2 para sua instância do Workfront, que permitem que outros aplicativos acessem o Workfront.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
source-git-commit: f7e3182776e6b62103cd755b2fbd5057efc95394
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 1%

---

# Exibir e gerenciar aplicativos OAuth2 personalizados

Como um [!DNL Adobe Workfront] administrador, você pode visualizar e gerenciar os aplicativos do OAuth2 para sua instância de [!DNL Workfront], que permitem o acesso de outros aplicativos [!UICONTROL Workfront].

>[!NOTE]
>
>No contexto do OAuth2, &quot;Aplicativo Oauth2&quot; refere-se a esse tipo de link de acesso entre um aplicativo e um servidor, como [!DNL Workfront]. Para obter mais informações, consulte [Crie aplicativos OAuth2 para [!DNL Workfront] integrações](../../administration-and-setup/configure-integrations/create-oauth-application.md)

* Para obter informações sobre como criar aplicativos OAuth2 personalizados, consulte [Crie aplicativos OAuth2 para [!DNL Workfront] integrações](../../administration-and-setup/configure-integrations/create-oauth-application.md)
* Para obter instruções sobre como configurar e usar o aplicativo OAuth2 com credenciais de usuário (fluxo do código de autorização), consulte [Configure e use os aplicativos OAuth 2 personalizados de sua organização usando o fluxo do código de autorização](../../wf-api/api/oauth-app-code-token-flow.md).
* Para obter instruções sobre como configurar e usar o aplicativo OAuth2 usando autenticação de servidor (fluxo JWT), consulte [Configure e use os aplicativos OAuth 2 personalizados de sua organização usando o fluxo JWT](../../wf-api/api/oauth-app-jwt-flow.md).
* Para obter instruções sobre como configurar e usar o aplicativo OAuth2 usando PKCE, consulte [Configure e use os aplicativos OAuth 2 personalizados de sua organização usando o fluxo PKCE](../../wf-api/api/oauth-app-pkce-flow.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!DNL Pro] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Plan] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> Você deve ser um [!DNL Workfront] administrador. </p>
    <p>Para obter informações sobre [!DNL Workfront] administradores, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p>
     </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Pré-requisitos

Você deve criar [!UICONTROL OAuth2] aplicativos para sua organização antes de visualizá-los ou gerenciá-los.

Para obter mais informações, consulte [Crie aplicativos OAuth2 para [!DNL Workfront] integrações](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## Gerenciar aplicativos OAuth2 personalizados

* [Exibir e editar aplicativos OAuth2 personalizados](#view-and-edit-custom-oauth2-applications)
* [Excluir aplicativos OAuth2 personalizados](#delete-custom-oauth2-applications)

### Exibir e editar aplicativos OAuth2 personalizados {#view-and-edit-custom-oauth2-applications}

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. No painel de navegação esquerdo, clique em **[!UICONTROL Sistema]**, em seguida selecione **[!UICONTROL Aplicativos OAuth]**.
1. Clique em **[!UICONTROL Criar integração de aplicativo]**.
1. Passe o mouse sobre o aplicativo e clique em **[!UICONTROL Editar]** ![](assets/edit-icon.png) quando aparece na extrema direita.
1. (Opcional) Edite quaisquer detalhes do aplicativo.

   Para campos relacionados aos aplicativos OAuth2 e JWT, consulte [Crie aplicativos OAuth2 para [!DNL Workfront] integrações](../../administration-and-setup/configure-integrations/create-oauth-application.md).

### Excluir aplicativos OAuth2 personalizados {#delete-custom-oauth2-applications}

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. No painel de navegação esquerdo, clique em **[!UICONTROL Sistema]**, em seguida selecione **[!UICONTROL Aplicativos OAuth]**.
1. Clique em **  **.
1. Passe o mouse sobre o aplicativo e clique em **[!UICONTROL Excluir]** ![](assets/delete.png) quando aparece na extrema direita.

## Gerenciar Segredos do Cliente em aplicativos OAuth2

* [Exibir detalhes do Segredo do Cliente](#view-client-secret-details)
* [Adicionar ou editar notas para o Segredo do Cliente](#add-or-edit-notes-for-client-secret)
* [Excluir segredo do cliente](#delete-client-secret)

### Exibir detalhes do Segredo do Cliente {#view-client-secret-details}

>[!IMPORTANT]
>
>Não é possível exibir o Segredo do cliente em si. Caso tenha perdido o Segredo do cliente, você deverá excluí-lo e criar um novo.
>
>* Para excluir um Segredo do cliente, consulte [Excluir segredo do cliente](#delete-client-secret) neste artigo.
>* Para criar um novo Segredo do cliente, consulte [Criar um aplicativo OAuth2](../../administration-and-setup/configure-integrations/create-oauth-application.md#create) em [Crie aplicativos OAuth2 para [!DNL Workfront] integrações](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>




1. Clique no botão *[!UICONTROL *Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. No painel de navegação esquerdo, clique em **[!UICONTROL Sistema]**, em seguida selecione **[!UICONTROL Aplicativos OAuth]**.
1. Passe o mouse sobre o aplicativo e clique no botão **[!UICONTROL Editar]** quando for exibido na extremidade direita.
1. Exibir detalhes na área Segredo do cliente:

   * Data de criação
   * Data da última utilização
   * Notas

      Para adicionar observações a um Segredo do cliente, consulte [Adicionar ou editar notas para o Segredo do Cliente](#add-or-edit-notes-for-client-secret).

### Adicionar ou editar notas para o Segredo do Cliente {#add-or-edit-notes-for-client-secret}

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. No painel de navegação esquerdo, clique em **[!UICONTROL Sistema]**, em seguida selecione **[!UICONTROL Aplicativos OAuth]**.
1. Clique em **[!UICONTROL Criar integração de aplicativo]**.
1. Passe o mouse sobre o aplicativo e clique no botão **[!UICONTROL Editar]** quando for exibido na extremidade direita.
1. Localize o Segredo do cliente para o qual deseja adicionar ou editar uma nota.
1. Clique na caixa que contém os detalhes do Segredo do cliente.

   Agora é possível adicionar texto de nota ou editar um texto de nota existente.

   >[!NOTE]
   >
   >O texto da observação tem no máximo 64 caracteres.

1. Clique para fora da caixa ou pressione **[!UICONTROL Enter]** para salvar o texto da nota.

### Excluir segredo do cliente {#delete-client-secret}

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. No painel de navegação esquerdo, clique em **[!UICONTROL Sistema]**, em seguida selecione **[!UICONTROL Aplicativos OAuth]**.
1. Clique em **[!UICONTROL Criar integração de aplicativo]**.
1. Passe o mouse sobre o aplicativo e clique no botão **[!UICONTROL Editar]** quando for exibido na extremidade direita.
1. Localize o Segredo do cliente que deseja excluir.
1. Clique no botão **[!UICONTROL Excluir]** ícone ![](assets/delete.png) ao lado do Segredo do cliente.
