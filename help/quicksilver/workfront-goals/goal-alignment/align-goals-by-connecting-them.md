---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Alinhar metas ao conectá-las às Metas do Adobe Workfront
description: Se você for um colaborador individual com uma meta pessoal, convém alinhá-la às metas da sua equipe para exibir efetivamente o progresso de sua própria meta no contexto maior da estratégia da organização.
author: Alina
feature: Workfront Goals
exl-id: 4276f1c9-2ee9-4f74-b011-ae1e19fefe35
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 0%

---

# Alinhar metas ao conectá-las às Metas do Adobe Workfront

<!--Audited P&P only: 10/2025-->

Se você for um colaborador individual com uma meta pessoal, convém alinhá-la às metas da sua equipe para exibir efetivamente o progresso de sua própria meta no contexto maior da estratégia da organização.

Quando todos na organização têm suas metas alinhadas às metas da organização, eles podem ver claramente como suas contribuições individuais e esforços de equipe ajudam a avançar em prioridades maiores no nível da empresa. Para obter mais informações sobre as práticas recomendadas para alinhar metas, consulte [Visão geral do alinhamento de metas em Metas do Adobe Workfront](../../workfront-goals/goal-alignment/goal-alignment-overview.md).

Há duas abordagens para conectar metas no Adobe Workfront Goals:

* Você pode criar alinhamento entre metas ao conectar metas umas às outras.

* Você pode alinhar duas metas manualmente ou converter resultados e atividades de uma meta existente para outra meta. O resultado ou a atividade convertida se torna a meta secundária da meta original.

>[!IMPORTANT]
>
>Uma meta pode ter um total de 1000 indicadores de progresso.

Este artigo descreve como alinhar metas ao conectá-las umas às outras. Para obter informações sobre como alinhar metas convertendo resultados e atividades em metas, consulte [Alinhar metas convertendo resultados e atividades em metas](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

## Requisitos de acesso

>[!NOTE]
>
>Sua empresa pode optar por continuar usando o Adobe Workfront Goals se ele comprou esse pacote no passado. Você precisa falar com o seu representante de conta para obter mais detalhes.
>
>O Adobe Workfront Goals não está mais disponível para compra.

+++Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<td> <p>Pacote do Adobe Workfront</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>Licença do Adobe Workfront</p> </td> 
   <td> <p>Colaborador ou superior</p> 
     <p>Solicitante ou superior</p> </td> 
  </tr>

<td><p>Configurações de nível de acesso</p> </td> 
   <td> <p>Editar acesso às Metas</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permissões de objeto </p> </td> 
   <td> <p>Gerenciar permissões para uma meta</p>  </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>Todos os usuários, incluindo Administradores do sistema, devem receber um modelo de layout que inclua a área Metas no Menu principal. </p>  
</td>
  </tr>
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso à documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
  <p> New product requirement: Workfront</p>
  Or
  <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Object permissions</td>
 <td>
  
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
   </td>
 </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Alinhar metas conectando-as entre si

<!--
Aligning goals by connecting them differs depending on what environment you use. 

### Align goals by connecting them in the Production environment

1. Create two goals that you want to align. For information about creating goals, see [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).
1. (Optional) Activate the goals that you want to align. You can align goals that have a Draft, Active, or Inactive status. For information about activating goals, see [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).
1. Go to the goal that you want to align (child goal) to another goal (parent goal) and click its name to open the **Goal Details** panel.

   For example, if you want Goal 2 to influence the progress of Goal 1, you must go to Goal 2. 

1. Click **Align to another goal** in the upper-right corner of the right panel.

   ![Align to another goal](assets/align-to-another-goal-link-highlighted-350x128.png)

1. Start typing the name of an existing goal or the name of an owner in the **Align to another goal** field, then select it when it appears in the list. Only goals that are from the same or future periods display in the list. 
1. Click **Save**.

   The goal you started with (Goal 2) is now the child goal of the goal you aligned it with (Goal 1).   
   The aligned goals display connected in the Goal Alignment section with Goal 2 as secondary to Goal 1.

   ![Aligned cards](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Optional) To view the goals in the Goal Alignment section, do one of the following:

   * Click the Goal Alignment section in the left panel and find the goals by applying the correct filter. For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).
   * Click the Goal List, Check-in, or Pulse sections in the left panel and find one of the goals, then click the **Alignment icon** ![Align icon](assets/align-icon.png) next to the goal name to go directly to the goal in the Goal Alignment section.

   For information about the Goal Alignment section, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md). 

1. (Optional) Add activities and results to either goal to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Optional) Remove the alignment between two goals, when you consider that no longer is relevant to your organization's overall strategy For information about removing alignment between goals, see [Remove goal alignment in Adobe Workfront Goals](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

-->
1. Crie duas metas que deseja alinhar. Para obter informações sobre como criar metas, consulte [Criar metas nas Metas do Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).
1. (Opcional) Ative as metas que deseja alinhar. Você pode alinhar metas com status Rascunho, Ativo ou Inativo. Para obter informações sobre como ativar metas, consulte [Ativar metas nas Metas da Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).
1. Vá para a meta que você deseja alinhar (meta secundária) a outra meta (meta principal) e clique no nome para abrir a página de metas.

   >[!INFO]
   >
   >Por exemplo, se você quiser que a Meta 2 influencie o progresso da Meta 1, vá para a Meta 2.

1. Clique em **Detalhes da meta** no painel esquerdo.

1. Na área **Informações da meta principal**, clique em **Adicionar** no campo **Meta principal** se não houver uma meta principal,

   Ou

   Clique no nome da meta principal para escolher outra.

1. Comece digitando o nome de uma meta existente no campo **Meta principal**, em seguida, selecione-a quando ela aparecer na lista. Somente as metas que são do mesmo período ou de períodos futuros são exibidas na lista.

1. Clique em **Salvar alterações**.

   A meta com a qual você começou (Meta 2) agora é a meta secundária da meta principal à qual você a alinhou (Meta 1).\
   As metas alinhadas são exibidas conectadas na seção Alinhamento de metas com a Meta 2 como secundária à Meta 1.
A meta secundária é exibida na seção Indicadores de progresso da meta principal, pois seu progresso atualiza o progresso da meta principal.

   ![Cartões alinhados](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Opcional) Para exibir as metas na seção Alinhamento de metas, vá para a área Metas do Workfront e clique na seção **Alinhamento de metas** no painel esquerdo. Para obter informações sobre a seção Alinhamento de Meta, consulte [Navegar pela seção Alinhamento de Meta em Metas do Adobe Workfront](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).

1. (Opcional) Adicione atividades e resultados a qualquer meta para indicar seu progresso. Para obter informações sobre como adicionar atividades e resultados, consulte os seguintes artigos:

   * [Adicionar atividades às metas no Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
   * [Adicionar resultados às metas no Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Opcional) Remova o alinhamento entre duas metas ao considerar que não é mais relevante para a estratégia geral da organização. Para obter informações sobre como remover o alinhamento entre metas, consulte [Remover alinhamento de meta em Metas do Adobe Workfront](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

