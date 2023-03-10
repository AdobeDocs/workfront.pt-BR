---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Criar um relatório personalizado
description: Entender como criar relatórios ajuda a fornecer acesso às informações de que sua organização precisa no Adobe Workfront. Você pode usar qualquer um dos relatórios internos disponíveis no Workfront ou criar seus próprios relatórios do zero.
author: Nolan
feature: Reports and Dashboards
exl-id: 10c4df37-f09f-4b91-9cfd-3d0c3835bc7b
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '1821'
ht-degree: 1%

---


# Criar um relatório personalizado

Entender como criar relatórios ajuda a fornecer acesso às informações de que sua organização precisa no Adobe Workfront. Você pode usar qualquer um dos relatórios internos disponíveis no Workfront ou criar seus próprios relatórios do zero.

Para obter mais informações sobre relatórios internos, consulte [Usar relatórios internos do Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md). Para obter informações sobre como criar um relatório copiando-o, consulte [Criar uma cópia de um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

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
   <td> <p>Você obterá permissões de gerenciamento para o relatório que criar</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Criar um relatório {#create-a-report}

Para assistir a um vídeo de como criar um relatório, consulte este [Criar um relatório personalizado](#Walk-thr) abaixo.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito, em seguida, clique em **Relatórios**.
1. Clique em **Novo relatório** e, em seguida, selecione o tipo de objeto que deseja para o relatório.

   O construtor de relatórios é carregado.

   Para obter informações específicas sobre relatórios de objetos disponíveis, consulte a seção [Relatório sobre objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) no artigo [Entender objetos no Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

   ![](assets/nwe-select-new-report-350x666.png)

   >[!TIP]
   >
   >Você também pode criar um relatório fazendo uma cópia de um relatório existente. Para obter mais informações, consulte [Criar uma cópia de um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. No Construtor de relatórios, adicione o seguinte ao relatório:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Recurso</th> 
      <th>Descrição</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>Colunas (visualizar)</td> 
      <td> <p>Adicionar colunas ao seu relatório determina quais informações ele contém.</p> <p>Para saber como adicionar uma coluna, consulte <a href="#add-columns-view-to-a-report" class="MCXref xref">Adicionar colunas (exibição) a um relatório</a>.<br></p> </td> 
     </tr> 
     <tr> 
      <td>Agrupamento</td> 
      <td> <p>Adicionar agrupamentos ao seu relatório determina como ele é organizado.</p> <p>Para saber como adicionar um agrupamento, consulte <a href="#add-groupings-to-a-report" class="MCXref xref">Adicionar agrupamentos a um relatório</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Filtros</td> 
      <td> <p>Adicionar regras de filtragem ao relatório determina as informações que você vê no relatório.</p> <p>Para saber como adicionar um filtro, consulte <a href="#add-filters-to-a-report" class="MCXref xref">Adicionar filtros a um relatório</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Gráfico</td> 
      <td> <p>Adicionar um gráfico ao relatório determina como as informações nele são apresentadas visualmente.</p> <p>Para saber como adicionar um gráfico, consulte <a href="#add-a-chart-to-a-report" class="MCXref xref">Adicionar um gráfico a um relatório</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Em qualquer momento durante o processo de criação do relatório, clique em **Aplicar** para salvar as alterações.
1. Depois de terminar, clique em **Salvar + Fechar**.

### Adicionar colunas (exibição) a um relatório {#add-columns-view-to-a-report}

1. Comece a criar um relatório conforme descrito na [Criar um relatório](#create-a-report) neste artigo.
1. No Construtor de relatórios, selecione o **Colunas (Exibir)** para identificar as colunas a serem exibidas no relatório.
1. (Opcional) Clique em **Aplicar uma visualização existente** para usar uma exibição existente.

   Para obter mais informações sobre como criar uma nova exibição, consulte [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Para adicionar uma nova coluna, clique em **Adicionar coluna**.

   Ou

   Para alterar uma coluna existente, selecione a coluna que deseja alterar e clique no (x) ao lado do nome atual.

1. Comece digitando o campo que deseja adicionar. Se o campo estiver disponível, ele será preenchido para cada objeto ao qual pode ser associado. Clique no nome do campo para adicioná-lo à coluna .

   Para obter mais informações sobre os campos que você vê nas colunas, consulte [Glossário da terminologia do Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

   ![](assets/nwe-add-column-typeahead-350x459.png)

1. (Opcional) Na seção **Configurações de coluna** , selecione **Classificar por esta coluna** para classificar os valores na coluna em ordem crescente em ordem alfabética decrescente, indique se a lista deve usar essa coluna como primeira classificação.

   É possível ter vários níveis de classificações em uma exibição de relatório se desejar classificar pelo valor em uma coluna primeiro, o valor em uma segunda coluna, segundo, etc.

   Se vários resultados forem idênticos de acordo com o primeiro critério de classificação, eles classificarão na ordem do segundo critério de classificação. Se vários resultados forem idênticos de acordo com o primeiro e o segundo critérios de classificação, eles serão classificados de acordo com a terceira classificação etc.

   >[!NOTE]
   >
   >Se você adicionar um campo que faça referência a um objeto muito distante do objeto para o qual você está relatando, talvez não seja possível classificar por esse campo.\
   >Por exemplo, um relatório de problema não pode ser classificado pelo campo Proprietário do projeto porque ele faz referência a três objetos adicionais: Projeto, Proprietário e Nome. No entanto, ainda é possível adicionar esse campo a um relatório de problema e ver as informações dele.\
   >Para saber mais sobre referências entre objetos em relatórios, consulte a seção &quot;Parte 1 do 3 do relatório avançado&quot; na seção [Caminho de aprendizagem de relatórios e painéis](https://one.workfront.com/s/learningpath2/workfront-reporting-MC7MZT2BOL2ZC2LMJ4MA3EMHOCNY?tabset-dc70e=2).

1. (Opcional) Se você estiver usando agrupamentos e deseja resumir (agregar) as informações em uma coluna, clique no botão **Resumir esta coluna por** na lista suspensa na **Configurações de coluna** selecione a opção que deseja usar para agregar as informações na coluna .

   As informações agregadas são exibidas na coluna nas linhas de agrupamento.

   ![Resumo agregado em agrupamentos](assets/aggregate-summary-displays-on-groupings-2022-350x195.png)

   Para obter mais informações sobre o resumo de dados em uma coluna, consulte [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

   >[!NOTE]
   >
   >As seguintes exceções se aplicam a objetos pai (por exemplo, tarefas pai) quando você está agregando valores para os seguintes campos em agrupamentos:
   >
   >* Todos os campos de número e moeda, exceto Horas Reais (por exemplo, Custo da Mão de obra Planejada/Real, Custo da Despesa Planejada/Real, Custo Planejado/Real, Horas Planejadas) agregam apenas os valores para as tarefas filhas e tarefas independentes. Eles não agregam os valores para as tarefas pai ou pais dos pais.
   >* As Horas reais agregam os valores do principal e das tarefas independentes; eles não agregam os números dos pais das tarefas pai ou filho.
   >* Os campos de dados personalizados para valores numéricos e de moeda agregam todas as tarefas: pais, filhos, pais e tarefas independentes.


   Para obter mais informações sobre o uso de agrupamentos em um relatório, consulte [Visão geral dos agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. (Opcional) Clique em **Opções avançadas** para especificar as seguintes informações para a coluna:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Personalizar rótulo da coluna</td> 
      <td> <p>Especifique um rótulo personalizado para a coluna. Esse rótulo substitui o rótulo padrão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formato do campo</td> 
      <td> <p>Selecione o formato no qual deseja que os valores sejam exibidos para os campos na coluna .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostrar esta coluna quando estiver em um Painel</td> 
      <td> <p>Selecione essa opção para mostrar essa coluna em um painel, quando o relatório for exibido lado a lado com outro relatório. Quando essa opção não está selecionada, essa coluna não é exibida ao exibir o relatório em um painel em que os relatórios são exibidos lado a lado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Regras de colunas</td> 
      <td> <p>Clique em <strong>Adicionar uma regra para esta coluna</strong> para adicionar formatação condicional à coluna. Após adicionar uma regra, é possível definir estilos de campo e texto para a forma como os campos que correspondem a essa regra são exibidos. Clique em <strong>Adicionar regra</strong> depois que terminar de definir a regra. Para obter mais informações sobre a formatação condicional em uma exibição, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md" class="MCXref xref">Usar formatação condicional em exibições</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Aplicar** para aplicar suas alterações até o momento e continuar editando o relatório com as seguintes opções.

   Clique em **Salvar + Fechar** se tiver terminado de editar as colunas no relatório e quiser salvar o relatório.

### Adicionar agrupamentos a um relatório {#add-groupings-to-a-report}

1. Comece a criar um relatório conforme descrito na [Criar um relatório](#create-a-report) neste artigo.
1. No Construtor de relatórios, selecione o **Agrupamentos** para identificar como deseja agrupar itens no relatório.
1. Clique em **Adicionar agrupamento** para adicionar um novo agrupamento.

   Ou

   Choose **Aplicar um agrupamento existente** para selecionar um agrupamento existente
   ![](assets/nwe-add-grouping-350x230.png)

1. Comece digitando o campo que deseja adicionar como um agrupamento. Se o campo estiver disponível, ele será preenchido para cada objeto ao qual pode ser associado. Clique no nome do campo para adicioná-lo a esse agrupamento.
1. (Opcional) Você pode optar por criar um agrupamento no modo de texto clicando em **Alternar para o modo de texto**. Para obter mais informações sobre como usar o modo de texto, consulte [Visão geral do modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

   Para obter mais informações sobre como criar novos agrupamentos, consulte [Visão geral dos agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. (Opcional) Selecione **Recolher este agrupamento por predefinição** se desejar que os resultados deste agrupamento exibam os resultados recolhidos em vez de expandidos.

   Essa configuração é desativada por padrão e os resultados do agrupamento sempre são exibidos em uma lista expandida.

   >[!TIP]
   >
   >* Ao ajustar manualmente os agrupamentos ao visualizar uma lista, o Workfront lembra de sua preferência manual até que você saia. Quando você faz logon novamente, a lista é exibida de acordo com essa configuração.
   >* Os resultados de um agrupamento sempre são exibidos expandidos depois de acessá-los a partir de um elemento de gráfico.


1. (Opcional) Você pode optar por criar um agrupamento em matriz para mostrar seus resultados em um formato de grade.

   Para obter mais informações sobre como criar um relatório de matriz, consulte [Criar um relatório de matriz](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. Clique em **Aplicar** para aplicar suas alterações até o momento e continuar editando o relatório com as seguintes opções.

   Clique em **Salvar + Fechar** se tiver terminado de editar os agrupamentos no relatório e quiser salvar o relatório.

### Adicionar filtros a um relatório {#add-filters-to-a-report}

1. Comece a criar um relatório conforme descrito na [Criar um relatório](#create-a-report) neste artigo.
1. No Construtor de relatórios, selecione o **Filtros** para identificar a quantidade de informações que deseja que o relatório inclua.
1. Clique em **Adicionar uma regra de filtro** para adicionar um filtro personalizado.\
   Ou\
   Choose **Aplicar um filtro existente** para usar um filtro existente.

   ![](assets/nwe-add-a-filter-350x93.png)

1. Se você clicou **Adicionar uma regra de filtro**, comece digitando o campo que deseja adicionar como filtro. Se o campo estiver disponível, ele será preenchido para cada objeto ao qual pode ser associado. Clique no nome do campo para adicioná-lo a esse filtro.\
   Use modificadores de filtro para criar seu filtro. Para obter mais informações sobre modificadores de filtro, consulte [Modificadores de filtro e condição](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   Para obter mais informações sobre como criar novos filtros, consulte [Visão geral dos filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Opcional) Você pode optar por criar um filtro no modo de texto clicando em **Alternar para o modo de texto**.

   Para obter mais informações sobre como usar o modo de texto, consulte [Visão geral do modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

1. Clique em **Aplicar** quando você terminar de editar os filtros no relatório para aplicar suas alterações até agora e continuar editando o relatório com as seguintes opções.

   Clique em **Salvar + Fechar** se o relatório e você quiser salvar o relatório.

### Adicionar um gráfico a um relatório {#add-a-chart-to-a-report}

1. Comece a criar um relatório conforme descrito na [Criar um relatório](#create-a-report) neste artigo.
1. No Construtor de relatórios, selecione o **Gráfico** e selecione o tipo de gráfico que deseja adicionar.

   ![](assets/nwe-add-a-chart-350x247.png)

   Para obter mais informações sobre como criar um gráfico em um relatório, consulte [Adicionar um gráfico a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. Clique em **Aplicar** para aplicar suas alterações até o momento e continuar editando o relatório com as seguintes opções.

   Clique em **Salvar + Fechar** se você terminar de editar o relatório e quiser salvá-lo.
