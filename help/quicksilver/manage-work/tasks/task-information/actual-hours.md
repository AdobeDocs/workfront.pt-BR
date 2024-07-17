---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visualizar Horas Efetivas
description: As horas em que você faz logon nos itens de trabalho no Adobe Workfront são consideradas Horas Reais.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# Visualizar Horas Efetivas

As horas em que você faz logon nos itens de trabalho no Adobe Workfront são consideradas Horas Reais.

As Horas Reais representam o tempo real que você levou para concluir uma tarefa, problema ou um projeto.

Recomendamos que as horas sejam registradas nos itens de trabalho, que são tarefas e problemas.

No entanto, como administrador do Workfront, você também pode permitir que os usuários façam logon em projetos, dependendo de quais workflows estão em sua organização.

Para obter mais informações sobre como configurar seu sistema para permitir que os usuários façam logon em projetos, consulte [Configurar preferências de horas e folha de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Trabalhar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Visualizar ou ter maior acesso a tarefas, projetos ou problemas</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualize ou aumente as permissões para uma tarefa, um projeto ou um problema</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Horas efetivas de tarefas e problemas versus Horas efetivas de projetos

As Horas Reais em tarefas e problemas representam o número de horas registradas diretamente nas tarefas e problemas.

>[!NOTE]
>
>As Horas Reais das tarefas filhas totalizam as Horas Reais da tarefa pai. A seguinte fórmula se aplica às Horas Reais em uma tarefa pai:

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

As horas efetivas de projetos representam um total de horas efetivas de todas as tarefas no projeto (incluindo horas registradas diretamente em tarefas pai), todas as questões no projeto, bem como as horas efetivas registradas no próprio projeto.

A fórmula a seguir se aplica às Horas Reais em um projeto:

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## Localizar Horas Efetivas

Encontrar o valor de Horas Reais de um item é idêntico para tarefas, projetos e problemas.

Você pode encontrar as informações de Horas Reais nas tarefas nos seguintes locais:

* [Horas Efetivas na seção Detalhes](#actual-hours-in-the-details-section)
* [Horas efetivas na seção de horas](#actual-hours-in-the-hours-section)
* [Horas efetivas em relatórios](#actual-hours-in-reports)
* [Horas efetivas nas ferramentas de gerenciamento de recursos](#actual-hours-in-resource-management-tools)

### Horas Efetivas na seção Detalhes {#actual-hours-in-the-details-section}

Encontrar as Horas efetivas na seção Detalhes é idêntico para projetos, tarefas e problemas.

Para localizar Horas Reais em Detalhes da Tarefa:

1. Vá para uma tarefa para a qual deseja revisar as Horas Efetivas.
1. Clique em **Detalhes da tarefa** no painel esquerdo.
1. Clique em **Visão geral** e observe o valor de **Horas efetivas**.

   Este é o total de horas registradas nesta tarefa.

### Horas efetivas na seção Horas {#actual-hours-in-the-hours-section}

Encontrar Horas efetivas na seção Horas é idêntico para projetos, tarefas e problemas.

Para localizar Horas Reais na seção Horas:

1. Vá para uma tarefa para a qual deseja revisar as Horas Efetivas.
1. Clique em **Horas** no painel esquerdo.

   Dependendo da sua configuração, a seção Horas pode estar listada em **Mostrar Mais**.

   Isso exibe uma lista de entradas de horas registradas na tarefa.

1. Certifique-se de que o modo de exibição **Padrão** e o agrupamento **Projeto** sejam aplicados a esta lista.

   O número mostrado na linha de agrupamento para a coluna **Hours** é o número total de Horas Reais na tarefa.

### Horas efetivas em relatórios {#actual-hours-in-reports}

Ao criar relatórios de tarefas, problemas ou projetos, você pode mostrar o valor de Horas efetivas para cada tarefa, problema ou projeto no relatório.

Adicionar a coluna Horas efetivas a uma visualização de tarefa é semelhante a criar uma visualização em um relatório.

Para mostrar Horas Reais em um relatório de tarefa:

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu principal** no canto superior direito do Workfront e em **Relatórios**.
1. Clique em **Novo Relatório** e escolha **Tarefa** como seu objeto.

1. Clique em **Adicionar coluna** e comece a digitar **Horas efetivas** quando o campo suspenso **Mostrar nesta coluna** for exibido. Selecione o campo quando ele aparecer na lista.

1. Clique em **Salvar + Fechar** para salvar o relatório.

   A coluna Horas Reais mostra o número de horas registradas em cada tarefa.

### Horas efetivas nas ferramentas de gerenciamento de recursos {#actual-hours-in-resource-management-tools}

Se quiser ver o progresso do trabalho que seus usuários estão fazendo nas tarefas e problemas atribuídos, você pode visualizá-los nas seguintes ferramentas de Gerenciamento de recursos:

* Relatório de Utilização.\
  Para obter informações sobre o relatório de utilização, consulte [Visão Geral do Relatório de Utilização de Recursos](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* Planejador de recursos.

  Para obter informações sobre a exibição de Horas Reais no Planejador de Recursos, consulte [Exibir Horas Disponíveis, Planejadas e Reais ou FTE no Planejador de Recursos ao usar a exibição Usuário](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).

## Registrar de tempo

Você pode registrar horas em tarefas, problemas e projetos de várias maneiras.

Para obter mais informações sobre como registrar horas no Workfront, consulte [Registrar horas](../../../timesheets/create-and-manage-timesheets/log-time.md).
