---
product-area: reporting
navigation-topic: reporting-elements
title: "Elementos de relatórios: filtros, visualizações e agrupamentos"
description: Os principais elementos que cada lista e relatório deve ter no Workfront são um filtro, uma visualização e um agrupamento. Cada elemento fornece informações diferentes em qualquer relatório.
author: Nolan
feature: Reports and Dashboards
exl-id: 5697905e-42c0-403b-85d4-798a1a3a2e7f
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 0%

---

# Elementos de relatórios: filtros, visualizações e agrupamentos

<!-- Audited: 11/2024 -->

<!--AL: Add information here about all the different kinds of FVGs: in reports, in lists, beta, etc // OR: this article should be a high-level overview of reporting elements. Then, each type of element should have:</p>
<p>- overview for Filters</p>
<p>- create a filter</p>
<p>- share a filter</p>
<p>ALL in Reporting elements but the Shared ones should be linked to Basics> Sharing; some of the articles in the Basics> Navigation> Use lists might beed to link here as well-->

Há vários elementos que tornam uma lista ou um relatório possível no Adobe Workfront. Os principais elementos que cada lista e relatório deve ter são um filtro, uma visualização e um agrupamento. Cada elemento fornece informações diferentes em qualquer relatório.

## Considerações sobre elementos de relatórios

Considere o seguinte ao trabalhar com filtros, exibições e agrupamentos:

* Os elementos de relatórios funcionam como os blocos de construção dos relatórios. Eles definem a aparência de um relatório ou de uma lista, bem como as informações contidas no relatório ou na lista.
* Os relatórios no Workfront são específicos para um objeto. Você deve definir o objeto principal de um relatório antes de criá-lo. Portanto, todos os elementos de relatórios são específicos do objeto.
* O administrador do Workfront deve conceder acesso a filtros, visualizações e agrupamentos no seu nível de acesso para poder exibi-los ou editá-los em listas e relatórios.

  Para obter informações sobre como conceder acesso a filtros, exibições e agrupamentos, consulte [Conceder acesso a filtros, exibições e agrupamentos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* O administrador do Workfront deve conceder acesso aos relatórios, painéis e calendários no seu nível de acesso para poder visualizar ou editar relatórios.

  Para obter informações sobre como conceder acesso a relatórios, painéis e calendários, consulte [Conceder acesso a relatórios, painéis e calendários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Se você selecionar um filtro, uma visualização ou um agrupamento em um relatório ou lista, o Workfront manterá essa seleção para as listas desse objeto mesmo depois de fazer logout ou fechar o navegador. Por exemplo, se você selecionar uma exibição específica para um relatório de tarefa, essa seleção aparecerá para outras listas de tarefas, como a lista de tarefas em um projeto.

## Filtros

O filtro controla os resultados que aparecem em um relatório, normalmente restringindo os resultados de geral para específico. Funciona como uma peneira que captura somente as informações necessárias e as traz de volta ao seu relatório.

Por exemplo, se você quiser ver apenas as tarefas atribuídas ao usuário conectado, é possível criar um filtro chamado &quot;Minhas tarefas&quot;, definir os critérios que devem ser atendidos para o filtro e executar o relatório para exibir apenas as tarefas atribuídas ao usuário conectado.

Alguns atributos de filtros são:

* O Workfront fornece vários filtros para vários objetos por padrão.
* É possível personalizar os filtros que você possui ou gerencia.

  Para obter mais informações sobre filtros, consulte o artigo [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Visualizações

Ao definir a exibição de um relatório, você define quais informações incluir no relatório. Como todos os elementos de relatórios, as exibições são baseadas em um tipo de objeto.

Por exemplo, um modo de exibição de um relatório de tarefa poderia mostrar Datas de Vencimento, incluir detalhes financeiros importantes como Custo, ou ser usado para mostrar detalhes de Atribuições e Data de Entrega. As exibições podem ser usadas para fornecer uma variedade de detalhes sobre os dados no relatório.

Alguns atributos de visualizações são:

* Você pode usar uma visualização padrão do Workfront ou criar a sua própria visualização.
* Você pode aplicar exibições adicionais no campo suspenso Exibir após executar um relatório.
* Exibições adicionais substituem temporariamente a exibição definida ao criar o relatório; no entanto, a exibição padrão é exibida na próxima vez que você retornar ao relatório.

  Para obter mais informações sobre exibições, consulte o artigo [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Agrupamento

Um agrupamento controla como você organiza os dados, facilitando sua leitura e compreensão. Os agrupamentos criam barras horizontais em um relatório que exibe resultados listados juntos por atributos comuns. Você define os critérios de como deseja agrupar os resultados do relatório ao criar o agrupamento.

Por exemplo, agrupar uma lista de tarefas que abrangem vários projetos pelo nome do projeto organiza todas as respectivas tarefas que pertencem a um único projeto sob esse nome.

Alguns atributos de agrupamentos são:

* Os agrupamentos são um elemento de relatório obrigatório se você quiser adicionar um gráfico posteriormente ao relatório.
* Os agrupamentos exibem um valor agregado nos resultados.&#x200B;
* Os agrupamentos determinam o eixo em gráficos.
* Os agrupamentos determinam a identificação do cabeçalho nos relatórios de matriz.\
  Para obter mais informações sobre relatórios de matriz, consulte o artigo [Criar um relatório de matriz](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

* Os agrupamentos ajudam a criar a guia Resumo de um relatório, fornecendo os valores agregados do relatório.
* O Workfront fornece vários agrupamentos para objetos diferentes por padrão.
* É possível personalizar os agrupamentos que você possui ou gerencia.

  Para obter mais informações sobre agrupamentos, consulte [Visão geral sobre agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## Outros elementos de relatório

Além de filtros, visualizações e agrupamentos, você também pode adicionar os seguintes elementos a um relatório:

* **Prompt**: um filtro aberto que pode ser personalizado e aplicado de forma diferente sempre que você executar um relatório.\
  Para obter mais informações sobre prompts, consulte o artigo [Adicionar prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* **Gráfico**: você pode aprimorar seus relatórios adicionando um gráfico a eles e exibindo as informações de forma visual.\
  Para obter mais informações sobre gráficos em relatórios, consulte o artigo [Adicionar um gráfico a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).
