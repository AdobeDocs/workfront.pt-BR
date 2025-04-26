---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Remover alinhamento de metas nas Metas do Adobe Workfront
description: Você pode remover o alinhamento entre duas metas se não fizer mais sentido conectá-las.
author: Alina
feature: Workfront Goals
exl-id: a6196356-ca11-4759-9cff-64850a60208e
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 2%

---

# Remover alinhamento de metas nas Metas do Adobe Workfront

<!--Audited P&P only: 4/2025-->

Você pode remover o alinhamento entre duas metas se não fizer mais sentido conectá-las.

Para obter informações sobre como alinhar metas, consulte os seguintes artigos:

* [Alinhar metas ao conectá-las às Metas do Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)
* [Alinhar metas convertendo resultados e atividades em metas](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md)

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
 <p>Licença atual: Solicitação ou superior</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produto*</td>
 <td>
   <p> Novo requisito de produto: Workfront</p>
   Ou
   <p>Requisito atual do produto: além de uma licença do Workfront, você deve comprar uma licença do Adobe Workfront Goals. </p> <p>Para obter informações, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para usar as Metas do Workfront</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Nível de acesso</td>
 <td> <p>Editar acesso às Metas</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Permissões de objeto</td>
 <td>
  <p>Exibir permissões ou mais altas para a meta para exibi-la</p>
  <p>Gerenciar permissões para a meta para editá-la</p>
  <p>Para obter informações sobre como compartilhar metas, consulte <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartilhar uma meta no Workfront Goals</a>. </p>
  </td>
 </tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclui a área Metas no Menu principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Você deve ter o seguinte antes de iniciar:

* Uma meta principal que tenha pelo menos uma meta secundária associada a ela. As metas secundárias são os indicadores de progresso da meta.

## Considerações sobre a remoção do alinhamento da meta

Considere o seguinte ao remover o alinhamento entre duas metas:

* A meta principal deve ter outra meta, atividade ou resultado associado para poder permanecer ativa.
* Não é possível remover uma meta secundária alinhada de uma meta principal se ela for o único indicador de progresso da meta principal.
* A meta secundária se torna uma meta independente ao remover seu alinhamento à meta principal.

## Remover alinhamento de metas

<!--
Removing goal alignment differs depending on which environment you use.

### Remove goal alignment in the Production environment


1. Go to a child goal aligned to a parent goal. 
1. Click the goal name to open the **Goal Details** panel. 
1. Click the **gear icon** ![Gear icon](assets/gear-icon-settings.png) next to the parent goal, then click **Remove alignment**.

   ![Reove alignment](assets/edit-remove-alignment-350x88.png)

   The goal becomes a standalone goal and its progress no longer influences the progress of the original parent goal. 

1. (Optional) Click **Undo** in the lower-left corner of the screen if you want to revert this change and keep the goals aligned. 
1. (Optional) Add activities and results to either goals to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)
-->

1. Acesse a área **Metas** no Workfront e clique no nome de uma meta para abrir a página da meta.
1. Na página da meta de uma meta principal, clique em **Indicadores de progresso** no painel esquerdo.

   ![REmover alinhamento da meta](assets/remove-goal-alignment-from-list-unshimmed.png)

1. No agrupamento **Tipo: Meta**, selecione uma meta e clique no ícone **Desconectar** ![Ícone Desconectar](assets/disconnect-goal-to-remove-alignment-icon-unshimmed.png) na parte superior da lista.

   A caixa Desconectar é exibida.

1. Clique em **Desconectar** para desconectar a meta selecionada de sua meta principal.

   A meta se torna uma meta independente e não é mais listada como um indicador de progresso da meta original. O progresso do objetivo desconectado não influencia mais o progresso do objetivo original.

   Uma mensagem de sucesso é exibida no canto superior direito da página para confirmar que a meta foi desconectada.
