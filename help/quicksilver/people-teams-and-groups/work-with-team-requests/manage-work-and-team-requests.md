---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Gerenciar requisições de trabalho e de equipe
description: Uma solicitação representa uma atribuição pendente de tarefa ou problema. As solicitações de trabalho são feitas a indivíduos e as solicitações de equipe são feitas a equipes.
author: Courtney
feature: People Teams and Groups, Work Management
exl-id: ef96e520-0d5f-4180-a27a-1fbbffff8f2b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/h9ebMyu8AQNPQTzfYkEMbEbHtghIj-wegaml3cM3RMY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: be65ef36-43e4-48e1-a062-caa3778e15be
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 488
ht-degree: 9%

---

# Gerenciar solicitações de trabalho e da equipe

Uma solicitação representa uma atribuição pendente de tarefa ou problema. As solicitações de trabalho são feitas a indivíduos e as solicitações de equipe são feitas a equipes.

>[!NOTE]
>
>As equipes Agile não têm solicitações de equipe.

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
   <p>Leve ou superior</p>
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

Gerentes de projeto e solicitantes de problemas podem atribuir trabalho a equipes quando não sabem qual recurso é certo para fazer o trabalho ou quando não importa quem conclui o trabalho.

As tarefas atribuídas à equipe permanecem na guia [!UICONTROL Solicitações de equipe] até que um usuário na equipe se voluntarie para trabalhar na solicitação.

Quando uma solicitação é atribuída a uma equipe e a um usuário que não é membro da equipe, a solicitação fica visível na guia [!UICONTROL Solicitações da equipe] e na área de solicitações de trabalho do usuário. Se o usuário que não está na equipe se voluntariar para trabalhar na tarefa, a tarefa ainda permanecerá na guia [!UICONTROL Solicitações da equipe] até que um usuário na equipe se voluntarie para trabalhar nela.

As equipes podem ser atribuídas a tarefas e problemas de qualquer uma das seguintes maneiras:

* Através do [!UICONTROL Gráfico de Gantt]
* De uma lista de tarefas ou problemas (individualmente ou em massa)
* Quando uma tarefa ou problema é criado ou modificado
* Por meio de regras de roteamento em uma solicitação (somente ocorrências)

Você pode atribuir uma solicitação manualmente a uma equipe na página da equipe, conforme descrito nesta seção.

Para atribuir manualmente uma solicitação a uma equipe na página da equipe:

{{step1-to-team}}

1. Clique no ícone **[!UICONTROL Equipe de comutação]** ![Ícone Equipe de comutação](assets/switch-team-icon.png) e selecione uma nova equipe no menu suspenso ou procure uma equipe na barra de pesquisa.

1. Clique no ícone **[!UICONTROL Mais]** ![](assets/more-icon.png) e selecione **[!UICONTROL Enviar solicitação de trabalho]**.

   ![](assets/edit-team-settings-350x205.png)

1. Preencha as informações na caixa que será aberta.
1. Clique em **[!UICONTROL Enviar solicitação]**.\
   Agora é atribuída à equipe uma nova tarefa, que é exibida na guia Solicitações da equipe. Esta tarefa não está atualmente associada a um projeto, mas pode ser movida, conforme descrito em [Mover tarefas](../../manage-work/tasks/manage-tasks/move-tasks.md).

## Reatribuir solicitações {#reassign-requests}

É possível reatribuir solicitações que foram atribuídas à sua equipe:

{{step1-to-team}}

1. Clique no ícone **[!UICONTROL Equipe de comutação]** ![Ícone Equipe de comutação](assets/switch-team-icon.png) e selecione uma nova equipe no menu suspenso ou procure uma equipe na barra de pesquisa.
1. No painel de navegação esquerdo, selecione **[!UICONTROL Solicitações da equipe]**.
1. Clique no ícone **[!UICONTROL Reatribuir]**.

1. Comece digitando o nome do usuário, grupo ou equipe para o qual deseja reatribuir a solicitação e clique em **[!UICONTROL Atribuir]**.\
   A solicitação é reatribuída.
