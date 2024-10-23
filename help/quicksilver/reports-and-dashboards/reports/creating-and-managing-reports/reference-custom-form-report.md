---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Referenciar um formulário personalizado em um relatório
description: Você pode fazer referência aos formulários personalizados de um objeto nas Exibições, Filtros e Agrupamentos de um relatório para esse objeto.
author: Nolan
feature: Reports and Dashboards
exl-id: 8b0d2e7f-cc92-4f43-a91c-ab2b2d8a1c01
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 2%

---

# Referenciar um formulário personalizado em um relatório

Você pode fazer referência aos formulários personalizados de um objeto nas Exibições, Filtros e Agrupamentos de um relatório para esse objeto.

Você pode fazer referência ao conteúdo de formulários personalizados para incluir em um relatório, ou pode fazer referência a informações sobre os próprios formulários personalizados para incluir em um relatório.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis, calendários</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Pré-requisitos

O formulário personalizado deve existir antes que você possa referenciá-lo em um relatório.

Para obter mais informações sobre como criar formulários personalizados, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Fazer referência ao conteúdo de formulários personalizados

Você pode referenciar campos em formulários personalizados. Depois que um formulário personalizado é aplicado a um objeto, todos os campos associados a esse formulário personalizado ficam disponíveis para serem referenciados em um relatório como qualquer outro campo no objeto seria.

>[!NOTE]
>
>Para campos que têm várias opções, todas as opções estão disponíveis nos Filtros e Avisos do relatório, incluindo aqueles que estão ocultos.\
>Para obter mais informações sobre como ocultar opções de um campo personalizado com várias opções, consulte o artigo [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

Ao criar o relatório, basta usar o tipo de objeto do formulário como a fonte do campo e usar o nome do campo personalizado como o nome do campo.

Por exemplo, você pode ter um formulário personalizado aplicado a todos os projetos que incluem o campo personalizado **Consultor**. Para criar um relatório que liste todos os projetos em que Olivia Kim é a consultora, use o tipo de objeto **Projeto** como a origem do campo e use **Consultor** como o nome do campo. Defina o qualificador de filtro como **Igual** e digite Olivia Kim.

![](assets/qs-consultant-filter-example-350x126.png)

Para obter mais informações sobre como criar um relatório, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Informações de referência sobre formulários personalizados

Você pode fazer referência a informações sobre formulários personalizados, como o nome de quaisquer formulários personalizados associados a um objeto.

&#x200B;Dependendo do elemento (Exibição, Filtro ou Agrupamento), você pode fazer referência a:

* O formulário personalizado principal aplicado a um objeto:

  Este é o formulário que aparece primeiro na página Detalhes do objeto.

* Todos os formulários personalizados (se mais de um formulário personalizado for aplicado a um objeto)

Você pode fazer referência a formulários personalizados em Exibições, Filtros e Agrupamentos:

* [Fazer referência a formulários personalizados em uma Exibição de relatório (Coluna)](#reference-custom-forms-in-a-report-view-column)
* [Fazer referência a formulários personalizados em um Filtro de relatório](#reference-custom-forms-in-a-report-filter)
* [Fazer referência a formulários personalizados em um agrupamento de relatório](#reference-custom-forms-in-a-report-grouping)

### Fazer referência a formulários personalizados em uma Exibição de relatório (Coluna) {#reference-custom-forms-in-a-report-view-column}

Para exibir todos os formulários personalizados associados a um objeto:

1. Comece a criar um relatório conforme descrito no artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Na guia **Colunas**, expanda o tipo de objeto ao qual o formulário personalizado que você deseja referenciar é aplicado e clique em **Nome da Categoria**.\
   Por exemplo, para exibir todos os formulários personalizados associados a uma tarefa, expanda a origem do campo **Tarefa** e clique no nome do campo **Nome da Categoria**.\
   ![](assets/qs-category-name-column-350x267.png)

Para exibir somente o formulário personalizado principal associado ao objeto:

1. Comece a criar um relatório conforme descrito no artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Na guia **Colunas**, expanda a origem do campo **Categoria** e clique no nome do campo **Nome**.\
   ![](assets/qs-category-name-column-2-350x248.png)

### Fazer referência a formulários personalizados em um filtro de relatório {#reference-custom-forms-in-a-report-filter}

Para filtrar em todos os formulários personalizados associados ao tipo de objeto:

1. Comece a criar um relatório conforme descrito no artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Na guia **Filtros**, expanda **Categorias** e clique em **Nome**.\
   ![](assets/qs-categories-name-filter-350x311.png)

1. Selecione o qualificador de condição que deseja usar:

   * Blank
   * Não Branco
   * Contém
   * Não Contém
   * Igual
   * Não igual

   Para obter mais informações sobre cada qualificador, consulte o artigo [Filtro e modificadores de condição](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >Se o campo que você está filtrando tiver várias opções e você usar os qualificadores **Não Igual** ou **Não Contém**, isso filtra os resultados que contêm apenas a opção especificada. Se o campo contiver opções adicionais, incluindo a especificada, esses resultados não serão filtrados do relatório. Isso inclui a filtragem de vários Forms personalizados, se estiverem anexados ao mesmo objeto.

1. Comece digitando o nome do formulário personalizado que deseja filtrar e clique no nome quando ele aparecer na lista suspensa.
1. (Opcional) Clique em **Adicionar outra regra de filtro** e repita as etapas de 2 a 4 para criar regras de filtro adicionais.
1. Clique em **Salvar+Fechar**.

Para filtrar somente no formulário personalizado principal associado ao tipo de objeto:

1. Comece a criar um relatório conforme descrito no artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Na guia **Filtros**, expanda a fonte de campo **Categoria** e clique no nome de campo **Nome**.\
   ![](assets/qs-category-name-filter-350x437.png)

1. Selecione o qualificador de condição que deseja usar:

   * Blank
   * Não Branco
   * Contém
   * Não Contém
   * Igual
   * Não igual

   Para obter mais informações sobre cada qualificador, consulte o artigo [Filtro e modificadores de condição](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. Comece digitando o nome do formulário personalizado que deseja filtrar e clique no nome quando ele aparecer na lista suspensa.
1. (Opcional) Clique em **Adicionar outra regra de filtro** e repita as etapas de 2 a 4 para criar regras de filtro adicionais.
1. Clique em **Salvar+Fechar**.

### Fazer referência a formulários personalizados em um agrupamento de relatório {#reference-custom-forms-in-a-report-grouping}

>[!NOTE]
>
>Você pode agrupar itens somente pelo formulário personalizado principal associado ao objeto; não é possível agrupar itens por todos os formulários associados ao objeto.

1. Comece a criar um relatório conforme descrito no artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Na guia **Agrupamentos**, expanda **Categoria** e clique em **Nome**.\
   ![](assets/qs-category-name-grouping-350x373.png)
