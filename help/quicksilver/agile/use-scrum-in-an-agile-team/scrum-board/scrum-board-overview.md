---
content-type: overview
product-area: agile-and-teams
navigation-topic: scrum-board
title: Visão geral da placa de som
description: O quadro de história ágil do Escrum é exibido junto com o status de conclusão e o gráfico de detalhamento.
author: Lisa
feature: Agile
exl-id: 584288bb-2d98-4b69-8deb-d3b8e54d328c
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '867'
ht-degree: 0%

---

# [!UICONTROL Scrum] visão geral da placa

O [!UICONTROL Scrum] o quadro de história ágil é exibido junto com o status de conclusão e o gráfico de detalhamento. Esses componentes ágeis estão disponíveis nas seguintes situações em [!UICONTROL Adobe Workfront]:

* Em iterações ágeis. Para obter mais detalhes sobre o uso do quadro de história ágil, do gráfico de detalhamento e do status de conclusão em um ambiente ágil puro (com registros retroativos e uma iteração), consulte [Trabalhar em um ambiente ágil](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).
* Ao visualizar um projeto em uma visualização ágil. Para obter informações sobre como você pode aproveitar o quadro de história ágil, o gráfico de detalhamento e o status de conclusão em um projeto existente, consulte [Gerenciar um projeto na Visualização ágil](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

![iteração ágil](assets/agile-iteration-with-callouts.png)

## Layout e funções do quadro de história

![Quadro de história ágil](assets/agile-storyboard-callouts.png)

O quadro de história consiste nos seguintes elementos:

* **[!UICONTROL História principal] Coluna:** Ao contrário das outras colunas no quadro de matérias, a variável  [!UICONTROL História principal]  não é um status de tarefa, mas existe para armazenar qualquer história que contenha subtarefas na iteração ou no projeto. Somente as histórias pai que têm pelo menos uma subtarefa no quadro de matérias podem residir nesta coluna. As próprias histórias-pai não mudam de status para status no quadro de histórias.

   Em uma iteração, essa coluna aparece no quadro de matérias somente quando uma ou mais histórias no quadro de matérias contêm pelo menos uma subtarefa que atende aos seguintes requisitos:

   * Atribuído à mesma equipe ágil que a tarefa pai
   * Pertence à iteração

      Em um projeto, essa coluna aparece sempre que uma tarefa tem pelo menos uma subtarefa.

      ![Coluna da história principal](assets/agile-parentstory-swimlane.png)

* **Status da tarefa:** Indique como uma história está progredindo pela iteração ou projeto com base em qual coluna de status a história está.

   Os status da tarefa podem ser personalizados para o projeto modificando a exibição ágil, conforme descrito em [Criar ou personalizar uma visualização ágil](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) em [Visão geral das exibições em [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

* **Swim Lane:** Quando uma história principal e suas subtarefas aparecem no quadro de histórias, uma faixa de natação é criada especificamente para a história e suas subtarefas. Isso fornece uma distinção visual para visualizar melhor como as subtarefas de uma história estão progredindo no quadro de história.

   Em uma iteração, as faixas de natação aparecem no quadro de histórias somente quando uma história no quadro de histórias contém pelo menos uma subtarefa que atende aos seguintes requisitos:

   * Atribuído à mesma equipe ágil que a tarefa pai
   * Pertence à iteração

   Em um projeto, as faixas de natação são exibidas sempre que uma tarefa tiver pelo menos uma subtarefa ou uma tarefa pai.

* **Histórias individuais:** Histórias e problemas individuais são exibidos abaixo de qualquer faixa de natação no quadro de histórias. Isto proporciona uma distinção visual das histórias que fazem parte de uma faixa de natação.

## Relação entre subtarefas e histórias

Se uma história contiver subtarefas, você não poderá atualizar nenhuma informação sobre a própria história principal (como pontos/horas ou porcentagem de conclusão). Além disso, você não pode mover a história através do quadro para atualizar seu status. Em vez disso, quaisquer mudanças que você faça nas subtarefas da história são refletidas na história. A história combinada de pontos ou horas para todas as subtarefas determina os pontos ou horas da história principal.

Por exemplo, se uma história tem apenas uma subtarefa avaliada em 4 pontos, a própria história também tem 4 pontos. Se você alterar o valor do ponto de subtarefa para 3, o valor do ponto da história pai será alterado para 3. Se você criar outra subtarefa na mesma história e definir o valor de ponto para essa subtarefa como 4, o valor de ponto da história será alterado para 7 para refletir o valor de ponto combinado para ambas as subtarefas.

Essa mesma lógica se aplica às subtarefas de segundo nível (subtarefas de subtarefas). Se uma subtarefa tiver uma ou mais subtarefas de segundo nível, a subtarefa será calculada com base nas subtarefas de segundo nível.

## Relação entre o Quadro de História e o Backlog

>[!NOTE]
>
>As informações desta seção aplicam-se apenas a visualizações ágeis em uma iteração; exibições ágeis em um projeto não usam um backlog. (Para obter mais informações sobre as diferenças entre exibições ágeis em uma iteração e um projeto, consulte &quot;Diferenças ao usar a variável [!UICONTROL Ágil] Exibir em um projeto versões de uma iteração&quot; em [Gerenciar um projeto na Visualização ágil](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).)

O backlog de iteração mostra somente histórias ou subtarefas, onde você pode definir uma estimativa. Se uma história pai tiver subtarefas exibidas no quadro de matérias (porque elas são atribuídas à mesma equipe ágil e pertencem à iteração), a tarefa pai não será exibida no backlog. Nessa situação, somente as subtarefas são exibidas no backlog, enquanto as subtarefas e a história pai são exibidas no quadro de matérias.

Por exemplo, suponha que a História A contenha Subtarefa 1 e Subtarefa 2 (e ambas as subtarefas são atribuídas à mesma equipe ágil). Nessa situação, a História A é exibida no quadro de histórias em uma faixa de natação com Subtarefa 1 e Subtarefa 2. No entanto, somente Subtarefa 1 e Subtarefa 2 são exibidas no backlog.

Essa mesma lógica se aplica às subtarefas de segundo nível (subtarefas de subtarefas). Se uma subtarefa tiver uma ou mais subtarefas de segundo nível atribuídas à mesma equipe ágil e pertencerem à iteração, somente a subtarefa de segundo nível será exibida no backlog.

Para obter mais informações sobre o backlog, consulte [Gerenciar o backlog ágil](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).
