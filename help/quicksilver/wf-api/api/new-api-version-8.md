---
content-type: api
navigation-topic: api-navigation-topic
title: Novidades da API versão 8
description: Esta é uma lista de recursos novos da API versão 9. Para obter uma lista de atualizações que foram feitas nos recursos da versão 8, visite Atualizações para a API versão 8
author: Becky
feature: Workfront API
role: Developer
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 29%

---

# Novidades da API versão 8

## Novos recursos

Esta é uma lista de recursos novos da API versão 9. Para obter uma lista de atualizações feitas nos recursos da versão 8, visite [Atualizações da API versão 8](../../wf-api/api/new-api-version-8-updates.md)

**TrabalhoAgile**

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| backlogOrder | cliente |   |   | bulkCopy  |   | COPIAR |
| cor | iteração  |   |   |   |   | CONTAGEM |
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
| storyBoardOrder |   |   |   |   |   |   |
| storyBoardParentID |   |   |   |   |   |   |
| taskID  |   |   |   |   |   |   |
| teamID |   |   |   |   |   |   |
| tipo |   |   |   |   |   |   |
| uiObjCode |   |   |   |   |   |   |
| uiObjectID |   |   |   |   |   |   |

{style="table-layout:auto"}

### APIVersionMetadata

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| deprecationRelease |   |   |   |   |   | CONTAGEM  |
| removeRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | RELATÓRIO |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

**QuadroKanban**

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | ADICIONAR |
| name |   |   |   |   |   | CONTAGEM |
|   |   |   |   |   |   | EXCLUIR |
|   |   |   |   |   |   | EDITAR |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RELATÓRIO |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### StatusAprovaçãoProva

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |
| proofApprovalStatusID |   |   |   |   |   |   |
| proofApprovalStatusLabel |   |   |   |   |   |   |

{style="table-layout:auto"}

**MetadadosDeArquivoDeProva**

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| documentVersionID | documentVersion |   |   |   |   |   |
| fileIndex |   |   |   |   |   |   |
| fileName |   |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| isURL |   |   |   |   |   |   |

{style="table-layout:auto"}

**HorasOrçadasRecursos**

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | ADICIONAR |
| budgetedHours |   |   |   |   |   | CONTAGEM |
| plannedBudgetedHours |   |   |   |   |   | EXCLUIR |
| projectID |   |   |   |   |   | EDITAR |
| roleID |   |   |   |   |   | GET |
| userID |   |   |   |   |   | RELATÓRIO |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### FiltroDoPlanejadorDeRecursos

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | ADICIONAR |
| name |   |   |   |   |   | CONTAGEM |
|   |   |   |   |   |   | EXCLUIR |
|   |   |   |   |   |   | EDITAR |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RELATÓRIO |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

**RichTextNote**

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | CONTAGEM |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RELATÓRIO |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### Assinar

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
|  ID |   |   |   | addSubscribers | assinantes | ADICIONAR |
|   |   |   |   | removeSubscribers |   | CONTAGEM  |
|   |   |   |   | assina |   | EXCLUIR |
|   |   |   |   | cancelamentos de assinatura |   | GET |
|   |   |   |   |   |   | RELATÓRIO |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### UserRole

| Campos | Referências | Coleções | Pesquisar | Ações | Consultas | Operações |
|---|---|---|---|---|---|---|
| roleID | função |   |   |   |   |   |
| timePercentage | usuário |   |   |   |   |   |
| userID |   |   |   |   |   |   |
