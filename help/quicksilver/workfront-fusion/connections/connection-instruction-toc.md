---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: connections-annd-webhooks
title: Criar conexões em [!DNL Adobe Workfront Fusion]
description: Uma conexão deve atender aos requisitos definidos pela API do aplicativo ou serviço Web ao qual ela se conecta. Por esse motivo, as instruções para configurar uma conexão variam com base no aplicativo ou serviço da Web. Este artigo pode ajudá-lo a identificar e localizar as instruções de conexão [!DNL Adobe Workfront Fusion] ao aplicativo ou serviço da web escolhido.
author: Becky
feature: Workfront Fusion
exl-id: fb1a2af4-da58-48ba-85b5-1903d6a3ceda
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 0%

---

# Criar conexões em [!DNL Adobe Workfront Fusion]

Uma conexão deve atender aos requisitos definidos pela API do aplicativo ou serviço Web ao qual ela se conecta. Por esse motivo, as instruções para configurar uma conexão variam com base no aplicativo ou serviço da Web. Este artigo pode ajudá-lo a identificar e localizar as instruções de conexão [!DNL Adobe Workfront Fusion] ao aplicativo ou serviço da web escolhido.

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!UICONTROL Pro] ou superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licença**</td> 
   <td>
   <p>Requisito de licença atual: Não [!DNL Workfront Fusion] requisito de licença.</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e integração do trabalho] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o [!UICONTROL Select] ou o [!UICONTROL Prime] [!DNL Adobe Workfront] Planejar, sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no [!UICONTROL Ultimate] [!DNL Workfront] plano.</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td>

</tbody> 
</table>

Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conectar [!DNL Adobe Workfront] para [!DNL Workfront Fusion]

WORKFRONT e [!DNL Workfront Fusion] são projetados para trabalhar em conjunto. A conexão criada determina a conta que [!DNL Workfront Fusion] O usa o para executar ações no Workfront.

