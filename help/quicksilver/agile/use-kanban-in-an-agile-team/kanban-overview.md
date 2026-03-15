---
content-type: overview
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: Visão Geral de Kanban
description: Revise este artigo para entender melhor como o quadro Kanban funciona.
author: Courtney
feature: Agile
exl-id: d7daa6c1-dae2-4e5c-a765-6a6ebdfaa331
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 1%

---

# Visão geral do Kanban

<!-- Audited: 01/2024 -->

As seções a seguir permitem compreender melhor como o quadro do [!UICONTROL Kanban] funciona.

Para uma descrição da metodologia K[!UICONTROL anban], consulte [Criar uma equipe ágil](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

Se você estiver interessado em migrar de um painel da equipe do Agile [!UICONTROL Kanban] para [!DNL Workfront] [!UICONTROL painéis], consulte [Migrar cartões do Agile team [!UICONTROL Kanban] para  [!DNL Workfront] painéis](/help/quicksilver/agile/use-boards-agile-planning-tools/migrate-kanban-cards-to-boards.md).

## Layout e funções do quadro do [!UICONTROL kanban]

O quadro do [!UICONTROL Kanban] consiste nos seguintes elementos:

**Coluna de Lista de Pendências**: exibe todas as tarefas que estão atualmente na lista de pendências. Esta coluna não é exibida por padrão. Para obter mais informações sobre a lista de pendências, incluindo como exibi-la no quadro [!UICONTROL Kanban], consulte [Gerenciar a lista de pendências ágil](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

**Status da matéria**: indica como uma matéria está progredindo com base em qual coluna de status a matéria está.

Para obter mais informações, consulte [Atualizar o status das histórias no quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md).

Os status de matéria podem ser personalizados para o projeto modificando a exibição Ágil, conforme descrito na seção [[!UICONTROL Criar ou personalizar uma exibição Ágil]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) em [Criar ou editar exibições em [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

>[!NOTE]
>
>Um máximo de cinquenta cartões é exibido no quadro Kanban por padrão, mas você pode clicar em **[!UICONTROL Mostrar Mais]** para exibir cartões adicionais.

## Relacionamento entre subtarefas e matérias

Se uma matéria contiver subtarefas, você não poderá atualizar nenhuma informação na própria matéria-pai (como pontos/horas ou porcentagem concluída). Além disso, não é possível mover a história no quadro [!UICONTROL Kanban] para atualizar seu status. Em vez disso, todas as alterações feitas nas subtarefas da matéria são refletidas na matéria. Os pontos ou horas combinados da matéria para todas as subtarefas determinam os pontos ou horas da matéria-pai.

Por exemplo, se uma matéria tem apenas uma subtarefa avaliada em 4 pontos, a própria matéria também tem 4 pontos. Se você alterar o valor do ponto da subtarefa para 3, o valor do ponto da matéria-pai será alterado para 3. Se você criar outra subtarefa na mesma matéria e definir o valor de ponto dessa subtarefa como 4, o valor de ponto da matéria será alterado para 7 para refletir o valor de ponto combinado de ambas as subtarefas.

Essa mesma lógica se aplica a subtarefas de segundo nível (subtarefas de subtarefas). Se uma subtarefa tiver uma ou mais subtarefas de segundo nível, ela será calculada com base nas subtarefas de segundo nível.

## Recursos compatíveis

Você pode fazer as seguintes ações ao usar o quadro Kanban:

* [Adicionar uma subtarefa a uma história existente no quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/add-a-subtask-to-an-existing-story.md)
* [Adicionar tarefas ou problemas existentes ao quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/add-existing-tasks-or-issues-to-the-kanban-board.md)
* [Atribuir usuários a uma história no quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/assign-users-to-a-story.md)
* [Adicionar histórias e questões do quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/add-story-from-kanban-board.md)
* [Excluir histórias ou problemas do quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md)
* [Editar informações do story](../../agile/use-kanban-in-an-agile-team/edit-story-information.md)
* [Filtrar por usuário no quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/filter-by-user.md)
* [Gerenciar o limite de trabalho em andamento (WIP) no quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)
* [Reordenar histórias no quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/reorder-stories-on-the-kanban-board.md)
* [Atualizar o status das histórias no quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)
* [Usar sinalizadores em histórias no quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md)
* [Adicionar a lista de pendências ao quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)
