---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: tarefas pessoais'
description: Este filtro de tarefa retorna solicitações de trabalho ad hoc enviadas a um usuário ou itens de tarefa adicionados por usuários em sua área de Início. As tarefas pessoais não estão conectadas a um projeto, mas podem ser movidas para um projeto, se necessário.
author: Courtney
feature: Reports and Dashboards
exl-id: 204cfae1-7c57-4223-9e00-ac94e1e2ba3a
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 14%

---

# Filtro: tarefas pessoais

<!--Audited: 10/2024-->

Este filtro de tarefas retorna solicitações de trabalho ad hoc enviadas a um usuário ou itens de tarefa adicionados por usuários em seus widgets de tarefas na área Página inicial.

As solicitações de trabalho ad hoc e os itens de tarefa são salvos no Adobe Workfront como tarefas pessoais.

As tarefas pessoais não estão conectadas a um projeto, mas podem ser movidas para um projeto, se necessário. Para obter informações, consulte [Criar tarefas pessoais](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md).

![Relatório de tarefas pessoais](assets/personal-tasks-report.png)

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Colaborador ou Solicitação para modificar um filtro </p>
   <p>Padrão ou Plano para modificar um relatório</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar um filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrar tarefas pessoais

Para criar esse filtro:

1. Ir para uma lista de tarefas ou um relatório de tarefas.
1. No menu suspenso **Filtro**, clique em **Novo filtro**.
1. (Condicional) Clique em **Adicionar uma regra de filtro** se você estiver acessando o filtro a partir de um relatório ou comece a selecionar seus critérios de filtro no primeiro campo, se estiver acessando o filtro a partir de uma lista.
1. (Condicional) Selecione os seguintes critérios de filtragem:

   * De um filtro de lista: **Tarefa** > **Pessoal** **É verdadeiro**
   * De um filtro de relatório: **Tarefa** > **Pessoal** > **Igual (diferencia maiúsculas de minúsculas)** > **Verdadeiro**.
1. Salve o filtro.

   A lista exibe somente tarefas pessoais que não estão em nenhum projeto.
