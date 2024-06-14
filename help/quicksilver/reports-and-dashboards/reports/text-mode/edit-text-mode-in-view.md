---
product-area: reporting
navigation-topic: text-mode-reporting
title: Editar uma visualização usando o modo de texto
description: "OBSERVAÇÃO: adicione uma seção a este artigo: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html *** Além disso, faça um rascunho desta área no artigo de visão geral do Modo de texto)"
author: Nolan
feature: Reports and Dashboards
exl-id: b99a2d14-a226-4075-9b1b-ac9426fd41b8
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 1%

---

# Editar uma visualização usando o modo de texto

<!--Audited: 01/2024-->

<!--
<add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html *** Also, draft this area in the Text Mode overview article) </p>
-->

É possível editar uma visualização em uma lista ou relatório usando o modo de texto para acessar campos que não estão disponíveis na interface padrão e criar visualizações mais complexas.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
   <td> <p>Novo: Padrão </p>
   <p>Atual: Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p> <p>Editar acesso a relatórios, painéis e calendários para editar elementos de relatórios em um relatório</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um relatório para editar exibições em um relatório</p> <p>Gerenciar permissões em uma exibição para editá-la</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.
Para obter mais informações sobre requisitos de acesso, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Antes de começar a usar o modo de texto em um relatório ou lista, sempre verifique se você está familiarizado com a sintaxe do modo de texto do Workfront.

Para obter mais informações, consulte:

