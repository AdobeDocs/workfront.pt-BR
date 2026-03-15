---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Desativar ou excluir uma equipe
description: Você pode desativar as equipes que não usam mais enquanto retém os dados históricos associados. Os administradores do Adobe Workfront podem reativar uma equipe a qualquer momento na área Equipes em Configuração.
author: Courtney
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 10%

---

# Desativar ou excluir uma equipe

Você pode desativar as equipes que não usam mais enquanto retém os dados históricos associados. Os administradores do [!DNL Adobe Workfront] podem reativar uma equipe a qualquer momento na área Equipes em Configuração. Se você desativar um grupo, ele não será mais exibido nas seguintes áreas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Campos de preenchimento automático em formulários personalizados</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Caixa de diálogo de compartilhamento para objetos</p> </li> 
     <li> <p>[!UICONTROL Perfil de Usuário]*</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Menu suspenso de seleção principal na área [!UICONTROL Teams]</p> </li> 
     <li> <p>Tipo [!UICONTROL Assignments]</p> </li> 
     <li> <p>Caixa de diálogo do quadro [!UICONTROL Add to Kanban] em um projeto</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

As equipes desativadas não aparecem quando você pesquisa uma equipe, mas ainda serão exibidas na [!UICONTROL Equipe Inicial] e em Outras Equipes se o usuário tiver sido atribuído à equipe antes da desativação.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Pacote do Adobe Workfront</p> </td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
   <p>Padrão</p>
   <p>Plano</p></td>
  </tr> 
  <tr>
   <td>Configurações de nível de acesso</td>
   <td><p>Nenhuma configuração é necessária para desativar um grupo.</p>
   <p>Para excluir um grupo, você precisa ser um administrador de sistema.</p></td>
  </tr>
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Desativar uma equipe

Qualquer trabalho atribuído à equipe antes da desativação permanece atribuído. Recomendamos reatribuir o trabalho antes de desativar a equipe.

>[!TIP]
>
>É possível criar um relatório para filtrar qualquer tarefa ou problema que tenha a equipe desativada atribuída.

Ao usar filas de solicitações, se você desativar uma equipe atribuída como a equipe padrão em uma regra de roteamento, a equipe permanecerá e as solicitações ainda serão roteadas para a equipe desativada. Recomendamos atualizar as regras de roteamento com equipes ativas antes de desativar a equipe.

{{step1-to-team}}

1. Clique no ícone **[!DNL Switch team]** e, em seguida, selecione uma nova equipe no menu suspenso ou pesquise uma equipe na barra de pesquisa.
1. Clique no menu **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.

   ![](assets/edit-team-settings.png)

1. Desmarque a caixa de seleção **[!UICONTROL Está ativo]** nas configurações da equipe.
1. Clique em **[!UICONTROL Salvar alterações]**.

## Limitações conhecidas de desativação de um grupo

Os grupos desativados são exibidos nas seguintes áreas:

* O campo Proprietário em [!DNL Workfront Goals]. Isso requer uma licença adicional para [!DNL Adobe Workfront Goals]. Para obter mais informações, consulte [Introdução a [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).

## Excluir uma equipe

Somente um administrador de sistema pode excluir um grupo. Se você for um proprietário de equipe (mas não um administrador) e tentar excluir uma equipe, aparecerá uma mensagem de erro.

Para excluir um grupo:

{{step1-to-team}}

1. Clique no ícone **[!DNL Switch team]** e, em seguida, selecione uma nova equipe no menu suspenso ou pesquise uma equipe na barra de pesquisa.
1. Clique no menu **[!UICONTROL Mais]** e selecione **[!UICONTROL Excluir]**.

   ![](assets/edit-team-settings.png)

1. Clique em [!UICONTROL **Confirmar**] na mensagem de confirmação para excluir permanentemente a equipe. As equipes excluídas não podem ser recuperadas.
