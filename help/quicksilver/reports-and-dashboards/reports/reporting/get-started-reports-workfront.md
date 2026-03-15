---
content-type: overview;reference
product-area: reporting
navigation-topic: reporting-navigation-topic
title: Introdução aos relatórios
description: Os relatórios fornecem visibilidade sobre o que está acontecendo com os usuários e o trabalho. Usando relatórios, você pode exibir informações sobre objetos no Adobe Workfront.
author: Courtney
feature: Reports and Dashboards
exl-id: 478512af-a47c-4488-878a-581e238e0064
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '3292'
ht-degree: 1%

---

# Introdução aos relatórios

<!-- Audited: 12/2023 -->

Os relatórios fornecem visibilidade sobre o que está acontecendo com os usuários e o trabalho. Usando relatórios, você pode exibir informações sobre objetos no Adobe Workfront.

Para obter informações sobre como entender objetos e como eles podem ser relatados no aplicativo Workfront, consulte [Visão geral de objetos do Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Elementos de relatório

Os relatórios são uma combinação dos três elementos a seguir no Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Exibir</td> 
   <td> <li>Define as colunas do relatório e quais informações podem ser incluídas em cada coluna.</li> <li>Para obter informações sobre exibições, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Visão geral de exibições no Adobe Workfront</a>.</li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Agrupamento</td> 
   <td> <li>Categoriza as informações com base em informações comuns e lista os resultados do relatório em títulos.</li> <li>Para obter informações sobre agrupamentos, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Visão geral de agrupamentos no Adobe Workfront</a>.</li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filtro</td> 
   <td> <li>Controla a quantidade de informações exibidas em um relatório.</li> <li>Para obter informações sobre filtros, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Visão geral sobre filtros</a>.</li> <li>Para obter informações sobre modificadores de filtro, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Modificadores de filtro e condição</a>.</li> <li>É possível filtrar usando curingas, para tornar seus filtros mais gerais e dar a eles mais flexibilidade de uso.</li> <li>Para obter informações sobre como usar curingas nos filtros, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">Variáveis de filtro de curingas</a>.</li> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Quando você seleciona um novo filtro, exibição ou agrupamento em uma lista, essa seleção é mantida mesmo se você sair do Workfront ou fechar o navegador.

Para obter informações sobre elementos de relatório, consulte [Elementos de relatório: filtros, exibições e agrupamentos](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

Para aprimorar seus relatórios, você pode adicionar os seguintes elementos:

* Um gráfico: uma representação visual dos resultados no relatório.\
  Para obter informações sobre relatórios de gráfico, consulte [Adicionar um gráfico a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Um agrupamento de matrizes: resume as informações do relatório em um formato de tabela agregada.\
  Para obter informações sobre relatórios de matriz, consulte [Criar um relatório de matriz](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

* Um prompt: um filtro aberto que pode ser personalizado e aplicado de forma diferente sempre que o relatório for executado.\
  Para obter informações sobre prompts, consulte [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

Ao criar um relatório, você pode modificar qualquer um desses elementos individualmente no Report Builder.

Outra maneira de aprimorar a relevância das informações incluídas em seus relatórios é aplicar formatação condicional às suas visualizações. Para obter informações sobre como usar a formatação condicional, consulte [Usar formatação condicional nas exibições](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Relatórios do sistema

O Workfront fornece vários relatórios de sistema que são carregados no sistema por padrão.\
Depois de inserir informações no sistema, você pode usar esses relatórios para exibir as informações visualmente.

Para obter mais informações sobre como acessar relatórios do sistema e quais relatórios do sistema estão disponíveis, consulte [Usar relatórios internos do Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

## Criar relatórios

Além dos relatórios de sistema fornecidos pela Workfront, você pode criar seus próprios relatórios personalizados para atender às necessidades da sua organização.

Para criar um relatório, siga um destes procedimentos:

* Crie um relatório do zero.
* Copiar um relatório existente.

  Você deve ter pelo menos a permissão Exibir para copiar um relatório criado por outra pessoa. Para obter mais informações sobre como copiar um relatório, consulte [Criar uma cópia de um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

Para obter informações sobre como criar relatórios, consulte [Criar um relatório personalizado](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### Pré-requisitos para a criação de relatórios {#prerequisites-for-creating-reports}

* Você deve ter uma licença Padrão ou de Plano para criar seus próprios relatórios.

  Para obter informações sobre os tipos de licença da Workfront, consulte [Visão geral de licenças](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md) para as licenças atuais e [Visão geral de novas licenças](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md) para as novas licenças.

* O administrador do Workfront deve fornecer acesso a Editar relatórios no seu nível de acesso.

  Para obter informações sobre como conceder acesso a Editar relatórios, consulte [Conceder acesso a relatórios, painéis e calendários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* O administrador do Workfront deve fornecer acesso a Editar filtros, Exibições e Agrupamentos no seu Nível de acesso.

  Para obter informações sobre como conceder acesso a Editar filtros, exibições e agrupamentos, consulte [Conceder acesso a filtros, exibições e agrupamentos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* Você deve definir um objeto sobre o qual deseja relatar. Os relatórios são específicos de objetos no Workfront e você deve começar selecionando um tipo de objeto antes de começar a criar o relatório. Você só pode gerar relatórios sobre objetos disponíveis na interface do Workfront.

### Denunciar propriedade {#report-ownership}

Ao criar um relatório no Workfront, você se torna o proprietário padrão do relatório e ele é exibido na seção Meus relatórios. Você não pode alterar o proprietário de um relatório.

Ao copiar um relatório, você automaticamente se torna o proprietário do relatório copiado.
Para obter informações sobre como copiar relatórios, consulte [Criar uma cópia de um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

Você pode ver quem possui um relatório ao revisar o campo **Inserido por**.

![Campo Inserido por](assets/unshimmed-entered-by.png)

### Criar relatórios na interface do construtor {#create-reports-in-the-builder-interface}

Recomendamos que você use primeiro a interface de criação de relatórios para criar um novo relatório. A interface oferece um conjunto simplificado de ferramentas que orientam você na criação de elementos para criar o relatório desejado. Você tem objetos e campos que pode selecionar nas listas e adicionar a todos os seus elementos de relatório.\
Para obter mais informações sobre como criar relatórios na interface de criação de relatórios, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para obter uma lista de objetos sobre os quais é possível gerar relatórios, consulte a seção [Relatório sobre objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#report-on-objects) no artigo [visão geral de objetos do Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

Para obter mais informações sobre os campos que podem ser exibidos nos relatórios, consulte o [Glossário de terminologia do Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

### Criar relatórios no Modo de Texto {#create-reports-in-text-mode}

Às vezes, você não consegue encontrar determinados campos na interface do construtor, mas eles podem estar disponíveis na API.\
Para obter informações sobre quais campos estão disponíveis na API, consulte o artigo [API Explorer](../../../wf-api/general/api-explorer.md).

Para obter informações sobre como usar o API Explorer, consulte o artigo [Como usar o API Explorer](../../../wf-api/general/using-api-explorer.md).

>[!NOTE]
>
>Não é possível gerar relatórios na interface do Workfront sobre objetos que não estão disponíveis no construtor de relatórios. No entanto, você pode gerar relatórios sobre campos associados aos objetos no construtor de relatórios se esses campos estiverem disponíveis por meio da API. Para fazer isso, use a interface Modo de texto.

O Modo de texto permite criar exibições, filtros, agrupamentos e prompts mais complexos, permitindo usar campos que não estão disponíveis na interface de modo padrão.

#### Terminologia do modo de texto {#text-mode-terminology}

É necessário usar uma sintaxe específica para usar a interface do Modo de texto do Workfront.

Para obter mais detalhes sobre a sintaxe do Workfront para o modo de texto, consulte [Visão geral da sintaxe do modo de texto](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

#### Colunas Calculadas, Formatação Condicional e outros usos do Modo de Texto {#calculated-columns-conditional-formatting-and-other-uses-of-text-mode}

Fora dos relatórios em campos que não estão disponíveis na interface do construtor, você pode usar o Modo Texto para exibir cálculos ou comparações entre determinados campos.

Para obter uma lista dos usos mais comuns do Modo Texto em um relatório, consulte [Visão geral dos usos comuns do Modo Texto](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

Para obter informações sobre como incluir dados personalizados calculados em relatórios, consulte [Dados personalizados calculados em relatórios](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

Para obter informações sobre como comparar campos na formatação condicional, consulte [Comparar campos na formatação condicional](../../../reports-and-dashboards/reports/text-mode/compare-fields-conditional-formatting.md).

Você também pode consultar os campos de coleta usando o Modo de texto nos relatórios.\
Para obter informações sobre como usar o Modo de Texto para exibir informações de coleção em um relatório, consulte [Referenciar coleções em um relatório](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

#### Amostras do Modo de texto {#text-mode-samples}

Temos uma biblioteca de amostras das exibições, filtros e agrupamentos mais usados que você pode criar com o Modo de texto.

Para navegar nesta biblioteca e usar algumas das amostras que oferecemos, consulte o artigo [Exibição personalizada, filtro e amostras de agrupamento: índice de artigo](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md).

## As guias de um relatório

Um relatório pode conter várias guias quando você o executa na interface.

Para obter informações sobre como executar um relatório, consulte o artigo [Executar um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md).

Em cada guia, as informações incluídas no relatório são exibidas em formatos um pouco diferentes. Escolha o formato que melhor atenda às necessidades de sua organização.

Você pode tornar qualquer guia a guia padrão do relatório. A guia padrão é a primeira guia exibida ao clicar no nome de um relatório para abri-lo, e é a guia exibida ao colocar o relatório em um painel.

### Guia Detalhes {#details-tab}

A guia Detalhes de um relatório exibe o objeto dos relatórios e os atributos escolhidos para esse objeto em um formulário de lista. Todos os relatórios têm uma guia Details.

>[!IMPORTANT]
>
>As informações na guia Detalhes podem ser exibidas de forma diferente da guia Gráfico com base no seu fuso horário.\
>Por exemplo, um usuário na Califórnia concluiu uma tarefa às 21h00 (horário do Pacífico) em 12 de fevereiro. :30 Quando um usuário em Nova York exibe um relatório que inclui a conclusão dessa tarefa, a Data de Conclusão Real é exibida como 13 de fevereiro na guia Detalhes e nos detalhes do Gráfico porque foi concluída às 12:30 am EST em 13 de fevereiro. Entretanto, no gráfico, ele será incluído no agrupamento de 12 de fevereiro até que você expanda o elemento do gráfico.

### Guia Resumo {#summary-tab}

Os relatórios que incluem um agrupamento têm uma guia Resumo.

As mesmas informações exibidas no formato de lista na guia Detalhes são resumidas e agregadas de acordo com os agrupamentos no relatório na guia Resumo.

Para obter informações sobre agrupamentos, consulte [Visão geral de agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

### Guia Matriz {#matrix-tab}

Os relatórios que incluem um Agrupamento de Matriz têm uma guia Matriz.

As mesmas informações exibidas no formato de lista na guia Detalhes são exibidas em um formato de tabela, agrupadas pelos agrupamentos no relatório na guia Matriz.

Quando você adiciona um agrupamento Matriz a um relatório, a guia Resumo é substituída pela guia Matriz.

Para obter informações sobre como criar um Agrupamento de Matriz, consulte o artigo [Criar um relatório de matriz](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

### Guia Gráfico {#chart-tab}

Os relatórios que incluem um gráfico têm uma guia Gráfico.

Considere incluir um gráfico em seus relatórios para painéis impactantes para seus executivos. Os gráficos são uma forma concisa de exibir as informações em um relatório. Você pode expandir um elemento de gráfico clicando nele para exibir os itens incluídos nesse elemento.

>[!IMPORTANT]
>
>Quando você clica em um elemento de gráfico, as informações expandidas podem ser exibidas de forma diferente do gráfico com base no seu fuso horário.\
>Por exemplo, um usuário na Califórnia concluiu uma tarefa às 21h00 (horário do Pacífico) em 12 de fevereiro. :30 Quando um usuário em Nova York exibe um relatório que inclui a conclusão dessa tarefa, a Data de Conclusão Real é exibida como 13 de fevereiro na guia Detalhes e nos detalhes do Gráfico porque foi concluída às 12:30 am EST em 13 de fevereiro. Entretanto, no gráfico, ele será incluído no agrupamento de 12 de fevereiro até que você expanda o elemento do gráfico.

Para obter informações sobre como criar um relatório com um gráfico, consulte o artigo [Adicionar um gráfico a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

### Guia Prompts {#prompts-tab}

Relatórios que incluem um prompt têm uma guia Prompts.

Um prompt permite que você adicione um filtro a um relatório sempre que executar o relatório. Quando você adiciona um prompt ao relatório, a guia Prompts se torna a guia padrão do relatório automaticamente. Isso não pode ser alterado para outra guia.

Para obter informações sobre como criar um prompt para um relatório, consulte o artigo [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

## Compartilhar relatórios

Depois de criar um relatório, você pode compartilhá-lo com outros usuários.

### Conceder permissões de compartilhamento a um relatório {#give-sharing-permissions-to-a-report}

Você pode conceder permissões de compartilhamento a outro usuário para que ele Visualize ou Gerencie um relatório que você criar. Você pode conceder a outro usuário um nível de permissões igual ou menor que o seu. Você também pode tornar um relatório público usando permissões de compartilhamento. Para obter informações sobre o compartilhamento de um relatório, consulte [Compartilhar um relatório no Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### Agendar a entrega de um relatório {#schedule-a-report-delivery}

Você pode agendar um relatório para entrega. Os usuários com os quais você está compartilhando o relatório recebem um email com um anexo dos resultados do relatório. O anexo pode estar nos seguintes formatos:

* HTML
* PDF
* Excel
* .TSV

Para obter informações sobre o agendamento da entrega de um relatório, consulte [Visão geral da entrega de relatórios](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

### Exportar os resultados de um relatório {#export-the-results-of-a-report}

É possível exportar os resultados de um relatório para os seguintes formatos de arquivo:

* PDF
* Excel (formatos .xls e .xlsx)
* Delimitado por tabulação

Para obter informações sobre como exportar os resultados de um relatório, consulte [Exportar dados](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

Depois que o relatório for exportado para um desses formatos, será possível compartilhá-lo com outros usuários enviando-o por email como um anexo ou imprimindo-o.

### Adicionar um relatório a um painel {#add-a-report-to-a-dashboard}

Você pode adicionar um relatório a um painel e compartilhar o painel com outros usuários. Para obter informações sobre como adicionar relatórios a um painel, consulte [Adicionar um relatório a um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

## Criar calendários

Se quiser exibir seus dados em um formato de calendário, crie calendários em vez de relatórios.

Para obter informações sobre a criação e o uso de calendários, consulte [Visão geral dos relatórios do calendário](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

## Uso do relatório

Depois de criar relatórios e compartilhá-los com outros usuários, você pode rastrear a frequência com que eles usam esses relatórios.
Para obter informações sobre o uso de relatórios, incluindo a frequência com que são exibidos, por qual usuário e em quais painéis são exibidos, consulte o artigo [Visão geral do uso de relatórios](../../../reports-and-dashboards/reports/report-usage/report-usage-overview.md).

## Termos comuns usados em referência a relatórios

Os termos a seguir são usados como referência aos relatórios da Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Termo ou Frase</strong> </th> 
   <th><strong>Definição</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Opções avançadas</td> 
   <td> <p>Refere-se ao link na guia Colunas (Exibição) do construtor de relatórios que fornece a capacidade de fazer o seguinte:</p> 
    <ul> 
     <li>Defina a formatação do estilo condicional da coluna para textos e imagens com base nos critérios selecionados.</li> 
     <li>Mude o rótulo da sua coluna.</li> 
     <li>Formate os valores na coluna.</li> 
    </ul> <p>Por exemplo, você pode desejar mostrar todas as tarefas-pai em negrito ou exibir a Data de Conclusão Planejada em vermelho se a tarefa estiver atrasada.</p> </td> 
  </tr> 
  <tr> 
   <td>Atributo</td> 
   <td> O campo de um objeto conforme definido no banco de dados. É usado em uma expressão do Modo de texto. <br>Por exemplo, o campo Status é exibido como <em>status</em> quando usado em uma expressão Text Mode. </td> 
  </tr> 
  <tr> 
   <td>Bean ou JavaBean</td> 
   <td>Um Bean representa um elemento de programação reutilizável. O termo Bean identifica relacionamentos entre diferentes objetos no aplicativo Workfront. É importante conhecer esses relacionamentos à medida que você tenta exibir atributos adicionais sobre um objeto que não estão disponíveis nas ferramentas básicas de geração de relatórios.</td> 
  </tr> 
  <tr> 
   <td>Interface ou Report Builder do Construtor</td> 
   <td>A Interface do construtor é a série de menus suspensos que contêm campos exibidos nas guias Colunas (Exibição), Filtro e Agrupamento. Ele fornece um mapeamento intuitivo das relações de Bean para auxiliar na identificação das colunas em uma visualização, os critérios de um filtro e os atributos comuns de um agrupamento.</td> 
  </tr> 
  <tr> 
   <td>Camel Case</td> 
   <td> <p>Camel Case refere-se a uma maneira específica de escrever elementos de programação para string atributos multi-word juntos. Ao soletrar um atributo no Camel Case, a primeira letra da primeira palavra é minúscula, não há espaço entre as palavras e a primeira letra de qualquer palavra subsequente é maiúscula.</p> <p>Por exemplo, o Grupo Doméstico seria gravado como <em>homeGroup</em>, o Pool de Recursos seria <em>resourcePool</em> e a Data de Início Real seria <em>atualStartDate</em>.</p> </td> 
  </tr> 
  <tr> 
   <td>Gráfico</td> 
   <td> <p>Uma guia dentro do construtor de relatórios, uma guia de relatório, depois que você salvar o relatório, bem como um elemento opcional de um relatório que permite adicionar um gráfico a qualquer relatório. Você deve definir um Agrupamento no relatório antes de criar um gráfico.</p> <p>Veja a seguir os tipos de gráficos que podem ser adicionados a qualquer relatório:<br></p> 
    <ul> 
     <li>Coluna</li> 
     <li>Barra</li> 
     <li>Pizza </li> 
     <li>Linha</li> 
     <li>Medidor</li> 
     <li>Bolha</li> 
    </ul> <p>Para obter mais informações sobre como adicionar gráficos a relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Adicionar um gráfico a um relatório</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Detalhes</td> 
   <td>Esta é uma das guias de um relatório depois que você o salva. Ela exibe as descobertas do seu relatório, exibidas na exibição e no agrupamento de sua escolha.</td> 
  </tr> 
  <tr> 
   <td>Expressão</td> 
   <td>Uma expressão é uma fórmula escrita no Modo de Texto para transmitir informações a serem pesquisadas ou exibidas ao usar a interface do Modo de Texto. Geralmente é uma linha em uma instrução de modo de texto maior.</td> 
  </tr> 
  <tr> 
   <td>Campos</td> 
   <td> <p>Refere-se aos atributos de seus objetos. Por exemplo, “Status” é um campo para Projetos, Tarefas ou Ocorrências. “Gerenciador de Portfolio" é um campo para o objeto Portfolio.</p> <p>Também é possível ter campos personalizados que você mesmo cria e adiciona aos formulários personalizados.<br>Para obter informações sobre como criar formulários personalizados, consulte o artigo <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Criar um formulário personalizado</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Nome do Campo </td> 
   <td>O valor de um atributo que é exibido em uma exibição ou usado na condição de um filtro ou como o elemento comum de um agrupamento. As opções para o Nome do campo dependem da seleção Origem do campo.</td> 
  </tr> 
  <tr> 
   <td>Origem do Campo </td> 
   <td>O valor de um objeto que é exibido em uma exibição, ou usado na condição de um filtro, ou como o elemento comum de um agrupamento. As opções na Origem do campo dependem do tipo de objeto do elemento de interface que está sendo criado. A Origem do campo permite que você faça referência a atributos de objetos que não sejam o tipo de objeto do elemento da interface.</td> 
  </tr> 
  <tr> 
   <td>Filtro</td> 
   <td>Um elemento principal do relatório que determina quais resultados são exibidos no relatório.</td> 
  </tr> 
  <tr> 
   <td>Formulário </td> 
   <td>Usado alternadamente com “Formulário personalizado”. Campos e seções são adicionados a formulários, que são então anexados a um objeto para estender o número de campos que você pode associar a um objeto.</td> 
  </tr> 
  <tr> 
   <td>Agrupamento </td> 
   <td>Um elemento principal do relatório que identifica como uma lista de resultados é organizada. O agrupamento cria barras horizontais em todo o relatório para agrupar os resultados por atributos comuns definidos ao criá-lo. Os agrupamentos são usados em Relatórios de Matriz para agregar dados, bem como em gráficos, para determinar os eixos dos gráficos.</td> 
  </tr> 
  <tr> 
   <td>Objeto ou tipo de objeto</td> 
   <td> Um objeto é um elemento de aplicativo do Workfront (por exemplo, Projeto, Tarefa, Grupo, Empresa, Filtro). O Tipo de Objeto é usado ao criar um novo relatório, exibição, filtro ou agrupamento para identificar qual objeto é o foco do relatório. Os relatórios podem ter somente um tipo de objeto, que é o objeto principal do relatório.<br>Objetos pai podem ser referenciados no mesmo relatório.<br>Para obter mais informações sobre a hierarquia de objetos, consulte a seção “Compreendendo a Interdependência e a Hierarquia de Objetos” no artigo <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Visão geral de objetos do Adobe Workfront</a>.</td> 
  </tr> 
  <tr> 
   <td>Prompt</td> 
   <td> <p>Um elemento de relatório opcional que pode ser adicionado a um relatório quando você precisa usar um filtro diferente toda vez que executa o relatório.</p> <p>Para obter informações sobre prompts, consulte <a href="/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md" class="MCXref xref">Adicionar um prompt a um relatório</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Qualificador ou Modificadores de Condição</td> 
   <td> <p>Esse campo aparece nas seguintes áreas de um relatório:</p> 
    <ul> 
     <li>Na guia Filtro</li> 
     <li>A tela Opções Avançadas da coluna na guia Colunas (Exibição). Definindo um qualificador, você pode comparar o Nome do Campo com outro campo ou valor.</li> 
     <li> Em um prompt personalizado<br><p>Para obter informações sobre prompts, consulte <a href="/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md" class="MCXref xref">Adicionar um prompt a um relatório</a>.</p>.</li> 
    </ul> <p>Por exemplo, ao criar um filtro para tarefas com uma Data de Conclusão Planejada de Hoje, você selecionaria <strong>Igual</strong> no campo Qualificador e a data de hoje no campo Data:</p> <p><em>Tarefa&gt; Data de conclusão planejada&gt;Igual&gt;(data de hoje)</em> </p> <p>Neste cenário, o Qualificador é <strong>Igual</strong>.<br>Para obter mais informações sobre qualificadores, consulte o artigo <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Modificadores de filtro e condição</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Relatório </td> 
   <td>A combinação de uma exibição, um filtro e (às vezes) um agrupamento. O objetivo de um relatório é exibir dados consistentemente na interface, distribuir informações e eliminar a necessidade de executar a mesma pesquisa ou consulta regularmente.</td> 
  </tr> 
  <tr> 
   <td>Demonstrativo</td> 
   <td>Consiste em várias expressões que são agrupadas para definir quais informações são exibidas em um relatório ao usar o modo de texto. Uma instrução pode ser criada para uma exibição, filtro, agrupamento ou para um Prompt Personalizado em um relatório.</td> 
  </tr> 
  <tr> 
   <td>Resumo</td> 
   <td>Esta é uma das guias de um relatório depois que você o salva. Esta guia é criada somente quando você define um agrupamento para o relatório. Ele resume informações com base no agrupamento definido durante a criação do relatório e fornece uma visão geral rápida dos objetos agregados do relatório. Ele não exibe todos os objetos no relatório, apenas os que estão agregados.</td> 
  </tr> 
  <tr> 
   <td>Interface do modo de texto</td> 
   <td>Fornece a capacidade de criar ou modificar o código de exibições, filtros, agrupamentos e prompts personalizados originalmente criados por meio da Interface do Construtor. Sugere-se que os elementos de relatório sejam criados inicialmente por meio da interface do Construtor e, em seguida, convertidos no Modo de texto depois de serem salvos para simplificar a codificação de exibições, filtros, agrupamentos ou prompts avançados.</td> 
  </tr> 
  <tr> 
   <td>Interface do usuário (UI)</td> 
   <td>Refere-se aos componentes ou blocos de construção do que é exibido na tela de um usuário a qualquer momento.</td> 
  </tr> 
  <tr> 
   <td>Exibição (ou Colunas)</td> 
   <td>Um dos principais elementos de um relatório. Identifica os cabeçalhos de coluna que serão exibidos na lista de um relatório.</td> 
  </tr> 
 </tbody> 
</table>
