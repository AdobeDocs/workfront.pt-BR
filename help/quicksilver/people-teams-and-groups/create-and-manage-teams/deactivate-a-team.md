---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Desativar ou excluir uma equipe
description: Você pode desativar as equipes que não usam mais enquanto retém os dados históricos associados. Os administradores do Adobe Workfront podem reativar uma equipe a qualquer momento na área Equipes em Configuração.
author: Lisa
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: 79da9f7ed5149ca33f6eaeac347188149f410695
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

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

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
   <p>Novo: Padrão</p>
   <p>ou</p>
   <p>Atual: Plano</p></td>
  </tr>
  <tr>
   <td>Configurações de nível de acesso</td>
   <td><p>Não são necessárias configurações para desativar um grupo.</p>
   <p>É necessário ser administrador do sistema para excluir uma equipe.</p></td>
  </tr>
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Desativar uma equipe

Qualquer trabalho atribuído à equipe antes da desativação permanece atribuído. Recomendamos reatribuir o trabalho antes de desativar a equipe.

>[!TIP]
>
>É possível criar um relatório para filtrar qualquer tarefa ou problema que tenha a equipe desativada atribuída.

Ao usar filas de solicitações, se você desativar uma equipe atribuída como a equipe padrão em uma regra de roteamento, a equipe permanecerá e as solicitações ainda serão encaminhadas para a equipe desativada. Recomendamos atualizar as regras de roteamento com equipes ativas antes de desativar a equipe.

{{step1-to-team}}

1. Clique no ícone **[!DNL Switch team]** e selecione uma nova equipe no menu suspenso ou procure uma equipe na barra de pesquisa.
1. Clique no menu **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.

   ![](assets/edit-team-settings.png)

1. Desmarque a caixa de seleção **[!UICONTROL Está ativo]** nas configurações da equipe.
1. Clique em **[!UICONTROL Salvar alterações]**.

## Limitações conhecidas da desativação de um grupo

As equipes desativadas são exibidas nas seguintes áreas:

* O campo Proprietário em [!DNL Workfront Goals]. Isso requer uma licença adicional para [!DNL Adobe Workfront Goals]. Para obter mais informações, consulte [Introdução a [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).

## Excluir uma equipe

Somente um administrador do sistema pode excluir uma equipe. Se você for um proprietário de equipe (mas não um administrador) e tentar excluir uma equipe, verá uma mensagem de erro.

Para excluir uma equipe:

{{step1-to-team}}

1. Clique no ícone **[!DNL Switch team]** e selecione uma nova equipe no menu suspenso ou procure uma equipe na barra de pesquisa.
1. Clique no menu **[!UICONTROL Mais]** e selecione **[!UICONTROL Excluir]**.

   ![](assets/edit-team-settings.png)

1. Clique em [!UICONTROL **Confirmar**] na mensagem de confirmação para excluir permanentemente a equipe. As equipes excluídas não podem ser recuperadas.
