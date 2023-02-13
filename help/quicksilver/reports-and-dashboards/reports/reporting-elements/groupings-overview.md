---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Visão geral dos agrupamentos no Adobe Workfront
description: É possível adicionar agrupamentos para gerenciar o layout das informações em seus relatórios e listas.
author: Lisa
feature: Reports and Dashboards
exl-id: d050372e-c4a0-4c49-b220-5b35334ab8d0
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 0%

---

# Visão geral dos agrupamentos no Adobe Workfront

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This article was supposed to be replaced by "Groupings overview", but decided to keep this here because this is linked in too many places. "Create groupings" and "Edit existing groupings" have been added also (with videos) to replace portions of the old content here.) </p>
-->

É possível adicionar agrupamentos para gerenciar o layout das informações em seus relatórios e listas.

Você pode adicionar agrupamentos aos relatórios das seguintes maneiras:

* É possível criar agrupamentos editando agrupamentos existentes.

   Para obter informações sobre como personalizar um Agrupamento existente, consulte [Editar agrupamentos existentes](../../../reports-and-dashboards/reports/reporting-elements/edit-existing-groupings.md).

* Você pode criar agrupamentos do zero.

   Para obter informações sobre como criar um agrupamento do zero, consulte [Criar agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

Por padrão, os agrupamentos são mostrados em um destaque cinza ou azul no seu relatório ou lista. Os resultados do relatório ou lista são listados em seu agrupamento individual, sem destaque.

É possível adicionar até três agrupamentos a um relatório. Você pode organizar suas informações com até quatro agrupamentos criando um relatório de matriz. Para obter mais informações sobre relatórios de matriz, consulte [Criar um relatório de matriz](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

Em um relatório de agrupamento padrão, o primeiro agrupamento é uma cor mais escura, o segundo e o terceiro agrupamentos são mais leves. Não é possível personalizar a cor do destaque para o agrupamento nem a fonte do nome do agrupamento. O número entre parênteses após o nome do agrupamento representa o número de resultados nesse agrupamento. Se o relatório se estender por várias páginas, certifique-se de exibir *Todos* os resultados no relatório ou na lista para obter uma contagem precisa dos resultados em cada agrupamento.

![Amostra de agrupamento](assets/grouping-example-blue.png)

Considere o seguinte ao trabalhar com agrupamentos:

* Você pode personalizar as informações em agrupamentos existentes. Todos os usuários que podem visualizar os agrupamentos também podem ver suas alterações.
* O administrador do Workfront deve conceder acesso a Editar filtros, exibições e agrupamentos para criar agrupamentos.

   Para obter informações sobre a concessão de acesso a Filtros, Exibições e Agrupamentos, consulte [Conceder acesso a filtros, visualizações e agrupamentos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* Seu nível de permissões para um agrupamento determina como um agrupamento é salvo. Se você criou o agrupamento originalmente, é possível salvar as alterações; caso contrário, será solicitado que você salve uma versão do agrupamento. Se você fizer alterações em um agrupamento que tenha compartilhado com outras pessoas, isso também as afetará.
* Você pode personalizar um agrupamento que foi compartilhado com você somente se o usuário que o compartilhou tiver concedido acesso a Gerenciar. Para obter informações sobre compartilhamento de um agrupamento, consulte [Compartilhar um filtro, visualização ou agrupamento](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
* Não é possível editar um agrupamento em linha.
* Não é possível agrupar por campos personalizados de seleção múltipla (por exemplo, caixas de seleção) ou por campos que podem ter vários valores (por exemplo, Gerenciador de Recursos).

## Informações adicionais sobre agrupamentos

Você pode gerenciar ainda mais as informações do relatório ao usar os Agrupamentos, agregando os valores em cada coluna na linha Agrupamento, bem como classificar suas informações pelo campo do Agrupamento. Você também pode remover um Agrupamento quando ele não for mais necessário.

* [Valores agregados em agrupamentos](#aggregate-values-in-groupings)
* [Classificar por um agrupamento](#sort-by-a-grouping)
* [Remover um agrupamento](#remove-a-grouping)

### Valores agregados em agrupamentos {#aggregate-values-in-groupings}

Você pode agregar os dados exibidos em seu relatório na linha de agrupamento resumindo os valores em cada coluna do relatório. Para obter mais informações sobre o resumo dos dados da coluna em um agrupamento, consulte [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

>[!NOTE]
>
>As seguintes exceções se aplicam a objetos pai (por exemplo, tarefas pai) quando você está agregando valores para os seguintes campos em agrupamentos:
>
>* Todos os campos de número e moeda, exceto Horas Reais (por exemplo, Custo da Mão de obra Planejada/Real, Custo da Despesa Planejada/Real, Custo Planejado/Real, Horas Planejadas) agregam apenas os valores para as tarefas filhas e tarefas independentes. Eles não agregam os valores para as tarefas pai ou pais dos pais.
>* As Horas reais agregam os valores do principal e das tarefas independentes; eles não agregam os números dos pais das tarefas pai ou filho.
>* Os campos de dados personalizados para valores numéricos e de moeda agregam todas as tarefas: pais, filhos, pais e tarefas independentes.


### Classificar por um agrupamento {#sort-by-a-grouping}

Os agrupamentos não podem ser classificados. As exibições podem ser classificadas. Para classificar uma lista pelo valor capturado no agrupamento, você deve incluir esse mesmo valor em uma das colunas da exibição e aplicar a classificação na exibição. Dessa forma, a lista classifica pelo valor no agrupamento indiretamente (classifica pelo valor na exibição que também é capturado no agrupamento). Para obter mais informações sobre como criar exibições e classificar por valores dentro das exibições, consulte [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### Remover um agrupamento {#remove-a-grouping}

A forma como você remove um agrupamento depende da criação inicial do agrupamento ou do compartilhamento do agrupamento com você. Não é possível remover um agrupamento padrão.

* **Se você criou o agrupamento e o removeu**, o agrupamento é removido do sistema Workfront. O agrupamento não está mais disponível para nenhum usuário com o qual você compartilhou anteriormente.
* **Se o agrupamento foi compartilhado com você e você o removeu**, o agrupamento é removido somente para você. O usuário que o criou originalmente e qualquer outro usuário com o qual ele foi compartilhado ainda têm acesso ao agrupamento.

Para obter informações sobre como remover um agrupamento, consulte o artigo [Remover filtros, visualizações e agrupamentos](../../../reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).
