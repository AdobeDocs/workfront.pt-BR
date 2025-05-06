---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visualizar Horas Efetivas
description: As horas em que você faz logon nos itens de trabalho no Adobe Workfront são consideradas Horas Reais.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: 3827e834a71084f14a99cb27aadefd97327b02d7
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# Visualizar Horas Efetivas

<!-- Audited: 5/2025 -->

As horas em que você faz logon nos itens de trabalho no Adobe Workfront são consideradas Horas Reais.

As Horas Reais representam o tempo real que você levou para concluir uma tarefa, problema ou um projeto.

Recomendamos que as horas sejam registradas nos itens de trabalho, que são tarefas e problemas. No entanto, como administrador do Workfront, você pode permitir que os usuários também façam logon em projetos, dependendo dos fluxos de trabalho da organização.

Para obter mais informações sobre como configurar seu sistema para permitir que os usuários façam logon em projetos, consulte [Configurar preferências de horas e folha de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Novo: Padrão<p>
   <p>Ou</p>
   <p>Atual: trabalho ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Visualizar ou ter maior acesso a tarefas, projetos ou problemas</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualize ou aumente as permissões para uma tarefa, um projeto ou um problema</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Horas efetivas de tarefas e problemas versus Horas efetivas de projetos

As Horas Reais em tarefas e problemas representam o número de horas registradas diretamente nas tarefas e problemas.

As Horas Reais das tarefas filhas totalizam as Horas Reais da tarefa pai. A seguinte fórmula se aplica às Horas Reais em uma tarefa pai:

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

As horas efetivas de projetos representam um total de horas efetivas de todas as tarefas do projeto (incluindo horas registradas diretamente em tarefas pai), todos os problemas do projeto e as horas efetivas registradas no próprio projeto.

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
1. No painel esquerdo, clique em **Detalhes da tarefa**. A seção **Visão geral** é exibida.
1. Localize o valor **Horas Efetivas** na seção **Horário de Trabalho**. Este é o total de horas registradas nesta tarefa.

### Horas efetivas na seção Horas {#actual-hours-in-the-hours-section}

Encontrar Horas efetivas na seção Horas é idêntico para projetos, tarefas e problemas.

Para localizar as Horas Reais na seção Horas:

1. Vá para uma tarefa para a qual deseja revisar as Horas Efetivas.

1. No painel esquerdo, clique em **Horas**. Uma lista de entradas de horas registradas na tarefa é exibida, com a coluna **Horas** mostrando o número total de Horas Efetivas da tarefa.

1. Certifique-se de que o modo de exibição **Padrão** e o agrupamento **Projeto** sejam aplicados a esta lista.

### Horas efetivas em relatórios {#actual-hours-in-reports}

Ao criar relatórios de tarefas, problemas ou projetos, você pode mostrar o valor de Horas efetivas para cada tarefa, problema ou projeto no relatório.

Para mostrar Horas Reais em um relatório de tarefa:

{{step1-to-reports}}

1. Na página **Relatórios**, clique em **Novo relatório** e escolha **Tarefa** como seu objeto.
1. No canto inferior direito da página, clique em **Adicionar coluna**.
1. No campo suspenso **Mostrar nesta coluna** exibido, comece digitando **Horas efetivas** e, em seguida, selecione o campo quando ele aparecer na lista.

1. No canto inferior esquerdo da página, clique em **Salvar + Fechar** para salvar o relatório.

1. Na caixa de diálogo **Nomear este Relatório para Salvá-lo**, digite um novo nome de relatório e clique em **Aplicar**.

### Horas efetivas nas ferramentas de gerenciamento de recursos {#actual-hours-in-resource-management-tools}

Se quiser ver o progresso do trabalho que seus usuários estão fazendo nas tarefas e problemas atribuídos, você pode visualizá-los nas seguintes ferramentas de Gerenciamento de recursos:

* O Relatório De Utilização.\
  Para obter informações, consulte [Visão Geral do Relatório de Utilização de Recursos](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* O Planejador de recursos.

  Para obter informações, consulte [Exibir Horas Disponíveis, Planejadas e Efetivas ou FTE no Planejador de Recursos ao usar a exibição Usuário](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).

## Registrar de tempo

Você pode registrar horas em tarefas, problemas e projetos de várias maneiras.

Para obter mais informações, consulte [Log time](../../../timesheets/create-and-manage-timesheets/log-time.md).
