---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: Visão geral das atribuições inteligentes
description: Ao gerenciar atribuições de tarefas e problemas, você pode usar atribuições inteligentes para identificar quem é o melhor usuário para concluir o trabalho. As atribuições inteligentes são sugestões que o Adobe Workfront apresenta ao atribuir itens de trabalho a recursos com base em um algoritmo que determina o recurso mais apropriado para o trabalho.
author: Alina
feature: Work Management
exl-id: 8d17eff6-5ff0-4985-b575-4934a3bb7c0b
source-git-commit: 412645a802bdf9057bb61a5a96df257daa1c3948
workflow-type: tm+mt
source-wordcount: '1255'
ht-degree: 0%

---

# Visão geral das atribuições inteligentes

<!--Audited: 07/2024-->

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">As informações destacadas nesta página se referem à funcionalidade disponível somente no ambiente de Produção para clientes que habilitaram versões rápidas.</span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview"> Essa funcionalidade será removida do ambiente de Produção para clientes que habilitaram a versão rápida com a versão 25.1 em janeiro de 2025. Para obter informações sobre a versão 25.1, consulte [Visão geral da versão do Primeiro Trimestre de 2025](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md).

Ao gerenciar atribuições de tarefas e problemas, você pode usar atribuições inteligentes para identificar quem é o melhor recurso para concluir o trabalho. As atribuições inteligentes são sugestões que o Adobe Workfront apresenta ao atribuir itens de trabalho a recursos com base em um algoritmo que determina o recurso mais apropriado para o trabalho. As atribuições inteligentes podem ser usuários, funções de trabalho ou equipes.

