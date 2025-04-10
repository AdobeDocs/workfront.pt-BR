---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Mover uma história ágil
description: É possível mover uma história ágil para uma iteração diferente (para equipes Scrum) ou para o backlog (para equipes Kanban e Scrum).
author: Lisa
feature: Agile
exl-id: 0058792e-66b8-4e54-8ce3-50171adff875
source-git-commit: 68aafe63ff8b60a542ed9dd0900b3742c26a1e4f
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

# Mover uma história ágil

É possível mover uma história ágil para uma iteração diferente (para equipes Scrum) ou para o backlog (para equipes Kanban e Scrum).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td> <p>Novo: [!UICONTROL Padrão]</p> 
   ou
   <p>Atual: [!UICONTROL Trabalho] ou superior</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td>[!UICONTROL Gerenciar] acesso à história</td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
