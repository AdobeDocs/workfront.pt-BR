---
content-type: overview
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: Visão geral do Kanban
description: Consulte este artigo para entender melhor como o quadro Kanban funciona.
author: Jenny
feature: Agile
exl-id: d7daa6c1-dae2-4e5c-a765-6a6ebdfaa331
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Visão geral do Kanban

<!-- Audited: 01/2024 -->

As seções a seguir permitem entender melhor como o quadro [!UICONTROL Kanban] funciona.

Para obter uma descrição da metodologia K[!UICONTROL anban], consulte [Criar uma equipe Agile](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

Se você estiver interessado em migrar de um quadro da Equipe Agile [!UICONTROL Kanban] para [!DNL Workfront] [!UICONTROL Quadros], consulte [Migrar cartões da Equipe Agile [!UICONTROL Kanban] para [!DNL Workfront] quadros](/help/quicksilver/agile/use-boards-agile-planning-tools/migrate-kanban-cards-to-boards.md).

## Layout e funções do quadro [!UICONTROL Kanban]

O quadro [!UICONTROL Kanban] consiste nos seguintes elementos:

**Coluna de lista de pendências**: exibe todas as tarefas que estão atualmente na lista de pendências. Essa coluna não é exibida por padrão. Para obter mais informações sobre a lista de pendências, incluindo como exibi-la no quadro [!UICONTROL Kanban], consulte [Gerenciar a lista de pendências Agile](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

**Status da história**: indica como uma história está progredindo com base em qual coluna de status a história está.

Para obter mais informações, consulte [Atualizar o status das histórias no quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md).

Os status da história podem ser personalizados para o projeto modificando a exibição ágil, conforme descrito na seção [[!UICONTROL Criar ou personalizar uma exibição Ágil]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) em [Criar ou editar exibições em [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

>[!NOTE]
>
>No máximo cinquenta cartões são exibidos no quadro Kanban por padrão, mas você pode clicar em **[!UICONTROL Mostrar mais]** para exibir cartões adicionais.

## Relação entre subtarefas e histórias

Se uma matéria contiver subtarefas, não será possível atualizar nenhuma informação sobre a própria matéria principal (como pontos/horas ou porcentagem concluída). Além disso, não é possível mover a história no quadro [!UICONTROL Kanban] para atualizar seu status. Em vez disso, quaisquer alterações feitas nas subtarefas da história são refletidas na história. A combinação de pontos ou horas da matéria para todas as subtarefas determina os pontos ou horas da matéria principal.

Por exemplo, se uma matéria tiver apenas uma subtarefa avaliada em 4 pontos, a própria matéria também terá 4 pontos. Se você alterar o valor do ponto da subtarefa para 3, o valor do ponto da matéria principal será alterado para 3. Se você criar outra subtarefa na mesma matéria e definir o valor do ponto para essa subtarefa como 4, o valor do ponto para a matéria será alterado para 7 a fim de refletir o valor do ponto combinado para ambas as subtarefas.

Essa mesma lógica se aplica às subtarefas de segundo nível (subtarefas de subtarefas). Se uma subtarefa tiver uma ou mais subtarefas de segundo nível, ela será calculada com base nas subtarefas de segundo nível.

## Recursos compatíveis

Você pode executar as seguintes ações ao usar o quadro Kanban:

* [Adicionar uma subtarefa a uma história existente no quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/add-a-subtask-to-an-existing-story.md)
* [Adicionar tarefas ou problemas existentes ao quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/add-existing-tasks-or-issues-to-the-kanban-board.md)
* [Atribuir usuários a uma história no quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/assign-users-to-a-story.md)
* [Adicione histórias e problemas do quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/add-story-from-kanban-board.md)
* [Exclua histórias ou problemas do quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md)
* [Editar informações da história](../../agile/use-kanban-in-an-agile-team/edit-story-information.md)
* [Filtrar por usuário no quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/filter-by-user.md)
* [Gerencie o limite do trabalho em andamento (WIP) no quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)
* [Reordenar histórias no quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/reorder-stories-on-the-kanban-board.md)
* [Atualize o status das histórias no quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)
* [Usar sinalizadores em histórias no quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md)
* [Adicionar o backlog ao quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)
