---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Alinhar metas ao conectá-las às metas da Adobe Workfront
description: Se você for um colaborador individual com uma meta pessoal, talvez queira alinhá-la às metas da sua equipe para exibir efetivamente o progresso da sua própria meta no contexto maior da estratégia da sua organização.
author: Alina
feature: Workfront Goals
exl-id: 4276f1c9-2ee9-4f74-b011-ae1e19fefe35
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 0%

---

# Alinhar metas ao conectá-las às metas da Adobe Workfront


Se você for um colaborador individual com uma meta pessoal, talvez queira alinhá-la às metas da sua equipe para exibir efetivamente o progresso da sua própria meta no contexto maior da estratégia da sua organização.

Quando todos em sua organização têm suas metas alinhadas às metas de sua organização, eles podem ver claramente como suas contribuições individuais e esforços de equipe ajudam a fazer avançar a agulha em prioridades maiores de nível de empresa. Para obter mais informações sobre as práticas recomendadas para alinhar metas, consulte [Visão geral do alinhamento da meta em Metas da Adobe Workfront](../../workfront-goals/goal-alignment/goal-alignment-overview.md).

Há duas abordagens para conectar metas nas Metas da Adobe Workfront:

* Você pode criar alinhamento entre metas conectando metas umas às outras.

* Você pode alinhar manualmente duas metas ou pode converter resultados e atividades de uma meta existente em outra meta. O resultado ou atividade convertido se torna a meta secundária da meta original.

>[!IMPORTANT]
>
>Uma meta pode ter um total de 1000 indicadores de progresso.

Este artigo descreve como você pode alinhar metas conectando-as umas às outras. Para obter informações sobre como alinhar metas convertendo resultados e atividades em metas, consulte [Alinhar metas convertendo resultados e atividades em metas](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

## Requisitos de acesso

<!--drfated for the P&P release: 

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
   <td> <p>Editar o acesso às Metas</p> <p><b>Nota</b>

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

## Alinhar metas conectando-as umas às outras

<!--
Aligning goals by connecting them differs depending on what environment you use. 

### Align goals by connecting them in the Production environment

1. Create two goals that you want to align. For information about creating goals, see [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).
1. (Optional) Activate the goals that you want to align. You can align goals that have a Draft, Active, or Inactive status. For information about activating goals, see [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).
1. Go to the goal that you want to align (child goal) to another goal (parent goal) and click its name to open the **Goal Details** panel.

   For example, if you want Goal 2 to influence the progress of Goal 1, you must go to Goal 2. 

1. Click **Align to another goal** in the upper-right corner of the right panel.

   ![](assets/align-to-another-goal-link-highlighted-350x128.png)

1. Start typing the name of an existing goal or the name of an owner in the **Align to another goal** field, then select it when it appears in the list. Only goals that are from the same or future periods display in the list. 
1. Click **Save**.

   The goal you started with (Goal 2) is now the child goal of the goal you aligned it with (Goal 1).   
   The aligned goals display connected in the Goal Alignment section with Goal 2 as secondary to Goal 1.

   ![](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Optional) To view the goals in the Goal Alignment section, do one of the following:

   * Click the Goal Alignment section in the left panel and find the goals by applying the correct filter. For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).
   * Click the Goal List, Check-in, or Pulse sections in the left panel and find one of the goals, then click the **Alignment icon** ![](assets/align-icon.png) next to the goal name to go directly to the goal in the Goal Alignment section.

   For information about the Goal Alignment section, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md). 

1. (Optional) Add activities and results to either goal to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Optional) Remove the alignment between two goals, when you consider that no longer is relevant to your organization's overall strategy For information about removing alignment between goals, see [Remove goal alignment in Adobe Workfront Goals](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

-->
1. Crie duas metas que deseja alinhar. Para obter informações sobre como criar metas, consulte [Criar metas nas metas da Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).
1. (Opcional) Ative as metas que deseja alinhar. Você pode alinhar metas que tenham um status de Rascunho, Ativo ou Inativo. Para obter informações sobre como ativar metas, consulte [Ativar metas nas metas da Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).
1. Vá para a meta que deseja alinhar (meta secundária) a outra meta (meta principal) e clique em seu nome para abrir a página de meta.

   >[!INFO]
   >
   >Por exemplo, se você deseja que a Meta 2 influencie o progresso da Meta 1, você deve ir para a Meta 2.

1. Clique em **Detalhes da meta** no painel esquerdo.

1. No **Informações da meta principal** , clique em **Adicionar** no **Objetivo principal** se não houver uma meta principal,

   Ou

   Clique no nome da meta principal para escolher outra.

1. Comece a digitar o nome de uma meta existente no **Objetivo principal** e selecione-o quando aparecer na lista. Somente as metas que são do mesmo período ou de períodos futuros são exibidas na lista.

1. Clique em **Salvar alterações**.

   A meta com a qual você começou (Meta 2) agora é a meta secundária da meta principal com a qual você a alinhou (Meta 1).\
   As metas alinhadas são exibidas conectadas na seção Alinhamento da Meta com a Meta 2 como secundárias com a Meta 1.
A meta-filho é exibida na seção Indicadores de progresso da meta-pai à medida que seu progresso atualiza o progresso da meta-pai.

   ![](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Opcional) Para exibir as metas na seção Alinhamento da meta , vá para a área Metas do Workfront e clique no botão **Alinhamento da meta** no painel esquerdo. Para obter informações sobre a seção Alinhamento da meta , consulte [Navegar na seção Alinhamento da meta em Metas do Adobe Workfront](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).

1. (Opcional) Adicione atividades e resultados a qualquer meta para indicar seu progresso. Para obter informações sobre como adicionar atividades e resultados, consulte os seguintes artigos:

   * [Adicionar atividades às metas em Metas da Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
   * [Adicionar resultados às metas em Metas da Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Opcional) Remova o alinhamento entre duas metas, quando considerar que não é mais relevante para a estratégia geral de sua organização. Para obter informações sobre como remover o alinhamento entre as metas, consulte [Remova o alinhamento da meta nas Metas da Adobe Workfront](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

