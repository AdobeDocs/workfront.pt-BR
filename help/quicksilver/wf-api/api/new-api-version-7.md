---
content-type: api
navigation-topic: api-navigation-topic
title: Novidades na API versão 7
description: Coleções
author: Becky
feature: Workfront API
exl-id: 8c575251-677b-474d-84aa-02b637ef7760
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 50%

---

# Novidades na API versão 7

## Novos objetos

### Bean de prova

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | Pesquisar |
| beca sem saída |   |   |   |   |   |   |
| name |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### DocMetadataLink

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Campos</th> 
   <th>Referências</th> 
   <th> <p data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Type&quot;}">Coleções</p> <p data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Type&quot;}">+++++++++++ </p> </th> 
   <th>Pesquisar</th> 
   <th>Ações</th> 
   <th>Queries</th> 
   <th>Operações</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>ID</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>Adicionar</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>Contagem </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>Excluir </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>Get  </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>Relatório </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>Pesquisar </td> 
  </tr> 
 </tbody> 
</table>

### DocMetadataLinkGroup

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | Adicionar |
|   |   |   |   |   |   | Contagem |
|   |   |   |   |   |   | Excluir |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | Relatório |
|   |   |   |   |   |   | Pesquisar |

{style=&quot;table-layout:auto&quot;}

### AprovaçãoDeProva

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | Contagem |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | Relatório |
|   |   |   |   |   |   | Pesquisar |

{style=&quot;table-layout:auto&quot;}

 

### ContornoRecurso

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | Adicionar |
|   |   |   |   |   |   | Contagem |
|   |   |   |   |   |   | Excluir |
|   |   |   |   |   |   | Editar |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | Relatório |
|   |   |   |   |   |   | Pesquisar |

{style=&quot;table-layout:auto&quot;}

 

### UserGroups

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| groupID | grupo |   |   |   |   |   |
| isOwner  | usuário  |   |   |   |   |   |
| userID  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### TimesheetProfile

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| ID |   |  hourTypes |   |   |   | Adicionar |
| name |   |   |   |   |   | Copiar |
|   |   |   |   |   |   | Contagem |
|   |   |   |   |   |   | Excluir |
|   |   |   |   |   |   | Editar |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | Relatório |
|   |   |   |   |   |   | Pesquisar |
|   |   |   |   |   |   | Substituir |

{style=&quot;table-layout:auto&quot;}

 

### RsrcPool

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| ID | cliente | usuários |   |   |   | Adicionar |
| customerID  | enteredBy  |   |   |   |   | Contagem |
| descrição  | lastUpdatedBy  |   |   |   |   | Excluir |
| enteredByID  |   |   |   |   |   | Editar |
| entryDate  |   |   |   |   |   | Get |
| extRefID  |   |   |   |   |   | Relatório |
| lastUpdateDate |   |   |   |   |   | Pesquisar |
| lastUpdateByID |   |   |   |   |   |   |
| name |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### DocMetadataLinkGroup

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | Contagem |
| articleName  |   |   |   |   |   | Get |
| pageID  |   |   |   |   |   | Relatório |
| url  |   |   |   |   |   | Pesquisar |

{style=&quot;table-layout:auto&quot;}

 

 

 

## Objetos atualizados

Alterações em objetos existentes: as adições são simplesmente listadas, as remoções têm tachado, as alterações nas existentes têm uma nota anexada após a tabela

### UpdateBean

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| updateType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Alterações aos valores possíveis 

 

### ApprovalServiceObject

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |   |   |   |
| approvalStartDate¹ |   |   |   |   |   |   |
| workPerDayList |   |   |   |   |   |    |

{style=&quot;table-layout:auto&quot;}

 

### AccessRule¹

¹ Sinalizado como reportável

 

### Processo de aprovação

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|   |   | `AttachedApprovalPaths`  |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

  

### Caminho de aprovação¹

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   | `Add` |
|   |   |   |   |   |   | `Delete` |
|   |   |   |   |   |   | `Edit` |

{style=&quot;table-layout:auto&quot;}

¹ Sinalizador Reportável Removido

 

