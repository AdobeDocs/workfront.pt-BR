---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Desativar uma equipe
description: Você pode desativar as equipes que não usam mais enquanto retém os dados históricos associados. Os administradores do Adobe Workfront podem reativar uma equipe a qualquer momento na área Equipes em Configuração.
author: Lisa
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Desativar uma equipe

Você pode desativar as equipes que não usam mais enquanto retém os dados históricos associados. Os administradores do [!DNL Adobe Workfront] podem reativar uma equipe a qualquer momento na área Equipes em Configuração. Se você desativar um grupo, ele não será mais exibido nas seguintes áreas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Campos de digitação antecipada em formulários personalizados</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Caixa de diálogo de compartilhamento para objetos</p> </li> 
     <li> <p>[!UICONTROL Perfil de Usuário]*</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Menu suspenso de seleção principal na área [!UICONTROL Teams]</p> </li> 
     <li> <p>Digitação antecipada de [!UICONTROL Atribuições]</p> </li> 
     <li> <p>Caixa de diálogo do quadro [!UICONTROL Adicionar ao Kanban] em um projeto</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

As equipes desativadas não aparecem quando você pesquisa por uma equipe, mas ainda serão exibidas na [!UICONTROL Equipe interna] e em Outras equipes se o usuário tiver sido atribuído à equipe antes da desativação.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano*</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>Plano</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber que tipo de plano ou licença você tem, contate o administrador do [!DNL Workfront].

## Desativar uma equipe

Qualquer trabalho atribuído à equipe antes da desativação permanece atribuído. Recomendamos reatribuir o trabalho antes de desativar a equipe.

>[!TIP]
>
>É possível criar um relatório para filtrar qualquer tarefa ou problema que tenha a equipe desativada atribuída.

Ao usar filas de solicitações, se você desativar uma equipe atribuída como a equipe padrão em uma regra de roteamento, a equipe permanecerá e as solicitações ainda serão encaminhadas para a equipe desativada. Recomendamos atualizar as regras de roteamento com equipes ativas antes de desativar a equipe.

1. Clique no ícone ![](assets/main-menu-icon.png) do **[!UICONTROL Menu principal]** no canto superior direito do Adobe Workfront e em **[!UICONTROL Equipes]**.
1. Clique no ícone **[!DNL Switch team]** e selecione uma nova equipe no menu suspenso ou procure uma equipe na barra de pesquisa.
1. Clique no menu **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.

   ![](assets/edit-team-settings-350x205.png)

1. Desmarque a caixa de seleção **[!UICONTROL Está ativo]**.
1. Clique em **[!UICONTROL Salvar alterações]**.

## Limitações conhecidas

As equipes desativadas são exibidas nas seguintes áreas:

* O campo Proprietário em [!DNL Workfront Goals]. Isso requer uma licença adicional para [!DNL Adobe Workfront Goals]. Para obter mais informações, consulte [Introdução a [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).
