---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Visão geral da atribuição de trabalho no Balanceador de carga de trabalho
description: Como gerenciador de recursos, você pode usar o Balanceador de carga de trabalho do Adobe Workfront para exibir itens de trabalho que ainda não foram atribuídos aos usuários, bem como atribuir esses itens a eles.
author: Alina
feature: Resource Management
exl-id: 98779b67-b975-4501-8426-63e255b1d7df
source-git-commit: 8420f65e84edd42204d91aa503ff0b95153a1e67
workflow-type: tm+mt
source-wordcount: '1027'
ht-degree: 0%

---

# Visão geral da atribuição de trabalho no Balanceador de carga de trabalho

Como gerenciador de recursos, você pode usar o Balanceador de carga de trabalho do Adobe Workfront para exibir itens de trabalho que ainda não foram atribuídos aos usuários, bem como atribuir esses itens a eles.

Para obter informações gerais sobre o Balanceador de carga de trabalho, consulte [Visão geral do Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

É possível atribuir itens de trabalho (tarefas e problemas) a usuários em outras áreas do Workfront. No entanto, usando o Balanceador de carga de trabalho, é possível entender facilmente a disponibilidade dos usuários e visualizar claramente todos os outros itens aos quais eles estão atribuídos antes de atribuir mais trabalho.

Para obter informações sobre como atribuir itens de trabalho em outras áreas do Workfront, consulte os seguintes artigos:

* [Atribuir tarefas](../../manage-work/tasks/assign-tasks/assign-tasks.md)
* [Atribuir problemas](../../manage-work/issues/manage-issues/assign-issues.md)

## Disponibilidade do usuário no Balanceador de carga de trabalho

Você pode atribuir trabalho no Balanceador de carga de trabalho para corresponder ao tempo disponível dos usuários. Para garantir que você atribua a quantidade certa de trabalho e não superaloque o usuário, o total de Horas planejadas dos itens de trabalho atribuídos ao usuário deve corresponder às alocações diárias ou semanais do usuário.

Você deve entender como o Workfront calcula o tempo disponível para um usuário.

O Workfront usa as seguintes informações para calcular a capacidade do usuário no Balanceador de carga de trabalho:

* As Preferências De Gerenciamento De Recursos. O administrador do Workfront determina como o tempo disponível é calculado para o sistema, selecionando para usar um dos seguintes itens na área Gerenciamento de recursos em Configuração:

   * O cronograma padrão do sistema Workfront e o FTE do usuário.
   * A programação do usuário, conforme indicado na área Perfil do usuário.

      Isso calcula a disponibilidade diária e semanal do usuário. Quaisquer exceções de agendamento no agendamento selecionado são refletidas na capacidade do usuário no Balanceador de carga de trabalho.
   Para obter mais informações, consulte [Configurar preferências de gerenciamento de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

   Para obter informações sobre programações, consulte [Criar um agendamento](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

* A folga do usuário. Isso indica quais dias o usuário planeja decolar.

   Para obter mais informações, consulte [Configurar o tempo de folga pessoal no Adobe Workfront](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

* O Horário Comercial do usuário. Isso indica a porcentagem de tempo FTE em que o usuário está disponível para executar o trabalho real relacionado ao projeto, sem incluir as despesas gerais. Defina o valor de Tempo de trabalho como 1 para indicar que o usuário está disponível para trabalho relacionado ao projeto em todo o equivalente de tempo integral.


## Atribuir trabalho no Balanceador de carga de trabalho

Você pode atribuir itens de trabalho que ainda não foram atribuídos a um usuário ou reatribuir itens que foram atribuídos a usuários no Balanceador de carga de trabalho.

Você pode atribuir trabalhos no Balanceador de carga de trabalho das seguintes maneiras:

* Um item de cada vez, atribuindo manualmente cada item.

   Você pode fazer atribuições avançadas ao atribuir itens manualmente, uma de cada vez.

   Para obter mais informações, consulte [Atribuir trabalho manualmente usando o Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

* Um item de cada vez, arrastando e soltando itens de trabalho para o usuário que precisa ser atribuído.

   Para obter mais informações, consulte [Atribuir trabalho no Balanceador de carga de trabalho arrastando e soltando](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md).

* Vários itens de cada vez, usando a opção Atribuições em massa. Você pode definir regras pelas quais os itens são atribuídos a vários usuários de cada vez.

   Para obter mais informações, consulte [Atribuir trabalho em massa usando o Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

Para obter informações sobre o cancelamento da atribuição de trabalho, consulte [Cancelar atribuição de trabalho no Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

## Áreas de atribuição no Balanceador de carga de trabalho

Você pode atribuir trabalho aos usuários usando o Balanceador de carga de trabalho na área Recursos, no projeto ou no nível da equipe. Para obter mais informações sobre onde o Balanceador de carga de trabalho está localizado no Workfront, consulte [Localize o Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

Há duas áreas no Balanceador de carga de trabalho em que você pode exibir itens de trabalho:

* **Trabalho não atribuído**: exibe itens que não estão atribuídos aos usuários.
* **Trabalho atribuído**: exibe itens atribuídos aos usuários.

A tabela a seguir descreve quais itens são exibidos em cada área com base em suas atribuições:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Tipo de atribuição</strong> </td> 
   <td colspan="2"><strong>Áreas em que as atribuições são visíveis</strong> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td>Trabalho Não Atribuído </td> 
   <td>Trabalho atribuído </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span style="font-weight: normal;">Item não atribuído</span> </td> 
   <td><span>✔</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Equipe</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span data-mc-edit-date="2020-04-08T15:57:40.7175506-04:00" data-mc-editor="alinawilson" data-mc-comment="Drafted because role only is not displayed; first it will be displayed in Unassigned - 20.2 beta" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2019-11-15T13:24:04.5189150-05:00">Função</span> </td> 
   <td><span>✔</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Função e equipe</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Usuário</td> 
   <td> </td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Usuário e equipe</td> 
   <td> <p> </p> </td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Usuário, Função e Equipe</td> 
   <td>✔*</td> 
   <td>✔**</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Usuário e Função</p> </td> 
   <td><span data-mc-edit-date="2019-11-15T13:37:42.5435254-05:00" data-mc-editor="alinawilson" data-mc-comment="drafted because it's not in the Unassigned" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2019-11-15T13:37:33.3097484-05:00">✔</span>*</td> 
   <td>✔**</td> 
  </tr> 
 </tbody> 
</table>

&#42;Quando um item de trabalho é atribuído a um usuário e a uma função, ele é exibido na área Trabalho não atribuído somente quando a função é o Destinatário principal.

&#42;&#42;Quando um item de trabalho é atribuído a um usuário e a outra entidade, ele é exibido na área Trabalho atribuído somente quando o usuário é o Destinatário principal.

Para obter mais informações sobre as áreas Não atribuído e atribuído do Balanceador de carga de trabalho, consulte [Navegar pelo Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Considerações para várias atribuições para funções de trabalho, equipes e usuários

Considere o seguinte ao atribuir vários recursos a um item de trabalho:

* Os usuários podem ter mais de uma função de trabalho associada ao seu perfil. Para obter informações sobre como associar usuários a funções de trabalho, consulte [Editar o perfil de um usuário](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Geralmente, tarefas ou problemas são atribuídos primeiro a uma ou várias funções de trabalho ou a uma equipe. Quando os projetos estiverem prontos para serem iniciados, talvez também seja necessário atribuí-los aos usuários.\
   Se uma tarefa ou um problema for atribuído a uma ou várias funções e você também atribuir um usuário, o Adobe Workfront decide qual função de trabalho deve ser associada ao usuário adicional (se houver) de acordo com as seguintes regras:

   * Se houver apenas uma função de trabalho atribuída e ela corresponder à função principal do usuário, a tarefa ou o problema será atribuído apenas ao usuário que desempenha sua função principal.
   * Se houver várias funções atribuídas e pelo menos uma das funções corresponder às funções secundárias do usuário, a tarefa ou o problema será atribuído ao usuário que desempenha uma de suas Outras funções — que o Workfront seleciona aleatoriamente se houver várias correspondências — bem como quaisquer funções adicionais atribuídas.
   * Se houver uma ou mais funções de trabalho atribuídas e não houver correspondência entre as funções do usuário, a tarefa ou o problema será atribuído à função ou às funções, bem como ao usuário.

* Se uma tarefa ou um problema for atribuído a uma equipe e você também atribuir um usuário, a tarefa ou o problema permanecerá atribuído à equipe e ao usuário.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2 data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Manually assign one item at a time</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Moved manual assignment and drag-and-drop to their own articles) </p>
<ol>
<li value="1">Go to the Workload Balancer.</li>
<li value="2"> <p>Go to the <strong>Unassigned Work</strong> area and apply a filter to view work items</p> <p>Or</p> <p>Go to the <strong>Assigned Work</strong> area and expand the name of a user to view the work items assigned to them.</p> <note type="important">
<span>You cannot view and assign issues from the Unassigned Work area. You can only reassign issues already assigned to users in the Assigned Work area. Otherwise,</span> you can assign issues from a list or at the issue level. For information, see
<a href="../../manage-work/issues/manage-issues/assign-issues.md" class="MCXref xref">Assign issues</a>.
</note> </li>
<li value="3"> <p>Click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> on the bar of a work item, then click <strong>Assign this to</strong>. </p> <p> <img src="assets/workload-balancer-assign-this-to-link-from-task-350x117.png" style="width: 350;height: 117;"> </p> <note type="tip">
<p><span>You can also use the following shortcuts to assign tasks or issues:</span> </p>
<ul>
<li><span>In Windows: CTRL+click the task or issue bar.</span> </li>
<li><span>In&nbsp;Mac: CMD+click the task or issue bar.</span> </li>
</ul>
</note> </li>
<li value="4"> <p>Start typing the name of a user, job role, or team that you want to assign to the item in the <strong>Search people, role or teams</strong> field, select it when it displays in the list, then click&nbsp;<strong>Save</strong>. </p> <p> <img src="assets/assignments-box-wb.png"> </p> <p>This assigns or reassigns the work item to the specified assignees.</p> <p>If you assign an item to just a team or a job role, the item displays only in the Unassigned Work area. You must assign work items to users in order to display them in the Assigned Work area of the Workload Balancer.</p> <note type="tip">
<p>You can assign multiple users or job roles, and you can assign only one team. <span>You can assign only active users, <span>job roles</span>, and teams.</span></p>
<p><span>If a user, <span>job role</span>, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:</span> </p>
<ul>
<li> <p><span>Reassign the work item to active resources.</span> </p> </li>
<li> <p><span>Associate the users in a deactivated team with an active team and reassign the work item to the active team.</span> </p> </li>
</ul>
</note> </li>
<li value="5"> <p>(Optional) Click the <strong>Show allocations icon</strong> <img src="assets/show-allocations-icon-small.png">, then click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> > <strong>Edit allocations</strong>.</p> <p>Or</p> <p>Double-click a daily or weekly allocation to modify the amount of time the user is allocated to the work item.</p> <p>For information about modifying user allocations in the Workload Balancer, see the "Modify user allocations"&nbsp;section in the article <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>.</p> </li>
</ol>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<h2>Assign an item by dragging and dropping</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider retitling this to "Assign one item at a time by dragging and dropping" when bulk assignments will come???)&nbsp;</p>
<p>You can assign an item from the Unassigned Work area to a user, or you can reassign an already assigned item to another user in the Assigned Work area.</p>
<ol>
<li value="1">Go to the Workload Balancer.</li>
<li value="2"> <p>Go to the <strong>Unassigned Work</strong> area and apply a filter to view work items.</p> <note type="important">
<span>You cannot view and assign issues from the Unassigned Work area.</span>
</note> </li>
<li value="3"> <p>Click the bar of a work item that indicates either the planned or the projected timeline and drag it over the name of a user in the <strong>Assigned</strong> area.</p> <p>The user you hover over to drop the work item to is highlighted.</p> <note type="tip">
The Planned Hours for the user you're hovering over update in real time with the number of daily Planned Hours from the work item, to indicate what the impact of adding a new item might be to their overall allocation.
</note> <p> <img src="assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png" style="width: 350;height: 152;"> </p> </li>
<li value="4"> <p>When you are ready, drop the selected work item in the same line as the user's name in the Assigned Area. The item is assigned and the allocated Planned Hours are updated for the user with the new hours from the work item.</p> <note type="tip">
<p>If you enabled Group by Project in the Settings area, the assigned task displays under the corresponding project. If the setting is disabled, the assigned task displays in the user area. </p>
<p>The item displays according to the Workload Balancer criteria for sorting work items.&nbsp;For more information, see <a href="../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navigate the Workload Balancer</a>.</p>
</note> </li>
<li value="5"> <p>(Optional) Click the <strong>Show allocations icon</strong> <img src="assets/show-allocations-icon-small.png">, then click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> > <strong>Edit allocations</strong>. (NOTE: make sure these are still called this, and that the icon has not changed)</p> <p>Or</p> <p>Double-click a daily or weekly allocation to modify the amount of time the user is allocated to the work item.</p> <p>For information about modifying user allocations in the Workload Balancer, see the "Modify user allocations"&nbsp;section in the article <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>.</p> </li>
</ol> 
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Assign items in bulk</h2>
<p>(NOTE: This is also a separate article. Should we keep this section or the separate article?) </p>
</div>
<p>&nbsp;</p>
</div>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Unassign work items in the Workload Balancer</h2>
<p>(NOTE: moved this section to a new article. Draft here at release to preview) </p>
<p>You can either unassign items from users and move them to the Unassigned Work area, or reassign them to other users. </p>
<p>To unassign work items from users: </p>
<ol>
<li value="1">In the Workload Balancer, go to the <strong>Assigned Work</strong> area and expand a user.</li>
<li value="2">Do 
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
one of
</MadCap:conditionalText>
the following:
<ul>
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Find the item you want to unassign in a user's area, click it, drag and drop it in the Unassigned area or in another user's area. </p></li>
<li><p>Click the <strong>More</strong> icon <img src="assets/more-icon-task-list.png"> to the right of the name of a work item, click&nbsp;<strong>Assign this to</strong> , then remove the name of the entities assigned to the work item or enter another name and click&nbsp;<strong>Save</strong>.</p><p><img src="assets/workload-balancer-assign-this-to-link-from-task-350x117.png" style="width: 350;height: 117;"></p></li>
</ul><p>The item displays in the Unassigned Work area if it matches the filtering criteria for that area and it is not assigned to any users or it displays in the user area if it is assigned to that user. </p><note type="tip">
Unassigned issues do not display in the Unassigned area.
</note><p>For information about filtering information in the Workload Balancer, see <a href="../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md" class="MCXref xref">Manage filters in the Workload Balancer</a>. </p></li>
</ol>
</div>
-->