Para obter instruções, consulte [Conectar [!DNL Workfront] para [!DNL Workfront Fusion]](../../workfront-fusion/apps-and-their-modules/workfront-modules.md#connect) in [[!DNL Adobe Workfront] módulos](../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

## Conexão com um aplicativo ou serviço Web que não requer configuração

Na maioria dos casos, você pode usar o módulo para criar uma conexão com pouca ou nenhuma informação extra. [!DNL Workfront Fusion] O lida com a autenticação automaticamente.

Para obter instruções sobre como criar uma conexão sem considerações especiais, consulte [Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas](../../workfront-fusion/connections/connect-to-fusion-general.md).

## Conectar-se a um [!DNL Microsoft] aplicativo ou serviço da web

A maioria dos [!DNL Microsoft] aplicativos em [!DNL Workfront Fusion] permite criar uma conexão sem informações adicionais.

As seguintes circunstâncias exigem etapas adicionais na criação de uma conexão:

* Usar [!DNL Microsoft Dynamics 365] módulos.

  Para obter instruções, consulte [[!DNL Microsoft Dynamics 365] módulos](../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

* Conexão com o [!DNL Microsoft Graph API] usando um [!UICONTROL HTTP] módulo

  Para obter instruções, consulte [Chame o [!DNL MS Graph REST API] por meio da [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Fazer uma solicitação do OAuth 2.0] módulo](../../workfront-fusion/connections/call-the-ms-graph-rest-api-.md).

## Conectar-se a um [!DNL Google] aplicativo ou serviço da web

O processo de conexão com o [!DNL Google] aplicativos podem diferir com base no tipo de [!DNL Google] conta que você está usando. Além disso, [!DNL Google] medidas de segurança podem exigir configuração extra ao se conectar ao [!DNL Workfront Fusion].

Para obter mais informações, consulte:

* [Conectar [!DNL Adobe Workfront Fusion] para [!DNL Google Services] uso de um cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)
* [Conectar [!DNL Adobe Workfront Fusion] para [!DNL Google Services] com medidas de segurança atualizadas](../../workfront-fusion/connections/connect-to-google-with-new-security-measures.md)

## Outros aplicativos que exigem configuração adicional

Os aplicativos a seguir não seguem a configuração básica para [!DNL Workfront Fusion] conexões. Você pode encontrar instruções para conectar esses aplicativos no artigo desse aplicativo.

<table style="table-layout:auto">
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Aplicativo / Serviço da Web</th> 
   <th>Informações adicionais sobre conexões</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md#connect" class="MCXref xref">Conectar [!DNL Adobe Workfront] para [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md" class="MCXref xref">[!DNL Adobe Workfront] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Allocadia]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md#connect" class="MCXref xref">Conectar [!DNL Allocadia] para [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md" class="MCXref xref">[!DNL Allocadia] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Anaplan]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md#connect" class="MCXref xref">Conectar [!DNL Anaplan] para [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md" class="MCXref xref">[!DNL Anaplan] módulos</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL AWS S3]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md#connecti" class="MCXref xref">Conectar [!DNL AWS] para [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md" class="MCXref xref">[!DNL AWS S3] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Azure DevOps]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md#connect" class="MCXref xref">Conectar [!DNL Azure DevOps] para [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md" class="MCXref xref">[!DNL Azure DevOps] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Bynder]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md#connect" class="MCXref xref">Conectar [!DNL Bynder] para [!DNL Workfront Fusion] </a> in <a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md" class="MCXref xref">[!DNL Bynder] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL CloudConvert]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md#connect" class="MCXref xref">Conectar [!DNL CloudConvert] para [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md" class="MCXref xref">[!DNL CloudConvert] módulos</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL Cvent]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md#connect" class="MCXref xref">Conectar [!DNL Cvent] para [!DNL Adobe Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md" class="MCXref xref">[!DNL Cvent] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Datadog]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md#connect" class="MCXref xref">Conectar [!DNL Datadog] para [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md" class="MCXref xref">[!DNL Datadog] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL DocuSign]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md#connect" class="MCXref xref">Conectar [!DNL DocuSign] para [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md" class="MCXref xref">[!DNL DocuSign] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>email</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/email-modules.md#connecti" class="MCXref xref">Conectar seu email ao [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/email-modules.md" class="MCXref xref">[!UICONTROL Email] módulos</a></td>

<tr> 
   <td role="rowheader"> <p>[!DNL Gmail]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md#connect3" class="MCXref xref">Conectar [!DNL Gmail] para [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md" class="MCXref xref">[!DNL Gmail] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Cloud]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect" class="MCXref xref">Conectar [!DNL Jira Cloud] para [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Server]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect2" class="MCXref xref">Conectar [!DNL Jira Server] para [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MariaDB]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md#connect" class="MCXref xref">Conectar [!DNL MariaDB] para [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md" class="MCXref xref">[!DNL MariaDB] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Marketo]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md#connect" class="MCXref xref">Conectar [!DNL Marketo] para [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md" class="MCXref xref">[!DNL Marketo] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MS Dynamics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md#connect" class="MCXref xref">Conectar [!DNL Microsoft Dynamics 365] para [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md" class="MCXref xref">[!DNL Microsoft Dynamics 365] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Qualtrics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md#connecti" class="MCXref xref">Conectando [!DNL Qualtrics] para [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md" class="MCXref xref">[!DNL Qualtrics] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL ServiceNow]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md#connect" class="MCXref xref">Conectar [!DNL ServiceNow] para [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md" class="MCXref xref">[!DNL ServiceNow] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>SFTP</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sftp.md#connect" class="MCXref xref">Conectar SFTP a [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/sftp.md" class="MCXref xref">[!UICONTROL SFTP] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL SharePoint]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md#connect" class="MCXref xref">Conectar [!DNL SharePoint] para [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md" class="MCXref xref">[!DNL SharePoint] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Split.io]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md#connect" class="MCXref xref">Conectar [!DNL Split.io] para [!DNL Workfront Fusion] </a> in <a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md" class="MCXref xref">[!DNL Split.io] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Ampliar</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md#connect" class="MCXref xref">Conectar [!DNL Widen] para [!DNL Workfront Fusion] </a> in <a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md" class="MCXref xref">[!DNL Widen] módulos</a></td> 
  </tr> 
 </tbody> 
</table>
