---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visualizar Horas Efetivas
description: As horas em que você faz logon nos itens de trabalho no Adobe Workfront são consideradas Horas Reais. As Horas Reais representam o tempo real que você levou para concluir uma tarefa, problema ou um projeto.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: d577fb1f84c2a91c7b4a37be271235ffa338c9fd
workflow-type: tm+mt
source-wordcount: '1253'
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
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> 
   <p>Novo: Padrão<p>
   <p>Ou</p>
   <p>Atual: trabalho ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Visualizar ou ter maior acesso a tarefas, projetos ou problemas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualize ou aumente as permissões para uma tarefa, um projeto ou um problema</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação da Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Horas efetivas vs. horas efetivas herdadas

Dependendo da área do Workfront em que você acessa as horas reais, elas podem se referir a uma das seguintes horas reportadas:

* Em relatórios e listas de projetos, tarefas e problemas:

   * **Horas efetivas**: horas registradas para projetos, tarefas ou problemas após maio de 2021. Eles são armazenados no banco de dados do Workfront em horas e seu campo de valor é `actualWorkRequiredDouble`.
   * **Horas Reais Herdadas**: horas registradas para projetos, tarefas ou problemas a qualquer momento, inclusive antes de maio de 2021. Eles são armazenados no banco de dados do Workfront como minutos e seu campo de valor é `actualWorkRequired`.

     >[!IMPORTANT]
     >
     >O Custo Efetivo do projeto usa as Horas Efetivas herdadas para calcular.

* Na área Detalhes do projeto, tarefa ou problema, horas reais podem ser exibidas nos seguintes campos:

   * **Horas efetivas**: na guia Detalhes, são horas registradas para projetos, tarefas ou problemas após maio de 2021. Eles são armazenados no banco de dados do Workfront em horas e seu campo de valor é `actualWorkRequiredDouble`.
   * **Horas efetivas**: em um formulário personalizado de projeto, tarefa ou problema, quando são acessadas usando um campo personalizado de referência de campo nativo que faz referência ao campo nativo Horas efetivas. Estas horas são registradas para projetos, tarefas ou problemas após maio de 2021. Eles são armazenados no banco de dados do Workfront em horas e seu campo de valor é `actualWorkRequiredDouble`.

>[!NOTE]
>
>É recomendável usar o campo Horas efetivas sempre que possível, pois o campo Horas efetivas herdadas pode exibir horas imprecisas devido à forma como os incrementos são arredondados.

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

### Horas Efetivas na seção Detalhes {#actual-hours-in-the-details-section}

Encontrar as Horas efetivas na seção Detalhes é idêntico para projetos, tarefas e problemas.

Para localizar Horas Reais em Detalhes da Tarefa:

1. Vá para uma tarefa para a qual deseja revisar as Horas Efetivas.
1. No painel esquerdo, clique em **Detalhes da tarefa**. A seção **Visão geral** é exibida.
1. Localize o valor **Horas Efetivas** na seção **Horário de Trabalho**. Este é o total de horas registradas nesta tarefa.
1. (Opcional e condicional) Se a referência do campo nativo Horas efetivas foi adicionada a um formulário personalizado de projeto, tarefa ou problema, vá para o formulário personalizado e localize as Horas efetivas no campo personalizado. Este é o total de horas registradas para o objeto.

### Horas efetivas na seção Horas {#actual-hours-in-the-hours-section}

Encontrar Horas efetivas na seção Horas é idêntico para projetos, tarefas e problemas.

Para localizar Horas Reais na seção Horas de uma tarefa:

1. Vá para uma tarefa para a qual deseja revisar as Horas Efetivas.

1. No painel esquerdo, clique em **Horas**. Uma lista de entradas de horas registradas na tarefa é exibida, com a coluna **Horas** mostrando o número total de Horas Efetivas da tarefa.

1. Certifique-se de que o modo de exibição **Padrão** e o agrupamento **Projeto** sejam aplicados a esta lista.
1. As horas efetivas da tarefa são exibidas na linha de agrupamento para a coluna **horas efetivas**.

