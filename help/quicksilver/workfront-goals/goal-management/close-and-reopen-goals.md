---
product-previous: workfront-goals
navigation-topic: goal-management
title: Fechar e reabrir metas em Metas da Adobe Workfront
description: Você pode fechar uma meta quando quiser indicar que a concluiu ou que não está mais trabalhando nela porque ela se tornou obsoleta.
author: Alina
feature: Workfront Goals
exl-id: bbb549c1-aea6-4f5e-8a6b-01fc04cf06ef
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# Fechar e reabrir metas em Metas da Adobe Workfront

Você pode fechar uma meta quando desejar indicar o seguinte:

* A meta é alcançada, seja porque você a atingiu, seja porque o período decorrido.
* Já não está a trabalhar nem planeia fazê-lo no futuro imediato.

Você pode reabrir metas que foram fechadas quando elas se tornam relevantes novamente.

## Requisitos de acesso

<!--drafted for P&P release: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">Object permissions</td>
   <td>
    <div>
     <p>View or higher permissions to the goal to view it</p>
     <p>Manage permissions to the goal to edit it</p>
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
    </div> </td>
  </tr>
 </tbody>
</table>

-->

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Pro ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitação ou superior</p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Visão geral das licenças do Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td> <p>Você deve comprar uma licença adicional para a funcionalidade Metas da Adobe Workfront para acessar descrita neste artigo. </p> <p>Para obter mais informações, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para usar as metas do Workfront</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar o acesso às Metas ou superior</p> <p><b>Nota</b><p>Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Conceder acesso às Metas da Adobe Workfront</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> 
    <div> 
     <p>Gerenciar permissões para a meta</p> 
     <p>Para obter informações sobre como compartilhar metas, consulte <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartilhar uma meta na Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Você deve ter o seguinte antes de começar:

* Um modelo de layout que inclui a área Metas no Menu principal.

## Considerações ao fechar ou reabrir metas

* Você deve ter acesso a Editar metas no seu nível de acesso para fechar e reabrir metas. Para obter informações sobre como conceder acesso às Metas, consulte [Conceder acesso às Metas da Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).
* Você só pode fechar metas ativas. Não é possível fechar metas que estejam no status de Rascunho.

   Para obter informações sobre status de metas, consulte [Visão geral do status da meta em Metas da Adobe Workfront](../../workfront-goals/goal-management/goal-status-overview.md).

* Fechar metas bloqueia seu progresso e permite que você avalie o desempenho ao realizá-lo.

   >[!CAUTION]
   >
   >Ao fechar uma meta que tenha metas de contribuição ativas, seu progresso muda após o fechamento para indicar o progresso das metas ativas de contribuição. Para obter informações sobre como alinhar metas, consulte [Alinhar metas ao conectá-las às metas da Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

* Atualize os indicadores de progresso da meta antes de fechá-la para garantir que ela se feche com um valor de progresso preciso. Se todos os indicadores de progresso tiverem sido alcançados, a porcentagem de meta concluída deve ser de 100% e seu objetivo foi atingido. Para obter informações sobre como atualizar suas metas, consulte [Atualizar o progresso da meta nas Metas da Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).
* Deixe quaisquer comentários finais como uma atualização para as metas que você fechar. Para obter informações sobre como adicionar comentários às metas, consulte [Gerenciar comentários da meta nas Metas da Adobe Workfront](../../workfront-goals/goal-management/manage-goal-comments.md).
* Não é mais possível atualizar o progresso dos resultados e atividades em uma meta que você fecha.
* Você pode reabrir uma meta fechada se quiser continuar trabalhando nela.
* Se a meta não tiver sido alcançada, considere copiar a maioria de suas informações para o próximo período (trimestre ou ano). Essa é uma ótima opção para metas que são as mesmas de um período de tempo para o próximo ou metas que talvez você ainda precise trabalhar para atingir no próximo período de tempo. Para obter informações sobre cópia de metas, consulte [Copiar metas nas metas do Adobe Workfront](../../workfront-goals/goal-management/copy-goals.md). Você também pode atualizar o período de tempo na meta em vez de copiá-lo para outro período.
* O Workfront exclui os comentários de uma meta fechada quando você a reabre. Se você precisar manter os comentários, recomendamos copiar a meta fechada, incluindo quaisquer resultados associados a ela, em vez de reabri-la.


## Fechar metas

<!--
Closing goals differs depending on what environment you use. 

### Close goals in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List opens. 

1. (Optional) Modify your filters to display only goals that are active.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md). 

