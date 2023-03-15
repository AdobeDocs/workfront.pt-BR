---
title: Visão geral da análise aprimorada
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: A análise aprimorada é uma ferramenta poderosa no Adobe Workfront com visualizações pré-criadas que permite analisar os dados do projeto e identificar tendências com o planejamento e a conclusão. Este insight nos projetos ajuda você a gerenciar seu trabalho atual e permite planejar com mais precisão o trabalho futuro.
author: Nolan
feature: Reports and Dashboards
exl-id: a14ad57c-859b-43df-84c0-575ccda86e50
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '1351'
ht-degree: 1%

---

# Visão geral da análise aprimorada

A análise aprimorada é uma ferramenta poderosa no Adobe Workfront com visualizações pré-criadas que permite analisar os dados do projeto e identificar tendências com o planejamento e a conclusão. Este insight nos projetos ajuda você a gerenciar seu trabalho atual e permite planejar com mais precisão o trabalho futuro.

As análises aprimoradas podem ajudar a identificar:

* A maneira como você planeja projetos
* Quando o trabalho é adicionado aos projetos
* O volume de trabalho a realizar para diferentes projetos
* A quantidade de horas ou dias necessários para concluir um projeto em comparação às horas ou dias em que uma equipe inicial está agendada
* Com que frequência os usuários concluem ações específicas durante um projeto
* O progresso dos projetos, bem como as tarefas individuais no âmbito de um projeto

![](assets/nwe-full-screen-analytics-350x222.png)

