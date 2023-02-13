---
title: Desativar integrações de documentos
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: As [!DNL anAdobe] [!DNL Workfront] administrador, você pode desativar a conexão entre o Workfront e qualquer um dos provedores de documento de terceiros.
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 1%

---

# Desativar integrações de documentos

Como um [!DNL Adobe] [!DNL Workfront] administrador, você pode desativar a conexão entre [!DNL Workfront] e qualquer provedor de documento de terceiros.

Quando você desativa a conexão entre [!DNL Workfront] e um provedor de documentos, os links para os documentos desaparecem do [!DNL Workfront]. Os usuários não podem mais visualizar os documentos vinculados, não podem fazer alterações nos documentos por meio da [!DNL Workfront] e não podem adicionar mais documentos a esse provedor.

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador. Para obter informações sobre [!DNL Workfront] administradores, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Desativar integrações do provedor de nuvem

Para desativar integrações de documentos para [!UICONTROL Workfront DAM], [!DNL Box], [!DNL Dropbox], [!DNL Google Drive], [!DNL Microsoft OneDrive], [!DNL WebDAM]:

1. Faça logon em [!DNL Workfront] como [!DNL Workfront] administrador.
1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Documentos]** > **[!UICONTROL Provedores de nuvem]**.

1. Desmarque qualquer um dos provedores de nuvem dos quais deseja se desconectar [!DNL Workfront].
1. Clique em **[!UICONTROL Salvar]**.

   Os usuários não podem se conectar ao provedor de nuvem específico que você desativou e não podem mais vincular documentos desse provedor de nuvem ao Workfront.

## Desative o [!DNL SharePoint] integração

1. Faça logon em [!DNL Workfront] como [!DNL Workfront] administrador.
1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Expandir **[!UICONTROL Documentos]**, depois clique em **[!UICONTROL [!DNL SharePoint]Integração]**.
1. Selecione o [!DNL SharePoint] integração que você deseja desativar.
1. Clique em **[!UICONTROL Desativar]**.\
   Os usuários não podem se conectar ao [!DNL SharePoint] site do qual você desativou e que não pode mais vincular documentos [!DNL SharePoint] para [!DNL Workfront].

## Desativar integrações personalizadas

1. Faça logon em [!DNL Workfront] como administrador.
1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Documentos]** > **[!UICONTROL Integração personalizada]**.
1. Selecione a integração personalizada que deseja desativar.
1. Clique em **[!UICONTROL Desativar]**.

   Os usuários não podem se conectar ao provedor de documentos de terceiros desativado e não podem mais vincular documentos desse provedor de nuvem a [!DNL Workfront].
