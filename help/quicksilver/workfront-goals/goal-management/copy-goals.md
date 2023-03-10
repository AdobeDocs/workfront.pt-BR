---
product-previous: workfront-goals
navigation-topic: goal-management
title: Copiar metas nas metas do Adobe Workfront
description: Você pode copiar metas no Adobe Workfront Metas para criar uma meta. Algumas das informações da meta original são transferidas para a nova meta.
author: Alina
feature: Workfront Goals
exl-id: 690a6030-ee29-4e50-869f-cd014050b364
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Copiar metas nas metas do Adobe Workfront

Você pode copiar metas no Adobe Workfront Metas para criar uma meta. Algumas das informações da meta original são transferidas para a nova meta.

## Requisitos de acesso

<!--drafted for P&P release: 

You must have the following:

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
   <td> <p>Editar o acesso às Metas ou superior</p> <p><b>Nota</b>

<p>Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte:</p> 
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

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Você deve ter o seguinte antes de começar:

* Um modelo de layout que inclui a área Metas no Menu principal.

## Considerações para cópia de metas

Você deve ter acesso a Editar metas no seu nível de acesso para poder copiar metas. Para obter informações sobre como conceder acesso às Metas, consulte [Conceder acesso às Metas da Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

Alguns dos motivos pelos quais você pode querer copiar uma meta existente são:

* No final de um período (trimestre ou ano), quando você deseja recriar a mesma meta para o próximo período.
* No final de um período de tempo, quando a meta não puder ser concluída e você quiser trabalhar nela por outro período de tempo.
* Quando vários membros da equipe têm metas semelhantes e você pode precisar criar uma para cada um deles.

>[!TIP]
>
>Você pode copiar uma meta em qualquer status. Para obter informações sobre status de metas, consulte [Visão geral do status da meta em Metas da Adobe Workfront](../../workfront-goals/goal-management/goal-status-overview.md).

Considere o seguinte ao copiar metas:

* Todas as informações sobre a meta também são copiadas para a nova meta.
* Você pode optar por copiar os resultados de uma meta existente. O nome dos resultados é transferido para a nova meta, mas o progresso atual dos resultados na meta existente não copia para a nova meta. Os resultados copiados são atribuídos ao mesmo proprietário, por padrão.

   >[!NOTE]
   >
   >Se o proprietário original tiver sido excluído ou desativado do Workfront, o novo resultado será atribuído ao usuário conectado.

* Não é possível copiar as atividades de uma meta ao copiar a meta.

## Copiar metas

<!--
Copying goals differs depending on what environment you use. 

To copy goals in the Production environment:

1. Go to a goal and click it to open the Goal Details panel.

   For information about accessing an individual goal, see the "Access individual goals" section in [Access and open goals in Adobe Workfront Goals](../../workfront-goals/goal-management/access-goals-in-wf-goals.md).

   This opens the Goal Details panel.

1. Click the **More icon** ![](assets/more-icon.png), then click **Copy**. 

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


1. Vá para uma meta e clique no botão **Mais** menu ![](assets/more-icon.png), depois clique em **Copiar meta**.

   ![](assets/copy-goal-box-unshimmed.png)

1. Atualize as seguintes informações para a meta copiada:
   * **Nome da meta**: O nome da nova meta. O nome padrão da meta copiada é &quot;Cópia de &lt;original goal=&quot;&quot;>&quot;.
   * **Período**: O período de tempo durante o qual você deseja atingir a meta. Selecione um período de tempo no menu suspenso

      Ou

      Selecionar **Ativar datas personalizadas** para especificar datas personalizadas para a meta **Iniciar** e **Datas finais**. A configuração Ativar datas personalizadas está desativada por padrão.

      >[!TIP]
      >
      >   Desmarcar Ativar datas personalizadas reverte para o período de tempo da meta original.

      * **Proprietário da meta**: O proprietário da meta. Pode ser um usuário, uma equipe, um grupo ou uma empresa. O padrão é o proprietário da meta original.
      * **Descrição**: Informações adicionais sobre a meta.
      * **Copiar resultados**: Selecione essa opção se desejar transferir os resultados da meta atual para a meta copiada. Isso duplica os resultados originais e os anexa à meta copiada. Os resultados da meta copiada têm o mesmo proprietário, nomes e valores medidos que os resultados da meta original.

         >[!NOTE]
         >
         >* O progresso do resultado original não é transferido para a meta copiada.
         >* Se o proprietário original tiver sido excluído ou desativado do Workfront, o novo resultado será atribuído ao usuário conectado.


1. Clique em **Meta de cópia**.

   Uma meta semelhante à original é criada e está em um status de Rascunho.

   >[!NOTE]
   >
   >Se você não tiver copiado os resultados da meta original, primeiro associe a nova meta a um indicador de progresso antes de ativá-la e começar a trabalhar para atingi-la.
   >Para obter informações sobre como associar metas a indicadores de progresso, consulte os seguintes artigos:
   >* [Adicionar resultados às metas em Metas da Adobe Workfront](../results-and-activities/add-results-to-goals.md)
   >* [Adicionar atividades às metas em Metas da Adobe Workfront](../results-and-activities/add-activities-to-goals.md)
   >* [Alinhar metas ao conectá-las às metas da Adobe Workfront](../goal-alignment/align-goals-by-connecting-them.md)

   >
   >Para obter informações sobre como ativar metas, consulte [Ativar metas](../goal-management/activate-goals.md).