### Objeto do Serviço de Trabalho

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |   |   |   |
| approvalStartDate |   |   |   |   |   |   |
| workPerDayList |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Validação de data adicionada

² Sinalizador Not_Filterable Adicionado

 

### Atribuição

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|  workPerDayList |   |   |   | assignUserToRoleOnProjects¹ |   |   |
|   |   |   |   | swapUsersOnProjects¹ |   |   |
|   |   |   |   | unassignUserFromProjects¹ |   |   |

{style=&quot;table-layout:auto&quot;}

¹ InclusãoProblemas de campo adicionados

 

### Cliente 

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| bizRuleExclusions¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Alterações aos valores possíveis 

 

### Enumerado Personalizado 

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| groupID  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Documento 

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| checkOutTimestamp |   |   |   |  createProof |   |   |

{style=&quot;table-layout:auto&quot;}

 

### DocumentVersion 

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|   |   |   |   |  getProofingTokens |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Grupo

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| isPublic |  layoutTemplate | userGroups  |   |   |   |   |
| layoutTemplateID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Validador de PRECISÃO alterado para 8 a 9

 

### HourType

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|   |   |   |   |   | defaultOpTaskHourType |   |
|   |   |   |   |   | defaultProjectHourType |   |
|   |   |   |   |   | defaultTaskHourType  |   |
|   |   |   |   |   | globalHourTypes  |   |
|   |   |   |   |   | objectHourTypes  |   |

{style=&quot;table-layout:auto&quot;}

 

### Entrada no Relatório

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| changeType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Alterações nos valores possíveis

 

### Optask (Edição)

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |  assignMultiple |   |   |
| approvalStartDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

 

### Projeto

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |   |   |   |
| approvalStartDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

 

### QueueDef

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| allowedLegacyQueueTopicIDs |  |  |  | getQueueDefTree |   |   |

{style=&quot;table-layout:auto&quot;}

 

### QueueTopic

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|   |   |   |   |   |  queueTopicID |   |

{style=&quot;table-layout:auto&quot;}

 

### Recentes

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|   |   |   |   |  updateLastViewedObject |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Tarefa

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   | assignMultiple  |   |   |
| approvalStartDate |   |   |   |   |   |   |
| workPerDayList |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### TemplateTask

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| workRequired¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Tipo alterado de Int para Double 

 

### Usuário

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Campos</th> 
   <th>Referências</th> 
   <th>Coleções</th> 
   <th>Pesquisar</th> 
   <th>Ações</th> 
   <th>Queries</th> 
   <th>Operações</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>
    <code>lastWhatsNew</code> </td> 
   <td> </td> 
   <td>
    <code>roles</code> </td> 
   <td> funções</td> 
   <td>addMobileDevice</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <span data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;scheduleDeactivationDate&quot;}" data-sheets-userformat="{&quot;2&quot;:8707,&quot;3&quot;:{&quot;1&quot;:0},&quot;4&quot;:{&quot;1&quot;:2,&quot;2&quot;:14277081},&quot;12&quot;:0,&quot;16&quot;:10}">scheduleDeativationDate</span></td> 
   <td> </td> 
   <td><span data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;timesheetProfileHourTypes&quot;}" data-sheets-userformat="{&quot;2&quot;:8707,&quot;3&quot;:{&quot;1&quot;:0},&quot;4&quot;:{&quot;1&quot;:2,&quot;2&quot;:14277081},&quot;12&quot;:0,&quot;16&quot;:10}">timesheetProfileHourTypes</span> </td> 
   <td> </td> 
   <td>getAvailableActions</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>hasAnyAccess</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>isUserTerminologyActive</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>removeMobileDevice</p> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>showshouldProofHQNavButton</td> 
   <td> </td> 
   <td>  </td> 
  </tr> 
 </tbody> 
</table>

### Nota do usuário

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| `acknowledgedmentIDs` |   |   |   |  unackknowledgeMany |   |   |
| ackDate |   |   |   |   |   |   |
| ackType |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

 

### CustomerPrefObject

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|  name |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Alterações nos valores possíveis
