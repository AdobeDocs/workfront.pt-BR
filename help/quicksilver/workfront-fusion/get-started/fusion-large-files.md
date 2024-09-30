---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Trabalhar com arquivos grandes no Adobe Workfront Fusion
description: Atualmente, há suporte para arquivos grandes nos conectores Workfront e HTTP.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
source-git-commit: 630467ca64281df0b257dae8cc5c6edc55ae56ad
workflow-type: tm+mt
source-wordcount: '143'
ht-degree: 0%

---

# Trabalhar com arquivos grandes no Adobe Workfront Fusion

Alguns conectores Fusion podem suportar arquivos dimensionados acima do limite de 1 GB.

## Conectores compatíveis com arquivos grandes

No momento, há suporte para arquivos grandes nos seguintes conectores:

* Workfront
* HTTP

## Efeito do tamanho de arquivo grande no tempo de execução do cenário

Arquivos grandes podem levar algum tempo para carregar, baixar ou processar em seu cenário do Fusion. Embora não haja limite para o tamanho do arquivo, há um limite de 40 minutos no tempo de execução do cenário. Portanto, se arquivos grandes fazem com que a execução demore mais de 40 minutos, o cenário falha.

O tempo de execução do cenário também pode ser afetado pelo tamanho do cenário, pela complexidade do módulo e pela velocidade da rede. Portanto, recomendamos que você considere esses aspectos de seus cenários ao usar arquivos grandes.


<!--
## Connectors that do not support large files

Some Fusion connectors do not support large files. For these connectors, Fusion's total processing capacity for files is **1 GB**. 

This limit is based on a total memory cost. Every operation contributes to that cost. If a single file of 400 MB is downloaded and uploaded then the total cost to the file capacity would be 800 MB.

The following connectors do **not** support large files. 

* Archive
* Box
* Convert
* CSV
* Datastores
* Flow control
* FTP
* JSON
* JWT
* Markdown
* Math
* Microsoft Word templates
* MIME
* Microsoft SQL
* SFTP
* Adobe Acrobat Sign
* SOAP
* Tools
* XML

If a connector is not on this list, it does not support large files. For these connectors, Fusion's total processing capacity for files is **1 GB**. 

This limit is based on a total memory cost. Every operation contributes to that cost. If a single file of 400 MB is downloaded and uploaded then the total cost to the file capacity would be 800 MB.-->






<!--## Connectors that support large files

The following connectors support large files.

Workfront
HTTP
Webhooks
Salesforce
Microsoft Email
Workfront Proof
AEM Assets
Email
Slack
Jira
Microsoft Excel
SharePoint
Frame.io
Adobe PDF Services
Marketo
Azure Devops 
Google Email
Jira Server
Google Sheets
Microsoft OneDrive
ServiceNow 
AWS S3
Bynder
OneDrive Business
Adobe Authenticator
Google Drive
Microsoft Dynamics
Google Docs
NetSuite
Airtable
Azure AD
QuickBase 
Adobe Target
Adobe Campaign Classic
Microsoft Calendar
Workfront Planning
HubSpot CRM  
DropBox
Cloud Convert
Egnyte
Adobe Firefly
OpenAI / Chat GPT
Allocadia
Cvent
GitLab 
Google Team Drive
Google Calendar
Workfront SDL Managed Translation
Widen
Workfront Boards
Google Slides
Qualtrics
Microsoft Power BI
Adobe Photoshop
Anaplan
DocuSign 
MariaDB
Adobe Creative Cloud Libraries
Figma
AEM Forms
Datadog
GitHub 
Google Forms
Adobe I/O Events
Trello
Workday
Adobe Journey Optimizer
Adobe Lightroom









If a file is not on this list, it does not support large files. For these connectors, Fusion's total processing capacity for files is **1 GB**. 

This limit is based on a total memory cost. Every operation contributes to that cost. If a single file of 400 MB is downloaded and uploaded then the total cost to the file capacity would be 800 MB.

-->