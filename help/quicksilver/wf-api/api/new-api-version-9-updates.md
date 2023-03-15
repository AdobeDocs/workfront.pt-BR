---
content-type: api
navigation-topic: api-navigation-topic
title: Atualizações da API versão 9
description: Recursos atualizados
author: Becky
feature: Workfront API
exl-id: 51892846-d93f-4363-8416-4118fb2ef84d
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 36%

---

# Atualizações da API versão 9

## Recursos atualizados

Os recursos existentes a seguir foram atualizados com esta versão da API do Adobe Workfront. Para visualizar os recursos novos da versão 9, você pode visitar [Novidades na API versão 9](../../wf-api/api/new-api-version-9.md) e [Novidades da API versão 9 (continuação)](../../wf-api/api/new-api-version-9-continue.md). As alterações feitas em um recurso são indicadas da seguinte maneira:

* As adições são simplesmente listadas
* As remoções são indicadas com texto tachado
* As alterações são anotadas na nota após a tabela

### TrabalhoÁgil

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| `opTaskID`<sup>2</sup> |  |  |  |  |  |  |
| `taskID`<sup>2</sup> |  |  |  |  |  |  |

{style="table-layout:auto"}

¹ Sinalizador removido: REPORTABLE\
² Sinalizador removido: NOT_GROUPABLE

### Aprovação

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| `storyBoardOrder` | `agileWork` |   |   |   |   |   |

{style="table-layout:auto"}

Atribuição

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|  |  |  |  | `assignUserToRoleOnProjects`<sup>1</sup> |  |  |
|  |  |  |  | `assignUserToRoleOnTasks`<sup>1</sup> |  |  |
|  |  |  |  | `swapUsersOnProjects`<sup>1</sup> |  |  |
|  |  |  |  | `swapUsersOnTasks`<sup>1</sup> |  |  |

{style="table-layout:auto"}

¹ Campo adicionado: lockToRole

### CustomerPreferences

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| `name`<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

¹ Alterações nos valores possíveis

### Hora

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| `days` |  |  |  |  |  |  |
| `workHoursPerDay` |  |  |  |  |  |  |

{style="table-layout:auto"}

### Iteração

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|  |  |  |  | `moveIssues` |  |  |

{style="table-layout:auto"}

### Modelos de layout

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| `groupID` | `group` |  |  |  |  |  |

{style="table-layout:auto"}

### Nota

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| `html` |  |  |  |  |  |  |
| `json` |  |  |  |  |  |  |
| `richTextNoteID` |  |  |  |  |  |  |

{style="table-layout:auto"}

### OpTask

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| `color` | `agileWork` |  |  | `convertToProject` |  |  |
| `isReady` |  |  |  | `convertToTask` |  |  |
| `storyBoardOrder` |  |  |  | `linkExternalObject` |  |  |
|  |  |  |  | `unlinkExternalObject` |  |  |

{style="table-layout:auto"}

### ResourceBudget

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| `ID` |  |  |  |  |  |  |

{style="table-layout:auto"}

¹ Sinalizador removido: REPORTABLE

### Cronograma

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| `homeGroupID` | `homeGroup` |  |  |  |  |  |

{style="table-layout:auto"}

### Tarefa

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|  | `agileWork` |  |  | `convertToProject` |  |  |
|  |  |  |  | `linkExternalObject` |  |  |
|  |  |  |  | `unlinkExternalObject` |  |  |

{style="table-layout:auto"}

### Equipe

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| `includeIssues` |  |  |  |  |  |  |

{style="table-layout:auto"}

### TimesheetProfile

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| `groupID` | `group` |  |  |  |  |  |

{style="table-layout:auto"}

### UIFilter

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|  |  |  |  |  | `filtersForObjCode` |  |

{style="table-layout:auto"}

### UIView

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|  |  |  |  |  | `viewsForObjCode` |  |

{style="table-layout:auto"}

### Usuário

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| `logTimeInDays` |  |  |  |  |  |  |
| `workHoursPerDay` |  |  |  |  |  |  |

{style="table-layout:auto"}

### Trabalho

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| `storyBoardOrder` | `agileWork` |  |  | `getWFHomeObjects` |  |  |
