---
product-previous: workfront-goals
navigation-topic: goal-management
title: Editar metas no Adobe Workfront Goals
description: É possível editar as metas existentes a partir de qualquer período e em qualquer status.
author: Alina
feature: Workfront Goals
exl-id: 74db534c-6897-40c2-bea9-a9d30a40f61c
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 1%

---

# Editar metas nas Metas do Adobe Workfront

<!--Audited for P&P only: 10/2025-->

É possível editar as metas existentes a partir de qualquer período e em qualquer status.

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
 <td role="rowheader">Licença do Adobe Workfront</td>
 <td>
 <p>Colaborador ou superior</p>
<p>Solicitação ou superior</p></td>
 </tr>
  <tr>
 <td role="rowheader">Configuração do nível de acesso</td>
 <td> <p>Editar acesso às Metas</p> </td>
 </tr>
 <tr data-mc-conditions="">
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

## Considerações sobre a edição de metas

* Não é possível editar metas com um status de Fechado.
* É possível editar metas a partir de qualquer período.

  É possível editar as seguintes informações para uma meta anterior:

   * Nome
   * Período
   * Status

     >[!TIP]
     >
     >Se a meta for Fechada, sua reabertura recalculará a porcentagem concluída do Progresso. Não é possível editar uma meta encerrada.

   * Descrição
   * Resultados e atividades

## Editar metas

<!--
Editing goals differs depending on what environment you use.

### Edit goals in the Production environment

1. Go to a goal that you want to edit and click the goal name to open the **Goal Details** panel. 
1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Edit**.

   ![Edit goal](assets/edit-goal-highlighted.png)

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

1. Clique no ícone **Menu Principal** ![Ícone do Menu Principal](assets/main-menu-icon.png) e em **Metas**.\
   Uma lista de metas é exibida.
1. Clique em uma meta.\
   A página da meta é exibida.

   ![Página de meta](assets/goal-page-unshimmed.png)

1. Siga um destes procedimentos para editar informações da meta:
   * Clique nos campos exibidos no cabeçalho da meta para atualizá-los. Nem todos os campos no cabeçalho são editáveis.
   * Clique no **ícone Mais** ![ícone Mais](assets/more-icon.png) à direita do nome da meta e clique em **Editar**.
   * Clique em **Detalhes da meta** no painel esquerdo e clique no **ícone Editar** ![ícone Editar](assets/edit-icon.png) no canto superior direito e, em seguida, clique em **Editar tudo**. Comece a atualizar campos na seção Detalhes da meta.

     >[!IMPORTANT]
     >
     >Nem todos os campos exibidos nas áreas mencionadas acima podem ser editados. O Workfront calcula alguns campos que são somente leitura.

1. (Condicional) Dependendo do que você selecionou na etapa anterior, atualize as seguintes informações sobre a meta:

   * Atualize as seguintes informações no cabeçalho da meta e pressione Enter para salvar as alterações:
      * **Nome da meta**: clique no nome da meta e comece a digitar um novo nome.
      * **Proprietário**: clique no nome do proprietário, comece a digitar o nome de um usuário, equipe, grupo ou empresa e selecione-o quando ele for exibido na lista. Você pode ter apenas um proprietário para uma meta.
   * Atualize as seguintes informações na caixa Editar Meta e clique em **Salvar**:
      * **Nome da meta**
      * **Período**: clique para atualizar o período de tempo da meta\
        Ou\
        Selecione **Habilitar datas personalizadas** para especificar datas para as **Datas de início** e **Datas de término** da meta.

        >[!TIP]
        >
        >Desmarque **Habilitar datas personalizadas** para retornar ao período original da meta.

      * **Proprietário da meta**
      * **Descrição**: adicionar ou atualizar informações sobre a meta.
   * Atualizar ou revisar informações na seção Detalhes da meta. Para obter mais informações, consulte [Atualizar metas na seção Detalhes da meta no Adobe Workfront Goals](../goal-management/update-goals-in-goal-details-panel.md).

   <!-- (should you update the title here after changing it at production??? - change it to Update goals in the goal Details section)-->

1. (Opcional) Clique em **Indicadores de progresso** no painel esquerdo para adicionar resultados, atividades ou projetos à meta. Ao adicionar indicadores de progresso, é possível rastrear o progresso da meta.
Para obter mais informações, consulte os seguintes artigos:
   * [Adicionar atividades às metas no Adobe Workfront Goals](../results-and-activities/add-activities-to-goals.md)
   * [Adicionar resultados às metas nas Metas do Adobe Workfront](../results-and-activities/add-results-to-goals.md).
   * [Adicionar projetos às metas no Adobe Workfront Goals](../results-and-activities/connect-projects-to-goals-overview.md).

</div>
