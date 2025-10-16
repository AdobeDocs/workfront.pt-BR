---
product-previous: workfront-goals
navigation-topic: goal-management
title: Copiar Metas nas Metas do Adobe Workfront
description: Você pode copiar metas nas Metas do Adobe Workfront para criar uma meta. Algumas das informações da meta original são transferidas para a nova meta.
author: Alina
feature: Workfront Goals
exl-id: 690a6030-ee29-4e50-869f-cd014050b364
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 4%

---

# Copiar metas nas Metas do Adobe Workfront

<!--Audited for P&P only: 4/2025-->

Você pode copiar metas nas Metas do Adobe Workfront para criar uma meta. Algumas das informações da meta original são transferidas para a nova meta.

## Requisitos de acesso

>[!NOTE]
>
>Sua empresa pode optar por continuar usando o Adobe Workfront Goals se ele comprou esse pacote no passado. Você precisa falar com o seu representante de conta para obter mais detalhes.
>
>O Adobe Workfront Goals não está mais disponível para compra.

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Pacote do Adobe Workfront</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr> 
 <tr>
 <tr>
 <td role="rowheader">Licença do Adobe Workfront</td>
 <td>
 <p>Colaborador ou superior</p>
 <p>Solicitação ou superior</p></td>
 </tr>
 <tr>
 <td role="rowheader">Configuração do nível de acesso</td>
 <td> <p>Editar acesso às Metas</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Permissões de objeto</td>
 <td>
  <div>
  <p>Exibir permissões ou mais altas para a meta para exibi-la</p>
  <p>Gerenciar permissões para a meta para editá-la</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>Todos os usuários, incluindo Administradores do sistema, devem receber um modelo de layout que inclua a área Metas no Menu principal. </p>  
</td>
  </tr>
</tbody>
</table>

Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td>  
  </tr>
 <tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
  <p> New product requirement: Workfront</p>
 <p>Or</p>
  <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
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
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Considerações para copiar metas

