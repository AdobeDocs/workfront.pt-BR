---
content-type: api
navigation-topic: api-navigation-topic
title: Novidades na API versão 6
description: Novidades na API versão 6
author: Becky
feature: Workfront API
exl-id: e671a881-b8c2-4234-a3a0-76b1fbfafd32
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 33%

---

# Novidades na API versão 6

## Novos objetos

### Gerenciador de Recursos

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| ID | cliente |   |   |   |   | Adicionar |
| customerID | projeto |   |   |   |   | Contagem |
| projectID | resourceManager |   |   |   |   | Excluir |
| resourceManagerID | modelo |   |   |   |   | Get |
| templateID |   |   |   |   |   | Relatório  |
|   |   |   |   |   |   | Pesquisar  |


### Ews

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| fileName |   |   |   |   | fazer upload |   |
| identificador |   |   |   |   |   |   |
| objCode |   |   |   |   |   |   |


### Rótulo personalizado

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| ID |   |   |   | checkDelete | customLabels | Adicionar |
|   |   |   |   | inUseByOtherLayoutTemplate | userCustomLabels | Contagem |
|   |   |   |   | removeCustomLabel |   | Excluir |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | Relatório |
|   |   |   |   |   |   | Pesquisar |


## Objetos atualizados

Alterações em objetos existentes: as adições são simplesmente listadas, as remoções têm tachado, as alterações nas existentes têm uma nota anexada após a tabela

### Atualizar

 

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| updateType¹ |   |   |   |   | `sinceDate` |   |
|   |   |   |   |   | objectUpdatesByCommentID² |   |

{style="table-layout:auto"}

¹ Alterações aos valores possíveis

² atributo hasFilters alterado para true

 

### Aprovação

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| completedHours |   | resourceManagers | resourceManagerIDs |   |   |   |
| constraintDate¹ |   |   |   |   |   |   |
| isOriginalPlannedHoursSet |   |   |   |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| workRequired² |   |   |   |   |   |   |

{style="table-layout:auto"}

¹ Validação de data adicionada

² Sinalizador NOT_FILTERABLE adicionado

 

### Processo de aprovação

|   | Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|---|
|  |  | `attachedApprovalPaths` |   |   |   |   |   |

{style="table-layout:auto"}

 

### Etapa de aprovação

 

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| approvalType¹ |   |   |   |   |   |   |

{style="table-layout:auto"}

¹ Alterações nos valores possíveis

 

### Caminho de aprovação¹

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| approvedStatus |   |   |   |   |   | Adicionar |
| approvedStatusLabel |   |   |   |   |   | Contagem |
| comentário |   |   |   |   |   | Excluir |
| enteredByID |   |   |   |   |   | Editar |
| entryDate |   |   |   |   |   | Get |
| globalPathID |   |   |   |   |   | Relatório |
| isPrivate |   |   |   |   |   | Pesquisar |
| lastUpdateDate |   |   |   |   |   |   |
| lastUpdateByID |   |   |   |   |   |   |
| name² |   |   |   |   |   |   |

{style="table-layout:auto"}

¹ Alterado para Reportável

² Validador de tamanho máximo adicionado

 

### Objeto do Serviço de Trabalho

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| constraintDate¹ |   |   |   | getMyWorkCountFiltered |   |   |
| workRequired² |   |   |   | workItemStatusLabels  |   |   |

{style="table-layout:auto"}

¹ Validação de data adicionada

² Sinalizador Not_Filterable Adicionado

 

### Atribuição

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnProjects |   |   |
|   |   |   |   | swapUsersOnProjects |   |   |
|   |   |   |   | unassignUserFromProjects |   |   |

{style="table-layout:auto"}

 

### Linha de base 

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| workRequired¹ |   |   |   |   |   |   |

{style="table-layout:auto"}

¹ Sinalizador não_filtrável adicionado

 

### Tarefa da Linha de Base

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| workRequired¹ |   |   |   |   |   |   |

{style="table-layout:auto"}

¹ Sinalizador não_filtrável adicionado

 

### Registro de Cobrança

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| billingDate¹ |   |   |   |   |   |   |

{style="table-layout:auto"}

¹ adição do sinalizador de campo NO_TIME

### Evento de detalhamento 

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| eventInitiator |   |   |   |   |   | `ADD` |
|   |   |   |   |   |   | `DELETE` |

{style="table-layout:auto"}

 

### Categoria 

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|   |   |   |   | getCascadingRules |   |   |
|   |   |   |   | reorderCategories |   |   |

{style="table-layout:auto"}

 

Enumerado Personalizado 

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|   |   |   |   | getGroupDefaultProjectStatus | opTaskGroupStatus |   |
|   |   |   |   | isPossibleToUnlockStatus | projectGroupStatus |   |
|   |   |   |   |   | taskGroupStatus |   |

{style="table-layout:auto"}

 

Documento 

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| `checkedOutByID` | `checkedOutBy`  |   |  isDir |   |   |   |
| `isDir`  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

Taxa de câmbio 

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| rate¹ |   |   |   |   |   |   |

{style="table-layout:auto"}

¹ Validador de PRECISÃO alterado para 8 a 9

 

### Integração

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| syncBurndownDate |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### Entrada no Relatório

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| changeType¹ |   |   |   |   |   |   |

{style="table-layout:auto"}

¹ Alterações nos valores possíveis

 

### Tarefa (Edição)¹ 

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| workRequired² |   |   |   |   |   |   |

{style="table-layout:auto"}

¹ Sinalizado como RESTAURÁVEL

² Sinalizador Not_Filterable Adicionado

 

### Projeto¹ 

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| completedHours |   | `openOpTasks` |  openOpTasks |   |   |   |
| isOriginalPlannedHoursSet |   | resourceManagers | resourceManagerIDs  |   |   |   |
| originalWorkRequired |   |   | `work` |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| trabalho |   |   |   |   |   |   |
| workRequired |   |   |   |   |   |   |

{style="table-layout:auto"}

¹ Sinalizado como RESTORABLE e RESOURCE_MANAGEABLE

² Sinalizador Not_Filterable Adicionado

 

### Tarefa¹

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| constraintDate² |   |   |   |   |   |   |
| workRequired³ |   |   |   |   |   |   |

{style="table-layout:auto"}

¹ Sinalizado como RESTAURÁVEL

² Adição do validador AT_DATE_YEAR_BEFORE

³ Sinalizador Not_Filterable Adicionado

 

### Equipe

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| `myWorkViewID` |  `myWorkView` |   |   |   |   |   |
| `requestsViewID`  | `myRequestsView`  |   |   |   |   |   |

{style="table-layout:auto"}

 

### Modelo¹ 

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|   |   | resourceManagers | resourceManagerIDs |   |   |   |

{style="table-layout:auto"}

¹ Sinalizado como RESTORABLE e RESOURCE_MANAGEABLE

### Modelo de Tarefa¹ 

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| workRequired² |   |   |   |   |   |   |

{style="table-layout:auto"}

¹ Sinalizado como RESTAURÁVEL

² Sinalizador Not_Filterable Adicionado

 

### Usuário

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| myInfo¹ |   |   |   |   |   |   |

{style="table-layout:auto"}

¹ Violadores MAX_LENGTH

 

### Nota do usuário

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| eventType¹ |   |   |   |   | myNotifications² |   |

{style="table-layout:auto"}

¹ Valores possíveis alterados

² tem filtros alterados para `[true]`

 

### Aviso

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|   |   |   |   | `fileHandle` |   |   |
|   |   |   |   | `zipAnnouncementAttachments`  |   |   |
