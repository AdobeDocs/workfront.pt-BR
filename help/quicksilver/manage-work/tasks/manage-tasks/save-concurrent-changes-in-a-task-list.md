---
product-area: projects
navigation-topic: manage-tasks
title: Visão geral de salvar alterações simultâneas em uma lista de tarefas
description: Ao editar tarefas em uma lista, você pode usar configurações de salvamento separadas para indicar se deseja que as alterações sejam salvas automaticamente em manualmente ao editar tarefas em uma lista.
author: Alina
feature: Work Management
exl-id: dff52425-4711-40a8-8f40-205d75c506ef
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Visão geral de salvar alterações simultâneas em uma lista de tarefas

Ao editar tarefas em uma lista, você pode usar configurações de salvamento separadas para indicar se deseja que as alterações sejam salvas automaticamente em manualmente ao editar tarefas em uma lista.

Para obter informações sobre como editar tarefas em uma lista de tarefas, consulte o artigo [Editar tarefas em uma lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

Às vezes, conflitos podem aparecer se dois usuários estiverem fazendo alterações nas mesmas tarefas.

Considere o seguinte ao editar tarefas em uma lista de tarefas:

* O Adobe Workfront salva as alterações feitas nas tarefas imediatamente quando você seleciona salvar as alterações automaticamente se o Tipo de atualização do projeto for Automático ou Automático ou On Change. Para obter informações sobre o Tipo de Atualização do projeto, consulte [Selecione o Tipo de Atualização do projeto](../../../manage-work/projects/manage-projects/select-project-update-type.md).
* O Workfront atualiza as informações na lista em que você está trabalhando a cada minuto com alterações que outros usuários podem fazer em qualquer outro lugar do sistema. Isso garante que você sempre obtenha as informações mais recentes sobre as tarefas.

Os seguintes cenários existem quando vários usuários estão editando as mesmas tarefas:

* **Um usuário salva as alterações em uma lista de tarefas automaticamente e outro manualmente**: Se um usuário (Usuário A) salvar as alterações manualmente enquanto o Usuário B estiver editando as mesmas tarefas, mas estiver salvando as alterações automaticamente, as alterações em tempo real feitas pelo Usuário B serão atualizadas na lista do Usuário A a cada minuto. Se houver conflitos entre as alterações feitas pelos dois usuários, o usuário salvando manualmente (Usuário A) vê uma mensagem de aviso antes de poder salvar suas alterações. A mensagem de aviso mostra os itens que têm as alterações em conflito. No momento, o Usuário A pode escolher se deve manter as alterações (o que substitui as alterações feitas pelo Usuário B) ou descartá-las (o que mantém as alterações feitas pelo Usuário B).

>[!NOTE]
>
>Quando você opta por descartar as alterações feitas, isso se aplica a todas as alterações e não apenas àquelas que estão em conflito com as edições feitas por outro usuário.

* **Vários usuários estão salvando as alterações em uma lista de tarefas manualmente**: Se vários usuários que estão fazendo alterações em tarefas em uma lista estiverem salvando manualmente ao mesmo tempo, o Workfront salvará as alterações feitas pelo usuário que salva primeiro. Salvar essas alterações não deve encontrar conflitos. Em seguida, o Workfront compara as alterações feitas por todos os outros usuários com as informações que já foram salvas e exibe um aviso sobre as alterações conflitantes para os outros usuários antes que eles possam salvar suas informações.

>[!IMPORTANT]
>
>Ao optar por manter as alterações em todas as outras alterações, todas as alterações são salvas, a menos que as tarefas que você realizou sejam excluídas por outro usuário. Nesse caso, a mensagem de aviso informa que as alterações feitas nas tarefas excluídas são perdidas.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
<p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted - when replaced with the above live section; does it need an edit??) </p>
<div>
<p>When editing tasks in a list, you can select whether you want each change to be saved automatically or if you want to manually save multiple changes at one time by clicking the Save button. This depends on whether you enable the Autosave setting in the task list or not. </p>
<p>For information about editing tasks in a task list, see the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref" xrefformat="{para}">Edit tasks</a>. </p>
<p>Sometimes, conflicts might appear if two users are making changes on the same tasks. </p>
<p>Consider the following when editing tasks in a task list: </p>
<ul>
<li>Workfront saves the changes you make to tasks immediately when you have enabled the Autosave setting. </li>
<li>Workfront updates the information on the list you are working on every minute with changes that other users might make anywhere else in the system. This ensures that you always get the latest information on the tasks. </li>
</ul>
<p>The following scenarios exist when multiple users are editing the same tasks:</p>
<ul>
<li>One user has Autosave disabled and another has it enabled: If a user (User A) has disabled the Autosave setting and is editing the task list while User B is editing the same tasks but they have enabled the Autosave setting, the live changes made by User B are updated on the list for User A every minute. If there are conflicts between the changes made by the two users, the user with the Autosave setting disabled (User A) sees a warning message before they can save their changes, that shows the items that have those conflicting changes. At this time, User A can choose whether they should keep their changes (which overwrites the changes made by User B), or discard them (which keeps the changes made by User B.) </li>
</ul> <note type="note">
When you select to discard the changes you made, this applies to all the changes and not just to those that have conflicts with the edits made by another user.
</note>
<ul>
<li>Several users have disabled the Autosave setting: If several users that have disabled the Autosave setting are making changes at the same time, Workfront saves the changes made by the user who saves first. Saving these changes should not encounter any conflicts. Workfrontthen compares the changes made by all the other users with the information that it already saved and displays a warning about the conflicting changes to the other users before they can save their information. </li>
</ul> <note type="important">
When you select to keep your changes over all other changes, your changes are saved, unless the tasks you made changes to were deleted by another user. In this case, the warning message informs you that the changes you made to the deleted tasks are lost.
</note>
</div>
</div>
-->
