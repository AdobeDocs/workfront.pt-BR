---
product-area: reporting
navigation-topic: reporting-elements
title: Filtro e modificadores de condição
description: Os modificadores de filtro e condição permitem criar filtros e estabelecer condições para formatar os resultados do relatório.
author: Nolan
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: c915c282c6258300b01600dd5b6247e96bf45185
workflow-type: tm+mt
source-wordcount: '1566'
ht-degree: 0%

---

# Filtro e modificadores de condição

<!-- Audited: 1/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit) </p>
-->

Os modificadores de filtro e condição permitem criar filtros e estabelecer condições para formatar os resultados do relatório.

Para obter mais informações sobre a criação de filtros, consulte o artigo [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Para obter mais informações sobre como usar a formatação condicional em Exibições, consulte o artigo [Usar formatação condicional em exibições](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Filtro e modificadores de condição

Alguns modificadores são incorporados e você pode escolhê-los de um menu suspenso dentro do filtro ou da instrução de formatação condicional. Outros modificadores só podem ser usados em filtros de modo de texto.

Para obter mais informações sobre como entender o modo de texto, consulte [Visão geral do modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Para obter uma lista de modificadores de período incorporados, consulte o artigo [Filtrar relatórios por períodos de tempo](../../../reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md).

Você pode usar os seguintes modificadores de condição em filtros e instruções de formatação condicional:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Modificador embutido</strong> </p> </th> 
   <th> <p><strong>Modificador do modo de texto</strong> </p> </th> 
   <th> <p><strong>Descrição</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td> <p><strong>Está em Branco</strong> </p> </td> 
   <td> <p><strong>blank</strong> </p> </td> 
   <td> <p>O campo existe para o objeto, mas o campo não tem um valor no momento.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Não está em branco</strong> </p> </td> 
   <td> <p><strong>notblank</strong> </p> </td> 
   <td> <p>O campo que você está filtrando existe e recebeu um valor.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>null</strong> </p> </td> 
   <td> <p>O campo está em branco ou não existe. Por exemplo, você deseja procurar itens sem uma ID de tarefa pai. Isso significa que você deseja ver apenas as tarefas independentes. O qualificador para a "ID da tarefa pai" seria <strong>null</strong>, já que uma tarefa sem uma ID (neste caso, o pai) não existe. </p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notnull</strong> </p> </td> 
   <td> <p>O campo que você está filtrando existe e contém um valor diferente de nulo.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Contém</strong> </p> </td> 
   <td> <p><strong>cicontains</strong> </p> </td> 
   <td> <p>Este é o <i>não diferencia maiúsculas de minúsculas</i> versão de <strong>contém</strong>. Por exemplo: <code>cicontains inf</code> captura qualquer valor que contenha <code>Inf</code> ou <code>inf</code>.</p> <p> <p>Observação: O Adobe Workfront procura a palavra ou frase exata que você está especificando para cada instrução de filtro. Por exemplo, se você estiver pesquisando qualquer projeto que contenha a frase <code>new project</code> no nome, o Workfront não exibe projetos que tenham apenas <code>new</code> ou apenas <code>project</code>ou <code>new main project</code> no nome. O filtro localiza somente projetos com a frase exata <code>new project</code> no nome.</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Não contém</strong> </p> </td> 
   <td> <p><strong>cinotcontains</strong> </p> </td> 
   <td> <p>Este é o <i>não diferencia maiúsculas de minúsculas</i> versão de <strong>notcontains</strong>.</p><p>Esse modificador filtra itens cujo valor especificado está faltando.</p> <p>Por exemplo, <code>does not contain inf</code> captura tudo sem <code>Inf</code> ou <code>inf</code> no nome.</p> <p>Nota: <span>Se o campo que você está filtrando tiver várias opções, o filtra os resultados que contêm tanto a escolha especificada, quanto a especificada e quaisquer opções adicionais.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>contém</strong> </p> </td> 
   <td> <p> Procura pela variável especificada <i>diferencia maiúsculas de minúsculas</i> texto em toda a cadeia de texto.</p> <p>Por exemplo, usando <code>contains Inf</code> captura qualquer coisa com <code>Inf</code> nele, como a palavra <code>Infinity.</code></p> <p>Este modificador só pode ser usado em filtros do modo de texto. Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notcontains</strong> </p> </td> 
   <td> <p>Ele filtra por itens que não têm o <i>diferencia maiúsculas de minúsculas</i> valor especificado.</p> <p>Por exemplo, <code>notcontains inf</code> captura tudo sem <code>inf</code>, mas exibe valores que contêm <code>Inf</code>.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>Este é o <i>não diferencia maiúsculas de minúsculas</i> opção de <strong>eq</strong>. Ela só retorna uma correspondência exata do valor pesquisado.</p> <p>Por exemplo, ao pesquisar uma tarefa com um nome específico, <code>task name cieq test</code> localiza tarefas cujo nome é <code>Test</code>, <code>TEST</code>ou <code>Test</code>, mas não localiza uma tarefa com o nome <code>test 123.</code></p> <p>Ao pesquisar por um status, a variável <strong>cieq</strong> modificador não suportado. Você deve usar o modificador que diferencia maiúsculas de minúsculas, <strong>eq</strong>, para procurar um status.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td>
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>cine</strong> </td> 
   <td> <p>Este é o <i>não diferencia maiúsculas de minúsculas</i> opção de <strong>ne</strong>e é o oposto do <b>cieq</b> modificador. Ela só retorna resultados que não são uma correspondência exata do valor pesquisado, não levando em conta a caixa do valor.</p> <p>Por exemplo, <b>cine</b> retorna quaisquer valores que não sejam iguais a "current" ou "Current". </p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr>   <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>Esse modificador retorna somente um valor exato, <i>diferencia maiúsculas de minúsculas</i> correspondência do valor pesquisado.</p> <p>Por exemplo, ao pesquisar por projetos completos, <code>eq CPL</code> retorna todos os projetos com o status Concluído. <code>eq CPL, CUR</code> não retorna um resultado porque um projeto não pode ser concluído e atualizado ao mesmo tempo.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>ne</strong> </td> 
   <td> <p>Este é o <i>diferencia maiúsculas de minúsculas</i> oposto de <strong>eq</strong>. Ele retorna somente os resultados que não são uma correspondência exata do valor pesquisado e também corresponde às letras maiúsculas e minúsculas do valor.</p> <p>Por exemplo, <b>ne</b> retorna quaisquer valores que não sejam iguais a "Atual", mas não retorna quaisquer valores que não sejam iguais a "atual". </p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>ciin</strong> </p> </td> 
   <td> <p> Este é o <i>não diferencia maiúsculas de minúsculas</i> versão de <strong>in</strong>.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cinotina</strong> </p> </td> 
   <td> <p>Este é o <i>não diferencia maiúsculas de minúsculas</i> versão de <strong>not</strong>.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>Igual</strong> </p> </td> 
   <td> <p><strong>in</strong> </p> </td> 
   <td> <p>Esse modificador permite criar uma lista separada por vírgulas de <i>diferencia maiúsculas de minúsculas</i> variáveis a serem comparadas com um único atributo avaliado em um filtro. A lista inteira é tratada como uma instrução OU e retorna quaisquer resultados que atendam aos critérios de uma ou mais das variáveis.</p> <p>Por exemplo, ao pesquisar por projetos, usando <code>in CUR, PLN, CPL</code> retorna todos os projetos que estão no status Atual, OU Planejando, OU Concluído.</p> <p>O modificador incorporado <strong>Igual</strong> corresponde ao modificador de modo de texto de <strong>in</strong>. Isso significa que você pode escolher Equal with multiple values para o campo.</p> <p>Por exemplo, você pode escolher um "Status igual a Atual, Planejamento, Inativo" em um relatório de projeto e pode visualizar os projetos em qualquer um desses status.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Não Igual</strong> </p> </td> 
   <td> <p><strong>not</strong> </p> </td> 
   <td> <p>Este é o <i>diferencia maiúsculas de minúsculas</i> oposto de <strong>in</strong>. Retorna apenas resultados que não estão na lista especificada.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> <p>Nota: <span>Se o campo que você está filtrando tiver várias opções, o filtra os resultados que contêm tanto a escolha especificada, quanto a especificada e quaisquer opções adicionais.</span> </p> </td> 
  </tr>
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>curtir</strong> </p> </td> 
   <td> <p>Esse modificador pesquisa partes de um <i>diferencia maiúsculas de minúsculas</i> sequência de texto de maneira semelhante a <strong>contém</strong>. No entanto, <strong>curtir</strong> O fornece a capacidade de inserir caracteres curingas para dividir o texto.</p> <p>Por exemplo, ao pesquisar notas, usando <code>like %Current% %Dead%</code> retorna qualquer nota que contenha a frase "Atual para Inativo". Ela não inclui notas que contenham "Inativo para atual". Cada valor é pesquisado na ordem em que é listado. % representa um curinga para substituir caracteres ou segmentos de texto. Um sublinhado também pode ser usado para um único caractere curinga, como em <code>like Project_</code> que retorna "Projeto" e "Projetos". Se você pretende usar um <strong>curtir</strong> ou <strong>clike</strong> modificador em sua filtragem, recomendamos evitar % ou _ caracteres em nomes de campos de dados personalizados, valores de opção de parâmetro ou outros nomes de objeto.</p><p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr>  
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cilike</strong> </p> </td> 
   <td> <p>Este é o <i>não diferencia maiúsculas de minúsculas</i> versão de <strong>curtir</strong>. Por exemplo: <code>cilike %Current% %Dead%</code> retorna quaisquer notas que contenham <code>Current to Dead</code> ou <code>current to dead</code>.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong>Não existe</strong> </td> 
   <td><strong>NOTEXISTAS</strong> </td> 
   <td> <p>Este modificador é usado apenas com filtros complexos em uma instrução EXISTS. Esses filtros se referem apenas aos seguintes objetos: </p> 
    <ul> 
     <li>Objetos que abrangem vários níveis na hierarquia de objetos </li> 
     <li>Objetos ausentes </li> 
    </ul> <p>Para obter informações sobre como criar filtros complexos usando instruções EXISTS, consulte o artigo <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">Criar filtros complexos do modo texto usando instruções EXISTS</a>. Este é o único modificador usado em instruções EXISTS.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Maior que</strong> </p> </td> 
   <td> <p><strong>gt</strong> </p> </td> 
   <td> <p>Pesquisa todos os resultados com um valor maior que o valor inserido, sem incluir o valor inserido.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Menor que</strong> </p> </td> 
   <td> <p><strong>lt</strong> </p> </td> 
   <td> <p>Pesquisa todos os resultados com um valor menor do que o inserido, sem incluir o valor inserido.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Maior que ou igual</strong> </p> </td> 
   <td> <p><strong>get</strong> </p> </td> 
   <td> <p>Pesquisa todos os resultados com valores maiores ou iguais ao valor inserido.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Menor que ou igual</strong> </p> </td> 
   <td> <p><strong>lte</strong> </p> </td> 
   <td> <p>Pesquisa todos os resultados com um valor menor ou igual ao valor inserido.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Entre</strong> </p> </td> 
   <td> <p><strong>entre</strong> </p> </td> 
   <td> <p>Fornece dois valores de campo obrigatórios e pesquisa todos os resultados na faixa de ambos os campos, incluindo os valores inseridos.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notbetween</strong> </p> </td> 
   <td> <p>Este é o inverso de <strong>entre</strong>. Ela fornece dois campos de valor obrigatórios e pesquisa todos os resultados fora do intervalo de ambos os campos, incluindo os valores inseridos.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr>

</tbody> 
</table>
