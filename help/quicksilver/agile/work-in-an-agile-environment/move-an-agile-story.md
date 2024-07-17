---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Mover uma história ágil
description: É possível mover uma história ágil para uma iteração diferente (para equipes Scrum) ou para o backlog (para equipes Kanban e Scrum).
author: Lisa
feature: Agile
exl-id: 0058792e-66b8-4e54-8ce3-50171adff875
source-git-commit: 11009f24cd482e83319ed9f1ecf3f7a2f4e79d52
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# Mover uma história ágil

É possível mover uma história ágil para uma iteração diferente (para equipes Scrum) ou para o backlog (para equipes Kanban e Scrum).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano*</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Work] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>[!UICONTROL Worker] ou superior</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do [!DNL Workfront] se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do [!DNL Workfront] pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>[!UICONTROL Gerenciar] acesso à história</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

## Mover uma história de uma iteração ou quadro Kanban para o backlog

1. Vá para a iteração ou quadro Kanban que contém a matéria que você deseja mover para o backlog.
1. Clique no cabeçalho de iteração na parte superior da página.
1. Na guia **[!UICONTROL Histórias]**, selecione as histórias que deseja mover.
1. Clique em **[!UICONTROL Mais]** > **[!UICONTROL Mover para]**.

   A caixa de diálogo **[!UICONTROL Mover História]** é exibida.

   ![Caixa de diálogo Mover História](assets/iteration-story-move.png)

1. Selecione o Backlog do *nome_da_equipe*.\
   No exemplo acima, o nome da equipe é&#x200B; **Marketing.**

1. Clique em **[!UICONTROL Mover história]**.

## Mover uma história para uma iteração diferente

Você pode mover uma história para uma iteração diferente para sua equipe do Scrum.

>[!NOTE]
>
>A opção **[!UICONTROL Mover para]** não está disponível para matérias pai em uma iteração. Só é possível mover subtarefas para outra iteração.

1. Vá para a iteração que contém a história que você deseja mover.
1. Clique no cabeçalho de iteração na parte superior da página.
1. Na guia **[!UICONTROL Histórias]**, selecione as histórias que deseja mover.
1. Clique em **[!UICONTROL Mais]** > **[!UICONTROL Mover para]**.

   A caixa de diálogo **[!UICONTROL Mover História]** é exibida.

   ![Caixa de diálogo Mover História](assets/iteration-story-move.png)

1. Selecione **[!UICONTROL Outra iteração]** e, no menu suspenso, selecione a iteração para onde deseja mover a história.

   >[!NOTE]
   >
   >O item de trabalho [!UICONTROL Data de Início Planejada] e [!UICONTROL Data de Conclusão Planejada] são afetados por uma configuração na página [!UICONTROL Editar Equipe]. Para obter informações, consulte a seção [[!UICONTROL Configurar] como as datas são aplicadas ao adicionar itens de trabalho a uma iteração](../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) no artigo [Configurar Scrum](../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Clique em **[!UICONTROL Mover história]**.
