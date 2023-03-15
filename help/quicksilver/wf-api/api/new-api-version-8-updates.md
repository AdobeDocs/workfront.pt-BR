---
content-type: api
navigation-topic: api-navigation-topic
title: Atualizações da API versão 8
description: Os recursos existentes a seguir foram atualizados com esta versão da API do Adobe Workfront. Para ver os recursos novos nas versões 8, consulte Novidades na API versão 8. As alterações feitas em um recurso são indicadas da seguinte maneira - EDITAR ME.
author: Becky
feature: Workfront API
exl-id: c6d7d2d2-cd21-4ca8-a5a0-afe3669dc959
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 26%

---

# Atualizações da API versão 8

## Recursos atualizados

Os recursos existentes a seguir foram atualizados com esta versão da API do Adobe Workfront. Para ver os recursos novos nas versões 8, consulte [Novidades na API versão 8](../../wf-api/api/new-api-version-8.md). As alterações feitas em um recurso são indicadas da seguinte maneira:

* As adições são simplesmente listadas
* As remoções são indicadas com texto tachado
* As alterações são anotadas na nota após a tabela

### AccessRequest

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| ação¹  |   |   |   |   |   |   |

{style="table-layout:auto"}

¹ Alterações aos valores possíveis

### AccessRule¹ 

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| coreAction²  |   |   |   |   |   |   |
| ações proibidas² |   |   |   |   |   |   |
| secundárioActions² |   |   |   |   |   |   |

{style="table-layout:auto"}

¹ Sinalizador removido: REPORTABLE\
² Alterações a valores possíveis

### Aprovação

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| auditTypes¹ | agileWork  | resourcePools |   |   |   |   |
| backlogOrder² | kanbanBoard  |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

¹Alterações em valores possíveis\
² Sinalizadores adicionados: DYNAMIC, LAZY_READ e NOT_GROUPABLE

### Atribuição

|   |   |   |   | Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnTasks | getAssignAssignmentsForTasks  |   |   |   |   |   |
|   |   |   |   | swapUsersOnTasks | getUnassignAssignmentsForTasks |   |   |   |   |   |
|   |   |   |   | unassignUserFromTasks |   |   |   |   |   |   |

{style="table-layout:auto"}

### Cliente

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| bizRuleExclusions¹ |   |   |   | getPackagingOptionValue |   |   |
| proofPlan¹ |   |   |   | isPackagingOptionEnabled |   |   |

{style="table-layout:auto"}

¹Alterações em valores possíveis

### CustomerPreferences

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| name¹ |   |   |   |   |   |   |

{style="table-layout:auto"}

¹Alterações em valores possíveis

### DocumentApproval

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| ID¹ |   |   |   |   |   |   |

{style="table-layout:auto"}

¹Flag acrescentou: NOT_FILTERABLE

### DocumentVersion

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| ativeProofStages |   |   |   |   |   |   |

{style="table-layout:auto"}

### Grupo

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|   |   | proprietários |   |   |   |   |

{style="table-layout:auto"}

### HourType

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| appGlobalID¹ |   |   |   |   |   |   |

{style="table-layout:auto"}

¹Flag acrescentou: NOT_FILTERABLE

### Iteração

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|   |   |   |   | moveStories |   |   |

{style="table-layout:auto"}

### Curtir

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |

{style="table-layout:auto"}

### Nota

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| auditType¹ |   |   |   |   |   |   |

{style="table-layout:auto"}

¹Alterações em valores possíveis

### OpTask

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| auditTypes¹ | agileWork  |   |   |   | defaultShownTimesheetIssues  |   |
| backlogOrder | iteração |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| estimativa |   |   |   |   |   |   |
| iterationID |   |   |   |   |   |   |

{style="table-layout:auto"}

¹Alterações em valores possíveis

### Portfólio

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| auditTypes¹ |   |   |   |   |   |   |

{style="table-layout:auto"}

¹Alterações em valores possíveis

### Programa

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| auditTypes¹ |   |   |   |   |   |   |

{style="table-layout:auto"}

¹Alterações em valores possíveis

### Projeto

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| auditTypes¹ |   | resourcePools |   |   | defaultShownTimesheetProjects |   |

{style="table-layout:auto"}

¹Alterações em valores possíveis

### AprovaçãoDeProva

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| approvalID | aprovador |   |   |   |   |   |
| documentVersionID | documentVersion |   |   |   |   |   |
| ID¹ |   |   |   |   |   |   |
| proofCreationDate |   |   |   |   |   |   |

{style="table-layout:auto"}

¹Flag acrescentou: NOT_FILTERABLE

### QueueDef

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| requestorCoreAction¹ |   |   |   |   |   |   |
| requestorForbiddenActions¹ |   |   |   |   |   |   |

{style="table-layout:auto"}

¹Alterações em valores possíveis

### Taxa

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| endDate |   |   |   | setRatesForRole  |   |   |
| name |   |   |   |   |   |   |
| startDate |   |   |   |   |   |   |

{style="table-layout:auto"}

### ReservedTime

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| extRefID |   |   |   |   |   |   |

{style="table-layout:auto"}

### ResourceManager

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| projectPriority |   |   |   |   |   |   |

{style="table-layout:auto"}

### Tarefa

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| auditTypes¹ | agileWork  |   |   |   | allTasksOnIterations  |   |
| backlogParent | kanbanBoard |   |   |   | defaultShownTimesheetTasks |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

¹Alterações em valores possíveis

### Equipe

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| agileMethodology |   |   |   |   |   |   |
| autoAddNextStory |   |   |   |   |   |   |
| includeIssues |   |   |   |   |   |   |
| TeamStoryBoardIssueStatus |   |   |   |   |   |   |
| wipLimit |   |   |   |   |   |   |

{style="table-layout:auto"}

### Modelo

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |

{style="table-layout:auto"}

### TemplateTask

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| auditTypes¹ |   |   |   |   |   |   |

{style="table-layout:auto"}

¹Alterações em valores possíveis

Atualizar

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| updateType¹ | `updateEndorsement` |   |   |   |   |   |

{style="table-layout:auto"}

¹Alterações em valores possíveis

### Usuário

|   |   | Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |   |   |
|   |   | userGroups |   |   |   |   |   |   |
|   |   | userRoles |   |   |   |   |   |   |

{style="table-layout:auto"}

### UserNote

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |
| `endorsementShareID` | `endorsementShare` |   |   |   |   |   |
| eventType¹ |   |   |   |   |   |   |

{style="table-layout:auto"}

¹Alterações em valores possíveis

### Trabalho

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| auditTypes¹ | agileWork  |   |   |   |   |   |
| backlogOrder² | kanbanBoard  |   |   |   |   |   |
| backlogParent  |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

¹Alterações em valores possíveis\
² Sinalizadores adicionados: DYNAMIC, LAZY_READ e NOT_GROUPABLE
