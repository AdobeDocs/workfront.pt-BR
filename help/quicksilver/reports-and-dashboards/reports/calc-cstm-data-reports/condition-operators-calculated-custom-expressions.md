---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Operadores de condição em expressões personalizadas calculadas
description: Você pode usar operadores de condição ou modificadores ao criar dados personalizados calculados no Adobe Workfront ao usar o modo de texto.
author: Nolan
feature: Reports and Dashboards
exl-id: ce98ca39-cb86-4ef7-b75c-29ceb916e885
source-git-commit: e10fd7a3237d38ece8a5213990306ce511bd2412
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 1%

---

# Operadores de condição em campos personalizados calculados

<!-- Audited: 2/2024 -->

Você pode usar operadores de condição ou modificadores ao criar dados personalizados calculados no Adobe Workfront ao usar o modo de texto. Para obter informações sobre como usar o modo de texto no Workfront, consulte [Visão geral do Modo de Texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Operadores ou modificadores de condição ajudam a criar uma declaração condicional conectando campos existentes do Workfront em declarações e gerando um novo campo. O uso mais comum de operadores de condição é criar a condição de uma instrução &quot;IF&quot;.

Você pode usar instruções &quot;IF&quot; no Workfront para comparar, formatar e reunir campos de dados para fins de relatório e dados personalizados.

Você pode criar instruções &quot;IF&quot; para os seguintes elementos do Workfront:

* Visualizações
* Agrupamento
* Campos personalizados calculados
* Regras de negócios

Para obter mais informações sobre a compilação de instruções &quot;IF&quot;, consulte a [ visão geral das instruções &quot;IF&quot;](../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md).

Os exemplos neste guia ilustram o uso de operadores de condição em campos personalizados calculados. Também é possível usá-los em colunas ou agrupamentos personalizados calculados, ao seguir a sintaxe correta para campos personalizados calculados em relatórios.

Para obter informações sobre a diferença na sintaxe entre os campos personalizados calculados e os dados personalizados calculados nos relatórios, consulte [Campos personalizados calculados versus colunas calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

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
   <td> <p>Use esse operador para indicar que a condição é atendida quando o primeiro campo da instrução é igual ao segundo campo.</p> <p>Por exemplo, use o seguinte demonstrativo em um campo personalizado calculado para criar um demonstrativo "IF" que compare a Data de conclusão planejada com a Data de conclusão projetada de uma tarefa: </p><p><code>IF({projectedCompletionDate}={plannedCompletionDate},"On Track","Off Track")</code></p> </td> 
  </tr> 
  <tr> 
   <td>Maior que </td> 
   <td>&gt; </td> 
   <td>Use esse operador para indicar que a condição é atendida quando o primeiro campo da instrução é maior que o segundo campo. <p>Por exemplo, use o seguinte demonstrativo em um campo personalizado calculado para criar um demonstrativo "IF" que compare a Data de conclusão planejada com a Data de conclusão projetada de uma tarefa: </p><p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Late","")</code></p></td> 
  </tr> 
  <tr> 
   <td>Maior que ou igual a </td> 
   <td>&gt;= </td> 
   <td>Use esse operador para indicar que a condição é atendida quando o primeiro campo da instrução é maior ou igual ao segundo campo. <p>Por exemplo, use o seguinte demonstrativo em um campo personalizado calculado para criar um demonstrativo "IF" que compare a Data de conclusão planejada com a Data de conclusão projetada de uma tarefa: </p><p><code>IF({projectedCompletionDate}&gt;={plannedCompletionDate},"Late","Early")</code></p></td> 
  </tr> 
  <tr> 
   <td>Menor que </td> 
   <td>&lt; </td> 
   <td>Use este operador para indicar que a condição é atendida quando  o primeiro campo da instrução é menor que o segundo. <p>Por exemplo, use o seguinte demonstrativo em um campo personalizado calculado para criar um demonstrativo "IF" que compare a Data de conclusão planejada com a Data de conclusão projetada de uma tarefa: </p><p><code>IF({projectedCompletionDate}&lt;{plannedCompletionDate},"Early","")</code></p></td> 
  </tr> 
  <tr> 
   <td>Menor que ou igual a </td> 
   <td>&lt;= </td> 
   <td>Use este operador para indicar que a condição é atendida quando  o primeiro campo da instrução é menor que ou igual ao segundo campo. <p>Por exemplo, use o seguinte demonstrativo em um campo personalizado calculado para criar um demonstrativo "IF" que compare a Data de conclusão planejada com a Data de conclusão projetada de uma tarefa: </p><p><code>IF({projectedCompletionDate}&lt;={plannedCompletionDate},"Early","Late")</code></p></td> 
  </tr> 
  <tr> 
   <td>Não </td> 
   <td>! </td> 
   <td> <p>Adicione este operador na frente de qualquer um dos operadores acima para negar o operador. </p> <p>Por exemplo: </p> 
    <ul> 
     <li>Igual a: = </li> 
     <li>Não é igual a: != </li> 
    </ul> <p>Adicionar esse operador na frente das seguintes expressões de dados adiciona uma instrução negativa às expressões: </p> 
    <ul> 
     <li>CONTÉM </li> 
     <li>EM </li> 
     <li>IFIN </li> 
     <li>ISBLANK </li> 
    </ul> <p>Para obter informações sobre essas expressões de dados e obter uma lista completa, consulte <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md" class="MCXref xref">Visão geral das expressões de dados calculadas</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>Ou </td> 
   <td>|| </td> 
   <td> <p>Use esse operador para indicar que a condição é atendida quando a expressão  O encontra o primeiro ou o segundo valor da instrução. </p> <p>Por exemplo, use a seguinte instrução em um campo personalizado calculado para criar uma instrução "IF" que marca os projetos nos status Atual ou Planejando como "Ativo": </p><p><code>IF({status}="PLN"||{status}="CUR","Active","Not Active")</code></p> </td> 
  </tr> 
  <tr> 
   <td> E </td> 
   <td>&amp;&amp; </td> 
   <td> <p>Use esse operador para indicar que a condição é atendida quando a expressão  localiza um item que preenche duas condições ao mesmo tempo. </p> <p>Por exemplo, use a seguinte instrução em um campo personalizado calculado para criar uma instrução "IF" que localize projetos que estejam no status Atual e tenham uma Condição de Em Risco e os marque como "Mediação Necessária". </p><p><code>IF({status}="CUR"&&{condition}="AR","Mediation Needed","")</code></p> </td> 
  </tr> 
 </tbody> 
</table>
