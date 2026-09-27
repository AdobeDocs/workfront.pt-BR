---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Mover uma história ágil
description: Você pode mover uma história Agile para uma iteração diferente (para equipes Scrum) ou para o backlog (para equipes Kanban e Scrum).
author: Courtney
feature: Agile
exl-id: 0058792e-66b8-4e54-8ce3-50171adff875
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/gVEWRh4iiYdy6CwzLubaY3GZ4EE5C5diJ-RvsYFFtE4'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: be65ef36-43e4-48e1-a062-caa3778e15be
    internal-label: Agile
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 11%
---
# Mover um story ágil

Você pode mover uma história Agile para uma iteração diferente (para equipes Scrum) ou para o backlog (para equipes Kanban e Scrum).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Padrão</p> 
   <p>Trabalho ou maior</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td>Gerenciar acesso à história</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Mover uma história de uma iteração ou quadro Kanban para o backlog

1. Vá para a iteração ou quadro Kanban que contém a matéria que você deseja mover para o backlog.
1. Clique no cabeçalho de iteração na parte superior da página.
1. Na guia **[!UICONTROL Histórias]**, selecione as histórias que deseja mover.
1. Clique em **[!UICONTROL Mais]** > **[!UICONTROL Mover para]**. A caixa de diálogo **[!UICONTROL Mover para]** é exibida.

   ![Caixa de diálogo Mover História](assets/iteration-story-move.png)

1. Selecione a Lista de Pendências do **team_name**. No exemplo acima, o nome da equipe é **Marketing**.

1. Clique em **[!UICONTROL Mover]**.

## Mover uma história para uma iteração diferente

Você pode mover uma história para uma iteração diferente para sua equipe do Scrum se for um administrador do sistema ou um membro da equipe à qual a iteração está associada.

>[!NOTE]
>
> A opção **[!UICONTROL Mover para]** não está disponível para matérias pai em uma iteração. Só é possível mover subtarefas para outra iteração.


1. Vá para a iteração que contém a história que você deseja mover.
1. Clique no cabeçalho de iteração na parte superior da página.
1. Na guia **[!UICONTROL Histórias]**, selecione as histórias que deseja mover.
1. Clique em **[!UICONTROL Mais]** > **[!UICONTROL Mover para]**. A caixa de diálogo **[!UICONTROL Mover para]** é exibida.

   ![Caixa de diálogo Mover História](assets/iteration-story-move.png)

1. Selecione **[!UICONTROL Outra Iteração]**.
1. No menu suspenso exibido, selecione a iteração para a qual deseja mover a matéria.

   >[!NOTE]
   >
   >O item de trabalho [!UICONTROL Data de Início Planejada] e [!UICONTROL Data de Conclusão Planejada] são afetados por uma configuração na página [!UICONTROL Editar Equipe]. Para obter informações, consulte a seção [[!UICONTROL Configurar] como as datas são aplicadas ao adicionar itens de trabalho a uma iteração](../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration) no artigo [Configurar Scrum](../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Clique em **[!UICONTROL Mover]**.
