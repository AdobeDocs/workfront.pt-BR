---
product-previous: workfront-goals
navigation-topic: goal-management
title: Editar metas em metas do Adobe Workfront
description: É possível editar metas existentes a partir de qualquer período de tempo e em qualquer status.
author: Alina
feature: Workfront Goals
exl-id: 74db534c-6897-40c2-bea9-a9d30a40f61c
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 1%

---

# Editar metas em metas do Adobe Workfront

É possível editar metas existentes a partir de qualquer período de tempo e em qualquer status.

## Requisitos de acesso

<!--drafted - for P&P releases: 

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
* Você criou as metas que deseja editar ou tem permissões de gerenciamento para elas.

## Considerações sobre a edição de metas

* Não é possível editar metas com um status Fechado.
* Você pode editar metas de qualquer período de tempo.

   Você pode editar as seguintes informações para uma meta anterior:

   * Nome
   * Período
   * Status

      >[!TIP]
      >
      >Se a meta for Fechada, reabri-la recalcula a porcentagem de Andamento concluída. Não é possível editar uma meta fechada.

   * Descrição
   * Resultados e atividades

## Editar metas

<!--
Editing goals differs depending on what environment you use.

### Edit goals in the Production environment

1. Go to a goal that you want to edit and click the goal name to open the **Goal Details** panel. 
1. Click the **More icon** ![](assets/more-icon.png), then click **Edit**.

   ![](assets/edit-goal-highlighted.png)

1. Update the name of the goal in the **Goal** field. 
1. Select a time period when the goal should be completed.

   Select from the following predefined options:

   * The current year
   * The quarters of the current year
   * The next two years
   * The quarters of the next two years

   Or

   Click **Define custom dates** to select a custom time frame. 

1. (Conditional) Select a start and an end date for your goal, if you clicked **Define custom dates**.

   
   <p>(NOTE: these fields don't yet have a name) </p>
   

   >[!CAUTION]
   >
   >You cannot create a goal with custom dates in the past.

1. (Optional) Click **Reset custom dates** to return to the predefined options.

   >[!TIP]
   >
   >We recommend that everyone in your organization selects the same time frames for similar goals or goals that are aligned. This provides better alignment between goals and ensures that everyone's work supports your larger organization-wide strategy.

1. Click the **Owner** field and select a new owner for the goal, if you want to indicate someone else as the owner of the goal. 
1. (Conditional) Start typing the name of a user, team, group, or the name of your organization in the **Owner** field, then select it when it displays in the list. You can have only one owner for a goal. 
1. Update the **Description** of the goal, then click **Save**.

-->

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png), depois clique em **Metas**.\
   Uma lista de metas é exibida.
1. Clique em uma meta.\
   A página de meta é exibida.

   ![](assets/goal-page-unshimmed.png)

1. Siga um destes procedimentos para editar informações para a meta:
   * Clique em campos que são exibidos no cabeçalho da meta para atualizá-los. Nem todos os campos no cabeçalho são editáveis.
   * Clique no botão **Ícone Mais** ![](assets/more-icon.png) à direita do nome da meta, em seguida, clique em **Editar**.
   * Clique em **Detalhes da meta** no painel esquerdo e clique no botão **Ícone Editar** ![](assets/edit-icon.png) no canto superior direito, em seguida, clique em **Editar tudo**. Comece a atualizar campos na seção Detalhes da meta .

      >[!IMPORTANT]
      >
      >Nem todos os campos exibidos nas áreas mencionadas acima podem ser editados. O Workfront calcula alguns campos e eles são somente leitura.

1. (Condicional) Dependendo do que você selecionou na etapa anterior, atualize as seguintes informações sobre a meta:

   * Atualize as seguintes informações no cabeçalho da meta e pressione Enter para salvar as alterações:
      * **Nome da meta**: Clique no nome da meta e comece a digitar um novo nome.
      * **Proprietário**: Clique no nome do proprietário e comece a digitar o nome de um usuário, equipe, grupo ou empresa, em seguida, selecione-o quando for exibido na lista. Você só pode ter um proprietário para uma meta.
   * Atualize as seguintes informações na caixa Editar meta e clique em **Salvar**:
      * **Nome da meta**
      * **Período**: Clique em para atualizar o período de tempo da meta\
         Ou\
         Selecionar **Ativar datas personalizadas** para especificar datas para a meta **Iniciar** e **Datas finais**.

         >[!TIP]
         >
         >Desmarcar **Ativar datas personalizadas** para retornar ao período de tempo original da meta.

      * **Proprietário da meta**
      * **Descrição**: Adicione ou atualize informações sobre a meta.
   * Atualize ou revise as informações na seção Detalhes da meta . Para obter mais informações, consulte [Atualizar metas na seção Detalhes da meta em Metas da Adobe Workfront](../goal-management/update-goals-in-goal-details-panel.md).

   <!-- (should you update the title here after changing it at production??? - change it to Update goals in the goal Details section)-->

1. (Opcional) Clique em **Indicadores de progresso** no painel esquerdo para adicionar resultados, atividades ou projetos à meta. Ao adicionar indicadores de progresso, é possível rastrear o progresso da meta.
Para obter mais informações, consulte os seguintes artigos:
   * [Adicionar atividades às metas em Metas da Adobe Workfront](../results-and-activities/add-activities-to-goals.md)
   * [Adicionar resultados às metas em Metas da Adobe Workfront](../results-and-activities/add-results-to-goals.md).
   * [Adicionar projetos às metas em Metas da Adobe Workfront](../results-and-activities/connect-projects-to-goals-overview.md).

</div>