Você deve ter acesso a Editar Metas no seu nível de acesso antes de poder copiar metas. Para obter informações sobre como conceder acesso às Metas, consulte [Conceder acesso às Metas do Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

Alguns motivos pelos quais você pode querer copiar uma meta existente são:

* No final de um período (trimestre ou ano), quando você deseja recriar a mesma meta para o próximo período.
* No final de um período, quando a meta não puder ser concluída e você quiser trabalhar nela por outro período.
* Quando vários membros da equipe têm metas semelhantes e pode ser necessário criar uma para cada um deles.

>[!TIP]
>
>Você pode copiar uma meta em qualquer status. Para obter informações sobre status de meta, consulte [Visão geral sobre status de meta em Metas do Adobe Workfront](../../workfront-goals/goal-management/goal-status-overview.md).

Considere o seguinte ao copiar metas:

* Todas as informações sobre a meta também são copiadas para a nova meta.
* Você pode optar por copiar os resultados de uma meta existente. O nome dos resultados é transferido para a nova meta, mas o progresso atual dos resultados na meta existente não é copiado para a nova meta. Os resultados copiados são atribuídos ao mesmo proprietário, por padrão.

  >[!NOTE]
  >
  >Se o proprietário original tiver sido excluído ou desativado do Workfront, o novo resultado será atribuído ao usuário conectado.

* Não é possível copiar as atividades de uma meta ao copiá-la.

## Copiar metas

<!--
Copying goals differs depending on what environment you use. 

To copy goals in the Production environment:

1. Go to a goal and click it to open the Goal Details panel.

   For information about accessing an individual goal, see the "Access individual goals" section in [Access and open goals in Adobe Workfront Goals](../../workfront-goals/goal-management/access-goals-in-wf-goals.md).

   This opens the Goal Details panel.

1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Copy**. 

1. Update any of the following information for the copied goal:

   | Field |Description  |
   |---|---|
   | New Goal |The name of the new goal. The default is the name of the original goal.  |
   | Period |The time period during which you want to achieve the goal. Select a time period from the drop-down menu or click **Define custom dates** to indicate a custom time period. By default, the Period is always the current quarter. |
   | Owner |The owner of the goal. It can be a user, team, group, or a company. The default is the owner of the original goal.  |
   | Description |Additional information about the goal.  |

1. (Conditional) Select **Copy results** if the original goal had results added to it and you want to copy them to the new goal. This duplicates the original results to the new goal. The results of the copied goal have the same owner, names and measured values as the results of the original goal.

   >[!TIP]
   >
   >* The progress of the original result does not transfer to the copied goal. 
   >* If the original owner was deleted or deactivated from Workfront, the new result is assigned to the logged in user.

1. Click **Save**.

   The copied goal is saved with a status of Draft and displays in the Goal Details panel.

   >[!IMPORTANT]
   >
   >If you have not copied the results from the original goal, you must first associate the new goal with a progress indicator before you can activate it and start working towards achieving it. 
   >
   >Do at least one of the following to be able to activate a goal: 
   >   
   >* Add a Result
   >   
   >  For information about adding results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   >   
   >* Add an Activity
   >   
   >  For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 
   >   
   >* Align another goal to it
   >   
   >  For information about aligning goals, see [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).
   >
   > For information about activating a goal, see [Activate goals in Adobe Workfront Goals](../goal-management/activate-goals.md). 

1. Click the **X** icon in the upper-right of the Goal Details panel to close it.

   The copied goal displays in the following sections:

   * Goal List 
   * Check-in (after it is activated)
   * Goal Alignment section (after it is activated) 
   * Pulse
(!--drafted - this was important when we could not update the goal timeframe in the past but we can do that now - not needed
1. (Optional and conditional) If you have copied a goal that was not achieved in a previous time period to continue working on it in the following time period, do the following:

   1. Go to the original goal in the Goal List, Check-in page, or Pulse section and comment on the goal, to indicate that this goal was copied to another, more current goal. For information about commenting on a goal, see [Manage goal comments in Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md).
   1. Close the original goal, to preserve the progress in its original time period. For information about closing goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   1. Update the the **Initial** value of the new Result to match the **End At** value of the previous result, so that your new goal progress will start calculating from the point you achieved in the previous period.
   
-->


1. Vá para uma meta e clique no **Mais** ícone ![Mais](assets/more-icon.png) do menu e clique em **Copiar Meta**.

   ![Copiar caixa de meta](assets/copy-goal-box-unshimmed.png)

1. Atualize as seguintes informações para a meta copiada:
   * **Nome da meta**: o nome da nova meta. O nome padrão da meta copiada é &quot;Cópia de &lt;meta original>&quot;.
   * **Período**: o período durante o qual você deseja atingir a meta. Selecione um período no menu suspenso

     Ou

     Selecione **Habilitar datas personalizadas** para especificar datas personalizadas para as **Datas de início** e **Datas de término** da meta. A configuração Habilitar datas personalizadas é desabilitada por padrão.

     >[!TIP]
     >
     >   Desmarcar Habilitar datas personalizadas reverte para o período de tempo da meta original.

      * **Proprietário da meta**: o proprietário da meta. Pode ser um usuário, equipe, grupo ou uma empresa. O padrão é o proprietário da meta original.
      * **Descrição**: informações adicionais sobre a meta.
      * **Copiar resultados**: selecione esta opção se desejar transferir os resultados da meta atual para a meta copiada. Isso duplica os resultados originais e os anexa à meta copiada. Os resultados da meta copiada têm o mesmo proprietário, nomes e valores medidos que os resultados da meta original.

        >[!NOTE]
        >
        >* O progresso do resultado original não é transferido para a meta copiada.
        >* Se o proprietário original tiver sido excluído ou desativado do Workfront, o novo resultado será atribuído ao usuário conectado.

1. Clique em **Copiar meta**.

   Uma meta semelhante à original é criada e está em um status de Rascunho.

   >[!NOTE]
   >
   >Se você não tiver copiado os resultados da meta original, deverá primeiro associar a nova meta a um indicador de progresso antes de ativá-la e começar a trabalhar para atingi-la.
   >Para obter informações sobre como associar metas a indicadores de progresso, consulte os seguintes artigos:
   >* [Adicionar resultados às metas nas Metas do Adobe Workfront](../results-and-activities/add-results-to-goals.md)
   >* [Adicionar atividades às metas no Adobe Workfront Goals](../results-and-activities/add-activities-to-goals.md)
   >* [Alinhar metas ao conectá-las às Metas do Adobe Workfront](../goal-alignment/align-goals-by-connecting-them.md)
   >
   >Para obter informações sobre como ativar metas, consulte [Ativar metas](../goal-management/activate-goals.md).

