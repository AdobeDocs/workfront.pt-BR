---
content-type: overview
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: Visão geral do Kanban
description: Revise este artigo para entender melhor como o quadro Kanban funciona.
author: Lisa
feature: Agile
exl-id: d7daa6c1-dae2-4e5c-a765-6a6ebdfaa331
source-git-commit: 2c6a828d95df1229780803a173d5013f5b1eb215
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 0%

---

# Visão geral do Kanban

As seções a seguir permitem compreender melhor como a função [!UICONTROL Kanban] funções da placa.

Se você estiver interessado em migrar de uma equipe ágil [!UICONTROL Kanban] quadro para [!DNL Workfront] [!UICONTROL Quadros], consulte [Migrar equipe ágil [!UICONTROL Kanban] cartões para [!DNL Workfront] quadros](/help/quicksilver/agile/use-boards-agile-planning-tools/migrate-kanban-cards-to-boards.md).

## [!UICONTROL Kanban] layout e funções do quadro

O [!UICONTROL Kanban] O quadro consiste nos seguintes elementos:

**Coluna de Backlog**: Exibe todas as tarefas que estão no backlog. Essa coluna não é exibida por padrão. Para obter mais informações sobre o backlog, incluindo como exibi-lo no [!UICONTROL Kanban] quadro, consulte [Gerenciar o backlog ágil](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

**Status da história**: Indica como uma história está progredindo com base em qual coluna de status a história está.

Para obter mais informações, consulte [Atualize o status de histórias no [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md).

Os status da história podem ser personalizados para o projeto modificando a visualização ágil, conforme descrito na seção [[!UICONTROL Criar ou personalizar uma visualização ágil]](../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) em [Visão geral das exibições em [!DNL Adobe Workfront]](../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

>[!NOTE]
>
>Um máximo de cinquenta cartões é exibido no quadro Kanban por padrão, mas você pode clicar em **[!UICONTROL Mostrar mais]** para exibir cartões adicionais.

## Relação entre subtarefas e histórias

Se uma história contiver subtarefas, você não poderá atualizar nenhuma informação sobre a própria história principal (como pontos/horas ou porcentagem de conclusão). Além disso, você não pode mover a história através do [!UICONTROL Kanban] quadro para atualizar seu status. Em vez disso, quaisquer mudanças que você faça nas subtarefas da história são refletidas na história. A história combinada de pontos ou horas para todas as subtarefas determina os pontos ou horas da história principal.

Por exemplo, se uma história tem apenas uma subtarefa avaliada em 4 pontos, a própria história também tem 4 pontos. Se você alterar o valor do ponto de subtarefa para 3, o valor do ponto da história pai será alterado para 3. Se você criar outra subtarefa na mesma história e definir o valor de ponto para essa subtarefa como 4, o valor de ponto da história será alterado para 7 para refletir o valor de ponto combinado para ambas as subtarefas.

Essa mesma lógica se aplica às subtarefas de segundo nível (subtarefas de subtarefas). Se uma subtarefa tiver uma ou mais subtarefas de segundo nível, a subtarefa será calculada com base nas subtarefas de segundo nível.

## Recursos compatíveis

Você pode realizar as seguintes ações ao usar o quadro Kanban:

* [Adicionar uma subtarefa a uma história existente no [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/add-a-subtask-to-an-existing-story.md)
* [Adicionar tarefas ou problemas existentes à [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/add-existing-tasks-or-issues-to-the-kanban-board.md)
* [Atribua usuários a uma história na [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/assign-users-to-a-story.md)
* [Adicionar histórias e problemas do [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/add-story-from-kanban-board.md)
* [Excluir histórias ou problemas do [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md)
* [Editar informações da história](../../agile/use-kanban-in-an-agile-team/edit-story-information.md)
* [Filtrar por usuário no [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/filter-by-user.md)
* [Gerenciar o limite de trabalho em andamento (WIP) no [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)
* [Reordenar histórias no [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/reorder-stories-on-the-kanban-board.md)
* [Atualize o status de histórias no [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)
* [Use sinalizadores em histórias no [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md)
* [Adicione o backlog ao [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)
