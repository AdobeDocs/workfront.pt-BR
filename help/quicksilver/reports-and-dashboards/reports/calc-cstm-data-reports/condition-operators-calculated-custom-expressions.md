---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Operadores de condição em expressões personalizadas calculadas
description: Você pode usar operadores ou modificadores de condição ao criar dados personalizados calculados no Adobe Workfront ao usar o modo de texto.
author: Nolan
feature: Reports and Dashboards
exl-id: ce98ca39-cb86-4ef7-b75c-29ceb916e885
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 1%

---

# Operadores de condição em campos personalizados calculados

Você pode usar operadores ou modificadores de condição ao criar dados personalizados calculados no Adobe Workfront ao usar o modo de texto.

Para obter informações sobre como usar o modo de texto no Workfront, consulte [Visão geral do modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Os operadores ou modificadores de condição ajudam a criar uma declaração de condição ao conectar campos Workfront existentes em instruções e gerar um novo campo. O uso mais comum dos operadores de condição é criar a condição de uma declaração &quot;IF&quot;.

Você pode usar instruções &quot;IF&quot; no Workfront para comparar, formatar e unir campos de dados para fins de relatórios e dados personalizados.

Você pode criar instruções &quot;IF&quot; para os seguintes elementos do Workfront:

* Visualizações
* Agrupamento
* Campos personalizados calculados

Para obter mais informações sobre a criação de instruções &quot;IF&quot;, consulte [Visão geral das instruções &quot;IF&quot;](../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md).

Os exemplos neste guia ilustram o uso de operadores de condição em campos personalizados calculados. Também é possível usá-los em colunas ou agrupamentos personalizados calculados, ao seguir a sintaxe correta para campos personalizados calculados em relatórios.

Para obter informações sobre a diferença na sintaxe entre os campos personalizados calculados e os dados personalizados calculados nos relatórios, consulte [Campos personalizados calculados vs. colunas calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

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
   <th>Definição de operador de condição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Igual (Distingue maiúsc. e minúsc.)</td> 
   <td>= </td> 
   <td> <p>Use esse operador para indicar que a condição é atendida quando o primeiro campo de sua declaração for igual ao segundo campo.</p> <p>Por exemplo, use a seguinte instrução em um campo personalizado calculado para criar uma instrução "IF" que compara a Data de conclusão planejada à Data de conclusão projetada de uma tarefa: </p><pre>IF({estimatedCompletionDate}={planCompletionDate},"On Track","Off Track")</pre> </td> 
  </tr> 
  <tr> 
   <td>Maior que </td> 
   <td>&gt; </td> 
   <td>Use esse operador para indicar que a condição é atendida quando o primeiro campo de sua declaração for maior que o segundo campo. <p>Por exemplo, use a seguinte instrução em um campo personalizado calculado para criar uma instrução "IF" que compara a Data de conclusão planejada à Data de conclusão projetada de uma tarefa: </p><pre>IF({projectCompletionDate}&gt;{planCompletionDate},"Late","")</pre></td> 
  </tr> 
  <tr> 
   <td>Maior que ou igual a </td> 
   <td>&gt;= </td> 
   <td>Use esse operador para indicar que a condição é atendida quando o primeiro campo de sua declaração for maior ou igual ao segundo campo. <p>Por exemplo, use a seguinte instrução em um campo personalizado calculado para criar uma instrução "IF" que compara a Data de conclusão planejada à Data de conclusão projetada de uma tarefa: </p><pre>IF({estimatedCompletionDate}&gt;={planCompletionDate},"Late","Early")</pre></td> 
  </tr> 
  <tr> 
   <td>Menor que </td> 
   <td>&lt; </td> 
   <td>Use esse operador para indicar que a condição é atendida quando o primeiro campo de sua declaração for menor que o segundo campo. <p>Por exemplo, use a seguinte instrução em um campo personalizado calculado para criar uma instrução "IF" que compara a Data de conclusão planejada à Data de conclusão projetada de uma tarefa: </p><pre>IF({projectCompletionDate}&lt;{planCompletionDate},"Early","")</pre></td> 
  </tr> 
  <tr> 
   <td>Menor que ou igual a </td> 
   <td>&lt;= </td> 
   <td>Use esse operador para indicar que a condição é cumprida quando o primeiro campo da declaração é menor ou igual ao segundo campo. <p>Por exemplo, use a seguinte instrução em um campo personalizado calculado para criar uma instrução "IF" que compara a Data de conclusão planejada à Data de conclusão projetada de uma tarefa: </p><pre>IF({estimatedCompletionDate}&lt;={planCompletionDate},"Early","Late")</pre></td> 
  </tr> 
  <tr> 
   <td>Não </td> 
   <td>! </td> 
   <td> <p>Adicione esse operador na frente de qualquer um dos operadores acima para negar o operador. </p> <p>Por exemplo: </p> 
    <ul> 
     <li>Igual: = </li> 
     <li>Não é igual a: != </li> 
    </ul> <p>Adicionar esse operador na frente das seguintes expressões de dados adiciona uma declaração negativa às expressões: </p> 
    <ul> 
     <li>CONTÉM </li> 
     <li>EM </li> 
     <li>IFIN </li> 
     <li>ISBLANK </li> 
    </ul> <p>Para obter informações sobre essas expressões de dados e para obter uma lista completa, consulte <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md" class="MCXref xref">Expressões de dados calculadas</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>Ou </td> 
   <td>|| </td> 
   <td> <p>Use esse operador para indicar que a condição é cumprida quando a expressão encontra o primeiro ou o segundo valor de sua declaração. </p> <p>Por exemplo, use a seguinte instrução em um campo personalizado calculado para criar uma instrução "IF" que marca os projetos nos status Atual ou Planejamento como "Ativo": </p><pre>IF({status}="PLN"||{status}="CUR","Ativo","Não Ativo")</pre> </td> 
  </tr> 
  <tr> 
   <td> E </td> 
   <td>&amp;&amp; </td> 
   <td> <p>Use esse operador para indicar que a condição é cumprida quando a expressão encontra um item que cumpre duas condições ao mesmo tempo. </p> <p>Por exemplo, use a seguinte instrução em um campo personalizado calculado para criar uma instrução "IF" que localize projetos que estejam no status Atual e tenham uma Condição de risco e os marque como "Mediação necessária". </p><pre>IF({status}="CUR"&amp;&amp;{condition}="AR","Mediação Necessária",""))</pre> </td> 
  </tr> 
 </tbody> 
</table>
