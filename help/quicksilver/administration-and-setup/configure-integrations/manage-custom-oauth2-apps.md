---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: Exibir e gerenciar aplicativos OAuth2 personalizados
description: Como administrador do Adobe Workfront, você pode exibir e gerenciar os aplicativos OAuth2 para sua instância do Workfront, que permitem que outros aplicativos acessem o Workfront.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
author: Becky
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '669'
ht-degree: 0%

---

# Exibir e gerenciar aplicativos OAuth2 personalizados

Como administrador do [!DNL Adobe Workfront], você pode exibir e gerenciar os aplicativos OAuth2 para sua instância do [!DNL Workfront], que permitem que outros aplicativos acessem o [!UICONTROL Workfront].

>[!NOTE]
>
>* No contexto de OAuth2, &quot;aplicativo OAuth2&quot; se refere a esse tipo de link de acesso entre um aplicativo e um servidor, como [!DNL Workfront]. Para obter mais informações, consulte [Criar aplicativos OAuth2 para [!DNL Workfront] integrações](../../administration-and-setup/configure-integrations/create-oauth-application.md)
>* Você pode ter até dez aplicativos OAuth2 ao mesmo tempo.

* Para obter informações sobre como criar aplicativos OAuth2 personalizados, consulte [Criar aplicativos OAuth2 para [!DNL Workfront] integrações](../../administration-and-setup/configure-integrations/create-oauth-application.md)
* Para obter instruções sobre como configurar e usar o aplicativo OAuth2 com credenciais de usuário (fluxo de código de autorização), consulte [Configurar e usar os aplicativos OAuth 2 personalizados da sua organização usando o fluxo de código de autorização](../../wf-api/api/oauth-app-code-token-flow.md).
* Para obter instruções sobre como configurar e usar o aplicativo OAuth2 usando a autenticação de servidor (fluxo JWT), consulte [Configurar e usar os aplicativos OAuth 2 personalizados da sua organização usando o fluxo JWT](../../wf-api/api/oauth-app-jwt-flow.md).
* Para obter instruções sobre como configurar e usar o aplicativo OAuth2 usando o PKCE, consulte [Configurar e usar os aplicativos OAuth 2 personalizados de sua organização usando o fluxo de PKCE](../../wf-api/api/oauth-app-pkce-flow.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

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
   <td> Você deve ser um administrador [!DNL Workfront]. </p>
    <p>Para obter informações sobre administradores do [!DNL Workfront], consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a um usuário acesso administrativo total</a>.</p>
     </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

+++

## Pré-requisitos

Você deve criar aplicativos [!UICONTROL OAuth2] para sua organização antes de exibi-los ou gerenciá-los.

Para obter mais informações, consulte [Criar aplicativos OAuth2 para [!DNL Workfront] integrações](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## Gerenciar aplicativos OAuth2 personalizados

* [Exibir e editar aplicativos OAuth2 personalizados](#view-and-edit-custom-oauth2-applications)
* [Excluir aplicativos OAuth2 personalizados](#delete-custom-oauth2-applications)

### Exibir e editar aplicativos OAuth2 personalizados {#view-and-edit-custom-oauth2-applications}

{{step-1-to-setup}}

1. No painel de navegação esquerdo, clique em **[!UICONTROL Sistema]** e selecione **[!UICONTROL Aplicativos OAuth]**.
1. Clique em **[!UICONTROL Criar integração de aplicativo]**.
1. Passe o mouse sobre o aplicativo e clique em **[!UICONTROL Editar]** ![Editar ícone](assets/edit-icon.png) quando ele aparecer na extremidade direita.
1. (Opcional) Edite todos os detalhes do aplicativo.

   Para campos relacionados a aplicativos OAuth2 e JWT, consulte [Criar aplicativos OAuth2 para [!DNL Workfront] integrações](../../administration-and-setup/configure-integrations/create-oauth-application.md).

### Excluir aplicativos OAuth2 personalizados {#delete-custom-oauth2-applications}

{{step-1-to-setup}}

1. No painel de navegação esquerdo, clique em **[!UICONTROL Sistema]** e selecione **[!UICONTROL Aplicativos OAuth]**.
1. Passe o mouse sobre o aplicativo e clique em **[!UICONTROL Excluir]** ![Excluir](assets/delete.png) quando ele aparecer na extremidade direita.

## Gerenciar segredos do cliente em aplicativos OAuth2

* [Exibir detalhes do Segredo do Cliente](#view-client-secret-details)
* [Adicionar ou editar notas do Segredo do cliente](#add-or-edit-notes-for-client-secret)
* [Excluir segredo do cliente](#delete-client-secret)

### Exibir detalhes do Segredo do Cliente {#view-client-secret-details}

>[!IMPORTANT]
>
>Você não pode ver o próprio Segredo do cliente. Caso tenha perdido o segredo do cliente, você deve excluí-lo e criar um novo.
>
>* Para excluir um segredo do cliente, consulte [Excluir segredo do cliente](#delete-client-secret) neste artigo.
>* Para criar um novo Segredo do Cliente, consulte [Criar um aplicativo OAuth2](../../administration-and-setup/configure-integrations/create-oauth-application.md#create) em [Criar aplicativos OAuth2 para [!DNL Workfront] integrações](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>

{{step-1-to-setup}}

1. No painel de navegação esquerdo, clique em **[!UICONTROL Sistema]** e selecione **[!UICONTROL Aplicativos OAuth]**.
1. Passe o mouse sobre o aplicativo e clique no ícone **[!UICONTROL Editar]** quando ele aparecer na extremidade direita.
1. Exibir detalhes na área Segredo do cliente:

   * Data de criação
   * Última data de uso
   * Notas

     Para adicionar observações a um Segredo do Cliente, consulte [Adicionar ou editar observações para o Segredo do Cliente](#add-or-edit-notes-for-client-secret).

### Adicionar ou editar notas do Segredo do cliente {#add-or-edit-notes-for-client-secret}

{{step-1-to-setup}}

1. No painel de navegação esquerdo, clique em **[!UICONTROL Sistema]** e selecione **[!UICONTROL Aplicativos OAuth]**.
1. Clique em **[!UICONTROL Criar integração de aplicativo]**.
1. Passe o mouse sobre o aplicativo e clique no ícone **[!UICONTROL Editar]** quando ele aparecer na extremidade direita.
1. Localize o Segredo do cliente para o qual você deseja adicionar ou editar uma nota.
1. Clique na caixa que contém os detalhes do Segredo do cliente.

   Agora é possível adicionar texto de nota ou editar texto de nota existente.

   >[!NOTE]
   >
   >O texto da nota tem no máximo 64 caracteres.

1. Clique fora da caixa ou pressione **[!UICONTROL Enter]** para salvar o texto da observação.

### Excluir segredo do cliente {#delete-client-secret}

{{step-1-to-setup}}

1. No painel de navegação esquerdo, clique em **[!UICONTROL Sistema]** e selecione **[!UICONTROL Aplicativos OAuth]**.
1. Clique em **[!UICONTROL Criar integração de aplicativo]**.
1. Passe o mouse sobre o aplicativo e clique no ícone **[!UICONTROL Editar]** quando ele aparecer na extremidade direita.
1. Localize o Segredo do cliente que deseja excluir.
1. Clique no ícone **[!UICONTROL Excluir]** ![Excluir](assets/delete.png) ao lado do Segredo do Cliente.
