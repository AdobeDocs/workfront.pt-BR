---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Visão geral das solicitações de equipe
description: As solicitações da equipe são encontradas na área Equipes no Menu principal.
author: Lisa
feature: People Teams and Groups
exl-id: c131c021-8bc0-4a48-a873-9ee0e189bcab
source-git-commit: 9693ac3792fec3eca6218a228f2067519ed433ac
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Visão geral das solicitações de equipe

## Entender as solicitações da equipe

As solicitações da equipe são encontradas na seção [!UICONTROL Equipes] na [!UICONTROL Menu principal]. Clique no botão [!UICONTROL Solicitações de equipe] ícone ![Ícone Solicitar](assets/request-icon.png) no painel esquerdo para exibir as solicitações do grupo.

>[!NOTE]
>
>As equipes ágil não têm solicitações de equipe.

O [!UICONTROL Solicitações de equipe] mostra as solicitações que aguardam atribuição para a equipe atualmente selecionada na lista suspensa. O número entre parênteses indica quantos itens estão prontos para serem trabalhados.

Uma solicitação de equipe representa um item de trabalho pendente que não é atribuído a um usuário específico. Em vez disso, é atribuído a uma equipe, e qualquer membro dessa equipe pode se voluntariar para aceitar a responsabilidade pelo item. Se um usuário se voluntariar para trabalhar em uma solicitação de equipe, o usuário está aceitando a atribuição de trabalho como sua própria. A tarefa é atribuída ao usuário individual, além da equipe.

>[!NOTE]
>
>Uma solicitação de equipe não deve ser usada para atribuições de tarefa colaborativa. Se precisar atribuir vários usuários para trabalhar em conjunto em uma tarefa, faça isso [!UICONTROL Atribuições avançadas] e não por meio de solicitações da equipe. Para obter mais informações, consulte [Criar atribuições avançadas](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

## Entenda o [!UICONTROL Pronto para começar] e [!UICONTROL Todos] opções

Há duas opções na parte superior da seção Solicitações de equipe: [!UICONTROL Pronto para começar] e [!UICONTROL Todos].

O [!UICONTROL Pronto para começar] mostra somente tarefas e problemas que atendem a todos os seguintes critérios:

* Todos os antecessores cumpriram as condições para os tipos de dependência dos antecessores.\
   Por exemplo, se o tipo de relacionamento do antecessor for [!UICONTROL Finish-Start] (a tarefa do antecessor deve ser concluída antes que a tarefa dependente possa iniciar), o antecessor deve ser marcado como [!UICONTROL Concluído]. (Para obter mais informações sobre tipos de dependência de antecessor, consulte [Visão geral dos tipos de dependência de tarefa](../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).)

* O usuário conectado é a pessoa atribuída a essas tarefas e problemas (para solicitações de trabalho) ou a equipe selecionada é atribuída a essas tarefas e problemas (para solicitações de equipe).
* O status do projeto está em um status de [!UICONTROL Atual].
* O [!UICONTROL Data Inicial Projetada] ou [!UICONTROL Data de início planejada] tenha passado ou esteja programado para começar dentro de duas semanas a partir da data de hoje (ou não [!UICONTROL Data Inicial Projetada] ou [!UICONTROL Data de início planejada] foi definida).
* O [!UICONTROL Data de transferência] já ocorreu ou ocorrerá dentro de duas semanas a partir da data atual.

>[!NOTE]
>
>Se a tarefa atender aos três primeiros critérios e tiver uma data de hansensibilidade dentro de duas semanas da data atual, ela será exibida como [!UICONTROL Pronto para começar] mesmo que as datas Planejadas/Projetadas estejam além de duas semanas. Se a tarefa não tiver uma data de transferência, as datas Planejadas/Projetadas devem estar dentro de duas semanas da data atual.

O [!UICONTROL Todos] mostra todas as tarefas e problemas em projetos atuais que são atribuídos ao usuário conectado ou a todas as tarefas ou problemas atribuídos à equipe.
