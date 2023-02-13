---
product-area: resource-management
navigation-topic: use-the-gantt-chart
title: Recursos de nível na  [!UICONTROL Gráfico de Gantt]
description: Informações sobre como nivelar recursos no Gráfico de Gantt.
author: Alina
feature: Work Management
exl-id: ba96c01d-03b8-4728-b5e3-b10d227f51b0
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: tm+mt
source-wordcount: '593'
ht-degree: 0%

---

# Recursos de nível na [!UICONTROL Gráfico de Gantt]

A alocação de recursos em um projeto tem dois objetivos:

* Para ajustar automaticamente a alocação excessiva de tempo para destinatários.
* Para criar automaticamente um agendamento de tarefa realista para um projeto.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>Qualquer Um </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] licença*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Acesso à [!UICONTROL Editar] para Projetos</p> <p><b>Nota</b>

Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Acesso ao projeto do [!UICONTROL Manager]</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Visão geral do nivelamento de recursos

Se o mesmo recurso for atribuído a duas tarefas diferentes, você poderá usar o nivelamento de recursos para ajustar a linha do tempo das tarefas, de modo que elas não ocorram ao mesmo tempo.

Considere o seguinte ao nivelar recursos em um projeto:

* O nivelamento de recursos se aplica somente a um projeto, portanto [!DNL Adobe Workfront] O não nivela recursos em mais de um projeto por vez.
* If **[!UICONTROL Esforço orientado]** é selecionado como um **[!UICONTROL Tipo de duração]**, [!DNL Workfront] não nivelará os recursos.
* Quando vários usuários são atribuídos à mesma tarefa, o nivelamento é cancelado.
* Condições para o tipo de **[!UICONTROL Restrição de tarefa]** terão precedência sobre o nivelamento dos recursos. Por exemplo, se **[!UICONTROL Datas fixas]** é selecionado como a variável [!UICONTROL Restrição de tarefa], o nivelamento de recursos não alterará as datas da tarefa.
* Os relacionamentos antecessores terão precedência sobre o nível de recursos.
* **[!UICONTROL Nivelamento de Recursos]** precisa ser definido como **[!UICONTROL Manual]** para o projeto, a fim de ajustar o nivelamento no [!UICONTROL Gráfico de Gantt]. Se você tiver permissões de gerenciamento no projeto, poderá ter o sistema automaticamente nivelando os recursos ajustando essa configuração no projeto e selecionando **[!UICONTROL Automático]** em vez de **[!UICONTROL Manual]** no **[!UICONTROL Editar projeto]** caixa.

   ![](assets/resource-leveling-mode-350x177.png)

* Como proprietário do projeto ou responsável pela tarefa, você pode introduzir um atraso de nivelamento para uma tarefa para indicar que há uma grande chance de a tarefa precisar de tempo extra. Para obter informações sobre como adicionar um atraso de nivelamento a uma tarefa, consulte [Atualizar Atraso de Nivelamento de Tarefa](../../../manage-work/tasks/task-information/task-leveling-delay.md).

## Aplicar o Nivelamento de Recursos na [!UICONTROL Gráfico de Gantt]

Você pode usar a Lista de tarefas [!UICONTROL Gráfico de Gantt] para nivelar seus recursos.

1. Vá para o projeto que deseja nivelar.
1. No **[!UICONTROL Tarefas]** clique no botão **[!UICONTROL Gráfico de Gantt]** ícone .

   Todas as alterações são salvas automaticamente quando a função **[!UICONTROL Salvar automaticamente]** está ativada. Está ativada por padrão.

1. (Opcional) Clique no botão **[!UICONTROL Plano] modo** e selecione **[!UICONTROL Salvar manualmente padrão]** ou **[!UICONTROL Planejamento de linha do tempo]** para salvar as alterações manualmente.

   >[!TIP]
   >
   >Não é possível nivelar recursos na variável  [!UICONTROL Gráfico de Gantt] quando a variável [!UICONTROL Salvar automaticamente] está ativada.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Clique no botão **[!UICONTROL Recursos de nível]** menu suspenso.

   ![Level_resources.png](assets/level-resouces.png)

1. Selecione uma das seguintes opções:

   * **[!UICONTROL Nível Agora]**: Aplica o nivelamento de recursos à tarefa selecionada.
   * **[!UICONTROL Limpar Nivelamento]**: Remove todo o nível de recursos da tarefa selecionada.

   >[!NOTE]
   >
   >Os recursos podem estar sobrealocados se forem atribuídos a várias tarefas que ocorrem durante o mesmo período.

1. (Opcional e condicional) Se tiver desativado a opção Salvar automaticamente, clique no botão **[!UICONTROL Desfazer]** ou &#x200B;**[!UICONTROL Refazer]** se desejar cancelar ou duplicar qualquer uma das alterações.

   >[!TIP]
   >
   >Você pode usar os seguintes atalhos de teclado para desfazer ou refazer as alterações no [!UICONTROL Gráfico de Gantt]:
   >
   >* [!DNL Mac]: Use [!UICONTROL Comando + Z] para desfazer e [!UICONTROL Comando + Shift + Z] para refazer.
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
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the <strong>More icon</strong> to the right of the task name, then click <strong>Edit</strong>. </p> <p> <img src="assets/qs-task-edit-icon-highlighted-350x154.png" style="width: 350;height: 154;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">Click <strong>Settings</strong>.<br></li>
<li value="4">Specify the <strong>Leveling Delay</strong>, in hours.<br>This is the time that the resource will be delayed starting the task due to resource conflicts.</li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
