---
title: Desabilitar Integrações de Documentos
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Como administrador do  [!DNL anAdobe] [!DNL Workfront], você pode desabilitar a conexão entre o Workfront e qualquer um dos provedores de documentos de terceiros.
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
author: Courtney, Becky
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 9%

---

# Desativar integrações de documentos

Como administrador do [!DNL Adobe] [!DNL Workfront], você pode desabilitar a conexão entre o [!DNL Workfront] e qualquer provedor de documentos de terceiros.

Quando você desabilita a conexão entre [!DNL Workfront] e um provedor de documentos, os links para os documentos desaparecem de [!DNL Workfront]. Os usuários não podem mais ver os documentos vinculados, não podem fazer alterações nos documentos por meio dos links [!DNL Workfront] e não podem adicionar mais documentos a esse provedor.

## Requisitos de acesso

+++Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table>
  <tr>
   <td>Pacote do Adobe Workfront
   </td>
   <td> <p>Prime ou Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr>
  <tr>
   <td>Licenças do Adobe Workfront
   </td>
   <td><p>Padrão</p>
   <p>Plano</p>
   </td>
  </tr>
   <tr>
   <td>Configurações de nível de acesso
   </td>
   <td>Você deve ser um administrador [!DNL Workfront].
   </td>
  </tr>
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Desabilitar integrações do provedor de nuvem

Para desabilitar integrações de documentos do [!UICONTROL Workfront DAM], [!DNL Box], [!DNL Dropbox], [!DNL Google Drive], [!DNL Microsoft OneDrive], [!DNL WebDAM]:

1. Faça logon em [!DNL Workfront] como administrador [!DNL Workfront].

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Documentos]** > **[!UICONTROL Provedores de Nuvem]**.

1. Desmarque qualquer um dos provedores de nuvem que você deseja desconectar de [!DNL Workfront].
1. Clique em **[!UICONTROL Salvar]**.

   Os usuários não podem se conectar ao provedor de nuvem específico desativado e não podem mais vincular documentos desse provedor de nuvem ao Workfront.

## Desabilitar a integração [!DNL SharePoint]

1. Faça logon em [!DNL Workfront] como administrador [!DNL Workfront].

{{step-1-to-setup}}

1. Expanda **[!UICONTROL Documentos]** e clique em **[!UICONTROL [!DNL SharePoint]Integração]**.
1. Selecione a integração do [!DNL SharePoint] que deseja desabilitar.
1. Clique em **[!UICONTROL Desabilitar]**.\
   Os usuários não podem se conectar ao site [!DNL SharePoint] que você desabilitou, e não podem mais vincular documentos de [!DNL SharePoint] a [!DNL Workfront].

## Desativar integrações personalizadas

1. Faça logon em [!DNL Workfront] como administrador.

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Documentos]** > **[!UICONTROL Integração personalizada]**.
1. Selecione a integração personalizada que deseja desativar.
1. Clique em **[!UICONTROL Desabilitar]**.

   Os usuários não podem se conectar ao provedor de documentos de terceiros que você desabilitou, e não podem mais vincular documentos desse provedor de nuvem ao [!DNL Workfront].
