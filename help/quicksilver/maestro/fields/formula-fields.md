---
title: Visão geral dos campos de fórmula
description: No Adobe Workfront Planning, é possível criar campos de fórmula que usam funções e campos existentes para calcular um novo valor personalizado.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: 1369269bcb64bd32f26603608782dc996b079cb9
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 8%

---

# Visão geral dos campos de fórmula

<!--update the metadata with real information when making this available in TOC and in the left nav - below-->

<!---
title: Formula fields overview
description: In Adobe Maestro, you can create formula fields that use functions and existing  fields to calculate a new custom value. 
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

<!--when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula-->

{{planning-important-intro}}

Você pode criar campos personalizados no Adobe Workfront Planning fazendo referência a campos existentes e os conectando em um campo do tipo Fórmula.

Os campos de fórmula geram um novo valor usando valores existentes de outros campos em um tipo de registro e uma função que indica como os valores existentes devem ser calculados.

Para obter informações, consulte a seção &quot;Fórmula&quot; no artigo [Criar campos](../fields/create-fields.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produto</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>contrato do Adobe Workfront</p></td>
   <td>
<p>Sua organização deve estar inscrita no estágio de acesso antecipado do Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plano do Adobe Workfront</p></td>
   <td>
<p>Qualquer</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td>
   <td>
   <p>Qualquer</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuração do nível de acesso</p></td>
   <td> <p>Não há controles de acesso para o Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>Gerenciar permissões em um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>O administrador do Workfront ou do grupo deve adicionar a área do Planning ao modelo de layout. Para obter informações, consulte <a href="../access/access-overview.md">Visão geral do Access</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->


## Considerações sobre campos de fórmula

* Os campos de fórmula fazem referência a campos que pertencem ao mesmo tipo de registro. Não é possível referenciar campos de outros tipos de registro ao criar um campo de fórmula. <!--is this still accurate??-->
* Não é possível alterar o tipo Field de um campo Formula depois de salvá-lo.
* É possível atualizar o cálculo de um campo de fórmula depois de salvá-lo, e os resultados do cálculo são atualizados automaticamente para todos os registros do mesmo tipo.
* É necessário adicionar os campos que você menciona nas fórmulas à medida que são exibidos na interface do Workfront Planning.

## Fórmulas compatíveis

Os campos de fórmula do Adobe Workfront Planning aceitam todas as expressões dos campos calculados do Workfront. Para obter mais informações, consulte [Visão geral das expressões de dados calculadas](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Além disso, oferecemos suporte às seguintes expressões para campos de fórmula do Workfront Planning:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Expressão</th> 
   <th>Explicação e exemplo</th> 
  </tr> 
 </thead> 
 <tbody>

<tr> 
   <td><strong>ARRAYJOIN</strong> </td> 
   <td> <p>Retorna a string concatenada por delimitador.</p> <p>A expressão é formatada da seguinte maneira:

<code>ARRAYJOIN(delimitador,matriz)</code>
</p>
   </td></tr>

<tr> 
   <td><strong>ARRAYUNIQUE</strong> </td> 
   <td> <p>Retorna a matriz com valores únicos.</p> <p>A expressão é formatada da seguinte maneira:

<code>ARRAYUNIQUE(matriz)</code>
</p>
   </td></tr>
     <tr> 
   <td><strong>ID</strong> </td> 
   <td> <p>Retorna a ID de um registro. Cada registro tem uma ID exclusiva.</p> <p>A expressão é formatada da seguinte maneira:

<code>{ID}</code>
</p>
   </td></tr>

<tr> 
   <td><strong>SETTIMEZONE</strong> </td> 
   <td> <p>Define o fuso horário de uma data e hora para um fuso horário específico.</p> <p>A expressão é formatada da seguinte maneira:

<code>SETTIMEZONE(data,&#39;América/Los_Angeles&#39;)</code>
</p>
   </td></tr>

<tr> 
   <td><strong>WEEKOFYEAR</strong> </td> 
   <td> <p>Retorna o número da semana em um ano. Como opção, é possível indicar em qual dia a semana começa (use 1 para domingo ou 2 para segunda-feira). Se omitido, as semanas começarão no domingo, por padrão.</p> <p>A expressão é formatada da seguinte maneira:

<code>WEEKOFYEAR(data,2)</code>
ou
<code>WEEKOFYEAR(data)</code>
</p>
   </td></tr>

</table>
