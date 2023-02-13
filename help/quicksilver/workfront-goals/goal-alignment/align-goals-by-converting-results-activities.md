---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Alinhar metas convertendo resultados e atividades em metas
description: É possível alinhar manualmente duas metas ou converter os resultados e as atividades de uma meta existente em outra meta. O resultado ou atividade convertido se torna a meta secundária da meta original. Para obter informações sobre como alinhar manualmente duas metas, consulte Alinhar metas conectando-as nas Metas da Adobe Workfront.
author: Alina
feature: Workfront Goals
exl-id: 48371389-952c-4732-b519-9774cd4d1b93
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 0%

---

# Alinhar metas convertendo resultados e atividades em metas

É possível alinhar manualmente duas metas ou converter os resultados e as atividades de uma meta existente em outra meta. O resultado ou atividade convertido se torna a meta secundária da meta original.
Para obter informações sobre como alinhar manualmente duas metas, consulte [Alinhar metas ao conectá-las às metas da Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

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
* Uma meta existente com resultados e atividades existentes.

   Para obter informações sobre como criar metas, consulte [Criar metas nas metas da Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>Uma meta pode ter até 1000 indicadores de progresso.

<!--drafted for goal redesign: At PRODUCTION: update the sentence above to remove Production/ Preview references-->

## Considerações ao converter resultados e atividades em metas

Por vezes, um resultado ou uma atividade pode ter um âmbito superior ao previsto e faria mais sentido que se tornassem objetivos. Você pode converter resultados e atividades de uma meta existente em uma nova meta. Esta é uma abordagem ascendente para o alinhamento dos objetivos.

Considere o seguinte ao converter resultados e atividades em metas:

* O resultado ou atividade convertido se torna a meta secundária da meta original, e as duas metas se tornam alinhadas.
* A meta recém-criada torna-se o indicador de progresso único para a meta original, se não houver resultados ou atividades adicionais na meta original. Você deve adicionar resultados e atividades à meta-filho para poder acompanhar o progresso nela.
* A conversão de um resultado ou atividade em uma meta é irreversível. Após a conversão, a nova meta secundária nunca poderá se tornar um resultado ou atividade para a meta principal novamente.

## Converter um resultado ou atividade em uma meta

<!--
<span class="preview">Converting results and activities differs depending on what environment you use. </span>

### Convert a result or activity to a goal in the Production environment

1. Go to a goal that has a result or an activity that you want to convert to a goal.
1. Click the name of the goal to open the **Goal Details** panel.
1. Expand the **Results** or **Activities** right-pointing arrows to see a list of results or activities for the goal. 

1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result or activity name that you want to convert, then click **Convert into a Goal**.

   ![](assets/convert-to-goal-link-highlighted-350x191.png)

1. (Optional) Remove the name of the original activity or result owner from the **Goal Owner** field and replace it with another user, team, group, or your organization's name. By default, Workfront selects the owner of the result or the activity as the goal owner. 
1. Click **Convert**. The activity or result displays as an aligned goal in the Goal Details panel of the original goal and the original activity or result is removed from the original goal and transferred to the second goal. By default, the new goal has the same name as the original converted result or activity. 
1. (Optional) Click the name of the new goal to open the **Goal Details** panel and edit the name of the goal. For information about editing any information for an existing goal, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
-->

1. Vá para uma meta que tenha um resultado ou uma atividade que você deseja converter em uma meta.
1. Na página da meta, clique em **Indicadores de progresso** no painel esquerdo.
1. Selecione um resultado ou atividade na lista de indicadores de progresso e clique no botão **Converter em meta** ícone ![](assets/convert-to-goal-icon-unshimmed.png) na parte superior da lista de indicadores de progresso. A caixa Converter em meta é aberta.

   ![](assets/convert-to-goal-box-unshimmed.png)
1. Atualize as seguintes informações:
   * **Nome da meta**: Por padrão, a nova meta tem o mesmo nome do resultado ou atividade original.
   * **Período**: Por padrão, o período da nova meta é o trimestre atual. Você pode selecionar a variável **Ativar datas personalizadas** definição para definir um período de tempo personalizado para a nova meta.
   * **Proprietário da meta**: Por padrão, o novo proprietário da meta é o proprietário do resultado ou atividade original.
   * **Descrição**: Adicione mais informações sobre a nova meta.
1. Clique em **Salvar**

   O resultado ou atividade agora é convertido em uma meta secundária da meta original. Ele é listado como uma meta na lista de Indicadores de progresso da meta original.



