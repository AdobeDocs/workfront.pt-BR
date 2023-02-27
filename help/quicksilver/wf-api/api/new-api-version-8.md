---
content-type: api
navigation-topic: api-navigation-topic
title: Novidades na API versão 8
description: Esta é uma lista de recursos novos para a API versão 9. Para obter uma lista de atualizações que foram feitas nos recursos da versão 8, visite Atualizações para a API versão 8
author: Becky
feature: Workfront API
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 32%

---

# Novidades na API versão 8

## Novos recursos

Esta é uma lista de recursos novos para a API versão 9. Para obter uma lista de atualizações que foram feitas nos recursos da versão 8, visite [Atualizações da API versão 8](../../wf-api/api/new-api-version-8-updates.md)

**TrabalhoÁgil**

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| backlogOrder | cliente |   |   | bulkCopy  |   | COPIAR |
| color | iteração  |   |   |   |   | CONTAGEM |
| customerID | lastUpdatedBy |   |   |   |   | EXCLUIR |
| estimativa | opTask |   |   |   |   | EDITAR |
| ID | projeto |   |   |   |   | GET  |
| isReady | storyboardParent |   |   |   |   | RELATÓRIO |
| iterationID | tarefa |   |   |   |   | SEARCH |
| lastUpdateDate | equipe |   |   |   |   |   |
| lastUpdatedByID |   |   |   |   |   |   |
| name |   |   |   |   |   |   |
| opTaskID |   |   |   |   |   |   |
| parentStoryBoardOrder |   |   |   |   |   |   |
| projectID |   |   |   |   |   |   |
| historyBoardOrder |   |   |   |   |   |   |
| storiesBoardParentID |   |   |   |   |   |   |
| taskID  |   |   |   |   |   |   |
| TeamID |   |   |   |   |   |   |
| tipo |   |   |   |   |   |   |
| uiObjCode |   |   |   |   |   |   |
| uiObjectID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### APIVersionMetadata

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| deprecationRelease |   |   |   |   |   | CONTAGEM  |
| removeRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | RELATÓRIO |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

**KanbanBoard**

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | ADICIONAR |
| name |   |   |   |   |   | CONTAGEM |
|   |   |   |   |   |   | EXCLUIR |
|   |   |   |   |   |   | EDITAR |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RELATÓRIO |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### ProofApprovalStatus

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |
| proofApprovalStatusID |   |   |   |   |   |   |
| proofApprovalStatusLabel |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

**ProofFileMetadata**

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| documentVersionID | documentVersion |   |   |   |   |   |
| fileIndex |   |   |   |   |   |   |
| fileName |   |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| isURL |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

**ResourceBudgetedHour**

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| allocateDate |   |   |   |   |   | ADICIONAR |
| budgetHours |   |   |   |   |   | CONTAGEM |
| planBudgetedHours |   |   |   |   |   | EXCLUIR |
| projectID |   |   |   |   |   | EDITAR |
| roleID |   |   |   |   |   | GET |
| userID |   |   |   |   |   | RELATÓRIO |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### ResourcePlannerFilter

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | ADICIONAR |
| name |   |   |   |   |   | CONTAGEM |
|   |   |   |   |   |   | EXCLUIR |
|   |   |   |   |   |   | EDITAR |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RELATÓRIO |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

**RichTextNote**

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | CONTAGEM |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RELATÓRIO |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### Assinar

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
|  ID |   |   |   | addSubscribers | assinantes | ADICIONAR |
|   |   |   |   | removeSubscribers |   | CONTAGEM  |
|   |   |   |   | subscriptions |   | EXCLUIR |
|   |   |   |   | cancelar assinaturas |   | GET |
|   |   |   |   |   |   | RELATÓRIO |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### UserRole

| Campos | Referências | Coleções | Pesquisar | Ações | Queries | Operações |
|---|---|---|---|---|---|---|
| roleID | função |   |   |   |   |   |
| timePercentage | usuário |   |   |   |   |   |
| userID |   |   |   |   |   |   |
