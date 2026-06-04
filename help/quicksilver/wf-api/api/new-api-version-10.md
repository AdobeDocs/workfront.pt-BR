---
content-type: api
navigation-topic: api-navigation-topic
title: Novidades na versão 10 da API
description: Recursos Atualizados
author: Becky
feature: Workfront API
role: Developer
exl-id: 8ac384ae-5d65-4c0e-98c1-cf38cfbff460
TQID: https://experienceleague.adobe.com/7paMh3l4zsoBaafv6U6pp1M-SQjk-kdmSho9GYa15SU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 484
ht-degree: 58%

---

# Novidades na versão 10 da API

* [Novos recursos](#new-resources)
* [Recursos Atualizados](#updated-resources)
* [Recursos removidos](#removed-resources)

## Novos recursos {#new-resources}

### ActivityLog

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   | ADICIONAR |
|   |   |   |   |   |   | CONTAGEM |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### EntradaCalendário

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | ADICIONAR |
|   |   |   |   |   |   | CONTAGEM  |
|   |   |   |   |   |   | EXCLUIR  |
|   |   |   |   |   |   | EDITAR  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | RELATÓRIO  |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### ReferênciaExternaDeEntradaDeCalendário

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | CONTAGEM |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | RELATÓRIO  |
|   |   |   |   |   |   | SEARCH  |

{style="table-layout:auto"}

### ExternalAuthToken

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | ADICIONAR |
|   |   |   |   |   |   | CONTAGEM |
|   |   |   |   |   |   | EXCLUIR  |
|   |   |   |   |   |   | EDITAR  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | RELATÓRIO  |
|   |   |   |   |   |   | SEARCH  |

{style="table-layout:auto"}

### LimitodeGrupoDeTiposDeLicença

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| customerID | cliente |   |   |   |   |   |
| groupID | grupo |   |   |   |   |   |
| planLimit |   |   |   |   |   |   |
| usedLicenses |   |   |   |   |   |   |
| limite de trabalho |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

### PreferênciadeCalendáriodeUsuário

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
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

**Recursos Atualizados**

Os recursos existentes a seguir foram atualizados com esta versão da API do Workfront. As alterações feitas em um recurso são indicadas da seguinte maneira:

* As adições são listadas apenas
* As remoções são indicadas com texto tachado
* As alterações são listadas na nota após a tabela

### Aprovação

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval `<sup>1</sup>`   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |
| custoOrçadoProjeto  |   |   |   |   |   |   |
| projectNetValue  |   |   |   |   |   |   |
| projectRoi  |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost  |   |   |   |   |   |   |

{style="table-layout:auto"}

`<sup>1</sup> Type changed from null to boolean`

### Atribuição

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| assignmentPercent `<sup>1</sup>` |   |   |   |   |   |   |
| viewedByAssignedToUser |   |   |   |   |   |   |

{style="table-layout:auto"}

`<sup>1</sup>`validador adicionado LESS_THAN_EQUAL

### BudgetedHour

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### PreferênciasDoCliente

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| nome `<sup>1</sup>` |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Alterações em possibleValues

### DocMetadataLinkGroup

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
|   |   |   |   | getMetadataForDocument |   |   |

{style="table-layout:auto"}

### Documento

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| `masterTaskID` |  |   |   |   |   |   |

{style="table-layout:auto"}

### DocumentRequest

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

VersãoDocumento

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| externalIntegrationType <sup>1</sup> |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Alterações em possibleValues

Despesa

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### Grupo

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
|   | licenseTypeLimit |   |   | addRemoveLicenseTypeLimits  |   |   |
|   |   |   |   | setLicenseTypeLimit |   |   |

{style="table-layout:auto"}

### LinkedFolder

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| externalIntegrationType<sup>1</sup> |  |  |  |  |   |   |

{style="table-layout:auto"}

<sup>1</sup> Alterações em possibleValues

### OpTask

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| priorityColor |   |  | pendingApproval<sup>1</sup> |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Tipo alterado de nulo para booleano

### PortalSection

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
|   |  |   | groupIDs |   |   |   |

{style="table-layout:auto"}

### Portfólio

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| portfolioNetValue |   |   |   |  |  |   |
| portfolioRoi |   |   |   |   |   |   |

{style="table-layout:auto"}

### Projeto

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| custoOrçadoProjeto  |   |   |   | linkExternalObject  |   |   |
| projectNetValue |   |   |   | unlinkExternalObject |   |   |
| projectRoi |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost |   |   |   |   |   |   |

{style="table-layout:auto"}

### AprovaçãoDaProva

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| approverDecision |   |   |   |   |   |   |

{style="table-layout:auto"}

### Taxa

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| rateValue <sup>1</sup> |  |  |  |  |  |   |

{style="table-layout:auto"}

<sup>1</sup>MOEDA do validador adicionada

### Tarefa

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| kanbanFlag |   |   |   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### Equipe

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| hoursPerPoint <sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> adicionou um validador LESS_THAN

### Atribuição da equipe

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### TarefaEquipe

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### Folha de horas

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

### Atualização

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| updateType `<sup>1</sup>` |   |   |   |   |   | objectUpdatesWithNoteAndJournalEntryIndex  |

{style="table-layout:auto"}

<sup>1</sup> alterações em possibleValues

### Usuário

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
|   | accessLevel  |   |   |   |   |   |

{style="table-layout:auto"}

### UserNote

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| eventType <sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> alterações em possibleValues

### Trabalho

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval <sup>1</sup>  |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Tipo alterado de nulo para booleano

## Recursos removidos {#removed-resources}

### ResourceBudgetedHour

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | ADICIONAR  |
| budgetedHours |   |   |   |   |   | CONTAGEM  |
| ID |   |   |   |   |   | EXCLUIR  |
| plannedBudgetedHours |   |   |   |   |   | EDITAR  |
| projectID |   |   |   |   |   | GET  |
| roleID |   |   |   |   |   | RELATÓRIO  |
| userID |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

 

 

 