* [Visão geral do modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Visão geral da sintaxe do modo de texto](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Exibição personalizada, filtro e amostras de agrupamento: índice do artigo](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Modo de edição de texto em uma visualização

A edição de uma visualização usando o modo de texto é idêntica para relatórios e listas. O acesso à visualização de um relatório ou de uma lista é diferente.

>[!TIP]
>
>Recomendamos que você crie o máximo possível da exibição no modo padrão e, em seguida, converta-a para o modo de texto para editá-la.

Para obter informações sobre a criação de exibições, consulte [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Para obter informações sobre como criar um relatório, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Siga um destes procedimentos:

   1. Para acessar a exibição de um relatório, vá para o relatório e clique em **Ações de Relatório** > **Editar** > **Colunas (Exibir)** guia.
   1. Para acessar a visualização em uma lista, vá para a lista e no **Exibir** menu suspenso, passe o mouse sobre a exibição que deseja modificar e clique no **Editar** ícone ![](assets/edit-icon.png).

      O construtor de exibições é aberto.

1. Selecione uma coluna na exibição.

   Ou

   Selecione o **Colunas (Exibir)** do report builder e, em seguida, selecione uma coluna.

   >[!TIP]
   >
   >Para editar uma visualização usando o modo texto, é necessário editar uma coluna de cada vez.

1. Clique em **Alternar para modo de texto** no canto superior direito do construtor.

   >[!NOTE]
   >
   >Ao editar uma coluna no modo texto, o Workfront adiciona a variável `textmode=true` linha de código para a coluna. Isso indica que a coluna é modificada no modo de texto.

   ![](assets/switch-to-text-mode-in-view-nwe-highlighted-350x447.png)

   A tabela a seguir descreve as linhas-chave em uma exibição de modo de texto:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make this a snippet and add it to the grouping article too)</p>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Linha de Exemplo</th> 
      <th>Descrição</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><ol><tr><tr><ol><tr><tr><tr><tr><tr><tr><tr><tr><tr><tr><div class="example" data-mc-autonum="<b>Example: </b>"><code><strong>valuefield</strong>=</cod></p> </td> 
      <td> <p>This is the name of the object or of the field as it appears in the database. For more information about how objects and fields appear in the database, see <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p>The following scenarios exist:</p> 
        
        <li value="1"> <p> If the name of the field you display is a phrase instead of a single noun, you must use camel case syntax for the <code>valuefield</code>. For example, for the Planned Start Date of a task the code is: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>If you want to display a custom field, the <code>valuefield</code> value is the actual name of the field, as you see it in the interface. For example, for a custom field named "More information", the code is:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valuefield=More information</code> </p> </li> 
        <li value="3"> <p>If you want to display objects that are related to other objects in a view using the <code>valuefield</code> line of code the object names and attributes are separated by colons. </p> <p>For example, a column in a task view that would display the name of the Portfolio Owner has the following value for the valuefield line:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valuefield=project:portfolio:owner:name</code> </p> <p>This indicates that from the object of the report (task), you can access the next related object (project), from there, you can access the following related object from project (portfolio), then the portfolio owner (owner) and then their name (name). </p> </li> 
       </ol> <p>For information about how objects connect to one another, see the section <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Interdependency and hierarchy of objects</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>.</p> <p>Note: If you choose a field in text mode that is not valid in the standard interface, you are not able to switch back to the standard interface within the column.</p> </td> 
     </tr> 
      
      <td><code><strong>valueformat=</strong></code> </td> 
      <td> <p>This line represents the format used to display the <code>valuefield</code>. The <code>valueformat</code> identifies whether an object or field displays as text, number, percentage, or date.</p> <p>We recommend using <code>HTML</code> for your <code>valueformat</code>, especially when using <code>valueexpression</code>, to ensure the most accurate display of your information. </p> <p>For information about additional values for this line, see <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Use conditional formatting in Text Mode</a>.</p> </td> 
     </tr> 
      
      <td> <p><code><strong>valueexpression=</strong></code> </p> </td> 
      <td> <p>You can add this line to replace <code>valuefield</code>, if you want to display a calculated field in the column.</p> <p>You must enclose the <code>valuefield</code> of the objects in curly brackets every time you use it in a <code>valueexpression</code>.</p> <p>The following scenarios exist: </p> 
        
        <li value="1"> <p>If you want to display a field in a column in upper case, you would use:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valueexpression=UPPER({valuefield})</code> </p> <p>The <code>valuefield</code> of the object is spelled as it appears in the API Explorer. </p> </li> 
        <li value="2">If you want to add multiple <code>valuefields</code> by stringing them together, you must separate them by a period.</li> 
        <li value="3"> <p>For example, if you want to display the name of the Primary Assignee of a task using <code>valueexpression</code>, you would use:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valueexpreesion={assignedTo}.{name}</code> </p> </li> 
        <li value="4"> <p>If you want to use a custom field in a <code>valueexpression</code> line you must precede the name of the field by <code>DE:</code> to indicate that it is a custom field. The name of the field is spelled as it appears in the interface. </p> <p>Important: When you use a custom field that is placed in a custom form section that has restricted permissions for some users, the calculation of the valueexpression is blank when those users view this calculation in a report. For information about adjusting permissions on custom form sections, see <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a></span>.</p> <p>For example, if you have a custom field labeled "Developer Name" and you want to display this field in upper case in a column, you can use the following <code>valueexpression</code> to indicate this:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valueexpression=UPPER({DE:Developer Name}</code>) </p> <p>When referencing a Typeahead type custom field, use the following expression to reference the name of the object selected in a field labeled "Developer Name":</p> <p><code>valueexpression=UPPER({DE:Developer Name:name})</code> </p> </li> 
       </ol> </td> 
     </tr> 
      
      <td> <p><code><strong>descriptionkey=</strong></code> / <code><strong>description=</strong></code> </p> </td> 
      <td> <p>This line defines the text of a tool tip as you mouse over the name of the column. In this case it is using a key to translate the name value in the description text. If you want to modify the description, change this line to read: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>description=Your Value</code>.</p> </td> 
     </tr> 
      
      <td><code><strong>namekey=</code> / <code><strong>name=</strong></code> </td> 
      <td> <p>This line defines the column label. In this case it is using the abbreviated value based on the key.</p> <p>If you want to modify the column name you can change this value to: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>name=Your Value</code> </p> <p><code>Name</code> allows you to enter any text for the column name, while<code>namekey</code> requires you enter a key that is used to translate the name of a column.</p> <p>To change the column name you can also add the <code>displayname </code>line, if one is not present.</p> </td> 
     </tr> 
      
      <td><code><strong>displayname =</strong></code> </td> 
      <td> <p>You can add the following line to change the name of a column, which suspends the <code>namekey/name</code> value:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>displayname=Your Value</code> </p> </td> 
     </tr> 
      
      <td><code><strong>querysort=</strong> </code></td> 
      <td>This line defines how the results are sorted when the column header is clicked. If it is not present then the column cannot be sorted after the report is run.</td> 
     </tr> 
      
      <td><code><strong>width=</strong></code> </td> 
      <td> <p>This line represents the number of pixels that are used for the column. If the line is omitted or set to 0 (zero) then the column does not appear in the view.</p> <p>When you modify this field manually in text mode, you must also add the <code>usewidths=true</code> value to your column.</p> </td> 
     </tr> 
      
      <td><code><strong>usewidths=true</strong></code> </td> 
      <td> <p>You must use this line in addition to the <code>width=</code> line when customizing the width of a column. </p> </td> 
     </tr> 
      
      <td><code><strong>makeFieldEditable=</strong></code> </td> 
      <td> <p>This line defines whether the value displayed in a column is inline editable or not. If this line equals <strong>true</strong>, the value in the column is inline editable. If this line equals <code>false</code>, the value in the column is not inline editable.</p> </td> 
     </tr> 
      
      <td><code><strong>link.valuefield=</strong> </code></td> 
      <td> <p>Insert this line only when you want the value displayed in a column to link to the object associated with it. The link opens the details page of the object. This value should match the <code>valuefield=</code> line. When you insert this, you must also add the <code>link.valueformat=</code> line. </p> <p> For example, you can insert <code>link.valuefield=priority</code> in an issue view, and the Priority of the issue displays as a link. Clicking this link opens the Issue page.</p> </td> 
     </tr> 
      
      <td><code><strong>link.valueformat=</strong> </code></td> 
      <td> <p>Insert this line only when you have inserted the <code>link.valuefield</code> line to add a link to the value in a column. The link opens the details page of the object. This value should match the <code>valueformat=</code> line and indicates the format used to display the <code>valuefield</code>. </p> <p>Important: When viewing the text mode in a built-in column that also includes a link, you notice a number of lines referring to the link. Some of those lines might no longer be supported or are unnecessary when you create your own custom column in text mode and add the link statements to it. The lines that are mandatory when adding a linked value are<code> link.valuefield</code> and <code>link.valueformat</code>. </p> </td> 
     </tr> 
      
      <td><code><strong>aggregator.function=</strong></code> </td> 
      <td> <p>This refers to how the values of each column are summarized. There are multiple lines that start with <code>aggregator.</code> and they all refer to the aggregator that summarizes the results of the column. </p> <p>As a general rule, the <code>aggregator.</code> lines match those of the column object. </p> 
       
        <span class="autonumber"><span><b>Example: </b></span></span> 
        <p>The Planned&nbsp;Hours column in a task report summarized by Sum may look like the following: </p>

   <div>
         <code>textmode=true</code>
         <code>valuefield=workRequired</code>
         <code>valueformat=compound</code>
         <code>aggregator.function=SUM</code>
         <code>aggregator.valuefield=workRequired</code>
         <code>aggregator.displayformat=minutesAsHoursString</code>
         <code>aggregator.valueformat=compound</code>
         <code>namekey=workRequired</code>
         <code>shortview=false</code> 
        </div> 
       </div>

   <div>
      A variável <code>aggregator. </code>as linhas podem conter um <code>valuefield </code>ou um <code>valueexpression</code>.
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Aplicar** se quiser salvar suas alterações e continuar editando a visualização.
1. Clique em **Salvar + Fechar** para salvar seu relatório.

   Ou

   Clique em **Salvar visualização** para salvar a visualização em uma lista.
