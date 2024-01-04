---
content-type: overview
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: Visão geral do Kanban
description: Consulte este artigo para entender melhor como o quadro Kanban funciona.
author: Lisa
feature: Agile
exl-id: d7daa6c1-dae2-4e5c-a765-6a6ebdfaa331
source-git-commit: fa499d74df891441e729c32188e9b2f74e4ef5c0
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Visão geral do Kanban

<!-- Audited: 01/2024 -->

As seções a seguir permitem entender melhor como a [!UICONTROL Kanban] funções da placa.

Para obter uma descrição do K[!UICONTROL Banban] metodologia, consulte [Criar uma equipe ágil](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

Se você estiver interessado em migrar de uma Equipe Ágil [!UICONTROL Kanban] quadro para [!DNL Workfront] [!UICONTROL Quadros], consulte [Migrar equipe ágil [!UICONTROL Kanban] cartões para [!DNL Workfront] quadros](/help/quicksilver/agile/use-boards-agile-planning-tools/migrate-kanban-cards-to-boards.md).

## [!UICONTROL Kanban] layout e funções do quadro

A variável [!UICONTROL Kanban] consiste nos seguintes elementos:

**Coluna de Backlog**: exibe todas as tarefas que estão atualmente no backlog. Essa coluna não é exibida por padrão. Para obter mais informações sobre o backlog, incluindo como exibi-lo no [!UICONTROL Kanban] quadro, consulte [Gerenciar o backlog ágil](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

**Status da história**: indica como uma história está progredindo com base em qual coluna de status a história está.

Para obter mais informações, consulte [Atualizar o status das histórias no [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md).

Os status da história podem ser personalizados para o projeto modificando a exibição ágil, conforme descrito na seção [[!UICONTROL Criar ou personalizar uma visualização Agile]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) in [Criar ou editar exibições no [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

>[!NOTE]
>
>No máximo cinquenta cartões são exibidos no quadro Kanban por padrão, mas você pode clicar em **[!UICONTROL Mostrar mais]** para exibir cartões adicionais.

## Relação entre subtarefas e histórias

Se uma matéria contiver subtarefas, não será possível atualizar nenhuma informação sobre a própria matéria principal (como pontos/horas ou porcentagem concluída). Além disso, não é possível mover a história pelo [!UICONTROL Kanban] para atualizar seu status. Em vez disso, quaisquer alterações feitas nas subtarefas da história são refletidas na história. A combinação de pontos ou horas da matéria para todas as subtarefas determina os pontos ou horas da matéria principal.

Por exemplo, se uma matéria tiver apenas uma subtarefa avaliada em 4 pontos, a própria matéria também terá 4 pontos. Se você alterar o valor do ponto da subtarefa para 3, o valor do ponto da matéria principal será alterado para 3. Se você criar outra subtarefa na mesma matéria e definir o valor do ponto para essa subtarefa como 4, o valor do ponto para a matéria será alterado para 7 a fim de refletir o valor do ponto combinado para ambas as subtarefas.

Essa mesma lógica se aplica às subtarefas de segundo nível (subtarefas de subtarefas). Se uma subtarefa tiver uma ou mais subtarefas de segundo nível, ela será calculada com base nas subtarefas de segundo nível.

## Recursos compatíveis

Você pode executar as seguintes ações ao usar o quadro Kanban:

* [Adicionar uma subtarefa a uma matéria existente no [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/add-a-subtask-to-an-existing-story.md)
* [Adicionar tarefas ou problemas existentes à [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/add-existing-tasks-or-issues-to-the-kanban-board.md)
* [Atribua usuários a uma história no [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/assign-users-to-a-story.md)
* [Adicionar histórias e problemas do [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/add-story-from-kanban-board.md)
* [Excluir histórias ou problemas do [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md)
* [Editar informações da história](../../agile/use-kanban-in-an-agile-team/edit-story-information.md)
* [Filtrar por usuário no [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/filter-by-user.md)
* [Gerencie o limite de trabalho em andamento (WIP) na [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)
* [Reordenar histórias no [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/reorder-stories-on-the-kanban-board.md)
* [Atualizar o status das histórias no [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)
* [Usar sinalizadores em histórias no [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md)
* [Adicione o backlog à [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)
