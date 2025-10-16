---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: Agrupar um relatório por um campo personalizado de seleção múltipla
description: Você pode agrupar pelo valor em um campo personalizado de várias seleções em um relatório do Adobe Workfront somente usando o modo de texto.
author: Nolan
feature: Reports and Dashboards
exl-id: 530dff59-0d4c-490e-b464-1d3bb1d0f36f
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---

# Agrupar um relatório por um campo personalizado de várias seleções

<!--Audited: 10/2024-->

Você pode agrupar pelo valor em um campo personalizado de várias seleções em um relatório do Adobe Workfront somente usando o modo de texto.

Exemplos de campos personalizados de seleção múltipla são:

* Caixa de Seleção
* Menus suspensos de seleção múltipla

Para obter informações sobre como usar o modo de texto, consulte o artigo [Visão geral do Modo de Texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Considerações ao agrupar por um campo personalizado de seleção múltipla

* Não é possível criar um gráfico de um relatório que usa um agrupamento de modo de texto. É necessário criar um campo calculado adicional que se refira ao campo personalizado de seleção múltipla para também representar o gráfico do relatório pelo valor do campo personalizado de seleção múltipla.

  Para obter mais informações, consulte [Criar gráfico de um relatório por campo personalizado de várias seleções](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/chart-report-by-multi-select-custom-field.md).
* Os itens que têm qualquer uma das opções selecionadas são contados apenas uma vez.

  Por exemplo, se você tiver um campo personalizado Caixa de seleção com Opção 1 e Opção 2 como opções e anexar o formulário a tarefas, as tarefas que tiverem Opção 1 e Opção 2 selecionadas serão agrupadas separadamente das tarefas que tiverem apenas Opção 1 ou Opção 2 selecionadas.


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Colaborador ou Solicitação para modificar um filtro </p>
   <p>Padrão ou Plano para modificar um relatório</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar um filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Agrupar um relatório por campos personalizados de seleção múltipla

Para poder agrupar por um campo personalizado de seleção múltipla, você deve ter os seguintes pré-requisitos:

* Crie o campo personalizado de várias seleções em um formulário personalizado.\
  Para obter informações sobre como criar formulários personalizados e adicionar campos personalizados a eles, consulte o artigo [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

* Anexe o formulário personalizado a objetos.
* Preencha o campo personalizado de várias seleções com um valor em cada objeto.

Para agrupar por um campo personalizado de várias seleções em um relatório:

1. Crie um relatório ou edite um existente onde deseja adicionar um agrupamento para um campo personalizado de seleção múltipla.\
   Para obter informações sobre como criar relatórios, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Clique em **Ações de Relatório** e depois em **Editar**.
1. Selecione a guia **Agrupamentos**.
1. Clique em **Alternar para Modo de Texto**.

1. Selecione o texto na caixa **Agrupar por** e substitua-o pelo seguinte código:

   <pre>
   group.0.displayname=Nome de campo personalizado de seleção múltipla
   group.0.valueexpression={DE:Multi-select Custom Field Name}
   group.0.valueformat=HTML
   group.0.textmode=true
   </pre>

1. Substitua &quot;Nome do campo personalizado de seleção múltipla&quot; pelo nome real do seu campo personalizado de seleção múltipla, como ele aparece na instância do Workfront.
1. Clique em **Salvar e fechar**.

   Os objetos no relatório são agrupados pelos valores do campo personalizado de seleção múltipla.

   ![Agrupando meu campo de seleção múltipla](assets/grouping-by-multi-select-field-text-mode-ui-example.png)

   Os nomes dos agrupamentos do relatório são os nomes do campo personalizado de seleção múltipla seguido dos valores selecionados no campo.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Chart a report by multi-select Custom Fields</h2>
<p>(NOTE: this moved to its own article, linked in the Note above!)</p>
<p>You cannot build a chart in a report by referencing a multi-select custom field. Instead, you can create a calculated field that records the values of the multi-select custom field on a given object and group by the calculated field.&nbsp;</p>
<ul>
<li><a href="#build-a-calculated-custom-field-that-references-a-multi-select-custom-field" class="MCXref xref">Build a calculated custom field that references a multi-select custom field</a> </li>
<li><a href="#build-a-chart-that-references-a-calculated-custom-field" class="MCXref xref">Build a chart that references a calculated custom field</a> </li>
</ul>
<p><strong>Build a calculated custom field that references a multi-select custom field</strong></p>
<p>To be able to build a calculated field that references a multi-select custom field, you must have the following prerequisites:</p>
<ul>
<li>Build the multi-select custom field in a custom form.<br>.</li>
<li>Attach the custom form to objects.</li>
<li>Populate the multi-select custom field with a value on each object.</li>
</ul>
<p>To build the calculated custom field that references the multi-select custom field:</p>
<ol>
<li value="1">Create a custom form, or edit an existing one.<br>.</li>
<li value="2">Click<strong>Add a Field</strong>, then <strong>Calculated</strong> to add the multi-select custom field to the form.</li>
<li value="3">In the <strong>Label</strong> box, name the new calculated field to indicate that it references the multi-select custom field.<br>For example: "Calculated Multi-select Field."</li>
<li value="4"> <p>In the <strong>Calculation</strong> box, enter the following code:</p><pre>{DE:Multi-select Custom Field}</pre> <p> <img src="assets/calculated-multi-select-custom-field-350x201.png" style="width: 350;height: 201;"> <br> </p> </li>
<li value="5">Replace "Multi-select Custom Field" with the actual name of your multi-select custom field, as it appears in Workfront.</li>
<li value="6"> <p>(Optional) If the multi-select custom field is already on this form and if this form is already attached to objects, enable the <strong>Update previous calculations</strong>&nbsp;option.</p> <p>This ensures that the new field is automatically populated with the value from the multi-select custom field as it is added to the forms attached to the objects already.</p> </li>
<li value="7">Click <strong>Done</strong>.</li>
<li value="8">Click <strong>Save +Close</strong>.</li>
</ol>
<p><strong>Build a chart that references a calculated custom field</strong></p>
<ol>
<li value="1"> Go to the report where you want to add the chart for the calculated field that references the multi-select custom field. </li>
<li value="2"> (Optional) To ensure that all the calculated fields that you want to chart by are populated with values, select all the objects in your report, then click <strong>Edit</strong>. </li>
<li value="3"> <p> (Optional and conditional) Enable the <strong>Recalculate Custom Expressions</strong> field, then click <strong>Save Changes</strong>.</p> <p> <img src="assets/recalculate-custom-expressions-350x259.png" style="width: 350;height: 259;"> <br> </p> </li>
<li value="4"> Click <strong>Report Actions</strong>, then <strong>Edit</strong>. </li>
<li value="5">Select the <strong>Groupings</strong> tab, then click <strong>Add Grouping</strong>. </li>
<li value="6">Add the<strong>Calculated Multi-select Field</strong> you created as your grouping. </li>
<li value="7"> <p>Select the <strong>Chart</strong> tab, and add a chart to your report.</p> <p>For information about adding a chart to a report, see the section <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">Add a chart to a report</a> in the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>. </p> </li>
<li value="8">Select the <strong>Calculated Multi-select Field</strong> as one of the fields to display in the chart. </li>
<li value="9"> <p>Click <strong>Save + Close</strong>.</p> <p>The report displays the results grouped by the Calculated Multi-select Field in a chart. </p> </li>
</ol>
</div>
-->
