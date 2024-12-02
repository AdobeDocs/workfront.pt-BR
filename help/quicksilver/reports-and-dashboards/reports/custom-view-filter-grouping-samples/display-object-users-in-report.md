---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Relatórios ou listas: exibir usuários associados a um objeto'
description: Você pode exibir usuários, funções de trabalho e equipes associados a objetos em relatórios ou listas, bem como referenciá-los em filtros. Não é possível agrupar por usuários, funções de trabalho ou equipes associados a objetos.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 9abdaafb-da2c-4b5d-9117-59afa4a1e71f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 2%

---

# Relatórios ou listas: exibir usuários associados a um objeto

Você pode exibir usuários, funções de trabalho e equipes associados a objetos em relatórios ou listas, bem como referenciá-los em filtros. Não é possível agrupar por usuários, funções de trabalho ou equipes associados a objetos.

Você pode exibir ou filtrar por usuários, funções de trabalho ou equipes associados aos seguintes objetos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Objeto</td> 
   <td>Usuários ou funções de trabalho associados</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Projeto</td> 
   <td> <p>Você pode exibir todos os usuários e as funções de trabalho que eles atendem no projeto em um relatório de projeto. Não é possível filtrar pelos usuários ou suas funções de trabalho associadas em um relatório de projeto. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tarefas</td> 
   <td>Você pode exibir e filtrar por todos os usuários, funções de trabalho e equipes atribuídas a uma tarefa em um relatório de tarefas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Problemas</td> 
   <td>Você pode exibir e filtrar por todos os usuários, funções de trabalho e equipes atribuídos a um problema em um relatório de problemas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Portfólios</td> 
   <td>Você pode exibir todos os usuários e as funções de trabalho que eles atendem no projeto em um relatório de projeto e agrupar o relatório por Portfolio. Não é possível filtrar pelos usuários ou suas funções de trabalho associadas em um relatório de projeto.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Programas</td> 
   <td>Você pode exibir todos os usuários e as funções de trabalho que eles atendem no projeto em um relatório de projeto e agrupar o relatório por programa. Não é possível filtrar pelos usuários ou suas funções de trabalho associadas em um relatório de projeto.</td> 
  </tr> 
 </tbody> 
</table>

## Exibir todos os usuários e funções de trabalho associados a um projeto

Você pode exibir todos os usuários associados ao no projeto na visualização de uma lista de projeto ou relatório. Isso inclui todos os usuários listados na seção Pessoas do projeto. Você também pode visualizar as funções às quais estão associados quando atribuídas a tarefas ou problemas no projeto em um relatório de projeto.

![](assets/project-with-user-and-role-information-report-350x100.png)

Para obter informações sobre como criar um relatório de projeto para exibir todos os usuários e suas funções no projeto, consulte [Exibir: lista de usuários do projeto com funções de trabalho](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md).

Não é possível filtrar usuários ou funções de trabalho associados a projetos em um filtro de projeto.

## Exibir todos os usuários, funções de trabalho ou equipes atribuídos a uma tarefa

Você pode exibir todos os usuários, funções ou equipes atribuídos a uma tarefa na exibição de uma lista de tarefas ou relatório adicionando o campo Atribuições à exibição.

![](assets/assignments-field-task-view-350x124.png)

É possível filtrar por usuários, funções de trabalho ou equipes atribuídas a tarefas, referenciando os seguintes campos em um filtro de tarefa:

* Usuários atribuídos
* Funções das atribuições
* Equipe

![](assets/assignment-users-roles-task-filter-350x334.png)

## Exibir todos os usuários, funções de trabalho ou equipes atribuídos a um problema

Você pode exibir todos os usuários, funções ou equipes atribuídos a um problema na exibição de uma lista de problemas ou relatório adicionando o campo Atribuições à exibição.

É possível filtrar por usuários, funções de trabalho ou equipes atribuídas a problemas, referenciando os seguintes campos em um filtro de problemas:

* Usuários atribuídos
* Funções das atribuições
* Equipe

## Exibir todos os usuários e funções de trabalho associados a um portfólio

É possível exibir todos os usuários e funções associados a um portfólio, exibindo-os em um relatório de projeto e agrupando o relatório por Portfolio.

Para obter informações sobre como criar um relatório de projeto para exibir todos os usuários e suas funções no projeto, consulte [Exibir: lista de usuários do projeto com funções de trabalho](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md).

Não é possível filtrar usuários ou funções de trabalho associados a projetos em um filtro de portfólio ou projeto.

## Exibir todos os usuários e funções de trabalho associados a um programa

Você pode exibir todos os usuários e funções associados a um programa exibindo-os em um relatório de projeto e, em seguida, agrupando o relatório por programa.

Para obter informações sobre como criar um relatório de projeto para exibir todos os usuários e suas funções no projeto, consulte [Exibir: lista de usuários do projeto com funções de trabalho](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md).

Não é possível filtrar usuários ou funções de trabalho associados a projetos em um programa ou filtro de projeto.
