---
product-area: reporting
navigation-topic: reporting-elements
title: Criar agrupamentos no Adobe Workfront
description: Você pode criar um agrupamento personalizado do zero ou personalizar um agrupamento existente.
author: Lisa
feature: Reports and Dashboards
exl-id: 64cc52b7-d97b-4b41-9101-530e7db2d26e
source-git-commit: 53a5aaed8880e6eb6227cc49d385a8ec182d481a
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# Criar agrupamentos no Adobe Workfront

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This is a third part of an article split in 3 about creating and customizing groupings (2 how-tos and one reference) </p>
-->

Os resultados de um relatório ou de uma lista podem ser organizados com um agrupamento. Os agrupamentos categorizam as informações com base em uma determinada informação.

Você pode criar um agrupamento personalizado do zero ou personalizar um agrupamento existente. Siga as etapas abaixo para criar um agrupamento do zero.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Plano Adobe Workfront*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença da Adobe Workfront*</strong></td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Editar acesso a Relatórios, Painéis, Calendários para criar um agrupamento em um relatório</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Gerenciar permissões de um relatório para editar um agrupamento em um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Criar um agrupamento

1. Vá para o relatório ou a lista onde deseja criar o agrupamento personalizado.
1. Clique no botão **Agrupamento** ícone .

   ![Selecionar novo agrupamento](assets/newgrouping-nwe-standard-350x304.png)

1. Clique em **Novo agrupamento**.
O construtor de interface para criar as inicializações de agrupamento.

1. No **Visualização de agrupamento** seção , clique em **Adicionar agrupamento** para definir como deseja que as informações no relatório sejam organizadas. Uma visualização da aparência do agrupamento no relatório é mostrada abaixo.

1. Comece digitando o nome do campo que representa a maneira como você deseja organizar as informações no relatório e clique nele quando ele for exibido na lista suspensa.
1. (Opcional e condicional) Ao criar um agrupamento em uma lista atualizada, selecione **Recolher este agrupamento por predefinição** se desejar que os resultados no agrupamento exibam os resultados recolhidos em vez de expandidos. Essa configuração é desativada por padrão e os resultados do agrupamento sempre são exibidos na lista expandida.

   Para obter informações sobre listas atualizadas e herdadas, consulte a seção [A diferença entre as listas atualizadas e herdadas](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) no artigo [Introdução a listas no Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Edit existing grouping article and Common uses of text mode)</p>
   -->

   >[!TIP]
   >
   >* Ao ajustar manualmente os agrupamentos ao visualizar uma lista, o Workfront lembra de sua preferência manual até que você saia. Quando você faz logon novamente, a lista é exibida de acordo com essa configuração.
   >* Os resultados de um agrupamento sempre são expandidos depois de acessá-los a partir de um elemento de gráfico ou em uma lista herdada. Nesses casos, essa configuração é ignorada.


