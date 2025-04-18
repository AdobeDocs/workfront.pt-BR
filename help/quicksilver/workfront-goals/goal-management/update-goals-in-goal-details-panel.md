---
product-previous: workfront-goals
navigation-topic: goal-management
title: Atualizar Metas na Seção Detalhes da Meta no Adobe Workfront Goals
description: Você pode atualizar informações de metas individuais acessando o painel Detalhes da Meta.
author: Alina
feature: Workfront Goals
exl-id: e9df0d98-05a1-4977-b7f1-426b8f5b3eae
source-git-commit: 4e1558b47f6041501aa4e4fbfa6317dec8aee571
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 1%

---

# Atualizar metas na seção Detalhes da meta no Adobe Workfront Goals

<!--Audited for P&P only: 4/2025-->

Você pode atualizar informações de metas individuais acessando o painel Detalhes da Meta.

>[!NOTE]
>
>Não é possível atualizar metas com status Fechado.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> 
   <p>Para o novo plano e estrutura de licença:
  <ul><li>Um plano do Ultimate </li></ul>
   </p>
<p>Para o plano e a estrutura de licença atuais: 
<ul><li> A Pro ou superior </li>
  <li>Uma licença do Adobe Workfront Goals, além de uma licença da Workfront.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licença da Adobe Workfront*</td>
 <td>
 <p>Nova licença: Contributor ou superior</p>
 Ou
 <p>Licença atual: Solicitação ou superior</p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">visão geral das licenças da Adobe Workfront</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produto*</td>
 <td>
  <p> Novo requisito de produto: Workfront</p>
  Ou
  <p>Requisito atual do produto: além de uma licença do Workfront, você deve comprar uma licença do Adobe Workfront Goals. </p> <p>Para obter informações, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para usar as Metas do Workfront</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Nível de acesso*</td>
 <td> <p>Editar acesso às Metas</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Permissões de objeto</td>
 <td>
  <div>
  <p>Exibir permissões ou mais altas para a meta para exibi-la</p>
  <p>Gerenciar permissões para a meta para editá-la</p>
  <p>Para obter informações sobre como compartilhar metas, consulte <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartilhar uma meta no Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclui a área Metas no Menu principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Atualizar metas na seção Detalhes da meta

Você pode acessar uma meta individual a partir de uma lista de metas.

<!--

Updating goals in the Goal Details panel differs depending on where you access the goal from. 

### Update goals in the Goal Details panel in the Production environment

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Goals area in Workfront. 

1. Click the name of a goal in the Goal List, then click the name of a goal.

   This opens the Goal Details panel on the right.
   ![Goal details summary](assets/goal-details-summary-tab-350x294.png)

   >[!TIP]
   >
   >You can also click the name of a goal in the Goal Alignment, Check-in, or Pulse sections. 
   >
   ><!-- drafted for goal redesign:
   >Add this to the TIP above with goal redesign: 
   >
   >The Check-in and Pulse sections have been removed from the Preview environment.
   >

1. On the Summary tab, click the **More icon** ![More icon](assets/more-icon.png), then click any of the following options:

   1. **Edit**. For information about editing goals, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
   1. **Copy**. For information about copying goals, see [Copy goals in Adobe Workfront Goals](../../workfront-goals/goal-management/copy-goals.md).
   1. **Activate**. This option is available only for drafted and inactive goals.

      For information about activating goals, see [Access and open goals in Adobe Workfront Goals](../../workfront-goals/goal-management/access-goals-in-wf-goals.md). 
   
   1. **Close**, then click**Close Goal**. This option is available only for active goals.

      For information about closing goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   
   1. **Deactivate**. This option is available only for active goals. This deactivates the goal immediately.

      For information about deactivating goals, see [Delete and deactivate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).
   
   1. **Delete**, then click **Yes, Delete**.

      For information about deleting goals, see [Delete and deactivate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

      >[!NOTE]
      >
      >Deleted goals cannot be recovered.

   1. **Reopen**, then click **Reopen**. This option is available only for closed goals that are from a current time period.

      For information about reopening goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   
   1. (Conditional) If you clicked any of the options between steps a-i above except Delete or Reopen, click **Save**.    
   
      (!--ensure this is accurate)--)

