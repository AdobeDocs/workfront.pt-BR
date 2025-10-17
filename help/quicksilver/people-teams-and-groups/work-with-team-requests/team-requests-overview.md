---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Visão geral das solicitações de equipe
description: As solicitações de equipe são encontradas na área Equipes do menu principal.
author: Jenny
feature: People Teams and Groups
exl-id: c131c021-8bc0-4a48-a873-9ee0e189bcab
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Visão geral de solicitações de equipe

## Entender as solicitações de equipe

As solicitações de equipe são encontradas na área [!UICONTROL Equipes] do [!UICONTROL Menu Principal]. Clique no ícone [!UICONTROL Solicitações de equipe] ![Ícone de solicitação](assets/request-icon.png) no painel esquerdo para exibir as solicitações de equipe.

>[!NOTE]
>
>As equipes Agile não têm solicitações de equipe.

A guia [!UICONTROL Solicitações da equipe] mostra as solicitações aguardando atribuição para a equipe atualmente selecionada na lista suspensa. O número entre parênteses indica quantos itens estão prontos para serem trabalhados.

Uma solicitação de equipe representa um item de trabalho pendente que não está atribuído a um usuário específico. Em vez disso, ele é atribuído a uma equipe, e qualquer membro dessa equipe pode se voluntariar para aceitar a responsabilidade pelo item. Se um usuário se voluntariar para trabalhar em uma solicitação de equipe, ele aceitará a atribuição de trabalho como sua própria atribuição. A tarefa é atribuída ao usuário individual, além da equipe.

>[!NOTE]
>
>Uma solicitação de equipe não deve ser usada para atribuições de tarefas colaborativas. Se precisar atribuir vários usuários para trabalharem juntos em uma tarefa, faça isso através de [!UICONTROL Atribuições avançadas] e não através de solicitações de Equipe. Para obter mais informações, consulte [Criar atribuições avançadas](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

## Compreender as opções [!UICONTROL Pronto para Iniciar] e [!UICONTROL Todas]

Há duas opções na parte superior da seção Solicitações de Equipe: [!UICONTROL Pronto para Iniciar] e [!UICONTROL Todas].

A opção [!UICONTROL Pronto para Iniciar] mostra somente tarefas e problemas que atendem a todos estes critérios:

* Todos os predecessores atenderam às condições para seus tipos de dependência predecessores.\
  Por exemplo, se o tipo de relação da predecessora for [!UICONTROL Finish-Start] (a tarefa predecessora deve terminar antes que a tarefa dependente possa iniciar), a predecessora deve ser marcada como [!UICONTROL Complete]. (Para obter mais informações sobre tipos de dependência predecessora, consulte [Visão geral dos tipos de dependência de tarefa](../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).)

* O usuário conectado é a pessoa atribuída a essas tarefas e problemas (para solicitações de trabalho) ou a equipe selecionada é atribuída a essas tarefas e problemas (para solicitações de equipe).
* O status do projeto é [!UICONTROL Atual].
* A [!UICONTROL Data de Início Projetada] ou a [!UICONTROL Data de Início Planejada] já passou ou está programada para começar dentro de duas semanas a partir da data de hoje (ou nenhuma [!UICONTROL Data de Início Projetada] ou [!UICONTROL Data de Início Planejada] foi definida).
* A [!UICONTROL Data de Transferência] já ocorreu ou ocorrerá dentro de duas semanas a partir da data atual.

>[!NOTE]
>
>Se a tarefa atender aos três primeiros critérios e tiver uma data de Transferência dentro de duas semanas da data atual, ela será exibida como [!UICONTROL Pronta para iniciar] mesmo se as datas Planejada/Projetada estiverem além de duas semanas. Se a tarefa não tiver uma data de Transferência, as datas Planejada/Projetada deverão estar dentro de duas semanas da data atual.

A opção [!UICONTROL Todos] mostra todas as tarefas e problemas em projetos atuais que são atribuídos ao usuário logado ou todas as tarefas ou problemas atribuídos à equipe.
