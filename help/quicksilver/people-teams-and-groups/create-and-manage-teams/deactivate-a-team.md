---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Desativar uma equipe
description: Você pode desativar equipes que não são mais usadas enquanto mantém os dados históricos associados. Os administradores do Adobe Workfront podem reativar uma equipe a qualquer momento na área Equipes em Configurar.
author: Lisa
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Desativar uma equipe

Você pode desativar equipes que não são mais usadas enquanto mantém os dados históricos associados. [!DNL Adobe Workfront] Os administradores podem reativar uma equipe a qualquer momento na área Equipes em Configurar. Se você desativar uma equipe, a equipe não será mais exibida nas seguintes áreas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Digitar campos avançados em formulários personalizados</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Caixa de diálogo Compartilhamento de objetos</p> </li> 
     <li> <p>[!UICONTROL Perfil do usuário]*</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Menu suspenso de seleção principal na área [!UICONTROL Equipes]</p> </li> 
     <li> <p>Tipo [!UICONTROL Atribuições]</p> </li> 
     <li> <p>Caixa de diálogo do quadro [!UICONTROL Adicionar ao Kanban] em um projeto</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

As equipes desativadas não aparecem quando você pesquisa por uma equipe, mas ainda serão exibidas em [!UICONTROL Equipe inicial] e Outras equipes se o usuário tiver sido atribuído à equipe antes da desativação.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>Plano</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano ou tipo de licença você possui, entre em contato com seu [!DNL Workfront] administrador.

## Desativar uma equipe

Qualquer trabalho atribuído à equipe antes da desativação permanece atribuído. Recomendamos reatribuir o trabalho antes de desativar a equipe.

>[!TIP]
>
>Você pode criar um relatório para filtrar quaisquer tarefas ou problemas em que a equipe desativada ainda esteja atribuída.

Ao usar filas de solicitação, se você desativar uma equipe atribuída como a equipe padrão em uma regra de roteamento, a equipe permanecerá e as solicitações ainda serão roteadas para a equipe desativada. Recomendamos atualizar as regras de roteamento com as equipes ativas antes de desativar a equipe.

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **[!UICONTROL Equipes]**.
1. Clique no botão **[!DNL Switch team]** em seguida, selecione uma nova equipe no menu suspenso ou pesquise por uma equipe na barra de pesquisa.
1. Clique no botão **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.

   ![](assets/edit-team-settings-350x205.png)

1. Limpe o **[!UICONTROL Está ativo]** caixa de seleção.
1. Clique em **[!UICONTROL Salvar alterações]**.

## Limitações conhecidas

As equipes desativadas são exibidas nas seguintes áreas:

* O campo Proprietário em [!DNL Workfront Goals]. Isso requer uma licença adicional para [!DNL Adobe Workfront Goals]. Para obter mais informações, consulte [Introdução a [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).
