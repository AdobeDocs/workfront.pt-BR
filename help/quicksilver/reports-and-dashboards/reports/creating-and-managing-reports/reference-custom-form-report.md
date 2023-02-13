---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Referência a um formulário personalizado em um relatório
description: É possível fazer referência aos formulários personalizados de um objeto nas Exibições, Filtros e Agrupamentos de um relatório para esse objeto.
author: Nolan
feature: Reports and Dashboards
exl-id: 8b0d2e7f-cc92-4f43-a91c-ab2b2d8a1c01
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 2%

---

# Referência a um formulário personalizado em um relatório

É possível fazer referência aos formulários personalizados de um objeto nas Exibições, Filtros e Agrupamentos de um relatório para esse objeto.

Você pode fazer referência ao conteúdo de formulários personalizados a serem incluídos em um relatório ou pode fazer referência a informações sobre os próprios formulários personalizados a serem incluídos em um relatório.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Relatórios, Painéis, Calendários</p> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

O formulário personalizado deve existir antes que você possa referenciá-lo em um relatório.

Para obter mais informações sobre como criar formulários personalizados, consulte [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Referência do conteúdo de formulários personalizados

Você pode fazer referência a campos em formulários personalizados. Depois que um formulário personalizado é aplicado a um objeto, todos os campos associados a esse formulário personalizado ficam disponíveis para referência em um relatório, como qualquer outro campo no objeto estaria.

>[!NOTE]
>
>Para campos que têm várias opções, todas as opções estão disponíveis em Filtros e Prompts do relatório, incluindo aqueles que estão ocultos.\
>Para obter mais informações sobre como ocultar opções de um campo personalizado com várias opções, consulte o artigo [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

Ao criar o relatório, basta usar o tipo de objeto do formulário como fonte de campo e usar o nome do campo personalizado como nome do campo.

Por exemplo, você pode ter um formulário personalizado aplicado a todos os projetos que incluem o campo personalizado **Consultor**. Para criar um relatório que lista todos os projetos em que Olivia Kim é a consultora, use a **Projeto** tipo de objeto como fonte do campo e use **Consultor** como o nome do campo. Defina o qualificador de filtro como **Igual** Então digite Olivia Kim.

![](assets/qs-consultant-filter-example-350x126.png)

Para obter mais informações sobre como criar um relatório, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Informações de referência sobre formulários personalizados

É possível fazer referência a informações sobre formulários personalizados, como o nome de qualquer formulário personalizado associado a um objeto.

&#x200B; Dependendo do elemento (Exibir, Filtro ou Agrupamento), você pode fazer referência a:

* O formulário personalizado principal aplicado a um objeto:

   Este é o formulário que aparece primeiro na página Detalhes do objeto.

* Todos os formulários personalizados (se mais de um formulário personalizado for aplicado a um objeto)

Você pode fazer referência a formulários personalizados em Exibições, Filtros e Agrupamentos:

* [Referência a formulários personalizados em uma Exibição de relatório (Coluna)](#reference-custom-forms-in-a-report-view-column)
* [Referência a formulários personalizados em um filtro de relatório](#reference-custom-forms-in-a-report-filter)
* [Referência a formulários personalizados em um Agrupamento de relatório](#reference-custom-forms-in-a-report-grouping)

### Referência a formulários personalizados em uma Exibição de relatório (Coluna) {#reference-custom-forms-in-a-report-view-column}

Para exibir todos os formulários personalizados associados a um objeto:

1. Comece a criar um relatório conforme descrito no artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. No **Colunas** , expanda o tipo de objeto ao qual o formulário personalizado que deseja referenciar é aplicado e clique em **Nome da categoria**.\
   Por exemplo, para exibir todos os formulários personalizados associados a uma tarefa, expanda a **Tarefa** fonte do campo e clique no botão **Nome da categoria** nome do campo.\
   ![](assets/qs-category-name-column-350x267.png)

Para exibir somente o formulário personalizado principal associado ao objeto:

1. Comece a criar um relatório conforme descrito no artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. No **Colunas** , expanda a **Categoria** fonte do campo e clique no botão **Nome** nome do campo.\
   ![](assets/qs-category-name-column-2-350x248.png)

### Referência a formulários personalizados em um filtro de relatório {#reference-custom-forms-in-a-report-filter}

Para filtrar todos os formulários personalizados associados ao tipo de objeto:

1. Comece a criar um relatório conforme descrito no artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. No **Filtros** guia , expandir **Categorias**, depois clique em **Nome**.\
   ![](assets/qs-categories-name-filter-350x311.png)

1. Selecione o qualificador de condição que deseja usar:

   * Blank
   * Não Branco
   * Contém
   * Não Contém (Distingue maiúsc. e minúsc.)
   * Igual (Distingue maiúsc. e minúsc.)
   * Não Igual (Distingue maiúsc. e minúsc.)

   Para obter mais informações sobre cada qualificador, consulte o artigo [Modificadores de filtro e condição](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >Se o campo que você está filtrando tiver várias opções e usar a variável **Diferente de** ou **Does Not Contain** qualificadores, isso filtra os resultados que contêm apenas a escolha especificada. Se o campo contiver opções adicionais, incluindo a especificada, esses resultados não serão filtrados do relatório. Isso inclui a filtragem de vários Forms personalizados, se eles estiverem anexados ao mesmo objeto.

1. Comece digitando o nome do formulário personalizado que deseja filtrar e clique no nome quando ele for exibido na lista suspensa.
1. (Opcional) Clique em **Adicionar outra regra de filtro** e repita as etapas de 2 a 4 para criar regras de filtro adicionais.
1. Clique em **Salvar+Fechar**.

Para filtrar somente no formulário personalizado principal associado ao tipo de objeto:

1. Comece a criar um relatório conforme descrito no artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. No **Filtros** , expanda a **Categoria** fonte do campo e clique no botão **Nome** nome do campo.\
   ![](assets/qs-category-name-filter-350x437.png)

1. Selecione o qualificador de condição que deseja usar:

   * Blank
   * Não Branco
   * Contém
   * Não Contém (Distingue maiúsc. e minúsc.)
   * Igual (Distingue maiúsc. e minúsc.)
   * Não Igual (Distingue maiúsc. e minúsc.)

   Para obter mais informações sobre cada qualificador, consulte o artigo [Modificadores de filtro e condição](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. Comece digitando o nome do formulário personalizado que deseja filtrar e clique no nome quando ele for exibido na lista suspensa.
1. (Opcional) Clique em **Adicionar outra regra de filtro** e repita as etapas de 2 a 4 para criar regras de filtro adicionais.
1. Clique em **Salvar+Fechar**.

### Referência a formulários personalizados em um Agrupamento de relatório {#reference-custom-forms-in-a-report-grouping}

>[!NOTE]
>
>É possível agrupar itens somente pelo formulário personalizado principal associado ao objeto; não é possível agrupar itens por todos os formulários associados ao objeto.

1. Comece a criar um relatório conforme descrito no artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. No **Agrupamentos** guia , expandir **Categoria**, depois clique em **Nome**.\
   ![](assets/qs-category-name-grouping-350x373.png)
