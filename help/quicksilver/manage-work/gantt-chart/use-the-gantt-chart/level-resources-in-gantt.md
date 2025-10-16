---
product-area: resource-management
navigation-topic: use-the-gantt-chart
title: Nivelar Recursos no [!UICONTROL Gráfico de Gantt]
description: Se o mesmo recurso for atribuído a duas tarefas diferentes, você poderá usar o nivelamento de recursos para ajustar a linha do tempo das tarefas para que elas não ocorram ao mesmo tempo. Este artigo fornece informações sobre como nivelar recursos no Gráfico de Gantt.
author: Alina
feature: Work Management
exl-id: ba96c01d-03b8-4728-b5e3-b10d227f51b0
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# Nivelar Recursos no [!UICONTROL Gráfico de Gantt]

<!--Audited: 08/2025-->

Você pode usar o nivelamento de recursos para ajustar a linha do tempo das tarefas para que elas não ocorram ao mesmo tempo, caso os mesmos recursos sejam atribuídos a várias tarefas ao mesmo tempo.

O nivelamento de recursos em um projeto tem duas finalidades:

* Para ajustar automaticamente a alocação excessiva de tempo para os designados.
* Para criar automaticamente um cronograma de tarefas realista para um projeto.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] pacote</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] licença</td> 
   <td> <p>[!UICONTROL Padrão]</p>
   <p>[!UICONTROL Plano]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>[!UICONTROL Editar] acesso a Projetos</p></td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Acesso de [!UICONTROL Manage] ao projeto</p>
</td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++
<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>[!UICONTROL Edit] access to Projects</p> <p><b>NOTE</b>

If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] access to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table> -->

## Visão Geral do Nivelamento de Recursos

Se o mesmo recurso for atribuído a duas tarefas diferentes, você poderá usar o nivelamento de recursos para ajustar a linha do tempo das tarefas para que elas não ocorram ao mesmo tempo.

Considere o seguinte ao nivelar recursos em um projeto:

* O nivelamento de recursos se aplica somente a um projeto, portanto, o [!DNL Adobe Workfront] não nivela recursos em mais de um projeto de cada vez.
* Se **[!UICONTROL Orientado pelo Esforço]** estiver selecionado como um **[!UICONTROL Tipo de Duração]**, [!DNL Workfront] não nivelará os recursos.
* Quando vários usuários forem atribuídos à mesma tarefa, o nivelamento será cancelado.
* As condições para o tipo de **[!UICONTROL Restrição de Tarefa]** terão precedência sobre o nivelamento de recursos. Por exemplo, se **[!UICONTROL Datas Fixas]** estiver selecionado como a [!UICONTROL Restrição de Tarefa], o nivelamento de recursos não alterará as datas da tarefa.
* As relações predecessoras terão prioridade sobre o nivelamento de recursos.
* O **[!UICONTROL Nivelamento de Recursos]** precisa ser definido como **[!UICONTROL Manual]** para o projeto para ajustar o nivelamento no [!UICONTROL Gráfico de Gantt]. Se você tiver permissões Gerenciar para o projeto, poderá fazer com que o sistema nivele recursos automaticamente ajustando esta configuração no projeto e selecionando **[!UICONTROL Automático]** em vez de **[!UICONTROL Manual]** na caixa **[!UICONTROL Editar Projeto]**.

  ![Modo de nivelamento de recursos](assets/resource-leveling-mode-350x177.png)

* Como proprietário do projeto ou destinatário da tarefa, você pode introduzir um atraso de nivelamento para uma tarefa para indicar que há uma grande chance de a tarefa precisar de tempo extra. Para obter informações sobre como adicionar um atraso de nivelamento a uma tarefa, consulte [Atualizar Atraso de Nivelamento da tarefa](../../../manage-work/tasks/task-information/task-leveling-delay.md).

## Aplicar nivelamento de recursos no [!UICONTROL Gráfico de Gantt]

Você pode usar o [!UICONTROL Gráfico de Gantt] da Lista de Tarefas para nivelar seus recursos.

1. Vá para o projeto que deseja nivelar.
1. Na área **[!UICONTROL Tarefas]**, clique no ícone do **[!UICONTROL Gráfico de Gantt]**.

   Todas as alterações são salvas automaticamente quando a opção **[!UICONTROL Salvar automaticamente]** está habilitada. Esta opção está habilitada por padrão.

1. (Opcional) Clique no ícone do **[!UICONTROL Modo de plano]** e selecione **[!UICONTROL Salvar manualmente o padrão]** ou **[!UICONTROL Planejamento de linha do tempo]** para salvar as alterações manualmente.

   >[!TIP]
   >
   >Você não pode nivelar recursos no [!UICONTROL Gráfico de Gantt] quando a opção [!UICONTROL Salvamento automático] está habilitada.

   ![Configuração manual habilitada](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Clique no menu suspenso **[!UICONTROL Recursos de Nível]**.

   ![Level_resources.png](assets/level-resouces.png)

1. Selecione uma das seguintes opções:

   * **[!UICONTROL Nivelar Agora]**: aplica o nivelamento de recursos à tarefa selecionada.
   * **[!UICONTROL Limpar Nivelamento]**: remove todos os nivelamentos de recursos da tarefa selecionada.

   >[!NOTE]
   >
   >Seus recursos podem estar superalocados se forem atribuídos a várias tarefas que ocorrem durante o mesmo período.

1. (Opcional e condicional) Se você desabilitou a opção de Salvamento automático, clique nos ícones **[!UICONTROL Desfazer]** ou **[!UICONTROL Refazer]** se deseja cancelar ou duplicar qualquer uma das alterações.

   >[!TIP]
   >
   >Você pode usar os seguintes atalhos de teclado para desfazer ou refazer alterações no [!UICONTROL Gráfico de Gantt]:
   >
   >* [!DNL Mac]: Use [!UICONTROL Command + Z] para desfazer e [!UICONTROL Command + Shift + Z] para refazer.
   >* Windows: Use [!UICONTROL Ctrl + Z] para desfazer e [!UICONTROL Ctrl + Y] para refazer.


1. Clique em **[!UICONTROL Salvar]** no canto superior direito do [!UICONTROL Gráfico de Gantt].

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Overview of Leveling Delay</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article: /Content/Manage work/Tasks/Task information/task-leveling-delay.htm) </p>
<p>At times, there might be conflicts between task schedules on a project. You can level resources or address resource conflicts by rescheduling resources and tasks so that all tasks can be completed within a realistic schedule. </p>
<p>As the project manager, or the task assignee, you can also add a Leveling Delay on individual tasks to account for any resource or scheduling conflicts. In other words, a task might be scheduled with a delay to ensure that when Adobe Workfront levels the tasks a more realistic schedule overcomes resource conflicts.</p>
<p>To manually add a Leveling Delay to a task:</p>
<ol>
<li value="1">Navigate to a task for which you want to add a Leveling Delay.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the <strong>More icon</strong> to the right of the task name, then click <strong>Edit</strong>. </p>  </li>
<li value="3">Click <strong>Settings</strong>.<br></li>
<li value="4">Specify the <strong>Leveling Delay</strong>, in hours.<br>This is the time that the resource will be delayed starting the task due to resource conflicts.</li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