1. Click **Align to another goal** in the upper-right of the Summary tab, then specify the name of a goal in the **Align to** **another goal** field that you want to align the current goal to. The current goal becomes the child of the goal you align it to. For information about child and parent goals, see [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md). 
1. Click **Add results**. Results drive the progress of your goal. For information about adding results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).

1. Click **Add activities**. Activities drive the progress of your goal. For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 

1. Click the **Updates** tab. Here, you can view goal comments and review the entire editing history of the goal, activities, and results, to understand who changed what and when.

   ![Goal details updates](assets/goal-details-updates-tab-350x280.png)

1. (Optional) Deselect any of the following options if you want to not display them in the Updates tab.&nbsp;They are selected by default: 

   | Option |Description  |
   |---|---|
   | Progress Updates |Displays information about the history of progress updates on results and activities.  |
   | Comments |Displays comments made by users on the goal.  |
   | Editing History |Displays information about creating and updating the goal, results, and activities.  |

1. (Optional) Click **Details** under a progress or an editing history update to display additional information about the update.

   ![Details in update tab](assets/update-details-in-updates-tab-expanded-highlighted-350x139.png)

-->



1. Clique no nome de uma meta na Lista de metas e clique no nome de uma meta.

   Isso abre a seção **Detalhes da meta** à esquerda.

   ![Página de meta](assets/goal-page-unshimmed.png)

1. Clique no **ícone Editar** ![ícone Editar](assets/edit-icon.png) no canto superior direito e clique em **Editar tudo** ou **Visão geral**

   Ou

   Comece a digitar informações em um dos campos editáveis na seção Detalhes da meta. A seção se torna editável.

   >[!IMPORTANT]
   >
   >Nem todos os campos exibidos na seção Detalhes da meta podem ser editados. O Workfront calcula alguns campos que são somente leitura.

1. Atualize ou revise os seguintes campos:

   * **Descrição**: adicionar ou atualizar informações sobre a meta.
   * **Progresso**: indica que porcentagem da meta foi concluída até agora. Não é possível atualizar manualmente o progresso de uma meta. O progresso da meta é um cálculo de todos os indicadores de progresso.
   * **Condição**: indica se a meta é nova e ainda não foi atualizada, se está no destino a ser concluído no prazo ou atrasada. Não é possível atualizar a condição de uma meta. A condição da meta é calculada automaticamente pelo Worfront.\
     Para obter mais informações sobre a condição da meta e o progresso, consulte
     [Visão geral do progresso e da condição da meta nas Metas do Adobe Workfront](../goal-management/calculate-goal-progress.md).
   * **Status**: não é possível atualizar manualmente o status de uma meta. Para obter mais informações, consulte [Visão geral do status da meta em Metas do Adobe Workfront](../goal-management/goal-status-overview.md).
   * **Proprietário da meta**: clique para atualizar o nome do proprietário da meta. Comece digitando o nome de um usuário, equipe, grupo ou o nome de sua organização e selecione-o quando ele for exibido na lista. Você pode ter apenas um proprietário para uma meta.
   * **Meta principal**: comece a digitar o nome de uma meta que você deseja definir como principal da meta selecionada. O progresso da meta selecionada atualizará automaticamente o progresso da meta principal.

     >[!TIP]
     >
     >Não é possível atualizar as seguintes informações sobre uma meta principal:
     >    * Período da meta principal
     >    * Progresso da meta principal
     >    * Proprietário da meta principal.
     >      
     >Você deve atualizar essas informações na própria meta principal.

   * **Período**: clique para atualizar o período de tempo da meta\
     Ou\
     Selecione **Habilitar datas personalizadas** para especificar datas para as **Datas de início** e **Datas de término** da meta.
   * **Notas de fechamento**: este campo está visível somente para metas com o status Fechado. Metas fechadas não podem ser editadas. Reabrir uma meta fechada exclui permanentemente as notas de fechamento.