Para ver casos de uso ou saber mais sobre o gerenciamento do trabalho atual e o planejamento para o trabalho futuro com o Enhanced Analytics, consulte [Caminhos de aprendizado aprimorados do analytics](https://one.workfront.com/s/enhanced-analytics-program).

## Pré-requisitos

Para acessar a área Análise aprimorada, você deve:

* Ter um plano de negócios ou de empresa.

   Para obter mais informações, consulte [Planos do Workfront](https://www.workfront.com/plans).

* Peça ao administrador do Workfront para adicionar Análise aprimorada ao modelo de layout.

   Para obter mais informações, consulte [Análise aprimorada: Adição de análises a modelos de layout](https://one.workfront.com/s/managed-content-videos/enhanced-analytics-adding-analytics-to-layout-templates-MCH7URDSIXRREHHHF7TRTYYP2LTE).

Para ver informações sobre projetos e tarefas, você deve:

* Ter permissão de Exibição para as áreas Projetos e Tarefas em seu nível de acesso.

   Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte [Criar ou modificar níveis de acesso personalizados](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Ter permissão de Exibição para tarefas e/ou projetos específicos.

   Para obter informações sobre como solicitar acesso adicional, consulte [Solicitar acesso a objetos](../workfront-basics/grant-and-request-access-to-objects/request-access.md).

## Práticas recomendadas para análises aprimoradas

Para obter os melhores dados para seus projetos, use modelos que tenham horas e dias de duração planejados precisos. Você também precisa garantir que seus usuários insiram e atualizem os campos abaixo da maneira mais precisa possível.

>[!NOTE]
>
>Alguns dos seguintes campos são cálculos executados pelo Workfront com base nas informações inseridas pelos usuários. Não é possível atualizar esses campos manualmente.

* Horas planejadas

   Este é o campo mais importante a ser preenchido.

   >[!NOTE]
   >
   >Se as equipes não usarem as horas planejadas, você ainda poderá ver alguns dados com base na duração do projeto.\
   >Para obter mais informações, consulte a seção [Visualização de duração](#duration-view) neste artigo.

* Nome do Projeto

   O nome deve ser descritivo do projeto.

* Condição do projeto
* Status do projeto
* Data Inicial Planejada do Projeto
* Data de conclusão planejada
* Data de Início Real do Projeto
* Data Final Real do Projeto
* Horas de Duração do Projeto
* Horas Reais do Projeto
* Status da tarefa (inclui a marcação de tarefas concluídas.)
* Nome da tarefa
* Porcentagem de Tarefa Concluída
* Data de Início Planejada da Tarefa
* Data de Término Planejada da Tarefa

>[!IMPORTANT]
>
>Pode levar até 24 horas para que as alterações feitas em tarefas e projetos sejam refletidas na Análise aprimorada.

## Visualização de duração {#duration-view}

Por padrão, as visualizações do Burndown e do Mapa de árvore do projeto se baseiam em horas planejadas. Se as equipes não usarem as horas planejadas, você poderá ver essas visualizações com base na duração do projeto.

Na Análise aprimorada, a duração de um projeto é calculada pelas seguintes fórmulas:

* Período planejado:

   ```
   Planned Completion Date of the project - Start Date of the project
   ```

* Dias trabalhados:

   ```
   Planned Duration for tasks completed in the selected date range / Typical hours per work day
   ```

   >[!NOTE]
   >
   >8 horas é o número padrão para **Horas típicas por dia de trabalho**. Um administrador do Adobe Workfront pode atualizar a variável **Horas típicas por dia de trabalho** definição em **Configuração** > **Preferências do projeto** > **Projetos** > **Linhas do tempo**.\
   >Para saber mais, consulte [Configurar preferências de projeto em todo o sistema](../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Para obter informações sobre a Duração planejada, consulte [Visão geral da duração do projeto](../manage-work/projects/planning-a-project/project-duration.md).

## Atalhos de teclado

Você pode usar as seguintes teclas no teclado para navegar ou concluir ações específicas na área de Análise aprimorada:

| Chave | Ação |
|---|---|
| **Guia** | Navegue até cada elemento na página, bem como para uma tabela com informações sobre cada visualização que não é exibida na página |
| **Enter** | Abra o widget de calendário, exclua um filtro existente, abra as opções de adicionar filtro, selecione/desmarque valores de filtro, aplique um filtro que você criou, abra as opções de exportação em cada visualização, abra os menus suspensos nas visualizações de Burndown, Tarefas em andamento e Mapa de árvore do projeto |
| **Teclas de seta** | Navegue até datas no widget de calendário, por meio de opções de filtro ao adicionar um filtro e por meio de opções em todos os menus suspensos nas visualizações |
| **Barra de espaço** | Selecione datas no widget calendário, selecione um tipo de filtro ao adicionar um filtro, selecione uma opção de exportação no menu suspenso de cada visualização e selecione opções nos menus suspensos nas visualizações de Burndown, Tarefas em andamento e Mapa de árvore do projeto |

{style="table-layout:auto"}

Se você estiver usando um software de leitura de tela ou um plug-in, o leitor de tela lê as informações na tela e descreve as ações que você está concluindo à medida que usa as teclas listadas acima.

## Visualizações e recursos aprimorados do Analytics

Para saber mais sobre os detalhes de um recurso específico no Enhanced Analytics, as ações que você pode concluir para obter mais informações e o que você pode aprender com esses dados, consulte os seguintes artigos:

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
   <td><a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">Aplicar filtros no Enhanced Analytics</a> </td> 
   <td> <p>Você pode aplicar filtros personalizados, filtros de campo de projeto ou filtros de equipe para exibir somente projetos que se encaixem em critérios específicos. À medida que você adiciona filtros, o número de projetos é atualizado adequadamente.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/understand-enhanced-analytics-kpis.md" class="MCXref xref">Entender os KPIs aprimorados do Analytics</a> </td> 
   <td> <p>Os indicadores-chave de desempenho (KPIs) para todos os projetos em um período específico estão localizados na parte superior da tela.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../enhanced-analytics/flight-plan-overview.md" class="MCXref xref">Exibir a visualização do Plano de voo na análise aprimorada</a> </p> </td> 
   <td> <p>O <b>Plano de voo</b> A visualização mostra que a condição foi alterada durante a vida de um projeto. Interagir com a visualização fornece mais detalhes sobre datas específicas. Selecionar um projeto abre as visualizações Burndown e Tasks in flight .</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/burndown-overview.md" class="MCXref xref">Visualizar a visualização do Detalhamento na análise aprimorada</a> </td> 
   <td> <p>O <b>Interrupção</b> A visualização mostra a velocidade planejada de um projeto em comparação à quantidade real de horas gastas em um projeto. Interagir com a visualização fornece mais detalhes sobre a condição do projeto em uma data específica.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/tasks-in-flight-overview.md" class="MCXref xref">Visualizar as Tarefas em andamento na análise aprimorada</a> </td> 
   <td> <p>O <b>Tarefas em voo</b> A visualização mostra o status de cada tarefa em um projeto. Interagir com a visualização permite fazer alterações rápidas e facilmente em uma tarefa.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-activity-overview.md" class="MCXref xref">Exibir a visualização da atividade do projeto no Enhanced Analytics</a> </td> 
   <td> <p>O <b>Atividade do projeto</b> A visualização mostra um mapa de calor de quando usuários atribuídos a um projeto conectados ao Workfront, alteraram o status da tarefa nesse projeto e concluíram as tarefas nesse projeto. Interagir com a visualização permite visualizar esses detalhes para cada usuário. Você também pode ver datas específicas para essas ações, bem como o número de vezes que cada ação foi concluída.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-treemap-overview.md" class="MCXref xref">Visualizar o mapa de árvore do projeto no Enhanced Analytics</a> </td> 
   <td> <p>O <b>Mapa de árvore do projeto</b> A visualização mostra quanto tempo foi gasto em alguns projetos em comparação a outros. Interagir com a visualização fornece detalhes sobre a condição do projeto, a conclusão planejada do projeto e a conclusão real do projeto.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/activity-by-team-overview.md" class="MCXref xref">Visualizar a Atividade por equipe na Análise aprimorada</a> </td> 
   <td> <p>O <b>Atividade por equipe</b> A visualização mostra um mapa de calor de quando os usuários em uma equipe inicial se conectaram ao Workfront, alteraram o status de uma tarefa e concluíram uma tarefa. Interagir com a visualização permite visualizar esses detalhes para cada usuário individual. Você também pode ver datas específicas para essas ações, bem como o número de vezes que cada ação foi concluída.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/resource-capacity-overview.md" class="MCXref xref">Visualizar a Visualização da capacidade dos recursos no Enhanced Analytics</a> </td> 
   <td> <p>O <b>Capacidade do recurso</b> A visualização mostra quais equipes domésticas têm a capacidade de trabalhar mais e quais equipes domésticas têm mais trabalho atribuído a elas do que podem concluir. Interagir com a visualização permite ver mais detalhes sobre o trabalho concluído e o horário disponível para mais trabalho. Selecionar uma equipe abre a visualização de capacidade do grupo.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/team-capacity-overview.md" class="MCXref xref">Visualização da capacidade do grupo na Análise aprimorada</a> </td> 
   <td> <p>O <b>Capacidade da equipe</b> A visualização mostra uma porcentagem da quantidade de trabalho que uma equipe inicial concluiu da quantidade de trabalho atribuído a ela. Interagir com a visualização permite ver as horas agendadas e as horas planejadas para uma data específica, bem como a porcentagem da capacidade e se a equipe residencial estava com excesso, abaixo ou na capacidade nesse dia.</p> </td> 
  </tr> 
 </tbody> 
</table>
