---
product-area: reporting
navigation-topic: reporting-elements
title: Filtro e modificadores de condição
description: Os modificadores de filtro e condição permitem criar filtros e estabelecer condições para formatar os resultados do relatório.
author: Nolan
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: b2b17c34fe4887e291e69facf76f5071bca43b06
workflow-type: tm+mt
source-wordcount: '1565'
ht-degree: 0%

---

# Filtro e modificadores de condição

<!-- Audited: 11/2024 -->

<!--(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit)-->

Os modificadores de filtro e condição permitem criar filtros e estabelecer condições para formatar os resultados do relatório.

Para obter mais informações sobre a criação de filtros, consulte o artigo [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Para obter mais informações sobre o uso de formatação condicional em Exibições, consulte o artigo [Usar formatação condicional em exibições](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Filtro e modificadores de condição

Alguns modificadores são incorporados e você pode escolhê-los de um menu suspenso dentro do filtro ou da instrução de formatação condicional. Outros modificadores só podem ser usados em filtros de modo de texto.

Para obter mais informações sobre como entender o modo de texto, consulte [Visão geral do Modo de Texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Para obter uma lista de modificadores de período predefinidos, consulte o artigo [Filtrar relatórios por período](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md).

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
   <td> <p>O campo existe para o objeto, mas o campo não tem um valor no momento.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Não Está Em Branco</strong> </p> </td> 
   <td> <p><strong>notblank</strong> </p> </td> 
   <td> <p>O campo que você está filtrando existe e recebeu um valor.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>nulo</strong> </p> </td> 
   <td> <p>O campo está em branco ou não existe. Por exemplo, você deseja procurar itens sem uma ID de tarefa pai. Isso significa que você deseja ver apenas as tarefas independentes. O qualificador para a "ID da tarefa pai" seria <strong>nulo</strong>, já que uma tarefa sem uma ID (neste caso, o pai) não existe. </p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notnull</strong> </p> </td> 
   <td> <p>O campo que você está filtrando existe e contém um valor diferente de nulo.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Contém</strong> </p> </td> 
   <td> <p><strong>cicontains</strong> </p> </td> 
   <td> <p>Esta é a versão <i>que não diferencia maiúsculas de minúsculas</i> de <strong>contém</strong>. Por exemplo: <code>cicontains inf</code> captura qualquer valor que contenha <code>Inf</code> ou <code>inf</code>.</p> <p> <p>Observação: O Adobe Workfront procura a palavra ou frase exata que você está especificando para cada instrução de filtro. Por exemplo, se você estiver pesquisando um projeto que contenha a frase <code>new project</code> no nome, o Workfront não exibirá projetos que tenham apenas <code>new</code> ou apenas <code>project</code>, ou <code>new main project</code> no nome. O filtro localiza somente projetos com a frase exata <code>new project</code> no nome.</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Não Contém</strong> </p> </td> 
   <td> <p><strong>cinotcontains</strong> </p> </td> 
   <td> <p>Esta é a versão <i>sem diferenciação de maiúsculas e minúsculas</i> de <strong>notcontains</strong>.</p><p>Esse modificador filtra itens cujo valor especificado está faltando.</p> <p>Por exemplo, <code>does not contain inf</code> captura algo sem <code>Inf</code> ou <code>inf</code> no nome.</p> <p>Observação: <span>Se o campo que você está filtrando tiver várias opções, isso filtra os resultados que contêm tanto a opção especificada, quanto a opção especificada e qualquer opção adicional.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>contém</strong> </p> </td> 
   <td> <p> Pesquisa o texto <i>que diferencia maiúsculas de minúsculas</i> especificado em uma cadeia de texto inteira.</p> <p>Por exemplo, usar <code>contains Inf</code> captura qualquer coisa com <code>Inf</code> nela, como a palavra <code>Infinity.</code></p> <p>Este modificador só pode ser usado em filtros do modo texto. Para obter mais informações sobre o modo texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo texto</a>.</p> </td> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notcontains</strong> </p> </td> 
   <td> <p>Ele filtra itens que não têm o valor <i>que diferencia maiúsculas de minúsculas</i> especificado.</p> <p>Por exemplo, <code>notcontains inf</code> captura qualquer item sem <code>inf</code>, mas exibe valores que contêm <code>Inf</code>.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo texto</a>.</p> </td> 
  </tr> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>Esta é a opção <i>que não diferencia maiúsculas de minúsculas</i> de <strong>eq</strong>. Ela só retorna uma correspondência exata do valor pesquisado.</p> <p>Por exemplo, ao procurar uma tarefa com um nome específico, <code>task name cieq test</code> encontra tarefas cujo nome é <code>Test</code>, <code>TEST</code> ou <code>Test</code>, mas não encontra uma tarefa com o nome <code>test 123.</code></p> <p>Ao procurar um status, o modificador <strong>cieq</strong> não é compatível. Você deve usar o modificador que diferencia maiúsculas de minúsculas, <strong>eq</strong>, para procurar um status.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo texto</a>.</p> </td>
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>cine</strong> </td> 
   <td> <p>Esta é a opção <i>que não diferencia maiúsculas de minúsculas</i> de <strong>ne</strong>, e é o oposto do modificador <b>cieq</b>. Ela só retorna resultados que não são uma correspondência exata do valor pesquisado, não levando em conta a caixa do valor.</p> <p>Por exemplo, <b>cine</b> retorna quaisquer valores que não sejam iguais a "current" ou "Current". </p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo texto</a>.</p> </td> 
  </tr>   <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>Este modificador retorna somente uma correspondência exata <i>que diferencia maiúsculas de minúsculas</i> do valor pesquisado.</p> <p>Por exemplo, ao pesquisar por projetos concluídos, <code>eq CPL</code> retorna todos os projetos com o status Concluído. <code>eq CPL, CUR</code> não retorna um resultado porque um projeto não pode ser concluído e atualizado ao mesmo tempo.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>ne</strong> </td> 
   <td> <p>Esta é a <i>distinção entre maiúsculas e minúsculas</i> oposta a <strong>eq</strong>. Ele retorna somente os resultados que não são uma correspondência exata do valor pesquisado e também corresponde às letras maiúsculas e minúsculas do valor.</p> <p>Por exemplo, <b>ne</b> retorna quaisquer valores que não sejam iguais a "Current", mas não retorna quaisquer valores que não sejam iguais a "current". </p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo texto</a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cidade</strong> </p> </td> 
   <td> <p> Esta é a versão <i>sem diferenciação de maiúsculas e minúsculas</i> de <strong>in</strong>.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cinotina</strong> </p> </td> 
   <td> <p>Esta é a versão <i>sem diferenciação de maiúsculas e minúsculas</i> de <strong>nãon</strong>.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>Igual</strong> </p> </td> 
   <td> <p><strong>em</strong> </p> </td> 
   <td> <p>Este modificador permite criar uma lista separada por vírgulas de variáveis <i>que diferenciam maiúsculas de minúsculas</i> para comparar a um único atributo avaliado em um filtro. A lista inteira é tratada como uma instrução OU e retorna quaisquer resultados que atendam aos critérios de uma ou mais das variáveis.</p> <p>Por exemplo, ao pesquisar por projetos, o uso de <code>in CUR, PLN, CPL</code> retorna todos os projetos com status Atual, OU Planejado ou Concluído.</p> <p>O modificador interno <strong>Equal</strong> corresponde ao modificador de modo de texto de <strong>in</strong>. Isso significa que você pode escolher Equal with multiple values para o campo.</p> <p>Por exemplo, você pode escolher um "Status igual a Atual, Planejamento, Inativo" em um relatório de projeto e pode visualizar os projetos em qualquer um desses status.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Não Igual</strong> </p> </td> 
   <td> <p><strong>não</strong> </p> </td> 
   <td> <p>Esta é a <i>distinção entre maiúsculas e minúsculas</i> oposta a <strong>em</strong>. Retorna apenas resultados que não estão na lista especificada.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo texto</a>.</p> <p>Observação: <span>Se o campo que você está filtrando tiver várias opções, isso filtra os resultados que contêm tanto a opção especificada, quanto a opção especificada e qualquer opção adicional.</span> </p> </td> 
  </tr>
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>curtir</strong> </p> </td> 
   <td> <p>Este modificador procura partes de uma cadeia de texto <i>que diferencia maiúsculas de minúsculas</i> de maneira semelhante a <strong>contém</strong>. Entretanto, <strong>like</strong> fornece a capacidade de inserir caracteres curinga para dividir o texto.</p> <p>Por exemplo, ao pesquisar anotações, o uso de <code>like %Current% %Dead%</code> retorna qualquer anotação que contenha a frase "Atualizado para Desativado". Ela não inclui notas que contenham "Inativo para atual". Cada valor é pesquisado na ordem em que é listado. % representa um curinga para substituir caracteres ou segmentos de texto. Um sublinhado também pode ser usado para um único caractere curinga, como em <code>like Project_</code>, que retorna "Projeto" e "Projetos". Se você pretende usar um modificador <strong>like</strong> ou <strong>clike</strong> na filtragem, recomendamos evitar % ou _ caracteres em nomes de campos de dados personalizados, valores de opção de parâmetro ou outros nomes de objeto.</p><p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo texto</a>.</p> </td> 
  </tr>  
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cilike</strong> </p> </td> 
   <td> <p>Esta é a versão <i>sem diferenciação de maiúsculas e minúsculas</i> de <strong>semelhante</strong>. Por exemplo: <code>cilike %Current% %Dead%</code> retorna quaisquer notas que contenham <code>Current to Dead</code> ou <code>current to dead</code>.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo texto</a>.</p> </td> 
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
   <td> <p><strong>Maior Que</strong> </p> </td> 
   <td> <p><strong>get</strong> </p> </td> 
   <td> <p>Pesquisa todos os resultados com um valor maior que o valor inserido, sem incluir o valor inserido.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Menor Que</strong> </p> </td> 
   <td> <p><strong>lt</strong> </p> </td> 
   <td> <p>Pesquisa todos os resultados com um valor menor do que o inserido, sem incluir o valor inserido.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Maior Que Igual</strong> </p> </td> 
   <td> <p><strong>get</strong> </p> </td> 
   <td> <p>Pesquisa todos os resultados com valores maiores ou iguais ao valor inserido.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Menor Que Igual</strong> </p> </td> 
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
   <td> <p><strong>nãoentre</strong> </p> </td> 
   <td> <p>Este é o inverso de <strong>entre</strong>. Ela fornece dois campos de valor obrigatórios e pesquisa todos os resultados fora do intervalo de ambos os campos, incluindo os valores inseridos.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo texto</a>.</p> </td> 
  </tr>

</tbody> 
</table>
