---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Gerenciar Solicitações de Trabalho e Equipe
description: Uma solicitação representa uma atribuição de tarefa ou ocorrência pendente. As solicitações de trabalho são feitas a indivíduos e as solicitações de equipe são feitas a equipes.
author: Courtney
feature: People Teams and Groups, Work Management
exl-id: ef96e520-0d5f-4180-a27a-1fbbffff8f2b
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 9%

---

# Gerenciar solicitações de trabalho e da equipe

Uma solicitação representa uma atribuição pendente de tarefa ou problema. As solicitações de trabalho são feitas a indivíduos e as solicitações de equipe são feitas a equipes.

>[!NOTE]
>
>Equipes ágeis não têm solicitações de equipe.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
   <p>Para atribuir ou trabalhar em uma solicitação:
   <p>Claro ou superior</p>
  <p>Revisar ou superior</p>
   <p>Para reatribuir uma solicitação:
   <p>Padrão</p>
   <p>Trabalho ou maior</p></td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Atribuir uma solicitação a uma equipe {#assign-a-request-to-a-team}

Os gerentes de projeto e os solicitantes de emissão podem atribuir trabalho às equipes quando não souberem qual recurso é certo para realizar o trabalho ou quando não importa quem o conclui.

As tarefas atribuídas à equipe permanecem na guia [!UICONTROL Solicitações de equipe] até que um usuário da equipe se volunte para trabalhar na solicitação.

Quando uma solicitação é atribuída a uma equipe e a um usuário que não é membro da equipe, a solicitação fica visível na guia [!UICONTROL Solicitações de equipe] e na área de solicitações de trabalho do usuário. Se o usuário que não está na equipe se voluntariar para trabalhar na tarefa, a tarefa ainda permanecerá na guia [!UICONTROL Solicitações de equipe] até que um usuário da equipe se voluntarie para trabalhar nela.

As equipes podem ser atribuídas a tarefas e problemas de qualquer uma das seguintes maneiras:

* Pelo [!UICONTROL Gráfico de Gantt]
* De uma lista de tarefas ou problemas (individualmente ou em massa)
* Quando uma tarefa ou problema é criado ou modificado
* Por meio de regras de roteamento em uma solicitação (somente emissões)

É possível atribuir manualmente uma solicitação a uma equipe na página da equipe, conforme descrito nesta seção.

Para atribuir manualmente uma solicitação a uma equipe na página da equipe:

{{step1-to-team}}

1. Clique no ícone **[!UICONTROL Alternar equipe]** ![Ícone Alternar equipe](assets/switch-team-icon.png) e, em seguida, selecione uma nova equipe no menu suspenso ou pesquise uma equipe na barra de pesquisa.

1. Clique no ícone **[!UICONTROL Mais]** ![](assets/more-icon.png) e selecione **[!UICONTROL Enviar solicitação de trabalho]**.

   ![](assets/edit-team-settings-350x205.png)

1. Preencha as informações na caixa que é aberta.
1. Clique em **[!UICONTROL Enviar Solicitação]**.\
   Agora é atribuída à equipe uma nova tarefa, que é exibida na guia Solicitações de equipe. Esta tarefa não está atualmente associada a um projeto, mas pode ser movida, conforme descrito em [Mover tarefas](../../manage-work/tasks/manage-tasks/move-tasks.md).

## Reatribuir solicitações {#reassign-requests}

É possível reatribuir solicitações que foram atribuídas à sua equipe:

{{step1-to-team}}

1. Clique no ícone **[!UICONTROL Equipe de comutação]** ![Ícone Equipe de comutação](assets/switch-team-icon.png) e selecione uma nova equipe no menu suspenso ou procure uma equipe na barra de pesquisa.
1. No painel de navegação esquerdo, selecione **[!UICONTROL Solicitações de equipe]**.
1. Clique no ícone **[!UICONTROL Reatribuir]**.

1. Comece a digitar o nome do usuário, grupo ou equipe à qual deseja reatribuir a solicitação e clique em **[!UICONTROL Atribuir]**.\
   A solicitação é reatribuída.
