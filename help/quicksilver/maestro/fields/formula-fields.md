---
title: Visão geral dos campos de fórmula
description: Em Adobe Maestri, você pode criar campos de fórmula que usam funções e campos existentes para calcular um novo valor personalizado.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 3c49657c929c414888e6678022ef61b1bba1a420
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---


# Visão geral dos campos de fórmula

<!--update the metadata with real information when making this available in TOC and in the left nav - below-->

<!--**********ADD TO miniTOC************>

<!---
title: Formula fields
description: In Adobe Maestro, you can create formula fields that use functions and existing  fields to calculate a new custom value. 
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

<!--when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula-->

>[!IMPORTANT]
>
>As informações neste artigo referem-se ao Adobe Maestro, que é uma nova oferta da Adobe Workfront.
>
>Atualmente, o Adobe Maestro faz parte de um programa beta aberto a um número limitado de clientes. Você deve ser um cliente do Workfront para usar os recursos do Maestro.
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro-overview.md).

Você pode criar campos personalizados no Adobe Maestro fazendo referência a campos existentes e conectando-os por uma fórmula. Você pode fazer isso criando um campo personalizado do tipo Fórmula.

Os campos de fórmula geram um novo valor usando valores existentes de outros campos em um tipo de registro e uma função que indica como os valores existentes devem ser calculados.

Para obter informações, consulte [Criar campos](../fields/create-fields.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> produto Adobe</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>contrato do Adobe Workfront</p></td>
   <td>
<p>Sua organização deve estar inscrita no programa beta fechado do Adobe Maestro. Entre em contato com seu representante de conta para obter mais informações sobre esta nova oferta. </p>
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
   <td role="rowheader">Nível de acesso</td>
   <td> <p>Qualquer</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Modelo de layout</td>
   <td> <p>O administrador do sistema deve adicionar a área Maestro no modelo de layout. Para obter informações, consulte <a href="../access/access-overview.md">Visão geral do Access</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->

## Considerações sobre campos de fórmula

* Os campos de fórmula fazem referência a campos que pertencem ao mesmo tipo de registro. Não é possível referenciar campos de outros tipos de registro ao criar um campo de fórmula. <!--is this still accurate??-->
* Não é possível alterar o tipo de campo de um campo Fórmula depois de salvá-lo.
* É possível atualizar o cálculo de um campo de fórmula depois de salvá-lo, e os resultados do cálculo são atualizados automaticamente para todos os registros do mesmo tipo.
* Você deve adicionar os campos referenciados nas fórmulas conforme eles são exibidos na interface do Maestro.
* O uso de campos de pesquisa de tipos de registro vinculados em uma fórmula estará disponível em uma data posterior.

## Fórmulas compatíveis

Oferecemos suporte a todas as fórmulas dos campos calculados do Workfront. Para obter mais informações, consulte [Visão geral das expressões de dados calculadas](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Além disso, suportamos as seguintes expressões para campos de fórmula Maestri:


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

    ARRAYJOIN(delimitador,matriz)
</p>
   </td></tr>

<tr> 
   <td><strong>ARRAYUNIQUE</strong> </td> 
   <td> <p>Retorna a matriz com valores únicos.</p> <p>A expressão é formatada da seguinte maneira:

    ARRAYUNIQUE(matriz)
</p>
   </td></tr>

<tr> 
   <td><strong>SETTIMEZONE</strong> </td> 
   <td> <p>Define o fuso horário de uma data e hora para um fuso horário específico.</p> <p>A expressão é formatada da seguinte maneira:

    SETTIMEZONE(data,&#39;América/Los_Angeles&#39;)
</p>
   </td></tr>

<tr> 
   <td><strong>WEEKOFYEAR</strong> </td> 
   <td> <p>Retorna o número da semana em um ano. Como opção, você pode indicar em qual dia a semana começa (use 1 para domingo ou 2 para segunda-feira). Se omitido, as semanas começarão no domingo, por padrão.</p> <p>A expressão é formatada da seguinte maneira:

    WEEKOFYEAR(data,2)
    ou
    WEEKOFYEAR(data)
</p>
   </td></tr>

</table>





