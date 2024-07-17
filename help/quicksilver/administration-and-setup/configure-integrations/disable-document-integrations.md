---
title: Desativar integrações de documentos
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Como administrador do  [!DNL anAdobe] [!DNL Workfront], você pode desabilitar a conexão entre o Workfront e qualquer um dos provedores de documentos de terceiros.
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# Desativar integrações de documentos

Como administrador do [!DNL Adobe] [!DNL Workfront], você pode desabilitar a conexão entre o [!DNL Workfront] e qualquer provedor de documentos de terceiros.

Quando você desabilita a conexão entre [!DNL Workfront] e um provedor de documentos, os links para os documentos desaparecem de [!DNL Workfront]. Os usuários não podem mais ver os documentos vinculados, não podem fazer alterações nos documentos por meio dos links [!DNL Workfront] e não podem adicionar mais documentos a esse provedor.

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Plano]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ser um administrador [!DNL Workfront]. Para obter informações sobre administradores do [!DNL Workfront], consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a um usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

## Desabilitar integrações do provedor de nuvem

Para desabilitar integrações de documentos do [!UICONTROL Workfront DAM], [!DNL Box], [!DNL Dropbox], [!DNL Google Drive], [!DNL Microsoft OneDrive], [!DNL WebDAM]:

1. Faça logon em [!DNL Workfront] como administrador [!DNL Workfront].
1. Clique no ícone ![](assets/main-menu-icon.png) do **[!UICONTROL Menu Principal]** no canto superior direito de [!DNL Adobe Workfront] e em **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Documentos]** > **[!UICONTROL Provedores de Nuvem]**.

1. Desmarque qualquer um dos provedores de nuvem que você deseja desconectar de [!DNL Workfront].
1. Clique em **[!UICONTROL Salvar]**.

   Os usuários não podem se conectar ao provedor de nuvem específico desativado e não podem mais vincular documentos desse provedor de nuvem ao Workfront.

## Desabilitar a integração [!DNL SharePoint]

1. Faça logon em [!DNL Workfront] como administrador [!DNL Workfront].
1. Clique no ícone ![](assets/main-menu-icon.png) do **[!UICONTROL Menu Principal]** no canto superior direito de [!DNL Adobe Workfront] e em **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. Expanda **[!UICONTROL Documentos]** e clique em **[!UICONTROL [!DNL SharePoint]Integração]**.
1. Selecione a integração do [!DNL SharePoint] que deseja desabilitar.
1. Clique em **[!UICONTROL Desabilitar]**.\
   Os usuários não podem se conectar ao site [!DNL SharePoint] que você desabilitou, e não podem mais vincular documentos de [!DNL SharePoint] a [!DNL Workfront].

## Desativar integrações personalizadas

1. Faça logon em [!DNL Workfront] como administrador.
1. Clique no ícone ![](assets/main-menu-icon.png) do **[!UICONTROL Menu Principal]** no canto superior direito de [!DNL Adobe Workfront] e em **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Documentos]** > **[!UICONTROL Integração personalizada]**.
1. Selecione a integração personalizada que deseja desativar.
1. Clique em **[!UICONTROL Desabilitar]**.

   Os usuários não podem se conectar ao provedor de documentos de terceiros que você desabilitou, e não podem mais vincular documentos desse provedor de nuvem ao [!DNL Workfront].
