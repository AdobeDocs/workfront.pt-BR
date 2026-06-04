---
product-area: projects
navigation-topic: issue-information
title: Usar "opTask" e "issue" ao fazer referência a problemas
description: O nome de um problema aparece como opTask no banco de dados do Adobe Workfront. Embora haja ocasiões em que você precisa usar o nome do campo de problema para fazer referência a problemas, na maioria das vezes você deve usar o nome do campo opTask em vez de problema ao fazer referência a problemas.
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jrNMdSfyMO3MgzcxxKSNtrgzuY3e4ZNJpJ-JdvylJN4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 257
ht-degree: 4%

---

# Use “opTask” e “issue” ao fazer referência aos problemas

<!--Audited: 08/2025-->

O nome de um problema aparece como `opTask` no banco de dados do Adobe Workfront. Embora haja ocasiões em que você precisa usar o nome de campo `issue` para fazer referência a problemas, na maioria das vezes você deve usar o nome de campo `opTask` em vez de `issue` ao fazer referência a problemas.

Para obter mais informações sobre como os objetos aparecem no banco de dados do Workfront, consulte o [API Explorer](https://developer.adobe.com/workfront/api-explorer/).

## Nome do campo `opTask`

Use o nome de campo `opTask` ao fazer referência a problemas nos seguintes contextos:

* Quando você cria um relatório personalizado em modo de texto para problemas e deseja referenciar problemas em exibições, filtros, agrupamentos ou prompts.

  Para obter mais informações sobre como usar o modo texto em um relatório, consulte [Visão geral do Modo Texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

<!--
* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)
  -->

* Ao atualizar campos de problema em uma folha do importador de dados de Início.

  Para obter mais informações sobre como importar dados no Workfront usando um Kick-Start, consulte [Importar dados para o Adobe Workfront usando um modelo Kick-Start](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## Nome do campo `issue`

Use o nome de campo `issue` para referenciar problemas nos seguintes contextos:

* Ao fazer referência a problemas em uma coleção usando o modo de texto em um relatório.
* Ao fazer referência a uma coleção de problemas usando a API do Workfront.

Para obter informações sobre relatórios de coleções, consulte [Coleções de referência em um relatório](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

<!--
<note type="tip">
For information about how issues appear in a collection, see the
<a href="https://developer.adobe.com/workfront/api-explorer/" target="_blank">API Explorer</a> and select the API Unsupported option from the upper-right corner of the page.
<br>(NOTE: Drafted because this might not be needed.)
</note>
-->