>[!NOTE]
>
>Ao sugerir usuários, as atribuições inteligentes não levam em conta a disponibilidade do usuário. No entanto, sua disponibilidade de acordo com seus agendamentos afeta as Datas Planejadas e Projetadas das tarefas e problemas quando são atribuídas. Para obter informações sobre agendamentos, consulte o artigo [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Este artigo contém informações gerais sobre atribuições inteligentes. Para obter informações sobre como usar atribuições inteligentes para atribuir tarefas e problemas a usuários, consulte [Fazer atribuições inteligentes](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md).

## Visão geral das atribuições inteligentes

Considere o seguinte ao trabalhar com atribuições inteligentes:

* <span class="preview">O algoritmo funciona independentemente para tarefas e problemas. Isso significa que a lista de usuários sugeridos para problemas pode ser diferente da lista de usuários sugeridos para uma tarefa, pois o Workfront cria as listas de acordo com critérios relacionados a problemas e tarefas separadamente. </span>
<!--not sure this is accurate: * Smart assignments do not recommend job roles or teams. Instead, they are suggestions of users who are best fit to complete a task or an issue. -->
* As atribuições sugeridas são sempre usuários ativos, funções de trabalho ou equipes.
* O recurso listado primeiro deve ser a melhor correspondência para a tarefa.

## Localizar sugestões de atribuição inteligente

Você pode ver as atribuições inteligentes nas seguintes áreas onde pode atribuir tarefas ou problemas:

* Uma lista de problemas ou um relatório na coluna Atribuições

  ![](assets/smart-assignments-issue-list.png)

* <span class="preview">Uma lista de tarefas ou um relatório na coluna Atribuições</span>

  ![](assets/smart-assignments-task-list.png)

* <span class="preview">Um cabeçalho de tarefa no campo Atribuições</span>

  ![](assets/smart-assignments-task-header-nwe-350x302.png)

* Um cabeçalho de problema no campo Atribuições

  ![](assets/smart-assignments-issue-header.png)

* O painel Resumo de tarefas ou problemas na área Atribuições

  ![](assets/issue-assignments-summary-panel.png)

* <span class="preview">O campo Atribuições na caixa Nova Tarefa, ao adicionar uma tarefa a um projeto</span>

  ![](assets/smart-assignments-new-task-modal.png)

<!--this is not possible in the new home  - we have Summary there: 
* The Assignments field for an item listed in the Home area, when you open a task or issue

  ![](assets/smart-assignments-in-home-nwe-350x216.png)
-->

* <span class="preview">Balanceador de carga de trabalho na área Atribuído a esta ao atribuir uma tarefa ou problema</span>

  ![](assets/smart-assignments-workload-balancer-bulk-assignments.png)


## Critérios de atribuições inteligentes

As atribuições inteligentes funcionam de forma diferente para tarefas e para problemas.

### Critérios de atribuições inteligentes para tarefas

O cálculo de atribuições inteligentes de tarefas funciona em <span class="preview">duas fases que usam dois algoritmos diferentes.</span>

<span class="preview">Dependendo de qual algoritmo encontrar a atribuição inteligente, as atribuições serão listadas em duas seções separadas no campo Atribuições.</span> Para obter informações, consulte [Fazer atribuições inteligentes](/help/quicksilver/manage-work/tasks/assign-tasks/make-smart-assignments.md).

![](assets/smart-assignments-task-list.png)

<div class="preview">

#### Primeira fase do cálculo de atribuição inteligente para tarefas

Na primeira fase do cálculo das atribuições inteligentes, o Workfront calcula uma pontuação de similaridade para cada atribuição.

>[!NOTE]
>
>A primeira fase do cálculo das atribuições inteligentes não se aplica às seguintes áreas de tarefa:
>
>* Atribuições em massa no Balanceador de carga de trabalho.
>* Placas conectadas nas placas.


O cálculo da pontuação de similaridade e a ordem na qual as atribuições são listadas consideram o seguinte:

* Uma pontuação de 100% é atribuída a uma atribuição existente na qual os nomes da tarefa, do projeto e do portfólio são idênticos à tarefa que você está tentando atribuir. Os nomes do projeto e do portfólio da tarefa de uma atribuição existente também devem corresponder ao projeto e ao portfólio da tarefa que você está tentando atribuir.

* Se apenas algumas dessas informações de outras atribuições corresponderem às tarefas existentes, a pontuação poderá ser inferior a 100%.

  Por exemplo, se você estiver atribuindo uma tarefa chamada &quot;Minha segunda tarefa&quot; em um projeto chamado &quot;Meu projeto&quot; em um portfólio chamado &quot;Meu portfólio&quot; e tiver uma tarefa existente chamada &quot;Minha tarefa&quot; em outro projeto chamado &quot;Meu projeto&quot; em um portfólio chamado &quot;Meu portfólio&quot;, o usuário atribuído a &quot;Minha tarefa&quot; poderá obter uma pontuação de 95%, pois o nome da tarefa existente e da tarefa que você está tentando atribuir agora são semelhantes, mas não idênticos.

  >[!TIP]
  >
  >  O Workfront procura correspondências somente nos campos Nome de tarefas, projetos e portfólios, e não em nenhum outro campo.

* Uma atribuição pode obter uma pontuação mais alta quando é atribuída a muitas tarefas no sistema que têm nomes semelhantes. Por exemplo, se uma equipe chamada &quot;Desenvolvimento&quot; for atribuída a 50% das tarefas no sistema que contém &quot;AI&quot; no nome e você estiver atribuindo outra tarefa com &quot;AI&quot; no nome, a pontuação da equipe de &quot;Desenvolvimento&quot; será maior. Nesse caso, os nomes dos projetos e portfólios não são tão importantes.

* Levando em conta esse sistema de pontuação, as primeiras 7 sugestões são listadas como atribuições inteligentes, na ordem decrescente de suas pontuações. Atribuições com pontuações inferiores a 40% não são exibidas.

* Se várias atribuições tiverem pontuações idênticas, elas serão exibidas na ordem da data em que foram feitas, a partir da data mais recente.

  Por exemplo, se Rick foi designado a uma tarefa semelhante hoje e Jennifer foi designada a uma tarefa semelhante dois dias atrás, Rick aparece primeiro.

* As atribuições identificadas nesta fase estão listadas no    Seção **Atribuições sugeridas** do campo Atribuições para tarefas.

* Se não houver correspondências usando esse cálculo, a segunda fase das atribuições inteligentes começa, que é calculada usando um algoritmo diferente.

</div>

#### Segunda fase do cálculo de atribuição inteligente para tarefas

Se a primeira etapa das atribuições inteligentes de tarefas não encontrar correspondências, o Workfront calcula as atribuições inteligentes para tarefas da mesma forma que as calcula para problemas.

Para obter mais informações, consulte a seção [Critérios de atribuições inteligentes para tarefas e problemas](#smart-assignments-criteria-for-tasks-and-issues) neste artigo.

As atribuições identificadas nesta fase estão listadas nas seções **Usuários e equipes**, **Atribuições de funções de trabalho** e <span class="preview">**Funções de cartão de taxa**</span> do campo Atribuições. <span class="preview">Para obter mais informações sobre cartões de taxa, consulte [Gerenciar cartões de taxa](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md)</span>. <!--keep the rate cards roles in yellow after the release of assignments to Prod-->

### Critérios de atribuições inteligentes para tarefas e problemas


>[!NOTE]
>
>Os critérios a seguir se aplicam às tarefas somente quando a primeira fase do cálculo de atribuição inteligente de tarefa não encontrou correspondências. Para obter informações, consulte a seção [Primeira fase do cálculo de atribuição inteligente para tarefas](#first-phase-of-smart-assignment-calculation-for-tasks) neste artigo. Os critérios a seguir sempre se aplicam a problemas, por padrão.

![](assets/smart-assignments-issue-header.png)

Os usuários são recomendados na lista suspensa atribuições inteligentes com base em uma combinação dos seguintes critérios (listados na ordem do mais importante para o menos importante):

1. Usuários atribuídos a outros itens de trabalho nos últimos 30 dias pelo usuário que fez a atribuição. Os primeiros 50 usuários que correspondem a esse critério são exibidos. O usuário atribuído com mais frequência é exibido primeiro.

2. Se o item de trabalho for atribuído a uma equipe ou função, a lista de usuários sugeridos será filtrada ainda mais levando em conta as atribuições existentes abaixo. Nesse caso, somente os seguintes usuários são exibidos na lista de sugestões:

   * Usuários cuja Equipe inicial é a equipe atribuída ao item de trabalho.
   * Usuários cuja função principal é a função atribuída ao item de trabalho.

>[!TIP]
>
>* Se não houver nenhuma função ou equipe atribuída na tarefa ou problema, o Workfront exibirá todos os usuários atribuídos nos últimos 30 dias, até 50 usuários.
>
>* Se você não tiver feito nenhuma atribuição nos últimos 30 dias, somente os usuários que pertencem à equipe atribuída ou têm a função atribuída ao item de trabalho serão exibidos na lista de atribuições inteligentes.



<!--the commented out piece in the tip above was live before but I am not totally sure that smart assignments look at your team. I think they look JUST at the team/ role assigned to the work item; see this help site request for more info: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/62fd222200037eb87572c5b6ad6bf53e/overview -->
<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h3>Smart assignments criteria for the Production environment</h3>
<p>(NOTE: drafted,this was the case BEFORE we updated the logic in the WB - with the 21.4 release)</p>
</div>
<p>Smart assignments display on tasks and issues when the following conditions are met:</p>
<ul>
<li>The task or issue is subordinate to a parent task or issue that has a user, team, or job role currently assigned. </li>
</ul>
<p>Smart assignments display the top twenty recommendations based on a proprietary algorithm that uses your own team information.</p>
<p>Users are recommended in the smart assignments drop-down list based on a combination of the following criteria (listed in order from most important to least important):</p>
<ul>
<li>The user has the team assigned to the task or issue designated as their Home Team</li>
<li>The user is also assigned to the parent task</li>
<li>The user has the same primary job role as is currently assigned to the task or issue</li>
<li>The user has the team assigned to the parent task or issue designated as their Home Team</li>
<li>The user is associated with the same primary job role currently assigned to the parent task</li>
<li>The user is a member of the same team as the user who assigned the task or issue and the team is designated as their Home Team</li>
<li>The user is a member of the same Home Group as the user who is assigning the task or issue</li>
<li>The user has the same primary job role as the user who is assigning the task or issue.</li>
</ul>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Make smart assignments</h2>
<p>(NOTE:&nbsp;this was moved to its own article: make-smart-assignments.) </p>
<p>Smart assignments are available in most locations where you can make assignments in Workfront.</p>
<p>You can use smart assignments on tasks and issues that have previously been assigned to a job role or a team.</p> <note type="note">
You must have a Plan or a Work license and have at least Contribute permissions to a task or an issue to be able to make assignments to the task or the issue. You must have the Make Assignments option enabled in your permission level to make assignments.
</note>
<p>To use smart assignments:</p>
<ol>
<li value="1">Navigate to an issue or a task and click one of the following fields to edit them: <br>
<ul>
<li><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">The <strong>Assignments</strong> field in the task or issue header</p></li>
<li>The <strong>Assignments</strong> field of a task or issue list using in-line editing in a task or issue list. </li>
<li>The <strong>Assignee</strong> field after you have clicked <strong>Advanced</strong> from a task or an issue. </li>
</ul></li>
<li value="2"> <p>Place your cursor in the assignment field, and wait for two seconds, then the <strong>Suggestions</strong> list is displayed.</p> <p>Users displayed in this list are the smart assignment suggestions for the task or the issue.<br></p> <p> <img src="assets/nwe-smart-assignment-suggestions-350x160.png" style="width: 350;height: 160;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3"> <p>Select the user in the recommendations list by clicking their name. </p> <p>If there are no suggestions, the suggestion list does not open.</p> </li>
<li value="4">(Optional) If you do not want to use one of the recommended users from the smart assignments list, start typing the name of the desired user and select the name when it appears in the list.</li>
<li value="5">Click <strong>Enter</strong> to make the assignment. </li>
</ol>
</div>
-->
