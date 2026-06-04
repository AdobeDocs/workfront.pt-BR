---
content-type: api
navigation-topic: api-navigation-topic
title: Novidades na versão 6 da API
description: Novidades na versão 6 da API
author: Becky
feature: Workfront API
role: Developer
exl-id: e671a881-b8c2-4234-a3a0-76b1fbfafd32
TQID: https://experienceleague.adobe.com/ZXBvvhz5ObfHlwX2BBBs2-F2DbSmgY4lj8TwWnMCzBM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 513
ht-degree: 53%

---

# Novidades na versão 6 da API

## Novos Objetos

### Gerenciador de Recursos

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| ID | cliente |   |   |   |   | Add |
| customerID | projeto |   |   |   |   | Contagem |
| projectID | resourceManager |   |   |   |   | Excluir |
| resourceManagerID | modelo |   |   |   |   | Obter |
| templateID |   |   |   |   |   | Relatório  |
|   |   |   |   |   |   | Pesquisar  |


### Ews

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| fileName |   |   |   |   | upload |   |
| identificador |   |   |   |   |   |   |
| objCode |   |   |   |   |   |   |


### Rótulo personalizado

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| ID |   |   |   | checkDelete | customLabels | Add |
|   |   |   |   | inUseByOtherLayoutTemplate | userCustomLabels | Contagem |
|   |   |   |   | removeCustomLabel |   | Excluir |
|   |   |   |   |   |   | Obter |
|   |   |   |   |   |   | Relatório |
|   |   |   |   |   |   | Pesquisar |


## Objetos Atualizados

Alterações em objetos existentes: as adições são simplesmente listadas, as remoções têm tachado, as alterações em objetos existentes têm uma nota anexada após a tabela

### Atualização

 

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> |   |   |   |   | `sinceDate` |   |
|   |   |   |   |   | objectUpdatesByCommentID<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> Alterações em valores possíveis

<sup>2</sup> atributo hasFilters alterado para verdadeiro

 

### Aprovação

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| completedHours |   | resourceManagers | resourceManagerIDs |   |   |   |
| constraintDate<sup>1</sup> |   |   |   |   |   |   |
| isOriginalPlannedHoursSet |   |   |   |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Validação de data adicionada

<sup>2</sup> sinalizador NOT_FILTERABLE adicionado

 

### Processo de aprovação

|   | Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|---|
|   |  | `attachedApprovalPaths` |   |   |   |   |   |

{style="table-layout:auto"}

 

### Etapa de aprovação

 

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| approvalType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Alterações em valores possíveis

 

### Caminho de aprovação<sup>1</sup>

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| approvedStatus |   |   |   |   |   | Add |
| approvedStatusLabel |   |   |   |   |   | Contagem |
| comentário |   |   |   |   |   | Excluir |
| enteredByID |   |   |   |   |   | Editar |
| entryDate |   |   |   |   |   | Obter |
| globalPathID |   |   |   |   |   | Relatório |
| isPrivate |   |   |   |   |   | Pesquisar |
| lastUpdateDate |   |   |   |   |   |   |
| lastUpdateByID |   |   |   |   |   |   |
| nome<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> alterado para reportável

<sup>2</sup> Adicionou O Validador De Comprimento Máximo

 

### Objeto de serviço de trabalho

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| constraintDate<sup>1</sup> |   |   |   | getMyWorkCountFiltered |   |   |
| workRequired<sup>2</sup> |   |   |   | workitemStatusLabels  |   |   |

{style="table-layout:auto"}

<sup>1</sup> Validação de data adicionada

<sup>2</sup> Sinalizador Not_Filterable Adicionado

 

### Atribuição

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnProjects |   |   |
|   |   |   |   | swapUsersOnProjects |   |   |
|   |   |   |   | unassignUserFromProjects |   |   |

{style="table-layout:auto"}

 

### Linha de base 

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Sinalizador Not_Filterable Adicionado

 

### Tarefa da Linha de Base

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Sinalizador Not_Filterable Adicionado

 

### Registro de cobrança

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| billingDate<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> adicionou sinalizador de campo NO_TIME

### Evento de burndown 

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| eventInitiator |   |   |   |   |   | `ADD` |
|   |   |   |   |   |   | `DELETE` |

{style="table-layout:auto"}

 

### Categoria 

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
|   |   |   |   | getCascadingRules |   |   |
|   |   |   |   | reorderCategories |   |   |

{style="table-layout:auto"}

 

Lista Discriminada Personalizada 

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
|   |   |   |   | getGroupDefaultProjectStatus | opTaskGroupStatuses |   |
|   |   |   |   | isPossibleToUnlockStatus | projectGroupStatus |   |
|   |   |   |   |   | taskGroupStatuses |   |

{style="table-layout:auto"}

 

Documento 

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| `checkedOutByID` | `checkedOutBy`  |   |  isDir |   |   |   |
| `isDir`  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

Taxa de câmbio 

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| taxa<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> alterou o validador PRECISION de 8 para 9

 

### Integração

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| syncBurndownDate |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### Lançamento documentado

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| changeType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Alterações em valores possíveis

 

### Optask (Problema)<sup>1</sup> 

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> sinalizado como RESTORÁVEL

<sup>2</sup> Sinalizador Not_Filterable Adicionado

 

### Projeto<sup>1</sup> 

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| completedHours |   | `openOpTasks` |  openOpTasks |   |   |   |
| isOriginalPlannedHoursSet |   | resourceManagers | resourceManagerIDs  |   |   |   |
| originalWorkRequired |   |   | `work` |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| trabalho |   |   |   |   |   |   |
| workRequired |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> sinalizado como RESTORABLE e RESOURCE_MANAGEABLE

<sup>2</sup> Sinalizador Not_Filterable Adicionado

 

### Tarefa<sup>1</sup>

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| constraintDate<sup>2</sup> |   |   |   |   |   |   |
| workRequired<sup>3</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> sinalizado como RESTORÁVEL

<sup>2</sup> validador AT_DATE_YEAR_BEFORE adicionado

<sup>3</sup> Sinalizador Not_Filterable Adicionado

 

### Equipe

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| `myWorkViewID` |  `myWorkView` |   |   |   |   |   |
| `requestsViewID`  | `myRequestsView`  |   |   |   |   |   |

{style="table-layout:auto"}

 

### Modelo<sup>1</sup> 

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
|   |   | resourceManagers | resourceManagerIDs |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> sinalizado como RESTORABLE e RESOURCE_MANAGEABLE

### Modelo de Tarefa<sup>1</sup> 

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> sinalizado como RESTORÁVEL

<sup>2</sup> Sinalizador Not_Filterable Adicionado

 

### Usuário

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| myInfo<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> violadores de MAX_LENGTH

 

### Observação do usuário

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| eventType<sup>1</sup> |   |   |   |   | myNotifications<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> Valores possíveis alterados

<sup>2</sup> tem filtros alterados para `[true]`

 

### Aviso

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
|   |   |   |   | `fileHandle` |   |   |
|   |   |   |   | `zipAnnouncementAttachments`  |   |   |
