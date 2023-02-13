---
product-area: projects
navigation-topic: issue-information
title: Use "opTask" e "problema" ao fazer referência a problemas
description: O nome de um problema aparece como opTask no banco de dados do Adobe Workfront. Embora algumas vezes você precise usar o nome do campo de ocorrência para se referir a problemas, na maioria das vezes, é necessário usar o nome do campo opTask em vez de emitir referência a problemas.
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# Use &quot;opTask&quot; e &quot;problema&quot; ao fazer referência a problemas

O nome de um problema aparece como `opTask` no banco de dados do Adobe Workfront. Embora algumas vezes você precise usar a variável `issue` nome do campo para se referir aos problemas, na maioria das vezes, é necessário usar o `opTask` nome do campo em vez de `issue` ao fazer referência a problemas.

Para obter mais informações sobre como os objetos aparecem no banco de dados do Workfront, consulte [API Explorer](https://one.workfront.com/s/api-explorer).

## `opTask` filename

Use o `opTask` nome do campo ao fazer referência a problemas nos seguintes contextos:

* Quando você cria um relatório personalizado de modo de texto para problemas e deseja fazer referência a problemas em exibições, filtros, agrupamentos ou prompts.

   Para obter mais informações sobre como usar o modo de texto em um relatório, consulte [Visão geral do modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

<!--* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)-->

* Ao atualizar campos de emissão em uma folha de importador de dados de Início Rápido.

   Para obter mais informações sobre como importar dados no Workfront usando um Início Rápido, consulte [Importar dados para o Adobe Workfront usando um modelo de Início rápido](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## `issue` nome do campo

Use o `issue` nome do campo para fazer referência a problemas nos seguintes contextos:

* Quando você faz referência a problemas em uma coleção usando o modo de texto em um relatório.
* Ao fazer referência a uma coleção de problemas usando a API do Workfront.

Para obter informações sobre relatórios sobre coleções, consulte [Fazer referência às coleções em um relatório](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

<!--
<note type="tip">
For information about how issues appear in a collection, see the
<a href="https://one.workfront.com/s/api-explorer" target="_blank">API Explorer</a> and select the API Unsupported option from the upper-right corner of the page.
<br>(NOTE: Drafted because this might not be needed.)
</note>
-->
