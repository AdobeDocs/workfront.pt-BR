---
product-area: reporting
navigation-topic: reporting-elements
title: '"Elementos do relatório: filtros, visualizações e agrupamentos'
description: Os principais elementos que cada lista e relatório devem ter no Workfront são um filtro, uma visualização e um agrupamento. Cada elemento fornece informações diferentes em qualquer relatório.
author: Lisa
feature: Reports and Dashboards
exl-id: 5697905e-42c0-403b-85d4-798a1a3a2e7f
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 0%

---

# Elementos de relatório: filtros, visualizações e agrupamentos

<!--
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>AL: Add information here about all the different kinds of FVGs: in reports, in lists, beta, etc // OR: this article should be a high-level overview of reporting elements. Then, each type of element should have:</p>
<p>- overview for Filters</p>
<p>- create a filter</p>
<p>- share a filter</p>
<p>ALL in Reporting elements but the Shared ones should be linked to Basics> Sharing; some of the articles in the Basics> Navigation> Use lists might beed to link here as well</p>
</div>
-->

Há vários elementos que possibilitam uma lista ou um relatório no Adobe Workfront. Os principais elementos que cada lista e relatório devem ter são um filtro, uma visualização e um agrupamento. Cada elemento fornece informações diferentes em qualquer relatório.

## Considerações sobre elementos de relatório

Considere o seguinte ao trabalhar com filtros, exibições e agrupamentos:

* Os elementos de relatório funcionam como os blocos fundamentais do relatório. Eles definem a aparência de um relatório ou lista, bem como as informações contidas no relatório ou lista.
* Os relatórios no Workfront são específicos de um objeto. Você deve definir o objeto principal de um relatório antes de poder criar o relatório. Assim, todos os elementos de relatório são específicos de objeto.
* O administrador do Workfront deve conceder acesso a filtros, visualizações e agrupamentos no seu nível de acesso para poder visualizá-los ou editá-los em listas e relatórios.

   Para obter informações sobre a concessão de acesso a filtros, visualizações e agrupamentos, consulte [Conceder acesso a filtros, visualizações e agrupamentos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* O administrador do Workfront deve conceder acesso aos relatórios, painéis e calendários no seu nível de acesso para visualizar ou editar relatórios.

   Para obter informações sobre como conceder acesso a relatórios, painéis e calendários, consulte [Conceder acesso a relatórios, painéis e calendários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Se você selecionar um filtro, visualização ou agrupamento em um relatório ou lista, o Workfront manterá essa seleção nas listas desse objeto mesmo depois que você sair ou fechar o navegador. Por exemplo, se você selecionar uma exibição específica para um relatório de tarefa, essa seleção aparecerá para outras listas de tarefas, como a lista de tarefas em um projeto.

## Filtros

O filtro controla os resultados que aparecem em um relatório, normalmente reduzindo os resultados de geral para específico. Funciona como um crivo, capturando apenas as informações necessárias e trazendo essas informações de volta ao seu relatório.

Por exemplo, se você quiser ver apenas as tarefas atribuídas ao usuário conectado, poderá criar um filtro intitulado &quot;Minhas tarefas&quot;, definir os critérios que devem ser atendidos para o filtro e executar o relatório para exibir somente as tarefas atribuídas ao usuário conectado.

Alguns atributos de filtros são:

* O Workfront fornece vários filtros para vários objetos por padrão.
* Você pode personalizar os filtros que possui ou gerencia.

   Para obter mais informações sobre filtros, consulte o artigo [Visão geral dos filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

![Ícone de filtro](assets/projects-list-with-filter-drop-down-highlighted-nwe.png)

## Visualizações

Ao definir a exibição de um relatório, você define quais informações inclui. Como todos os elementos de relatório, as exibições são baseadas em um tipo de objeto.\
Por exemplo, uma exibição de um relatório de tarefa pode mostrar Datas de Vencimento, incluir detalhes financeiros principais, como Custo, ou ser usada para mostrar detalhes de Atribuições e Data de Entrega. As exibições podem ser usadas para fornecer uma variedade de detalhes sobre os dados no relatório.

Alguns atributos de exibições são:

* Você pode usar uma visualização padrão do Workfront ou criar a sua própria visualização.
* É possível aplicar exibições adicionais a partir do campo suspenso Exibição após executar um relatório.
* As exibições adicionais substituem temporariamente a exibição definida ao criar o relatório; no entanto, a exibição padrão será exibida na próxima vez que você retornar ao relatório.

   Para obter mais informações sobre visualizações, consulte o artigo [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Agrupamento

Um agrupamento controla como você organiza os dados, facilitando a leitura e a compreensão. Os agrupamentos criam barras horizontais em um relatório que exibe resultados listados juntos por atributos comuns. Você define os critérios de como deseja agrupar os resultados do relatório ao criar o agrupamento.

Por exemplo, agrupar uma lista de tarefas que abrangem vários projetos pelo nome do projeto organiza todas as tarefas respectivas que pertencem a um único projeto com esse nome.

Alguns atributos de agrupamentos são:

* Os agrupamentos são um elemento de relatório obrigatório se você quiser adicionar posteriormente um gráfico ao seu relatório.
* Os agrupamentos exibem um valor agregado nos resultados. &#x200B;
* Os agrupamentos determinam o eixo nos gráficos.
* Os agrupamentos determinam a identificação do cabeçalho nos relatórios de matriz.\
   Para obter mais informações sobre relatórios de matriz, consulte o artigo [Criar um relatório de matriz](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

* Os agrupamentos ajudam a criar a guia Resumo de um relatório, fornecendo os valores agregados do relatório.
* O Workfront fornece vários agrupamentos para diferentes objetos por padrão.
* Você pode personalizar agrupamentos que possui ou gerencia.

   Para obter mais informações sobre agrupamentos, consulte [Visão geral dos agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## Outros elementos de relatório

Além de filtros, visualizações e agrupamentos, você também pode adicionar os seguintes elementos a um relatório:

* **Aviso**: Um filtro aberto que pode ser personalizado e aplicado de forma diferente toda vez que você executa um relatório.\
   Para obter mais informações sobre prompts, consulte o artigo [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* **Gráfico**: Você pode aprimorar seus relatórios adicionando um gráfico a eles e exibindo as informações de forma visual.\
   Para obter mais informações sobre gráficos em relatórios, consulte o artigo [Adicionar um gráfico a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).
