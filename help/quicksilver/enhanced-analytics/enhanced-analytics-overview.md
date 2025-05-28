---
title: Visão geral da análise aprimorada
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: A análise aprimorada é uma ferramenta eficiente no Adobe Workfront com visualizações pré-criadas que permitem examinar os dados do projeto e identificar tendências com planejamento e conclusão. Essa insight em seus projetos ajuda você a gerenciar o trabalho atual e permite que você planeje com mais precisão trabalhos futuros.
author: Nolan
feature: Reports and Dashboards
exl-id: a14ad57c-859b-43df-84c0-575ccda86e50
source-git-commit: 2a6e767036ae702f6c19dc71cdb11dae8e9e37ea
workflow-type: tm+mt
source-wordcount: '1243'
ht-degree: 3%

---

# Visão geral da análise aprimorada

>[!IMPORTANT]
>
>O Analytics aprimorado foi removido do Workfront em 27 de maio. O Workfront Data Connect é uma solução nova e alternativa e pode ser usada para replicar qualquer visualização do Enhanced Analytics que você usa atualmente. <br>Consulte o [guia de descontinuação do Enhanced Analytics](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md) para obter mais informações.


A análise aprimorada é uma ferramenta eficiente no Adobe Workfront com visualizações pré-criadas que permitem examinar os dados do projeto e identificar tendências com planejamento e conclusão. Essa insight em seus projetos ajuda você a gerenciar o trabalho atual e permite que você planeje com mais precisão trabalhos futuros.

A análise aprimorada pode ajudar a identificar:

* A forma como você planeja projetos
* Quando o trabalho é adicionado aos projetos
* A quantidade de trabalho que está sendo concluída para projetos diferentes
* A quantidade de horas ou dias necessários para concluir um projeto em comparação às horas ou dias que uma equipe doméstica está agendada
* Com que frequência os usuários concluem ações específicas durante um projeto
* O progresso dos projetos, bem como as tarefas individuais dentro de um projeto

![Análises](assets/nwe-full-screen-analytics-350x222.png)

Para ver casos de uso ou saber mais sobre o gerenciamento do trabalho atual e o planejamento de trabalho futuro com a Análise aprimorada, consulte [Caminhos de aprendizado da Análise aprimorada](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home).

## Pré-requisitos

Para acessar a área Analítica aprimorada, você deve:

