---
content-type: api
navigation-topic: general-api
title: Versão de Assinatura de Evento
description: API de assinatura de evento
author: Becky
feature: Workfront API
role: Developer
exl-id: 151b9d0d-0dd6-4ece-9601-dda04356b436
source-git-commit: 3e082ddde7cb84fb8bf3b5a23c363fd3b4cfe3d2
workflow-type: tm+mt
source-wordcount: '1124'
ht-degree: 0%

---

# Versão de assinatura do evento

O Workfront tem duas versões de assinaturas de evento. Este artigo descreve as diferenças entre elas.

A nova versão não é uma alteração na API do Workfront, mas uma alteração na funcionalidade de assinatura do evento.

A capacidade de atualizar ou fazer downgrade de assinaturas de eventos garante que, quando alterações forem feitas na estrutura dos eventos, as assinaturas existentes não sejam interrompidas, permitindo testar e atualizar para a nova versão sem uma lacuna na assinatura do evento.

Para obter informações sobre os pontos de extremidade usados para atualizar ou rebaixar assinaturas de eventos, consulte [Versão de assinatura de eventos](/help/quicksilver/wf-api/general/event-subs-api.md#event-subscription-versioning) no artigo API de assinatura de eventos.

>[!IMPORTANT]
>
>As seguintes versões afetarão o controle de versão de assinaturas de eventos:
>
>* **25.2 Versão** (10 de abril de 2025): todas as novas assinaturas criadas após a versão 25.2 são criadas como Versão 2.
>* **25.3 Versão** (17 de julho de 2025): não é mais possível fazer downgrade das assinaturas para a Versão 1 após a versão 25.3.

## Alterações entre a versão 1 e a versão 2

As seguintes alterações foram feitas para assinaturas de evento Versão 2:


### Alterações gerais


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><b>Campos afetados</b></p> </th> 
   <th> <p><b>Versão 1 (comportamento anterior)</b></p> </th> 
   <th> <p><b>Versão 2 (Alterar)</b></p> </th> 
   <th> <p><b>Ação de remediação</b></p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Valores de parâmetro</p> </td> 
   <td> <p>Para qualquer objeto criado a partir de um modelo que incluísse um formulário personalizado, um evento <code>CREATE</code> era enviado e <code>UPDATE</code> era enviado com os valores de parâmetro (incluindo campos calculados e seus valores).    </p> </td> 
   <td> <p>Somente um evento <code>CREATE</code> é enviado, que contém valores de parâmetro incluindo campos calculados.</p> </td> 
   <td> <p>Se você tiver um filtro em <code>UPDATE</code> eventos com valores de parâmetro (incluindo campos personalizados calculados) e estiver esperando recebê-lo após um evento de objeto <code>CREATE</code> que inclua valores de parâmetro, você não receberá mais esse evento <code>UPDATE</code>. Se quiser ver valores de parâmetro na criação do objeto, você deve criar uma assinatura <code>CREATE</code> adicional.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Campos do tipo Seleção múltipla</p> </td> 
   <td> <p>Para qualquer tipo de evento que contenha uma alteração em um campo de tipo de seleção múltipla, se o campo contivesse apenas um valor, ele seria convertido em e enviado como uma string. Caso contrário, ele será enviado como uma matriz. </p><p>Exemplos:</p><ul><li><code>myMultiSelectField: ["oneValue"]</code> é convertido e enviado como <code>myMultiSelectField: "oneValue"</code>.</li><li><code>myMultiSelectField: ["first", "second"]</code> é enviado como <code>myMultiSelectField: ["first", "second"]</code>.</li></ul> </td> 
   <td> <p>Independentemente de quantos valores existam na matriz, ela será enviada como uma matriz. </p><p>Exemplos:</p><ul><li><code>myMultiSelectField: ["oneValue"]</code> é enviado como <code>myMultiSelectField: ["oneValue"]</code>.</li><li><code>myMultiSelectField: ["first", "second"]</code> é enviado como <code>myMultiSelectField: ["first", "second"]</code>.</li></ul> </td> 
   <td> <p>Se você tiver uma assinatura com um filtro em um campo de seleção múltipla e o valor como uma cadeia de caracteres, deverá criar uma nova assinatura com o mesmo filtro que tem o valor como uma matriz. </p> </td> 
  </tr> 
 </tbody> 
</table>

### Alterações específicas do objeto

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <b>Código do objeto</b> </th> 
   <th> <b>Campos afetados</b> </th> 
   <th> <b>Versão 1 (comportamento anterior)</b></th> 
   <th> <b>Versão 2 (Alterar)</b> </th> 
   <th> <b>Ação de correção</b> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th rowspan="1">ATRIBUIR</th> 
   <td>
    <ul>
     <li><code>projectID</code></li>
     <li><code>taskID</code></li>
     <li><code>opTaskID</code></li>
     <li><code>customerID</code></li>
    </ul> 
   </td> 
   <td>Quando este objeto é atualizado, o evento <code>UPDATE</code> às vezes mostra incorretamente que os campos afetados mudam de <code>null</code> para <code>ID value</code>.</td> 
   <td>Todos os eventos <code>UPDATE</code> mostram o valor correto para os campos afetados.</td> 
   <td>Nenhum. Se você tiver um filtro nos campos afetados, receberá um evento <code>UPDATE</code> somente se esses campos tiverem sido realmente alterados, não se qualquer outro valor tiver sido alterado.
   </td> 
  </tr> 
  <tr> 
   <th rowspan="2">DOCU</th> 
   <td>
    <ul>
     <li><code>referenceObjID</code></li>
    </ul> 
   </td> 
   <td>Quando qualquer valor de parâmetro é atualizado neste objeto, o evento <code>UPDATE</code> mostra incorretamente a alteração do campo afetado de <code>null</code> para <code>object id</code>. </td> 
   <td>Todos os eventos <code>UPDATE</code> mostram o valor correto para os campos afetados.</td> 
   <td>Nenhum. Se você tiver um filtro nos campos afetados, receberá um evento <code>UPDATE</code> somente se esses campos tiverem sido realmente alterados, não se qualquer outro valor tiver sido alterado.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>groups</code></li>
    </ul> 
   </td> 
   <td>Quando um documento foi excluído, o evento <code>DELETE</code> mostrava incorretamente o campo afetado como uma matriz vazia no estado anterior.    </td> 
   <td>O evento <code>DELETE</code> mostra corretamente o campo afetado no estado anterior.</td> 
   <td>Nenhum. O evento <code>DELETE</code> ainda será enviado, mas agora mostra os dados corretos para o campo afetado. 
</td> 
  </tr> 
  <tr> 
   <th rowspan="1">DOCV</th> 
  <td>
    <ul>
     <li><code>proofDecision</code></li>
     <li><code>proofName</code></li>
     <li><code>proofProgress</code></li>
    </ul> 
   </td> 
   <td>Quando este objeto for atualizado, dois eventos <code>UPDATE</code> serão enviados. O primeiro não incluiu os campos afetados, enquanto o segundo evento incluiu.</td> 
   <td>Todas as atualizações de campo, incluindo os campos afetados, estão presentes em apenas um evento <code>UPDATE</code>, e um segundo evento desnecessário não é enviado.     </td> 
   <td>Nenhum. Se você tiver um filtro nos campos afetados, os eventos serão entregues no primeiro evento. 
</td> 
  </tr> 
  <tr> 
   <th rowspan="2">EXPNS</th> 
  <td>
    <ul>
     <li><code>topReferenceObjCode</code></li>
     <li><code>referenceObjectName</code></li>
    </ul> 
   </td> 
   <td>Quando qualquer valor de parâmetro é atualizado em uma Despesa, o evento <code>UPDATE</code> mostra incorretamente a alteração de topReferenceObjCode de <code>EXPNS</code> para <code>PROJ</code> e a alteração de <code>referenceObjectName</code> de <code>null</code> para <code>string value of project name</code>.      </td> 
   <td>Todos os eventos <code>UPDATE</code> mostram o valor correto para os campos afetados.</td> 
   <td>Nenhum. Se você tiver um filtro nos campos afetados, receberá um evento <code>UPDATE</code> somente se esses campos tiverem sido realmente alterados, não se qualquer outro valor tiver sido alterado.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>topReferenceObjCode</code></li>
     <li><code>referenceObjectName</code></li>
    </ul> 
   </td> 
   <td>Quando um objeto Expense era excluído, um evento <code>UPDATE</code> era enviado alterando os campos afetados para null antes do envio do evento <code>DELETE</code>.    </td> 
   <td>O evento <code>UPDATE</code> extra não é enviado. O evento <code>DELETE</code> tem valores corretos para os campos afetados no estado anterior. </td> 
   <td>Se você tiver um filtro para os campos afetados em <code>UPDATE</code> eventos e estiver esperando recebê-lo quando o objeto for excluído, você não receberá mais esse evento <code>UPDATE</code>. Para ver esses campos quando o objeto for excluído, crie uma assinatura <code>DELETE</code> adicional.
</td> 
  </tr> 
  <tr> 
   <th rowspan="1">HORA</th> 
  <td>
    <ul>
     <li><code>projectID </code></li>
     <li><code>taskID </code></li>
     <li><code>roleID</code></li>
     <li><code>timesheetID</code></li>
     <li><code>hourTypeID </code></li>
     <li><code>projectOverheadID</code></li>
     <li><code>referenceObjID</code></li>
     <li><code>referenceObjCode</code></li>
     <li><code>securityRootID</code></li>
    </ul> 
   </td> 
   <td>Quando este objeto foi excluído, o evento <code>DELETE</code> mostrava incorretamente os campos afetados como <code>null</code> no estado anterior. </td> 
   <td>O evento <code>DELETE</code> mostra corretamente os campos afetados no estado antes.</td> 
   <td>Nenhum. O evento <code>DELETE</code> ainda é enviado, mas agora mostra os dados corretos para os campos afetados. </td> 
  </tr> 
  <tr> 
   <th rowspan="2">OPTASK</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   </td> 
   <td>Quando qualquer valor de parâmetro é atualizado neste objeto, o evento <code>UPDATE</code> mostra incorretamente a alteração do campo afetado de <code>null</code> para <code>ID value</code>. </td> 
   <td>Todos os eventos <code>UPDATE</code> mostram o valor correto para o campo afetado.</td> 
   <td>Nenhum. Se você tiver um filtro no campo afetado, você receberá um evento <code>UPDATE</code> somente se esse campo tiver sido realmente alterado, não se qualquer outro valor de parâmetro tiver sido alterado.
</td> 
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>resolveProjectID</code></li>
     <li><code>resolveTaskID</code></li>
     <li><code>resolvingObjID</code></li>
    </ul> 
   </td> 
   <td>Quando este objeto é atualizado, o evento <code>UPDATE</code> às vezes mostra incorretamente que os campos afetados mudam de <code>null</code> para <code>ID value</code>.</td> 
   <td>Todos os eventos <code>UPDATE</code> mostrarão o valor correto para os campos afetados.    </td> 
   <td></td> 
  </tr> 
  <tr> 
   <th rowspan="2">PROJ</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   <td>Quando qualquer valor de parâmetro é atualizado neste objeto, o evento <code>UPDATE</code> mostra incorretamente a alteração do campo afetado de <code>null</code> para <code>ID value</code>. </td> 
   <td>Todos os eventos <code>UPDATE</code> mostram o valor correto para o campo afetado.</td> 
   <td>Nenhum. Se você tiver um filtro no campo afetado, você receberá um evento <code>UPDATE</code> somente se esse campo tiver sido realmente alterado, não se qualquer outro valor de parâmetro tiver sido alterado.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>convertedOpTaskID</code></li>
    </ul> 
   </td> 
   <td>Quando este objeto é atualizado, o evento <code>UPDATE</code> às vezes mostra incorretamente que os campos afetados mudam de <code>null</code> para <code>ID value</code>.</td> 
   <td>Todos os eventos <code>UPDATE</code> mostram o valor correto para o campo afetado.</td> 
   <td>Nenhum. Se você tiver um filtro no campo afetado, você receberá um evento <code>UPDATE</code> somente se esse campo tiver sido realmente alterado, não se qualquer outro valor de parâmetro tiver sido alterado.
  </tr> 
  <tr> 
   <th rowspan="2">TAREFA</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   </td> 
   <td>Quando qualquer valor de parâmetro é atualizado neste objeto, o evento <code>UPDATE</code> mostra incorretamente a alteração do campo afetado de <code>null</code> para <code>ID value</code>. </td> 
   <td>Todos os eventos <code>UPDATE</code> mostram o valor correto para o campo afetado.</td> 
   <td>Nenhum. Se você tiver um filtro no campo afetado, você receberá um evento <code>UPDATE</code> somente se esse campo tiver sido realmente alterado, não se qualquer outro valor de parâmetro tiver sido alterado.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>convertedOpTaskID</code></li>
    </ul> 
   </td> 
   <td>Quando este objeto é atualizado, o evento <code>UPDATE</code> às vezes mostra incorretamente que os campos afetados mudam de <code>null</code> para <code>ID value</code>.</td> 
   <td>Todos os eventos <code>UPDATE</code> mostram o valor correto para o campo afetado.</td> 
   <td>Nenhum. Se você tiver um filtro no campo afetado, você receberá um evento <code>UPDATE</code> somente se esse campo tiver sido realmente alterado, não se qualquer outro valor de parâmetro tiver sido alterado.
 </tbody> 
</table>
