---
content-type: overview
product-area: projects
navigation-topic: update-work-in-a-project
title: Visão geral da data de confirmação
description: A Data de Confirmação é a data pela qual um usuário atribuído à tarefa ou um problema se compromete a concluir a tarefa ou o problema. Isso é diferente da Data de conclusão planejada, pois é uma estimativa mais realista da data de conclusão fornecida somente pelo usuário responsável pelo trabalho. Para obter informações sobre a Data de Conclusão Planejada, consulte Visão Geral da Data de Conclusão Planejada da tarefa.
author: Alina
feature: Work Management
exl-id: 47072433-bb8e-4210-947a-8bfa41ec47a9
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---

# Visão geral da data de confirmação

A Data de Confirmação é a data pela qual um usuário atribuído à tarefa ou um problema se compromete a concluir a tarefa ou o problema. Isso é diferente da Data de conclusão planejada, pois é uma estimativa mais realista da data de conclusão fornecida somente pelo usuário responsável pelo trabalho. Para obter informações sobre a Data de Conclusão Planejada, consulte [Visão geral da data de conclusão planejada da tarefa](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

## Visão geral da data de confirmação

Considere o seguinte ao trabalhar com datas de confirmação:

* Somente tarefas e problemas têm uma Data de confirmação.
* As datas de confirmação não são definidas automaticamente pelo Adobe Workfront.\
   Quando você cria uma tarefa ou um problema, não há uma data de confirmação atribuída à tarefa ou ao problema.
* Se você estiver atribuído a uma tarefa ou ocorrência, poderá definir a Data de confirmação executando um dos seguintes procedimentos:

   * Permita que o Workfront defina a Data da Confirmação para corresponder à Data de Conclusão Planejada existente da tarefa ou emissão clicando em Trabalhar nela, Iniciar Edição ou Iniciar Tarefa na tarefa ou emissão. Para obter informações sobre a substituição do botão Trabalho nele por um botão Iniciar, consulte  [Substitua o botão Trabalho nele por um botão Iniciar](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).
   * Configure manualmente a Data de confirmação por conta própria, de acordo com quando achar que a tarefa ou problema pode ser concluído. Essa é a estimativa e compromisso, como responsável, com o Gerenciador de projetos de que você terá a tarefa ou emissão concluída em uma data específica.

>[!NOTE]
>
>Você deve ser o Proprietário da Tarefa de uma tarefa para alterar a Data da Confirmação. Os usuários a seguir não podem alterar a Data de confirmação de uma tarefa:
>
>* Proprietário do projeto
>* Patrocinador do Projeto
>* Gerenciador de Recursos
>* Administrador de Sistema
>* Qualquer outro destinatário na tarefa
>* Qualquer outro usuário com permissões para a tarefa.
>
>Para obter mais informações sobre o Proprietário da Tarefa, consulte a seção [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) no artigo [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Notificações e atualizações acionadas pela alteração da Data de Confirmação {#notifications-and-updates-triggered-by-changing-the-commit-date}

Quando uma tarefa ou um destinatário de ocorrência seleciona uma Data de Confirmação diferente da Data de Conclusão Planejada definida pelo Proprietário do Projeto, há várias notificações e atualizações que alertam o Proprietário do Projeto e outros usuários dessa alteração.

>[!NOTE]
>
>As alterações feitas na Data da Confirmação não alteram automaticamente as datas planejadas, e as alterações feitas nas datas planejadas não alteram automaticamente a Data da Confirmação. 

Definir a data de confirmação para uma tarefa ou ocorrência aciona as seguintes alterações:

* A Data da confirmação é preenchida na Atualização do fluxo da tarefa ou problema.

   ![](assets/update-stream-confirmation-that-commit-date-changed-nwe-350x73.png)

   A alteração da Data da confirmação é exibida na área Atualizações da tarefa ou problema quando o administrador do Workfront ativa essa atualização na área Feeds de atualizações em Configurar. Para obter mais informações, consulte [Atualizações controladas pelo sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

* A Data de Conclusão Projetada da tarefa ou problema é definida como a mesma data, pois a tarefa agora tem uma indicação mais precisa de quando provavelmente será concluída.

   Para obter mais informações sobre a Data de Conclusão Projetada, consulte [Visão geral da data de conclusão projetada para projetos, tarefas e problemas](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

   ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

* O Proprietário do projeto é notificado na área de notificações e na guia Atualizações da tarefa se essa alteração afetará a linha do tempo do projeto.

   ![](assets/in-product-notification-commit-date-changed-nwe-350x149.png)

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tip below is actually wrong and the updates feeds should not control this setting, but at this time it does, according to this issue in Hub: https://hub.workfront.com/issue/61e1aa5e0002a186fdd0a73a10db0fc3/updates?email-source=comm</p>
  -->

   >[!TIP]
   A notificação de que a Data de confirmação foi alterada é enviada para o Proprietário do projeto somente quando o administrador do Workfront ativa a exibição da Data de confirmação na área Feeds de atualizações em Configurar. Para obter mais informações, consulte [Atualizações controladas pelo sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

   Se um Proprietário do projeto não quiser aceitar a alteração, recomendamos que ele faça um comentário ao usuário propondo uma nova data para solicitar que ele altere a Data da confirmação para a Data planejada original ou selecione uma nova data. Se um Proprietário do Projeto aceitar a alteração, ele poderá ajustar manualmente a Data de Conclusão Planejada para corresponder à Data de Confirmação oferecida pelo usuário atribuído ao item.

   O Proprietário do projeto pode usar a Data da confirmação para redefinir a Data de conclusão planejada. Para fazer isso, selecione a opção Set plan date to na guia Updates da tarefa. Você deve ter acesso para gerenciar a tarefa e o projeto para aceitar essa alteração.

   >[!NOTE]
   Se quiser ver como a linha do tempo do projeto é afetada pela aceitação para alterar a Data de conclusão planejada da tarefa, clique em **Linha do tempo do projeto**. Isso abre o Gráfico de Gantt, onde você pode avaliar as alterações de data.
   ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)  >

Para obter informações sobre a funcionalidade adicional que está disponível ao atualizar um item de trabalho, consulte  [Atualizar trabalho](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 

Para obter informações sobre como atualizar Datas da Confirmação para tarefas e problemas, consulte [Atualizar datas de confirmação em tarefas e problemas](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update Commit Dates on tasks and issues</h2>
<p>(NOTE:&nbsp;moved to its own article) </p>
<p>Updating the Commit Date is identical for tasks and issues.</p>
<ol>
<li value="1"> <p>Go to a task or issue that you are assigned to as the <strong>Task Owner</strong>.</p> <p>For more information about finding out who the Task Owner for an issue or task is, see the section <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments" class="MCXref xref">Edit tasks</a> in the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref">Edit tasks</a>.</p> </li>
<li value="2"> <p>Click Work on it in the task or issue header</p> <p>Or</p> <p>Click <strong>Start Task</strong> or <strong>Start Issue</strong> if the Work on it button has been customized in your environment to indicate that you are now working on the work item. </p> <p>At this time, the Commit Date and the Planned Completion Date of the task or issue are the same.</p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) If you clicked Start Task or Start Issue, click <strong>Undo</strong> in the lower-left corner of the screen. The Commit Date is removed. </p> <p>For information about replacing the Work On&nbsp;It button with a Start button, see <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a></span>.</p> <note type="tip">
The option to undo your selection to start your work is not available when you click
<span style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Work on it</span>.
</note> </li>
<li value="4"> <p> Expand the <strong>This will be done by</strong> date picker, and select a new Commit Date.</p>
<div>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Click <strong>Updates</strong> in the left panel, then click the <strong>Start a new update</strong>><strong>Commit Date</strong></p>
<p>Or</p>
<p>Click <strong>Task Details</strong> or <strong>Issue Details</strong> in the left panel, then double click&nbsp;<strong>Commit Date</strong> and select a new date from calendar. </p>
</div>
<p>The Commit Date and the Planned Completion date are no longer the same.</p>
<p>Instead, the Commit Date and the Projected Completion Date of the task or issue become the same.</p>
<p>The changes are saved automatically.</p>
<p>The Project Owner is notified that you have suggested a new Commit Date for the task or issue and can, at this time, update the Planned Completion Date of the task or issue to match the Commit Date you suggested. For information about the notifications and updates that are triggered by this change, see the section <a href="#notifications-and-updates-triggered-by-changing-the-commit-date" class="MCXref xref">Notifications and updates triggered by changing the Commit Date</a> in this article.</p>
</div> </li>
</ol>
</div>
-->
