---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Operadores de condição em expressões personalizadas calculadas
description: You can use condition operators or modifiers when building calculated custom data in Adobe Workfront when using text mode.
author: Courtney
feature: Reports and Dashboards
exl-id: ce98ca39-cb86-4ef7-b75c-29ceb916e885
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 5%

---

# Condition operators in calculated custom fields

<!-- Audited: 2/2024 -->

You can use condition operators or modifiers when building calculated custom data in Adobe Workfront when using text mode. For information about using text mode in Workfront, see [Text Mode overview](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Operadores ou modificadores de condição ajudam a criar uma declaração condicional conectando campos existentes do Workfront em declarações e gerando um novo campo. O uso mais comum de operadores de condição é criar a condição de uma instrução &quot;IF&quot;.

Você pode usar instruções &quot;IF&quot; no Workfront para comparar, formatar e reunir campos de dados para fins de relatório e dados personalizados.

Você pode criar instruções &quot;IF&quot; para os seguintes elementos do Workfront:

* Exibições
* Agrupamento
* Campos personalizados calculados
* Regras de negócios

Para obter mais informações sobre como criar instruções “IF”, consulte [Visão geral das instruções “IF”](../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md).

The examples in this guide illustrate the use of condition operators in calculated custom fields. You can also use them in calculated custom columns or groupings as well, when following the correct syntax for calculated custom fields in reports.

For information about the difference in syntax between the calculated custom fields and calculated custom data in reports, see [Calculated custom fields vs. calculated columns](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

Para obter informações sobre regras de negócios, consulte [Criar e editar regras de negócios](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md).

Consulte o API Explorer para encontrar os campos que você deseja referenciar em suas expressões personalizadas calculadas. Para obter informações sobre o API Explorer, consulte [API Explorer](../../../wf-api/general/api-explorer.md).

Você pode usar os seguintes modificadores de condição no Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Operador de condição</th> 
   <th>Sintaxe do operador de condição</th> 
   <th>Definição do operador de condição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Igual</td> 
   <td>= </td> 
   <td> <p>Use this operator to indicate that the condition is fulfilled when the first field of your statement is equal to the second field.</p> <p>Por exemplo, use o seguinte demonstrativo em um campo personalizado calculado para criar um demonstrativo "IF" que compare a Data de conclusão planejada com a Data de conclusão projetada de uma tarefa: </p><p><code>IF({projectedCompletionDate}={plannedCompletionDate},"On Track","Off Track")</code></p> </td> 
  </tr> 
  <tr> 
   <td>Maior que </td> 
   <td>&gt; </td> 
   <td>Use esse operador para indicar que a condição é atendida quando o primeiro campo da instrução é maior que o segundo campo. <p>Por exemplo, use o seguinte demonstrativo em um campo personalizado calculado para criar um demonstrativo "IF" que compare a Data de conclusão planejada com a Data de conclusão projetada de uma tarefa: </p><p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Late","")</code></p></td> 
  </tr> 
  <tr> 
   <td>Maior ou igual a </td> 
   <td>&gt;= </td> 
   <td>Use esse operador para indicar que a condição é atendida quando o primeiro campo da instrução é maior ou igual ao segundo campo. <p>Por exemplo, use o seguinte demonstrativo em um campo personalizado calculado para criar um demonstrativo "IF" que compare a Data de conclusão planejada com a Data de conclusão projetada de uma tarefa: </p><p><code>IF({projectedCompletionDate}&gt;={plannedCompletionDate},"Late","Early")</code></p></td> 
  </tr> 
  <tr> 
   <td>Lesser than </td> 
   <td>&lt; </td> 
   <td>Use este operador para indicar que a condição é atendida quando  the first field of your statement is lesser than the second field. <p>Por exemplo, use o seguinte demonstrativo em um campo personalizado calculado para criar um demonstrativo "IF" que compare a Data de conclusão planejada com a Data de conclusão projetada de uma tarefa: </p><p><code>IF({projectedCompletionDate}&lt;{plannedCompletionDate},"Early","")</code></p></td> 
  </tr> 
  <tr> 
   <td>Menor que ou igual a </td> 
   <td>&lt;= </td> 
   <td>Use este operador para indicar que a condição é atendida quando  o primeiro campo da instrução é menor que ou igual ao segundo campo. <p>Por exemplo, use o seguinte demonstrativo em um campo personalizado calculado para criar um demonstrativo "IF" que compare a Data de conclusão planejada com a Data de conclusão projetada de uma tarefa: </p><p><code>IF({projectedCompletionDate}&lt;={plannedCompletionDate},"Early","Late")</code></p></td> 
  </tr> 
  <tr> 
   <td>Não </td> 
   <td>! </td> 
   <td> <p>Add this operator in front of any of the above operators to negate the operator. </p> <p>Por exemplo: </p> 
    <ul> 
     <li>Equals: = </li> 
     <li>Does not equal: != </li> 
    </ul> <p>Adicionar esse operador na frente das seguintes expressões de dados adiciona uma instrução negativa às expressões: </p> 
    <ul> 
     <li>CONTÉM </li> 
     <li>EM </li> 
     <li>IFIN </li> 
     <li>ISBLANK </li> 
    </ul> <p>For information about these data expressions and for a complete list, see <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md" class="MCXref xref">Overview of calculated data expressions</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>Ou </td> 
   <td>|| </td> 
   <td> <p>Use esse operador para indicar que a condição é atendida quando a expressão  O encontra o primeiro ou o segundo valor da instrução. </p> <p>Por exemplo, use a seguinte instrução em um campo personalizado calculado para criar uma instrução "IF" que marca os projetos nos status Atual ou Planejando como "Ativo": </p><p><code>IF({status}="PLN"||{status}="CUR","Active","Not Active")</code></p> </td> 
  </tr> 
  <tr> 
   <td> E </td> 
   <td>&amp;&amp; </td> 
   <td> <p>Use esse operador para indicar que a condição é atendida quando a expressão  finds an item that fulfills two conditions at the same time. </p> <p>For example, use the following statement in a calculated custom field to build an "IF" statement that finds projects that are in Current status and have a Condition of At Risk and marks them as "Mediation Needed." </p><p><code>IF({status}="CUR"&&{condition}="AR","Mediation Needed","")</code></p> </td> 
  </tr> 
 </tbody> 
</table>