1. Click an active goal.

   The Goal Details panel displays on the right. 

1. (Optional and recommended) Click the **Updates** tab and add an update in the **Comment here** field about the reason you are closing the goal, then click **Post**. 

1. Click the **More icon** ![](assets/more-icon.png) to the right of the goal name, then click **Close** > **Close Goal**.

   This closes the goal and saves the current progress on the goal and its results and activities.

   >[!IMPORTANT]
   >
   >If the goal has contributing goals that are still active, the progress of the goal continues to update based on the progress of the aligned goals.
   >
   >
   >![](assets/closing-goals-with-active-aligned-goals-warning-350x71.png)   >
   >

1. (Optional) Modify your filters again to display only closed goals. The goals you closed display on the screen.
-->

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) > **Metas** no canto superior direito.

   A Lista de metas é aberta.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Opcional) Modifique seus filtros para exibir somente as metas que estão ativas.

   Para obter informações sobre como filtrar informações nas Metas do Workfront, consulte [Filtrar informações em metas do Adobe Workfront](../goal-management/filter-information-wf-goals.md).
1. Clique em uma meta ativa.

   A página de meta é aberta.

   ![](assets/goal-page-unshimmed.png)
1. Clique no botão **Mais** menu ![](assets/more-icon.png) à direita do nome da meta, em seguida, clique em **Fechar**.

   A meta é fechada e você recebe uma confirmação no canto superior direito da tela.

   ![](assets/goal-close-confirmation-with-add-closing-notes-link.png)

1. (Opcional) Na caixa de confirmação, clique em **Adicionar notas de fechamento** para adicionar comentários sobre essa meta e por que você precisa fechá-la.
1. Adicione as notas de fechamento, em seguida, clique em **Adicionar observações**.

   ![](assets/add-closing-notes-box-unshimmed.png)

   Os comentários são exibidos na seção Detalhes da meta da página da meta, na área Notas de fechamento .

   >[!NOTE]
   >
   >O Workfront exclui as notas de fechamento se você reabrir posteriormente uma meta fechada.


## Reabrir metas

Você pode reabrir metas fechadas se decidir que elas se tornaram relevantes novamente e que é necessário continuar atualizando seu progresso.

<!--
Reopening goals differs depending on what environment you use.

### Reopen goals in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List opens. 

1. (Optional) Modify your filters to display only goals that are closed.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).


1. Click a closed goal.

   This opens the Goal Details panel on the right. 

1. Click the **More icon** ![](assets/more-icon.png) to the right of the goal name, then click **Reopen** > **Reopen**.

   This reopens the goal and places it in a status of Active. The progress of the goal is recalculated starting with the current date. 

1. (Optional) Modify your filters again to display only active goals. The goals you opened display on the screen.

-->

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png)> **Metas** no canto superior direito.

   A Lista de metas é aberta.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Opcional) Modifique seus filtros para exibir somente as metas que estão fechadas.

   Para obter informações sobre como filtrar informações nas Metas do Workfront, consulte [Filtrar informações em metas do Adobe Workfront](../goal-management/filter-information-wf-goals.md).
1. Clique no nome de uma meta fechada.

   A página de meta é aberta.
1. Clique no botão **Mais** menu ![](assets/more-icon.png) à direita do nome da meta, em seguida **Reabrir** > **Reabrir**.

   Os seguintes itens ocorrem:
   * O objetivo agora está aberto e tem um status Ativo.
   * O progresso da meta é recalculado a partir da data atual.
   * Todas as notas de fechamento são excluídas da página Detalhes da meta . Não é possível recuperar as notas de fechamento excluídas.

1. (Opcional) Modifique seus filtros novamente para exibir somente as metas ativas.

   As metas que você abriu são exibidas na tela .

