---
product-area: reporting
navigation-topic: reporting-elements
title: Modificadores de filtro e condição
description: Os modificadores de filtro e condição permitem criar filtros e estabelecer condições para formatar os resultados do relatório.
author: Courtney
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '1593'
ht-degree: 0%

---

# Modificadores de filtro e condição

<!-- Audited: 11/2024 -->

<!--(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit)-->

Os modificadores de filtro e condição permitem criar filtros e estabelecer condições para formatar os resultados do relatório.

Para obter mais informações sobre a criação de filtros, consulte o artigo [Visão geral de filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

For more information about using conditional formatting in Views, see the article [Use conditional formatting in views](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Modificadores de filtro e condição

Some modifiers are built-in and you can choose them from a drop-down menu inside your filter or conditional formatting statement. Other modifiers can only be used in text mode filters.

For more information about understanding text mode, see [Text Mode overview](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

For a list of built-in time frame modifiers, see the article [Filter reports by timeframes](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md).

Você pode usar os seguintes modificadores de condição em filtros e instruções de formatação condicional:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Modificador Interno</strong> </p> </th> 
   <th> <p><strong>Modificador de Modo de Texto</strong> </p> </th> 
   <th> <p><strong>Descrição</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td> <p><strong>Está em Branco</strong> </p> </td> 
   <td> <p><strong>em branco</strong> </p> </td> 
   <td> <p>O campo existe para o objeto, mas atualmente não tem um valor.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Não Está Em Branco</strong> </p> </td> 
   <td> <p><strong>notblank</strong> </p> </td> 
   <td> <p>O campo que você está filtrando existe e recebeu um valor.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>nulo</strong> </p> </td> 
   <td> <p>O campo está em branco ou não existe. Por exemplo, você deseja procurar itens sem uma ID de tarefa pai. Isso significa que você deseja ver somente as tarefas independentes. The qualifier for the "parent task ID" would be <strong>null</strong>, since a task without an ID (in this case the parent) does not exist. </p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notnull</strong> </p> </td> 
   <td> <p>O campo que você está filtrando existe e contém um valor diferente de nulo.</p> <p>Este modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto nos filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Contém</strong> </p> </td> 
   <td> <p><strong>cicontém</strong> </p> </td> 
   <td> <p>Esta é a versão <i>sem distinção entre maiúsculas e minúsculas</i> de <strong>contém</strong>. Por exemplo: <code>cicontains inf</code> captura qualquer valor que contenha <code>Inf</code> ou <code>inf</code>.</p> <p> <p>Observação: O Adobe Workfront procura a palavra ou frase exata que você está especificando para cada instrução de filtro. Por exemplo, se você estiver pesquisando um projeto que contenha a frase <code>new project</code> no nome, o Workfront não exibirá projetos que tenham apenas <code>new</code> ou apenas <code>project</code>, ou <code>new main project</code> no nome. O filtro localiza somente projetos com a frase exata <code>new project</code> no nome.</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Does Not Contain</strong> </p> </td> 
   <td> <p><strong>cinotcontains</strong> </p> </td> 
   <td> <p>This is the <i>case insensitive</i> version of <strong>notcontains</strong>.</p><p>This modifier filters for items that are missing the value specified.</p> <p>For example, <code>does not contain inf</code> captures anything without <code>Inf</code> or <code>inf</code> in the name.</p> <p>Observação: quando aplicado a campos que contêm vários valores (como uma coleção de notas em um projeto), o filtro determina a exclusão da seguinte maneira:
<ul>
    <li>Se todos os itens em uma coleção contiverem o texto especificado, todo o registro será excluído dos resultados.</li>
    <li>Se pelo menos um item na coleção não contiver o texto especificado, o registro permanecerá nos resultados.</li>
</ul>
 </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>contains</strong> </p> </td> 
   <td> <p> Procura o texto <i>com distinção entre maiúsculas e minúsculas</i> especificado em uma cadeia de texto inteira.</p> <p>Por exemplo, o uso de <code>contains Inf</code> captura algo com <code>Inf</code>, como a palavra <code>Infinity.</code></p> <p>Este modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>nãocontém</strong> </p> </td> 
   <td> <p>It filters for items that are missing the <i>case sensitive</i> value specified.</p> <p>Por exemplo, <code>notcontains inf</code> captura qualquer item sem <code>inf</code>, mas exibe valores que contêm <code>Inf</code>.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo texto</a>.</p> </td> 
  </tr> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>Esta é a opção <i>que não diferencia maiúsculas de minúsculas</i> de <strong>eq</strong>. Ela só retorna uma correspondência exata do valor pesquisado.</p> <p>For example, when searching for a task with a specific name, <code>task name cieq test</code> finds tasks where the name is <code>Test</code>, <code>TEST</code>, or <code>Test</code>, but it does not find a task with the name <code>test 123.</code></p> <p>When searching for a status, the <strong>cieq</strong> modifier is not supported. You should use the case sensitive modifier, <strong>eq</strong>, to search for a status.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td>
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>cine</strong> </td> 
   <td> <p>Esta é a opção <i>não diferencia maiúsculas de minúsculas</i> de <strong>ne</strong> e é o oposto do modificador <b>cieq</b>. Ela só retorna resultados que não correspondem exatamente ao valor pesquisado, sem levar em conta a capitalização do valor.</p> <p>Por exemplo, <b>cine</b> retorna quaisquer valores que não sejam iguais a “current” ou “Current”. </p> <p>Este modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto nos filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr>   <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>This modifier returns only an exact, <i>case sensitive</i> match of the searched value.</p> <p>For example, when searching for complete projects, <code>eq CPL</code> returns all projects in the Complete status. <code>eq CPL, CUR</code> does not return a result because a project cannot be complete and current at the same time.</p> <p>Este modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto nos filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>ne</strong> </td> 
   <td> <p>Esta é a <i>distinção entre maiúsculas e minúsculas</i> oposta a <strong>eq</strong>. Ele retorna somente os resultados que não são uma correspondência exata do valor pesquisado e também corresponde às letras maiúsculas e minúsculas do valor.</p> <p>Por exemplo, <b>ne</b> retorna quaisquer valores que não sejam iguais a "Current", mas não retorna quaisquer valores que não sejam iguais a "current". </p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo texto</a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cidade</strong> </p> </td> 
   <td> <p> Esta é a versão <i>sem distinção entre maiúsculas e minúsculas</i> de <strong>pol</strong>.</p> <p>Este modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto nos filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cinotina</strong> </p> </td> 
   <td> <p>Esta é a versão <i>sem diferenciação de maiúsculas e minúsculas</i> de <strong>nãon</strong>.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto nos filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>Equal</strong> </p> </td> 
   <td> <p><strong>in</strong> </p> </td> 
   <td> <p>This modifier allows you to create a comma-separated list of <i>case sensitive</i> variables to compare to a single attribute evaluated in a filter. The entire list is treated as an OR statement and returns any results that meet the criteria of one or more of the variables.</p> <p>For example, when searching for projects, using <code>in CUR, PLN, CPL</code> returns all projects that are in the Current, OR Planning, OR Complete status.</p> <p>O modificador interno <strong>Equal</strong> corresponde ao modificador do modo de texto de <strong>in</strong>. Isso significa que você pode escolher Igual com vários valores para o campo.</p> <p>Por exemplo, você pode escolher um “Status igual a Atual, Planejamento, Inativo” em um relatório de projeto e pode exibir projetos em qualquer um desses status.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Não Igual</strong> </p> </td> 
   <td> <p><strong>não</strong> </p> </td> 
   <td> <p>Este é o oposto de <i>em</i>, que diferencia maiúsculas de minúsculas<strong>. </strong> Retorna apenas resultados que não estejam na lista especificada.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo texto</a>.</p> <p>Observação: <span>Se o campo que você está filtrando tiver várias opções, isso filtra os resultados que contêm tanto a opção especificada, quanto a opção especificada e qualquer opção adicional.</span> </p> </td> 
  </tr>
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>curtir</strong> </p> </td> 
   <td> <p>This modifier searches for portions of a <i>case sensitive</i> text string in similar fashion to <strong>contains</strong>. However, <strong>like</strong> provides the ability to insert wild card characters to break up the text.</p> <p>For example, when searching for notes, using <code>like %Current% %Dead%</code> returns any note that contains the phrase "Current to Dead". It does not include any notes that contain "Dead to Current". Each value is searched in the order it is listed. O % representa um curinga para substituir caracteres ou segmentos de texto. An underscore can also be used for a single wildcard character, as in <code>like Project_</code> that returns both "Project" and "Projects". If you intend on using a <strong>like</strong> or <strong>clike</strong> modifier in your filtering, we recommend avoiding % or _ characters in custom data field names, parameter option values, or other object names.</p><p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr>  
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cilike</strong> </p> </td> 
   <td> <p>Esta é a versão <i>sem distinção entre maiúsculas e minúsculas</i> de <strong>curtida</strong>. Por exemplo: <code>cilike %Current% %Dead%</code> retorna qualquer anotação que contenha <code>Current to Dead</code> ou <code>current to dead</code>.</p> <p>Este modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto nos filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong>Não Existe</strong> </td> 
   <td><strong>NOTEXISTS</strong> </td> 
   <td> <p>Este modificador é usado apenas com filtros complexos em uma instrução EXISTS. Esses filtros se referem apenas aos seguintes objetos: </p> 
    <ul> 
     <li>Objetos que abrangem vários níveis na hierarquia de objetos </li> 
     <li>Objetos ausentes </li> 
    </ul> <p>Para obter informações sobre como criar filtros complexos usando instruções EXISTS, consulte o artigo <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">Criar filtros complexos no modo texto usando instruções EXISTS</a>. Este é o único modificador usado em instruções EXISTS.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Greater Than</strong> </p> </td> 
   <td> <p><strong>gt</strong> </p> </td> 
   <td> <p>This searches for all results with a value greater than the value entered, not including the entered value.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Less Than</strong> </p> </td> 
   <td> <p><strong>lt</strong> </p> </td> 
   <td> <p>Pesquisa todos os resultados com um valor menor do que o inserido, sem incluir o valor inserido.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Maior Que Igual</strong> </p> </td> 
   <td> <p><strong>obter</strong> </p> </td> 
   <td> <p>Pesquisa todos os resultados com valores maiores ou iguais ao valor inserido.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Menor que Igual</strong> </p> </td> 
   <td> <p><strong>tarde</strong> </p> </td> 
   <td> <p>Pesquisa todos os resultados com um valor menor ou igual ao valor inserido.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Between</strong> </p> </td> 
   <td> <p><strong>between</strong> </p> </td> 
   <td> <p>Provides two required field values and searches for all results within range of both fields, including the entered values.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notbetween</strong> </p> </td> 
   <td> <p>This is the inverse of <strong>between</strong>. It provides two required value fields and searches for all results outside the range of both fields including the entered values.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo texto</a>.</p> </td> 
  </tr>

</tbody> 
</table>
