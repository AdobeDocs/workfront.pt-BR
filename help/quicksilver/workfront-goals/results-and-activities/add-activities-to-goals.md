---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Adicionar atividades às metas no Adobe Workfront Goals
description: As atividades medem o progresso de uma meta. Sem resultados associados, atividades ou metas alinhadas, uma meta não pode ser ativada e o progresso não pode ser registrado nela.
author: Alina
feature: Workfront Goals
exl-id: 4d6ef324-4b5c-402b-b64d-b1a2a7d2ab57
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 1%

---

# Adicionar atividades às metas no Adobe Workfront Goals

As atividades medem o progresso de uma meta. Sem associar resultados, atividades, projetos ou metas alinhadas, não é possível ativar uma meta e registrar o progresso nela.

## Requisitos de acesso

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
  <ul><li>Um plano Ultimate </li>
  Ou
  <li>Uma licença adicional para o Adobe Workfront Goals para os planos Prime ou Select Adobe Workfront. </li></ul> </p>
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
 <p>Licença atual: Solicitação ou superior</p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Visão geral das licenças do Adobe Workfront</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produto*</td>
 <td>
 <p> Novo requisito de produto, um dos seguintes: </p>
<ul>
<li>Um plano Select ou Prime do Adobe Workfront e uma licença adicional do Adobe Workfront Goals.</li>
<li>Um plano do Ultimate Workfront que inclui o Workfront Goals por padrão. </li></ul>
 <p>Ou</p>
 <p>Requisito atual do produto: um plano do Workfront e uma licença adicional para o Adobe Workfront Goals. </p> <p>Para obter informações, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para usar as metas do Workfront</a>. </p> </td>
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

## Pré-requisitos

Você deve ter uma meta existente para adicionar atividades a ela.

Para obter informações sobre como criar metas, consulte [Criar metas no Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>Uma meta não pode ter mais de 1.000 atividades, resultados ou metas alinhadas.

Para obter mais informações sobre atividades, consulte [Introdução aos resultados e atividades nos Adobe Workfront Goals](../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md).

## Adicionar uma atividade a uma meta

<!--
Adding activities to goals differs depending on which environment you use.

### Add an activity to a goal in the Production environment

1. Go to the goal for which you want to add an activity and click the name to open the **Goal Details** panel.
1. Click **Add activities**.

   ![](assets/add-activity-inside-goal-details-highlighted-350x152.png)

1. From the **Activity Type** drop-down menu, select the type of activity you want to associate with your goal.&nbsp;Select **Manual progress bar** or **Project**. Manual progress bar is the default selection. 
1. (Conditional) Depending on which activity type you selected, do the following:

   1. If you selected **Manual progress bar**:

      1. Start typing a name for your activity in the **Activity** field. 
      1. (Optional) If you want to set the activity owner as someone other than yourself, click your name in the **Owner** field and begin typing the name of the user that you want to assign as the activity owner, then click it when it appears in the drop-down list.

         >[!NOTE]
         >
         >You cannot assign a team or group as an activity owner.

         When you update the progress of an activity, the progress of the goal automatically updates.

   1. If you selected **Project**:

      1. Click the **Connect projects** field.

         Existing projects that you have access to View display in the Connect projects list. Projects that are in a status of Dead do not display in the list. 
      
      1. Click the name of a project to add it as an activity to the goal. You can select several projects at one time.

         Workfront uses the project percent complete of all the attached projects to calculate the progress of the goal.

         For more information about associating projects with goals, see [Add projects to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

         >[!TIP]
         >
         >   
         >   * The owner of the project becomes the owner of this activity. If the project has no owner, then the activity has no owner. 
         >   * You cannot manually update the progress of a project. Workfront calculates the progress of the project based on the project percent complete. When the project percent complete updates in Workfront this also updates the connected project in Workfront Goals including the percent complete of the goal. 
         >   
         >

1. Click **Save**.

   The activity is saved for the selected goal. After you activate the goal, the progress of the goal automatically updates when you update the progress of an activity or when the percent complete of a project updates. For information about activating a goal, see [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).

-->


1. Clique em **Menu principal** ![](assets/main-menu-icon.png), depois **Metas**.
1. Na Lista de metas, clique no nome de uma meta para abrir a página da meta.
1. Clique em **Indicadores de progresso** no painel esquerdo.
1. No menu suspenso Novo indicador de progresso, clique em **Criar atividade**.

   A caixa Nova atividade é aberta.

   ![](assets/new-activity-box-unshimmed.png)

1. Insira um nome para a atividade no campo Nome da atividade. Este campo é obrigatório.
1. (Opcional) Remova seu nome da lista **Proprietário da atividade** se desejar atribuir a atividade a outro usuário. Por padrão, você é o proprietário de uma atividade criada.

   >[!NOTE]
   >
   >Não é possível atribuir uma equipe, um grupo ou uma empresa como um proprietário de atividade.

1. Clique em **Criar atividade** para salvá-la e adicioná-la à meta selecionada.

   A atividade é exibida na seção Progress indicators da página de metas, no Agrupamento de atividades.