1. Repita as Etapas 4, 5 e 6 para definir agrupamentos adicionais.\
   É possível definir até três agrupamentos para organizar informações. Você pode ainda organizar suas informações com até quatro agrupamentos, criando um relatório de matriz. Para obter mais informações sobre relatórios de matriz, consulte [Criar um relatório de matriz](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. Clique em **Salvar Agrupamento**.

## Informações adicionais

Consulte também:

* [Visão geral dos agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)
* [Elementos de relatório: filtros, visualizações e agrupamentos](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)
* [Editar agrupamentos existentes](../../../reports-and-dashboards/reports/reporting-elements/edit-existing-groupings.md)

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h1>Create or edit groupings in Adobe Workfront</h1>
<p class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.</p>
<p>You can organize the results of a report or list with a grouping. Groupings categorize data based on a particular piece of information. For more information on groupings, see <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Groupings overview in Adobe Workfront</a>.</p>
<p>You can create groupings in lists and reports in the following ways:</p>
<ul>
<li> <p>From scratch</p> </li>
<li> <p>Edit an existing grouping that you originally created or that was shared with you</p> </li>
<li> <p>Copy an existing grouping</p> <p>To copy an existing grouping, you can edit it and save it as a new grouping.</p> </li>
</ul>
<h2>Types of grouping-building interfaces</h2>
<p>You can create groupings using the types of grouping builders described in the table below.</p>
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<col>
</col>
<tbody>
<tr>
<td><strong>Builder type</strong> </td>
<td><strong>Grouping object</strong> </td>
<td><strong>Where available</strong> </td>
</tr>
<tr>
<td><strong>Standard builder</strong> </td>
<td>All objects</td>
<td>Reports and lists</td>
</tr>
<tr data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<td rowspan="2">
<div class="preview">
<p><strong>Beta builder</strong> </p>
</div> </td>
<td>
<div class="preview">
<p>Projects</p>
<p>Tasks</p>
<p>Issues</p>
</div> </td>
<td>
<div class="preview">
<p>Lists</p>
</div> </td>
</tr>
<tr data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<td colspan="2"> <note type="note">
<span class="preview">Beta builders for groupings are not available in reports.</span>
</note> </td>
</tr>
</tbody>
</table>
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Consider the following when creating groupings using the different builders:
</div>
<ul data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<li>
<div class="preview">
You can switch back and forth between the standard builder and the beta builder, where the beta option is available.
</div> </li>
<li>
<div class="preview">
After you have enabled the beta builder in one area, it is the default experience for all areas where it is available.
</div> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><span class="preview">If you enable the beta builder in a project list, it is the default experience for building task and issue groupings in lists as well.</span> </p> </li>
<li> <p><span class="preview">Groupings are available in both builders, regardless of which experience you used to originally build them.</span> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><span class="preview">If you created a grouping using the standard builder, you can find and modify it in the beta builder interface as well.</span> </p> </li>
</ul>
<h2>Access requirements</h2>
<p>You must have the following access to perform the steps in this article:</p>
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
<tr>
<td role="rowheader">Adobe Workfront plan*</td>
<td> <p>Any</p> </td>
</tr>
<tr>
<td role="rowheader">Adobe Workfront license*</td>
<td> <p>Request or higher</p> </td>
</tr>
<tr>
<td role="rowheader">Access level configurations*</td>
<td> <p>Edit access to&nbsp;filters, views, and groupings</p> <note type="note">
If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see
<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.
</note> </td>
</tr>
<tr>
<td role="rowheader">Object permissions</td>
<td> <p>Manage access to a grouping to be able to modify or copy it</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td>
</tr>
</tbody>
</table>
<p>*To find out what plan, license type, or access you have, contact your Workfront administrator.</p>
<h2>Create a grouping in the standard builder</h2>
<p>Regardless of the method you use to create groupings, creating a grouping from scratch or from an existing grouping is similar.</p>
<ol>
<li value="1"> <p>Go to a list or a report where you want to create a grouping or that contains the grouping that you want to customize.</p> </li>
<li value="2"> <p>Click the <strong>Grouping</strong> icon .</p> <p> <img src="assets/newgrouping-nwe-standard-350x304.png" alt="Select New Grouping" style="width: 350;height: 304;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Click <strong>New Grouping</strong> at the top of the list of groupings.</p>
<p>Or</p>
<p>Hover over the grouping you want to modify and click the <strong>Edit</strong> icon <img src="assets/edit-icon.png">.</p>
</div> <p>The builder for customizing the grouping opens.</p> </li>
<li value="4"> <p>In the <strong>Grouping Preview</strong> section, click <strong>Add Grouping</strong> to define how you want information in the report to be organized. A preview of what the grouping looks like in the report is shown below.</p> </li>
<li value="5"> <p>Begin typing the name of the field that represents the way that you want to organize information in the report, then click it when it appears in the drop-down list.</p> </li>
<li value="6"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional and conditional) When customizing a grouping in an updated list, select <strong>Collapse this grouping by default</strong> if you want the results in the grouping to display collapsed rather than expanded.&nbsp;This setting is disabled by default and the results of the grouping always display in the expanded list.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> For information about updated and legacy lists, see the section <a href="../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated" class="MCXref xref">The difference between the updated and the legacy lists</a>&nbsp;in the article <a href="../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md" class="MCXref xref">Get started with lists in&nbsp;Adobe Workfront</a>.</p>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Edit existing grouping article and Common uses of text mode)</p>
<note type="tip">  
<ul>
<li>When you manually adjust groupings when viewing a list, Workfront remembers your manual preference until you log out. When you log back in, the list displays according to this setting.</li>
<li> <p>The results of a grouping always display expanded after accessing them from a chart element or in a legacy list. In these cases, this setting is ignored.</p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Legacy lists in classic do NOT have this option; legacy lists in NWE DO have this option but it's not functional; this is conditioned only for QS)</p>
</li>
</ul>
</note> </li>
<li value="7"> <p>Repeat Steps  4, 5, and 6  to define additional groupings.</p> <p>You can define up to three groupings for organizing information. You can further organize your information with up to four groupings by creating a matrix report. For more information on matrix reports, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">Create a matrix report</a>.</p> </li>
<li value="8"> <p>(Optional) Click <strong>Switch to Text Mode</strong> to add a grouping using the Text Mode interface.</p> <p>For more information about creating a grouping using the text mode interface, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md" class="MCXref xref">Edit text mode in a grouping</a>.</p> </li>
<li value="9"> <p>Click <strong>Save Grouping</strong> to create a new grouping.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Or</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Save as New Grouping</strong> to create a new grouping from the selected one.</p> <p>The new grouping displays in the list of groupings.</p> </li>
<li value="10"> <p>(Optional) Remove groupings you no longer want to display in the list.</p> <p>For information, see <a href="../../../reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md" class="MCXref xref">Remove filters, views, and groupings</a>.</p> </li>
</ol>
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<h2>Create a grouping in the beta builder</h2>
<h3>Enable the beta builder</h3>
<p>The beta builder toggle is disabled by default. You must enable it to use the beta builder.</p>
<ol>
<li value="1">Go to a project, task, or issue list.</li>
<li value="2"> <p>Click the <strong>Grouping</strong> icon <img src="assets/groupingicon.png" alt="Grouping icon">, then enable the beta builder toggle.</p> <p>The beta builder interface opens.</p> <note type="tip">
The header of the grouping builder interface is blue when the beta builder is enabled. This enables the beta builder for all areas of Workfront where it is available.
</note> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replace shot below!)</p>
<p> <img src="assets/beta-toggle-groupings-nwe-350x300.png" alt="Beta toggle for groupings" style="width: 350;height: 300;"> </p> </li>
<li value="3"> <p>Continue with <a href="#create-a-grouping-in-the-beta-builder" class="MCXref xref">Create a grouping in the beta builder</a>, below.</p> </li>
</ol>
<p><strong>Create a grouping in the beta builder</strong></p>
<ol>
<li value="1"> <p>Go to a project, task, or issue list where you want to create a grouping, and click the <strong>Grouping</strong> icon <img src="assets/groupingicon.png" alt="Grouping icon">.</p> </li>
<li value="2"> <p>Click <strong>New Grouping</strong> to create a new grouping.</p> <p>Or</p> <p>Hover over an existing grouping in the My groupings area, then click the <strong>Edit</strong> icon <img src="assets/edit-icon.png"> to edit an existing grouping.</p> <p>Or</p> <p>Hover over an existing grouping in the My groupings area, select the <strong>More</strong> icon <img src="assets/more-icon.png" alt="More icon">, and select <strong>Duplicate</strong> to copy a grouping.</p> </li>
<li value="3"> <p>Start typing the name of a field in the Group by area, then select it when it displays in the list.</p> <p>You can also select <strong>Search all fields</strong> to view a list of all fields to group by. The fields in the advanced search are grouped by object category.</p> <note type="tip">
As you build the grouping, the results appear immediately in the list.
</note> </li>
<li value="4"> <p>(Optional) Click <strong>Add grouping</strong> to add a second or third grouping.</p> <p> <img src="assets/gouping-groupby-options-350x202.png" alt="Group by options" style="width: 350;height: 202;"> </p> </li>
<li value="5"> <p>(Optional) To reorder the groupings, select a grouping and drag it to the new position.</p> <p>Or</p> <p>Select a grouping and use the keyboard arrow keys to change the order.</p> </li>
<li value="6"> <p>(Optional) Make other selections for the groupings as needed:</p>
<ul>
<li> <p>When grouping by date you must choose a date option such as week, month, or quarter.</p> </li>
<li> <p>Select <img src="assets/grouping-expandicon.png" alt="Expand grouping icon"> to set a grouping to be expanded by default.</p> </li>
<li> <p>Select <img src="assets/delete.png" alt="Delete icon"> to delete a grouping.</p> </li>
</ul> <p> <img src="assets/grouping-editgrouping-350x409.png" alt="Edit grouping" style="width: 350;height: 409;"> </p> </li>
<li value="7"> <p>(Optional) Select <strong>Text Mode</strong> to continue building the grouping using the Text Mode interface.</p> <p>For more information about creating a grouping using the text mode interface, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md" class="MCXref xref">Edit text mode in a grouping</a>.</p> </li>
<li value="8"> <p>(Optional) To use the grouping as an ad hoc grouping without saving it:</p>
<ul>
<li> <p>When working in a new grouping, close the beta builder.</p> </li>
<li> <p>When editing an existing grouping, select <strong>Apply</strong>.</p> </li>
</ul> </li>
<li value="9"> <p>Select <strong>Save as new</strong> for a new grouping, or <strong>Save</strong> for an existing grouping.</p> </li>
<li value="10"> <p>Type a name for the grouping.</p> </li>
<li value="11"> <p>(Optional) Select an icon for the grouping to represent the field type.</p> </li>
<li value="12"> <p>(Optional) Type a description of the grouping.</p> </li>
<li value="13"> <p>Select <strong>Save</strong>.</p> <p>The grouping is saved in the My groupings list.</p> </li>
</ol>
</div>
</div>
-->
