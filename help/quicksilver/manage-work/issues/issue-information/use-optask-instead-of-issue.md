---
product-area: projects
navigation-topic: issue-information
title: Use "opTask" e "issue" ao fazer referência a problemas
description: O nome de um problema aparece como opTask no banco de dados do Adobe Workfront. Embora haja ocasiões em que você precisa usar o nome do campo de problema para fazer referência a problemas, na maioria das vezes você deve usar o nome do campo opTask em vez de problema ao fazer referência a problemas.
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
source-git-commit: a00776ecd9f8dc14b9dce14ce9463c2bb709a363
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Use &quot;opTask&quot; e &quot;issue&quot; ao fazer referência a problemas

O nome de um problema aparece como `opTask` no banco de dados do Adobe Workfront. Embora haja ocasiões em que você precisa usar o nome de campo `issue` para fazer referência a problemas, na maioria das vezes você deve usar o nome de campo `opTask` em vez de `issue` ao fazer referência a problemas.

Para obter mais informações sobre como os objetos aparecem no banco de dados do Workfront, consulte o [API Explorer](https://developer.adobe.com/workfront/api-explorer/).

## Nome do campo `opTask`

Use o nome de campo `opTask` ao fazer referência a problemas nos seguintes contextos:

* Quando você cria um relatório personalizado em modo de texto para problemas e deseja referenciar problemas em exibições, filtros, agrupamentos ou prompts.

  Para obter mais informações sobre como usar o modo texto em um relatório, consulte [Visão geral do Modo Texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

<!--* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)-->

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