* Ter um plano Business ou Enterprise.

  Para obter mais informações, consulte [Planos do Workfront](https://business.adobe.com/products/workfront/pricing.html).

* Peça ao administrador do Workfront para adicionar Análises aprimoradas ao modelo de layout.

  Para obter mais informações, consulte [Análises aprimoradas: adicionando análises a modelos de layout](https://experienceleague.adobe.com/en/docs/workfront/using/home).

Para ver informações de projetos e tarefas, você deve:

* Ter permissão de Visualização para as áreas Projetos e Tarefas no seu nível de acesso.

  Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte [Criar ou modificar níveis de acesso personalizados](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Ter permissão de Visualização para tarefas e/ou projetos específicos.

  Para obter informações sobre como solicitar acesso adicional, consulte [Solicitar acesso a objetos](../workfront-basics/grant-and-request-access-to-objects/request-access.md).

## Práticas recomendadas para análise aprimorada

Para obter os melhores dados para seus projetos, use modelos com horas planejadas e dias de duração precisos. Você também precisa garantir que seus usuários insiram e atualizem os campos abaixo da maneira mais precisa possível.

>[!NOTE]
>
>Alguns dos campos a seguir são cálculos que o Workfront executa com base nas informações inseridas pelos usuários. Não é possível atualizar esses campos manualmente.

* Horas planejadas

  Este é o campo mais importante para preencher.

  >[!NOTE]
  >
  >Se suas equipes não usarem as horas planejadas, você ainda poderá ver alguns dados com base na duração do projeto.\
  >Para obter mais informações, consulte a seção [Exibição de duração](#duration-view) neste artigo.

* Nome do Projeto

  O nome deve descrever o projeto.

* Condição do projeto
* Status do projeto
* Data inicial planejada do projeto
* Data de conclusão planejada
* Data inicial efetiva do projeto
* Data de término real do projeto
* Horas de duração do projeto
* Horas efetivas do projeto
* Status da tarefa (Isso inclui marcar as tarefas como Concluídas.)
* Nome da tarefa
* Porcentagem de tarefas concluídas
* Data inicial planejada da tarefa
* Data de Término Planejada da Tarefa

>[!IMPORTANT]
>
>Pode levar até 24 horas para que as alterações feitas em tarefas e projetos sejam refletidas na Análise aprimorada.

## Visualização de duração {#duration-view}

Por padrão, as visualizações de Burndown e Mapa de árvore do projeto são baseadas em horas planejadas. Se suas equipes não usarem as horas planejadas, você poderá observar essas visualizações com base na duração do projeto.

Na Análise aprimorada, a duração de um projeto é calculada pelas seguintes fórmulas:

* Período Planejado:

  ```
  Planned Completion Date of the project - Start Date of the project
  ```

* Dias trabalhados:

  ```
  Planned Duration for tasks completed in the selected date range / Typical hours per work day
  ```

  >[!NOTE]
  >
  >8 horas é o número padrão de **horas típicas por dia útil**. Um administrador do Adobe Workfront pode atualizar a configuração **Horas típicas por dia de trabalho** em **Configuração** > **Preferências do projeto** > **Projetos** > **Linhas do tempo**.\
  >Para saber mais, consulte [Configurar preferências de projeto do sistema](../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Para obter informações sobre a Duração Planejada, consulte [Visão Geral da Duração do Projeto](../manage-work/projects/planning-a-project/project-duration.md).

## Atalhos de teclado

Você pode usar as seguintes teclas no teclado para navegar ou concluir ações específicas na área Analítica aprimorada:

| Chave | Ação |
|---|---|
| **Guia** | Navegue até cada elemento na página, bem como até uma tabela com informações sobre cada visualização que não é exibida na página |
| **Inserir** | Abrir o widget de calendário, excluir um filtro existente, abrir as opções adicionar filtro, selecionar/desmarcar valores de filtro, aplicar um filtro criado, abrir as opções de exportação em cada visualização, abrir os menus suspensos nas visualizações Burndown, Tarefas em andamento e Mapa de árvore do projeto |
| **Teclas de seta** | Navegue até datas no widget de calendário, por meio de opções de filtro ao adicionar um filtro e por meio de opções em todos os menus suspensos nas visualizações |
| **Barra de espaços** | Selecionar datas no widget de calendário, selecionar um tipo de filtro ao adicionar um filtro, selecionar uma opção de exportação no menu suspenso de cada visualização e selecionar opções nos menus suspensos nas visualizações Burndown, Tarefas em andamento e Mapa de árvore do projeto |

{style="table-layout:auto"}

Se você estiver usando um software de leitura de tela ou um plug-in, o leitor de tela lerá as informações na tela em voz alta e descreverá as ações que você está realizando ao usar as teclas listadas acima.

## Visualizações e recursos aprimorados do Analytics

Para saber mais sobre os detalhes de um recurso específico na Análise aprimorada, as ações que você pode concluir para obter mais insight e o que pode aprender com esses dados, consulte os seguintes artigos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Artigo</th> 
   <th>Explicação</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">Aplicar filtros na análise aprimorada</a> </td> 
   <td> <p>É possível aplicar filtros personalizados, filtros de campo de projeto ou filtros de equipe para visualizar apenas os projetos que se encaixam em critérios específicos. À medida que você adiciona filtros, o número de projetos é atualizado de acordo.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/understand-enhanced-analytics-kpis.md" class="MCXref xref">Entender KPIs de análise aprimorada</a> </td> 
   <td> <p>Os indicadores-chave de desempenho (KPIs) para todos os projetos em um período específico estão localizados na parte superior da tela.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../enhanced-analytics/flight-plan-overview.md" class="MCXref xref">Exibir a visualização do Plano de voo na análise aprimorada</a> </p> </td> 
   <td> <p>A visualização do <b>Plano de voo</b> mostra que a condição mudou durante a vida útil de um projeto. Interagir com a visualização fornece mais detalhes sobre datas específicas. Selecionar um projeto abre as visualizações Burndown e Tarefas em andamento.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/burndown-overview.md" class="MCXref xref">Exibir a visualização de Burndown na análise aprimorada</a> </td> 
   <td> <p>A visualização de <b>Burndown</b> mostra a velocidade planejada de um projeto em comparação à quantidade real de horas gastas em um projeto. Interagir com a visualização fornece mais detalhes sobre a condição do projeto em uma data específica.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/tasks-in-flight-overview.md" class="MCXref xref">Exibir as Tarefas na visualização em andamento na análise aprimorada</a> </td> 
   <td> <p>A visualização de <b>Tarefas em andamento</b> mostra o status de cada tarefa em um projeto. Interagir com a visualização permite fazer alterações em uma tarefa de maneira rápida e fácil.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-activity-overview.md" class="MCXref xref">Exibir a visualização da atividade de Projeto na Análise aprimorada</a> </td> 
   <td> <p>A visualização da <b>Atividade do projeto</b> mostra um mapa de calor de quando os usuários atribuídos a um projeto fizeram logon no Workfront, alteraram o status da tarefa nesse projeto e concluíram tarefas nesse projeto. Interagir com a visualização permite ver esses detalhes para cada usuário. Você também pode ver datas específicas para essas ações, bem como o número de vezes que cada ação foi concluída.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-treemap-overview.md" class="MCXref xref">Exibir a visualização do mapa de árvore do projeto na análise aprimorada</a> </td> 
   <td> <p>A visualização do <b>Mapa de árvore do projeto</b> mostra quanto tempo foi gasto em alguns projetos em comparação a outros. Interagir com a visualização fornece detalhes sobre a condição do projeto, a conclusão planejada do projeto e a conclusão real do projeto.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/activity-by-team-overview.md" class="MCXref xref">Exibir a visualização Atividade por equipe na análise aprimorada</a> </td> 
   <td> <p>A visualização <b>Atividade por equipe</b> mostra um mapa de calor de quando os usuários em uma equipe doméstica fizeram logon no Workfront, alteraram o status de uma tarefa e concluíram uma tarefa. Interagir com a visualização permite ver esses detalhes para cada usuário individual. Você também pode ver datas específicas para essas ações, bem como o número de vezes que cada ação foi concluída.</p> </td> 
  </tr> 
  <!-- Features permanently removed from Workfront
  <tr> 
   <td><a href="../enhanced-analytics/resource-capacity-overview.md" class="MCXref xref">View the Resource capacity visualization in Enhanced analytics</a> </td> 
   <td> <p>The <b>Resource capacity</b> visualization shows you which home teams have the capacity to take on more work and which home teams have more work assigned to them than they can complete. Interacting with the visualization allows you to see more details about work completed and available hours for more work.&nbsp;Selecting a team opens the Team capacity visualization.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/team-capacity-overview.md" class="MCXref xref">View the Team capacity visualization in Enhanced analytics</a> </td> 
   <td> <p>The <b>Team capacity</b> visualization shows you a percentage of the amount of work a home team has completed out of the amount of work assigned to them. Interacting with the visualization allows you to see scheduled hours and planned hours for a specific date, as well as the capacity percentage and whether the home team was over, under, or at capacity on that day.</p> </td> 
  </tr>--> 
 </tbody> 
</table>
