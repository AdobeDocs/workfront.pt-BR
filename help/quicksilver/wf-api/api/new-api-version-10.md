---
content-type: api
navigation-topic: api-navigation-topic
title: Novidades na API versão 10
description: Recursos atualizados
author: Becky
feature: Workfront API
exl-id: 8ac384ae-5d65-4c0e-98c1-cf38cfbff460
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 34%

---

# Novidades na API versão 10

* [Novos recursos](#new-resources)
* [Recursos atualizados](#updated-resources)
* [Recursos removidos](#removed-resources)

## Novos recursos {#new-resources}

### ActivityLog

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   | ADICIONAR |
|   |   |   |   |   |   | CONTAGEM |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### CalendarEntry

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | ADICIONAR |
|   |   |   |   |   |   | CONTAGEM  |
|   |   |   |   |   |   | EXCLUIR  |
|   |   |   |   |   |   | EDITAR  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | RELATÓRIO  |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### CalendarEntryExternalReference

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | CONTAGEM |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | RELATÓRIO  |
|   |   |   |   |   |   | SEARCH  |

{style="table-layout:auto"}

### ExternalAuthToken

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | ADICIONAR |
|   |   |   |   |   |   | CONTAGEM |
|   |   |   |   |   |   | EXCLUIR  |
|   |   |   |   |   |   | EDITAR  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | RELATÓRIO  |
|   |   |   |   |   |   | SEARCH  |

{style="table-layout:auto"}

### LicenseTypeGroupLimit

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| customerID | cliente |   |   |   |   |   |
| groupID | grupo |   |   |   |   |   |
| planLimit |   |   |   |   |   |   |
| usedLicenses |   |   |   |   |   |   |
| limite de trabalho |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

### UserHomeCalendarPreference

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| customerID | cliente |   |   |   |   | ADICIONAR |
| edTime | usuário |   |   |   |   | CONTAGEM |
| firstDayOfWeek |   |   |   |   |   | EXCLUIR |
| ID |   |   |   |   |   | EDITAR |
| showPTO |   |   |   |   |   | GET |
| startTime |   |   |   |   |   | RELATÓRIO |
| userID |   |   |   |   |   | SEARCH |
| workDate |   |   |   |   |   |   |

{style="table-layout:auto"}

**Recursos atualizados**

Os recursos existentes a seguir foram atualizados com esta versão da API do Workfront. As alterações feitas em um recurso são indicadas da seguinte maneira:

* As adições são simplesmente listadas
* As remoções são indicadas com texto tachado
* As alterações são listadas na nota após a tabela

### Aprovação

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval `¹`   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |
| projectBudgetedCost  |   |   |   |   |   |   |
| projectNetValue  |   |   |   |   |   |   |
| projectRoi  |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost  |   |   |   |   |   |   |

{style="table-layout:auto"}

`¹ Type changed from null to boolean`

### Atribuição

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| assignPercent `¹` |   |   |   |   |   |   |
| viewedByAssignedToUser |   |   |   |   |   |   |

{style="table-layout:auto"}

`¹`adicionado validador LESS_THAN_EQUAL

### HoraDeOrçamento

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### CustomerPreferences

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| name `¹` |   |   |   |   |   |   |

{style="table-layout:auto"}

¹ Alterações nos valores possíveis

### DocMetadataLinkGroup

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|   |   |   |   | getMetadataForDocument |   |   |

{style="table-layout:auto"}

### Documento

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| `masterTaskID` |  |  |  |  |  |  |

{style="table-layout:auto"}

### DocumentRequest

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| `masterTaskID` |  |  |  |  |  |  |

{style="table-layout:auto"}

DocumentVersion

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| externalIntegrationType ¹ |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

¹ Alterações nos valores possíveis

Despesa

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### Grupo

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|   | licenseTypeLimit |   |   | addRemoveLicenseTypeLimits  |   |   |
|   |   |   |   | setLicenseTypeLimit |   |   |

{style="table-layout:auto"}

### LinkedFolder

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| externalIntegrationType¹ |  |  |  |  |  |  |

{style="table-layout:auto"}

¹ Alterações nos valores possíveis

### OpTask

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| priorityColor |  |  | pendingApproval¹ |  |  |  |

{style="table-layout:auto"}

¹ Tipo alterado de nulo para booleano

### PortalSection

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|  |  |  | groupIDs |  |  |  |

{style="table-layout:auto"}

### Portfólio

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| portfolioNetValue |  |  |  |  |  |  |
| portfólioRoi |   |   |   |   |   |   |

{style="table-layout:auto"}

### Projeto

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| projectBudgetedCost  |   |   |   | linkExternalObject  |   |   |
| projectNetValue |   |   |   | unlinkExternalObject |   |   |
| projectRoi |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost |   |   |   |   |   |   |

{style="table-layout:auto"}

### AprovaçãoDeProva

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| aproverDecision |  |  |  |  |  |  |

{style="table-layout:auto"}

### Taxa

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| rateValue ¹ |  |  |  |  |  |  |

{style="table-layout:auto"}

¹MOEDA do validador adicionado

### Tarefa

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| kanbanFlag |   |   |   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### Equipe

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| horasPorPonto ¹ |   |   |   |   |   |   |

{style="table-layout:auto"}

¹ validador adicionado LESS_THAN

### AtribuiçãoEquipe

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### TeamTask

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### Planilha de horas

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

### Atualizar

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| updateType `¹` |   |   |   |   |   | objectUpdatesWithNoteAndJournalEntryIndex  |

{style="table-layout:auto"}

¹ alterações nos valores possíveis

### Usuário

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|   | accessLevel  |   |   |   |   |   |

{style="table-layout:auto"}

### UserNote

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| eventType ¹ |   |   |   |   |   |   |

{style="table-layout:auto"}

¹ alterações nos valores possíveis

### Trabalho

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval ¹  |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style="table-layout:auto"}

¹ Tipo alterado de nulo para booleano

## Recursos removidos {#removed-resources}

### ResourceBudgetedHour

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| allocateDate |   |   |   |   |   | ADICIONAR  |
| budgetHours |   |   |   |   |   | CONTAGEM  |
| ID |   |   |   |   |   | EXCLUIR  |
| planBudgetedHours |   |   |   |   |   | EDITAR  |
| projectID |   |   |   |   |   | GET  |
| roleID |   |   |   |   |   | RELATÓRIO  |
| userID |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

 

 

 