### Horas efetivas e horas efetivas herdadas em relatórios

Ao criar relatórios de tarefas, problemas ou projetos, você pode mostrar as Horas efetivas e os valores de Horas efetivas herdadas para cada tarefa, problema ou projeto no relatório.

Para obter informações sobre a diferença entre Horas Reais e Horas Reais Herdadas, consulte a seção [Horas Reais vs. Horas Reais Herdadas](#actual-hours-vs-legacy-actual-hours) neste artigo.

Para mostrar Horas Reais e Horas Reais Herdadas em um relatório de tarefa:

{{step1-to-reports}}

1. Na página **Relatórios**, clique em **Novo relatório** e escolha **Tarefa** como seu objeto.
1. No canto inferior direito da página, clique em **Adicionar coluna**.
1. No campo suspenso **Mostrar nesta coluna**, comece digitando **Horas efetivas** e, em seguida, selecione o campo quando ele aparecer na lista.
1. Repita a etapa acima para adicionar o campo **Horas Reais Herdadas** ao relatório.

1. No canto inferior esquerdo da página, clique em **Salvar + Fechar** para salvar o relatório.

1. Na caixa de diálogo **Nomear este Relatório para Salvá-lo**, digite um novo nome de relatório e clique em **Aplicar**.
1. Repita as mesmas etapas para um relatório de projeto ou problema.

### Horas efetivas nas ferramentas de gerenciamento de recursos {#actual-hours-in-resource-management-tools}

Se quiser ver o progresso do trabalho que seus usuários estão fazendo nas tarefas e problemas atribuídos, você pode visualizá-los nas seguintes ferramentas de Gerenciamento de recursos:

* O Relatório De Utilização.\
  Para obter informações, consulte [Visão Geral do Relatório de Utilização de Recursos](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* O Planejador de recursos.

  Para obter informações, consulte [Exibir Horas Disponíveis, Planejadas e Efetivas ou FTE no Planejador de Recursos ao usar a exibição Usuário](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).


### Horas efetivas na API do Workfront

<!--this section was added as a result to this issue: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/task/6810910e0001b932e0948336208e76f2/overview-->

A maioria dos campos do Workfront que armazenam horas é salva no banco de dados do Workfront em minutos. Por exemplo, o nome do campo Horas planejadas de uma tarefa é `workRequired` no banco de dados do Workfront e ele é armazenado em minutos.

Você deve considerar a conversão de minutos em horas ao acessar esses campos em chamadas de API ou em campos ou colunas personalizados calculados.

As Horas Reais registradas de projetos, tarefas ou problemas estão atualmente armazenadas no banco de dados do Workfront como minutos e seu campo de valor é `actualWorkRequired`.

Com a seguinte versão da API do Workfront programada para ser lançada posteriormente em 2025, as Horas efetivas são armazenadas nos seguintes campos e unidades no banco de dados:

* **Horas efetivas**: horas registradas para projetos, tarefas ou problemas após maio de 2021. Eles são armazenados no banco de dados do Workfront em horas e seu campo de valor é `actualWorkRequiredDouble`.
* **Horas Reais Herdadas**: horas registradas para projetos, tarefas ou problemas a qualquer momento, inclusive antes de maio de 2021. Eles são armazenados no banco de dados do Workfront como minutos e seu campo de valor é `actualWorkRequired`.

  >[!IMPORTANT]
  >
  >O Custo Efetivo do projeto usa as Horas Efetivas herdadas para calcular.

  Para obter informações sobre como usar as Horas Efetivas em colunas calculadas ou campos, consulte [Perguntas Frequentes sobre Relatórios](/help/quicksilver/reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md).

## Registrar de tempo

Você pode registrar horas em tarefas, problemas e projetos de várias maneiras.

Para obter mais informações, consulte [Log time](../../../timesheets/create-and-manage-timesheets/log-time.md).
