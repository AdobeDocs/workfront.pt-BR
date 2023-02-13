---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Exibir Horas Reais
description: As horas em que você faz logon em seus itens de trabalho no Adobe Workfront são consideradas Horas reais.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# Exibir Horas Reais

As horas em que você faz logon em seus itens de trabalho no Adobe Workfront são consideradas Horas reais.

As Horas Reais representam o tempo real necessário para concluir uma tarefa, um problema ou um projeto.

Recomendamos que as horas sejam registradas em itens de trabalho, que são tarefas e problemas.

No entanto, como administrador do Workfront, você também pode permitir que os usuários façam logon em projetos, dependendo dos fluxos de trabalho na organização.

Para obter mais informações sobre como configurar seu sistema para permitir que os usuários façam logon nos projetos, consulte [Configurar preferências de hora e folha de ponto](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Trabalho ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Visualizar ou aumentar o acesso a Tarefas, Projetos ou Problemas</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualizar ou aumentar permissões para uma tarefa, projeto ou problema</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Horas reais em tarefas e problemas vs. Horas reais em projetos

As Horas Reais em tarefas e problemas representam o número de horas registradas diretamente nas tarefas e problemas.

>[!NOTE]
>
>Horas Reais de tarefas filhas acumulam-se até Horas Reais na tarefa pai. A seguinte fórmula se aplica às Horas Reais em uma tarefa pai:

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

As Horas Reais para Projetos representam um total de Horas Reais de todas as tarefas no projeto (incluindo horas registradas diretamente nas tarefas pai), todos os problemas no projeto, bem como as Horas Reais registradas no próprio projeto.

A seguinte fórmula se aplica às Horas Reais em um projeto:

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## Localizar Horas Reais

Encontrar o valor de Horas Reais para um item é idêntico para tarefas, projetos e problemas.

Você pode encontrar as informações de Horas Reais sobre tarefas nos seguintes locais:

* [Horas reais na seção Detalhes](#actual-hours-in-the-details-section)
* [Horas reais na seção Horas](#actual-hours-in-the-hours-section)
* [Horas reais em relatórios](#actual-hours-in-reports)
* [Horas reais nas ferramentas de Gerenciamento de recursos](#actual-hours-in-resource-management-tools)

### Horas reais na seção Detalhes {#actual-hours-in-the-details-section}

Encontrar horas reais na seção Detalhes é idêntico para projetos, tarefas e problemas.

Para localizar Horas Reais em Detalhes da Tarefa:

1. Vá para uma tarefa para a qual deseja revisar as Horas Reais.
1. Clique em **Detalhes da tarefa** no painel esquerdo.
1. Clique em **Visão geral** e observe o **Horas reais** valor.

   Este é o total de horas registradas nesta tarefa.

### Horas reais na seção Horas {#actual-hours-in-the-hours-section}

Encontrar horas reais na seção Horas é idêntico para projetos, tarefas e problemas.

Para localizar as Horas reais na seção Horas :

1. Vá para uma tarefa para a qual deseja revisar as Horas Reais.
1. Clique em **Horas** no painel esquerdo.

   Dependendo da sua configuração, a seção Horas pode ser listada em **Mostrar mais**.

   Isso exibe uma lista de entradas de hora registradas na tarefa.

1. Certifique-se de que **Padrão** e a **Projeto** os agrupamentos são aplicados a esta lista.

   O número mostrado na linha de agrupamento para o **Horas** é o número total de Horas Reais na tarefa.

### Horas reais em relatórios {#actual-hours-in-reports}

Ao criar relatórios de tarefas, problemas ou projetos, é possível exibir o valor Horas reais para cada tarefa, problema ou projeto no relatório.

Adicionar a coluna Horas reais a uma exibição de tarefa é semelhante a criar uma exibição em um relatório.

Para mostrar Horas Reais em um relatório de tarefa:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, em seguida, clique em **Relatórios**.
1. Clique em **Novo relatório** e escolha **Tarefa** como seu objeto.

1. Clique em **Adicionar coluna** e comece a digitar **Horas reais** quando a variável **Mostrar nesta coluna** o campo suspenso é exibido. Selecione o campo quando ele aparecer na lista.

1. Clique em **Salvar + Fechar** para salvar o relatório.

   A coluna Horas Reais mostra o número de horas registradas em cada tarefa.

### Horas reais nas ferramentas de Gerenciamento de recursos {#actual-hours-in-resource-management-tools}

Se quiser ver o progresso do trabalho que seus usuários estão fazendo nas tarefas e problemas atribuídos, você poderá visualizá-los nas seguintes ferramentas de Gerenciamento de Recursos:

* Relatório de utilização.\
   Para obter informações sobre o relatório de utilização, consulte [Visão Geral do Relatório de Utilização de Recursos](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* Planejamento de recursos.

   Para obter informações sobre como visualizar Horas Reais no Planejador de Recursos, consulte [Exibir Horas Disponíveis, Planejadas e Reais ou FTE no Planejador de Recursos ao usar a exibição Usuário](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).

## Tempo de registro

Você pode registrar o tempo em tarefas, problemas e projetos de várias maneiras.

Para obter mais informações sobre o tempo de logon no Workfront, consulte [Tempo de registro](../../../timesheets/create-and-manage-timesheets/log-time.md).
