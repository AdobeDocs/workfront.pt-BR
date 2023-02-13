---
product-area: reporting
navigation-topic: reporting-elements
title: Modificadores de filtro e condição
description: Os modificadores de filtro e condição permitem que você crie filtros e estabeleça condições para formatar os resultados do relatório.
author: Lisa
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '1556'
ht-degree: 1%

---

# Modificadores de filtro e condição

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit) </p>
-->

Os modificadores de filtro e condição permitem que você crie filtros e estabeleça condições para formatar os resultados do relatório.

Para obter mais informações sobre criação de filtros, consulte o artigo [Visão geral dos filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Para obter mais informações sobre o uso da formatação condicional em Exibições, consulte o artigo [Usar formatação condicional em exibições](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Modificadores de filtro e condição

Para obter uma lista de modificadores integrados de período, consulte o artigo [Filtrar relatórios por intervalos de tempo](../../../reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md).

Alguns modificadores são incorporados e você pode escolhê-los em um menu suspenso dentro do filtro ou da declaração de formatação condicional. Outros modificadores só podem ser usados em filtros de modo de texto. Para obter mais informações sobre como entender o modo de texto, consulte [Visão geral do modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Você pode usar os seguintes modificadores de condição em filtros e declarações de formatação condicional:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Modificador incorporado</strong> </p> </th> 
   <th> <p><strong>Modificador do modo de texto</strong> </p> </th> 
   <th> <p><strong>Descrição</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td> <p><strong>Blank</strong> </p> </td> 
   <td> <p><strong>Vazio</strong> </p> </td> 
   <td> <p>O campo existe para o objeto, mas o campo ainda não recebeu um valor.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Não Branco</strong> </p> </td> 
   <td> <p><strong>notblank</strong> </p> </td> 
   <td> <p>O campo para o qual você está filtrando existe e recebeu um valor.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>null</strong> </p> </td> 
   <td> <p>O campo está em branco ou não existe. Por exemplo, você deseja procurar itens sem uma ID de tarefa pai. Isso significa que você deseja ver somente tarefas independentes. O qualificador para a "ID da tarefa pai" seria <strong>null</strong>, já que uma tarefa sem uma ID (nesse caso, o pai) não existe. </p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notnull</strong> </p> </td> 
   <td> <p>O campo para o qual você está filtrando existe e contém um valor diferente de nulo.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Contém</strong> </p> </td> 
   <td> <p><strong>cicontains</strong> </p> </td> 
   <td> <p>(Não diferencia maiúsculas de minúsculas) Essa é a versão não diferencia maiúsculas de minúsculas <strong>contém</strong>. Por exemplo: "contine inf" captura qualquer valor que contenha "Inf" ou "inf".</p> <p> <p>Observação: O Adobe Workfront pesquisa a palavra ou frase exata que você está especificando para cada instrução de filtro. Por exemplo, se você estiver procurando por qualquer projeto que contenha a frase "novo projeto" no nome, o Workfront não exibirá projetos que tenham apenas "novo" ou "projeto", ou "novo projeto principal" no nome. O filtro encontra apenas projetos com a frase exata "novo projeto" no nome.</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>(Não diferencia maiúsculas de minúsculas) Essa é a opção não diferencia maiúsculas de minúsculas <strong>eq</strong>. Ele retorna apenas uma correspondência exata do valor pesquisado.</p> <p>Por exemplo, ao pesquisar por uma tarefa com um nome específico, o "nome da tarefa cieq test" encontra tarefas em que o nome é "Test", "TEST" ou "Test", mas não encontra uma tarefa com o nome "test 123".</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cifra</strong> </p> </td> 
   <td> <p>(Não diferencia maiúsculas de minúsculas) Essa é a versão não diferencia maiúsculas de minúsculas <strong>em</strong>.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>chata</strong> </p> </td> 
   <td> <p>Esta é a versão que não diferencia maiúsculas de minúsculas de <strong>like</strong>. Por exemplo: "cilike %Current% %Dead%" retorna quaisquer observações que contenham "Current to Dead" ou "current to becad".</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cinotina</strong> </p> </td> 
   <td> <p>(Não diferencia maiúsculas de minúsculas) Essa é a versão não diferencia maiúsculas de minúsculas <strong>nota</strong>.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre como criar filtros usando o modo de texto, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>contém</strong> </p> </td> 
   <td> <p>(Diferencia maiúsculas de minúsculas) Pesquisa o texto especificado em uma string de texto inteira.</p> <p>Por exemplo, usar "contém Inf" captura qualquer coisa com "Inf", como a palavra "Infinity".</p> <p>Este modificador só pode ser usado em filtros de modo de texto.Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Não Contém (Distingue maiúsc. e minúsc.)</strong> </p> </td> 
   <td> <p><strong>cinotcontém</strong> </p> </td> 
   <td> <p>(Não diferencia maiúsculas de minúsculas) Ela filtra itens cujo valor especificado está ausente.</p> <p>Por exemplo, "não contém inf" captura qualquer coisa sem "Inf" ou "inf" no nome.</p> <p>Observação: <span>Se o campo para o qual você está filtrando tiver várias opções, isso filtra os resultados que contêm a escolha especificada, bem como a escolha especificada e quaisquer opções adicionais.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong>Não Existe</strong> </td> 
   <td><strong>NOTEXISTAS</strong> </td> 
   <td> <p>Esse modificador é usado somente com filtros complexos em uma instrução EXISTS. Esses filtros se referem apenas aos seguintes objetos: </p> 
    <ul> 
     <li>Objetos que abrangem vários níveis na hierarquia de objetos </li> 
     <li>Objetos ausentes </li> 
    </ul> <p>Para obter informações sobre como criar filtros complexos usando instruções EXISTS, consulte o artigo <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">Criar filtros complexos em modo de texto usando declarações EXISTENTES</a>. Este é o único modificador usado em instruções EXISTS.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>Igual (Distingue maiúsc. e minúsc.)</strong> </p> </td> 
   <td> <p><strong>em</strong> </p> </td> 
   <td> <p>(Diferencia maiúsculas de minúsculas) Esse modificador permite criar uma lista separada por vírgulas de variáveis a serem comparadas a um único atributo avaliado em um filtro. A lista inteira é tratada como uma instrução OR e retorna quaisquer resultados que atendam aos critérios de uma ou mais variáveis.</p> <p>Por exemplo, ao pesquisar projetos, usando "em CUR, PLN, CPL" retorna todos os projetos que estão no status Atual, OU Planejamento, OU Concluído.</p> <p>O modificador incorporado <strong>Igual</strong> corresponde ao modificador de modo de texto de <strong>em</strong>. Isso significa que é possível escolher Igual com vários valores para o campo.</p> <p>Por exemplo, você pode escolher "Status igual a Atual, Planejamento, Adiado" em um relatório de projeto e pode exibir projetos em qualquer um desses status.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>(Diferencia maiúsculas e minúsculas) Retorna apenas uma correspondência exata do valor pesquisado.</p> <p>Por exemplo, ao pesquisar por projetos completos, "eq CPL" retorna todos os projetos no status completo. "eq CPL, CUR" não retorna um resultado porque um projeto não pode ser concluído e atualizado ao mesmo tempo.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre como usar o modo de texto para criar filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Maior Que</strong> </p> </td> 
   <td> <p><strong>gt</strong> </p> </td> 
   <td> <p>Isso pesquisa todos os resultados com um valor maior que o valor inserido, sem incluir o valor inserido.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>like</strong> </p> </td> 
   <td> <p>(Diferencia maiúsculas de minúsculas) Pesquisa por partes de uma string de texto de maneira semelhante a <strong>contém</strong>. No entanto, <strong>like</strong> O fornece a capacidade de inserir caracteres curingas para quebrar o texto.</p> <p>Por exemplo, ao pesquisar notas, usando "como %Current% %Dead%" retorna qualquer observação que contenha a frase "Atual para inativo". Ela não inclui notas que contenham "Atual". Cada valor é pesquisado na ordem listada. O % representa um curinga para substituir caracteres ou segmentos de texto.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Menor Que</strong> </p> </td> 
   <td> <p><strong>lt</strong> </p> </td> 
   <td> <p>Isso pesquisa todos os resultados com um valor menor que o inserido, sem incluir o valor inserido.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Maior Que ou Igual</strong> </p> </td> 
   <td> <p><strong>gte</strong> </p> </td> 
   <td> <p>Isso pesquisa todos os resultados com valores maiores ou iguais ao valor inserido.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Menor Que ou Igual</strong> </p> </td> 
   <td> <p><strong>lte</strong> </p> </td> 
   <td> <p>Isso pesquisa todos os resultados com um valor menor ou igual ao valor inserido.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Entre</strong> </p> </td> 
   <td> <p><strong>entre</strong> </p> </td> 
   <td> <p>Fornece dois valores de campo obrigatórios e pesquisa todos os resultados dentro do intervalo de ambos os campos, incluindo os valores inseridos.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notcontains</strong> </p> </td> 
   <td> <p>(Diferencia maiúsculas de minúsculas) Ela filtra itens cujo valor especificado está faltando.</p> <p>Por exemplo, "notcontains inf" captura qualquer item sem "inf", mas exibe valores que contêm "Inf".</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>não entre</strong> </p> </td> 
   <td> <p>É o inverso de <strong>entre</strong>. Ele fornece dois campos de valor obrigatórios e pesquisa todos os resultados fora do intervalo de ambos os campos, incluindo os valores inseridos.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Não Igual (Distingue maiúsc. e minúsc.)</strong> </p> </td> 
   <td> <p><strong>nota</strong> </p> </td> 
   <td> <p>(Diferencia maiúsculas de minúsculas) É o oposto de <strong>em</strong>. Ele retorna somente resultados que não estão na lista especificada.</p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> <p>Observação: <span>Se o campo para o qual você está filtrando tiver várias opções, isso filtra os resultados que contêm a escolha especificada, bem como a escolha especificada e quaisquer opções adicionais.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>ne</strong> </td> 
   <td> <p>(Diferencia maiúsculas de minúsculas) É o oposto de <strong>eq</strong>. Ele retorna somente resultados que não são uma correspondência exata do valor pesquisado e também corresponde ao caso do valor.</p> <p>Por exemplo, <b>ne</b> retorna qualquer valor que não seja igual a "Atual", mas não retorna qualquer valor que não seja igual a "atual". </p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>canina</strong> </td> 
   <td> <p>(Não diferencia maiúsculas de minúsculas) Essa é a opção não diferencia maiúsculas de minúsculas <strong>ne</strong> e é o oposto de <b>cieq</b> modificador. Ele retorna somente resultados que não são uma correspondência exata do valor pesquisado, não considerando o caso do valor.</p> <p>Por exemplo, <b>canina</b> retorna qualquer valor que não seja igual a "atual" ou "Atual". </p> <p>Esse modificador só pode ser usado em filtros de modo de texto. Para obter mais informações sobre o modo de texto em filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar um filtro usando o modo de texto</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
