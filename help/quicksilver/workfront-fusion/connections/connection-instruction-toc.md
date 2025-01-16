---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: connections-annd-webhooks
title: Criar conexões em  [!DNL Adobe Workfront Fusion]
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: fb1a2af4-da58-48ba-85b5-1903d6a3ceda
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 1%

---

# Criar conexões em [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Conectar aos aplicativos: índice do artigo](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/connect-to-apps-toc.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

<!-- Audited: 3/2024-->

Uma conexão deve atender aos requisitos definidos pela API do aplicativo ou serviço Web ao qual ela se conecta. Por esse motivo, as instruções para configurar uma conexão variam com base no aplicativo ou serviço da Web. Este artigo pode ajudá-lo a identificar e localizar as instruções para conectar o [!DNL Adobe Workfront Fusion] ao aplicativo ou serviço Web escolhido.

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] plano</td>  
   <td> <p>Qualquer</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] licença</td>  
   <td> <p>Novo: [!UICONTROL Padrão]</p><p>Ou</p><p>Atual: [!UICONTROL Trabalho] ou superior</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licença**</td>  
   <td> 
   <p>Atual: nenhum requisito de licença [!DNL Workfront Fusion].</p> 
   <p>Ou</p> 
   <p>Herdados: Qualquer um </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Produto</td>  
   <td> 
   <p>Novo:</p> <ul><li>[!UICONTROL Select] ou [!UICONTROL Prime] Plano [!DNL Workfront]: sua organização deve comprar [!DNL Adobe Workfront Fusion].</li><li>Plano [!DNL Workfront] da [!UICONTROL Ultimate] [!DNL Workfront Fusion] incluído.</li></ul> 
   <p>Ou</p> 
   <p>Atual: sua organização deve comprar o [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conexão com um aplicativo ou serviço Web que não requer configuração

Na maioria dos casos, você pode usar o módulo para criar uma conexão com pouca ou nenhuma informação extra. [!DNL Workfront Fusion] manipula a autenticação automaticamente.

Para obter instruções sobre como criar uma conexão sem considerações especiais, consulte [Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas](../../workfront-fusion/connections/connect-to-fusion-general.md).

## Conectar a um aplicativo ou serviço Web [!DNL Microsoft]

A maioria dos aplicativos [!DNL Microsoft] em [!DNL Workfront Fusion] permite que você crie uma conexão sem informações adicionais.

As seguintes circunstâncias exigem etapas adicionais na criação de uma conexão:

* Usando módulos [!DNL Microsoft Dynamics 365].

  Para obter instruções, consulte [[!DNL Microsoft Dynamics 365] módulos](../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

* Conectando ao [!DNL Microsoft Graph API] usando um módulo [!UICONTROL HTTP]

  Para obter instruções, consulte [Chamar [!DNL MS Graph REST API] via [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Fazer uma solicitação OAuth 2.0] para o módulo](../../workfront-fusion/connections/call-the-ms-graph-rest-api.md).

## Conectar a um aplicativo ou serviço Web [!DNL Google]

O processo de conexão com os aplicativos do [!DNL Google] pode ser diferente de acordo com o tipo de conta do [!DNL Google] que você está usando. Além disso, as medidas de segurança do [!DNL Google] podem exigir configuração extra quando você estiver se conectando ao [!DNL Workfront Fusion].

Para obter mais informações, consulte:

* [Conectar [!DNL Adobe Workfront Fusion] a [!DNL Google Services] usando um cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)
* [Conectar [!DNL Adobe Workfront Fusion] a [!DNL Google Services] com medidas de segurança atualizadas](../../workfront-fusion/connections/connect-to-google-with-new-security-measures.md)

## Outros aplicativos que exigem configuração adicional

Os aplicativos a seguir não seguem a configuração básica para conexões [!DNL Workfront Fusion]. Você pode encontrar instruções para conectar esses aplicativos no artigo desse aplicativo.

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
   <td><a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md#connect" class="MCXref xref">Conectar [!DNL Adobe Workfront] a [!DNL Workfront Fusion]</a> em <a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md" class="MCXref xref">[!DNL Adobe Workfront] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Allocadia]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md#connect" class="MCXref xref">Conectar [!DNL Allocadia] a [!DNL Workfront Fusion]</a> em <a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md" class="MCXref xref">[!DNL Allocadia] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Anaplan]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md#connect" class="MCXref xref">Conectar [!DNL Anaplan] a [!DNL Workfront Fusion]</a> em <a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md" class="MCXref xref">[!DNL Anaplan] módulos</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL AWS S3]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md#connecti" class="MCXref xref">Conectar [!DNL AWS] a [!DNL Workfront Fusion]</a> em <a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md" class="MCXref xref">[!DNL AWS S3] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Azure DevOps]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md#connect" class="MCXref xref">Conectar [!DNL Azure DevOps] a [!DNL Workfront Fusion]</a> em <a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md" class="MCXref xref">[!DNL Azure DevOps] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Bynder]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md#connect" class="MCXref xref">Conectar [!DNL Bynder] a [!DNL Workfront Fusion] </a> em <a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md" class="MCXref xref">[!DNL Bynder] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL CloudConvert]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md#connect" class="MCXref xref">Conectar [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> em <a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md" class="MCXref xref">[!DNL CloudConvert] módulos</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL Cvent]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md#connect" class="MCXref xref">Conectar [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> em <a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md" class="MCXref xref">[!DNL Cvent] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Datadog]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md#connect" class="MCXref xref">Conectar [!DNL Datadog] a [!DNL Workfront Fusion]</a> em <a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md" class="MCXref xref">[!DNL Datadog] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL DocuSign]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md#connect" class="MCXref xref">Conectar [!DNL DocuSign] a [!DNL Workfront Fusion]</a> em <a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md" class="MCXref xref">[!DNL DocuSign] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Email</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/email-modules.md#connecti" class="MCXref xref">Conectar seu email a [!DNL Workfront Fusion]</a> nos módulos <a href="../../workfront-fusion/apps-and-their-modules/email-modules.md" class="MCXref xref">[!UICONTROL Email]</a></td>

<tr> 
   <td role="rowheader"> <p>[!DNL Gmail]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md#connect3" class="MCXref xref">Conectar [!DNL Gmail] a [!DNL Workfront Fusion]</a> em <a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md" class="MCXref xref">[!DNL Gmail] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Cloud]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect" class="MCXref xref">Conectar [!DNL Jira Cloud] a [!DNL Workfront Fusion]</a> em <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Server]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect2" class="MCXref xref">Conectar [!DNL Jira Server] a [!DNL Workfront Fusion]</a> em <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MariaDB]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md#connect" class="MCXref xref">Conectar [!DNL MariaDB] a [!DNL Workfront Fusion]</a> em <a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md" class="MCXref xref">[!DNL MariaDB] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Marketo]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md#connect" class="MCXref xref">Conectar [!DNL Marketo] a [!DNL Workfront Fusion]</a> em <a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md" class="MCXref xref">[!DNL Marketo] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MS Dynamics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md#connect" class="MCXref xref">Conectar [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> em <a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md" class="MCXref xref">[!DNL Microsoft Dynamics 365] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Qualtrics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md#connecti" class="MCXref xref">Conectando [!DNL Qualtrics] a [!DNL Workfront Fusion]</a> em <a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md" class="MCXref xref">[!DNL Qualtrics] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL ServiceNow]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md#connect" class="MCXref xref">Conectar [!DNL ServiceNow] a [!DNL Workfront Fusion]</a> em <a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md" class="MCXref xref">[!DNL ServiceNow] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>SFTP</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sftp.md#connect" class="MCXref xref">Conectar SFTP a [!DNL Workfront Fusion]</a> em <a href="../../workfront-fusion/apps-and-their-modules/sftp.md" class="MCXref xref">[!UICONTROL SFTP] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL SharePoint]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md#connect" class="MCXref xref">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> em <a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md" class="MCXref xref">[!DNL SharePoint] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Split.io]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md#connect" class="MCXref xref">Conectar [!DNL Split.io] a [!DNL Workfront Fusion] </a> em <a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md" class="MCXref xref">[!DNL Split.io] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Ampliar</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md#connect" class="MCXref xref">Conectar [!DNL Widen] a [!DNL Workfront Fusion] </a> em <a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md" class="MCXref xref">[!DNL Widen] módulos</a></td> 
  </tr> 
 </tbody> 
</table>
