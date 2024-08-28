---
content-type: overview
product-area: agile-and-teams
navigation-topic: scrum-board
title: Visão geral do quadro Scrum
description: O storyboard Scrum ágil é exibido junto com o status de conclusão e o gráfico de burndown.
author: Lisa
feature: Agile
exl-id: 584288bb-2d98-4b69-8deb-d3b8e54d328c
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---

# Visão geral do quadro [!UICONTROL Scrum]

O storyboard ágil [!UICONTROL Scrum] é exibido junto com o status de conclusão e o gráfico de burndown. Estes componentes ágeis estão disponíveis nas seguintes situações no [!UICONTROL Adobe Workfront]:

* Em iterações ágeis. Para obter mais detalhes sobre como usar o storyboard Agile, o gráfico de burndown e o status de conclusão em um ambiente exclusivamente ágil (com listas de pendências e uma iteração), consulte [Trabalhar em um ambiente Agile](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).
* Ao visualizar um projeto em uma visualização ágil. Para obter informações sobre como aproveitar o storyboard Agile, o gráfico de burndown e o status de conclusão em um projeto existente, consulte [Gerenciar um projeto na Exibição Agile](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

![Iteração Agile](assets/agile-iteration-with-callouts.png)

## Layout e funções do Storyboard

![Storyboard Agile](assets/agile-storyboard-callouts.png)

O storyboard consiste nos seguintes elementos:

* **[!UICONTROL História Pai] Coluna:** Ao contrário das outras colunas no storyboard, a coluna [!UICONTROL História Pai] não é um status de tarefa, mas existe para hospedar qualquer história que contenha subtarefas na iteração ou no projeto. Somente matérias principais que tenham pelo menos uma subtarefa no storyboard podem residir nessa coluna. As histórias principais em si não se movem de status para status no storyboard.

  Em uma iteração, essa coluna aparece no storyboard somente quando uma ou mais matérias no storyboard contêm pelo menos uma subtarefa que atende aos seguintes requisitos:

   * Atribuída à mesma equipe ágil que a tarefa pai
   * Pertence à iteração

     Em um projeto, essa coluna aparece sempre que uma tarefa tem pelo menos uma subtarefa.

     ![Coluna de história principal](assets/agile-parentstory-swimlane.png)

* **Status de Tarefa:** Indica como uma história está progredindo pela iteração ou projeto com base em qual coluna de status a história está.

  Os status das tarefas podem ser personalizados para o projeto modificando a exibição Agile, conforme descrito em [Criar ou personalizar uma exibição Agile](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) na [Visão geral das exibições no [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

* **Swim Lane:** quando uma história principal e suas subtarefas aparecem no storyboard, uma pista de natação é criada especificamente para a história e suas subtarefas. Isso fornece uma distinção visual para ver melhor como as subtarefas de uma história estão progredindo no storyboard.

  Em uma iteração, as faixas de natação aparecem no storyboard somente quando uma história no storyboard contém pelo menos uma subtarefa que atende aos seguintes requisitos:

   * Atribuída à mesma equipe ágil que a tarefa pai
   * Pertence à iteração

  Em um projeto, as faixas de natação aparecem sempre que uma tarefa tem pelo menos uma subtarefa ou uma tarefa pai.

* **Histórias Individuais:** Histórias e problemas individuais são exibidos abaixo de qualquer pista de natação no storyboard. Isso fornece uma distinção visual das histórias que fazem parte de uma pista de natação.

## Relação entre Subtarefas e Histórias

Se uma matéria contiver subtarefas, não será possível atualizar nenhuma informação sobre a própria matéria principal (como pontos/horas ou porcentagem concluída). Além disso, não é possível mover a matéria pelo storyboard para atualizar o status. Em vez disso, quaisquer alterações feitas nas subtarefas da história são refletidas na história. A combinação de pontos ou horas da matéria para todas as subtarefas determina os pontos ou horas da matéria principal.

Por exemplo, se uma matéria tiver apenas uma subtarefa avaliada em 4 pontos, a própria matéria também terá 4 pontos. Se você alterar o valor do ponto da subtarefa para 3, o valor do ponto da matéria principal será alterado para 3. Se você criar outra subtarefa na mesma matéria e definir o valor do ponto para essa subtarefa como 4, o valor do ponto para a matéria será alterado para 7 a fim de refletir o valor do ponto combinado para ambas as subtarefas.

Essa mesma lógica se aplica às subtarefas de segundo nível (subtarefas de subtarefas). Se uma subtarefa tiver uma ou mais subtarefas de segundo nível, ela será calculada com base nas subtarefas de segundo nível.

## Relação entre o Storyboard e o Backlog

>[!NOTE]
>
>As informações nesta seção se aplicam apenas às exibições ágeis em uma iteração; as exibições ágeis em um projeto não usam um backlog. (Para obter mais informações sobre as diferenças entre as exibições Agile em uma iteração e um projeto, consulte &quot;Diferenças ao Usar a Exibição [!UICONTROL Agile] em um Projeto versus em uma Iteração&quot; em [Gerenciar um projeto na Exibição Agile](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).)

O backlog de iteração mostra apenas histórias ou subtarefas em que é possível definir uma estimativa. Se uma matéria pai tiver subtarefas que são exibidas no storyboard (porque elas são atribuídas à mesma equipe ágil e pertencem à iteração), a tarefa pai não será exibida no backlog. Nessa situação, somente as subtarefas são exibidas no backlog, enquanto as subtarefas e a matéria pai são exibidas no storyboard.

Por exemplo, suponha que a História A contenha Subtarefa 1 e Subtarefa 2 (e ambas as subtarefas sejam atribuídas à mesma equipe ágil). Nessa situação, a História A é exibida no storyboard em uma pista de natação com Subtarefa 1 e Subtarefa 2. No entanto, somente a Subtarefa 1 e a Subtarefa 2 são exibidas no backlog.

Essa mesma lógica se aplica às subtarefas de segundo nível (subtarefas de subtarefas). Se uma subtarefa tiver uma ou mais subtarefas de segundo nível atribuídas à mesma equipe ágil e pertencer à iteração, somente a subtarefa de segundo nível será exibida no backlog.

Para obter mais informações sobre a lista de pendências, consulte [Gerenciar a lista de pendências ágil](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).
