---
product-area: projects
navigation-topic: convert-issues
title: Visão geral da conversão de problemas no Adobe Workfront
description: Se for necessário trabalhar mais para concluir um problema depois que ele for enviado, você pode converter o problema em um projeto ou em uma tarefa.
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 97c83b65-208b-4e3f-b4cc-681237d82aa3
source-git-commit: 36bdacb5f6d04245552aeeb4ab82d210597645a2
workflow-type: tm+mt
source-wordcount: '1441'
ht-degree: 2%

---

# Visão geral da conversão de problemas no Adobe Workfront

Se for necessário trabalhar mais para concluir um problema depois que ele for enviado, você pode converter o problema em um projeto ou em uma tarefa.

Para obter informações sobre como converter problemas em tarefas, consulte [Converter um problema em uma tarefa no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-task.md).

Para obter informações sobre como converter problemas em projetos, consulte [Converter um problema em um projeto no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## Considerações ao converter problemas

* Ao converter problemas em tarefas ou projetos, a maioria das informações do problema é transferida para a tarefa ou projeto, a menos que especificado de outra forma neste artigo.
* O administrador do Workfront ou do grupo já definiu as preferências para o que acontece com um problema, sua resolução e o acesso do contato principal quando ele é convertido em um projeto ou uma tarefa, conforme descrito em [Configurar preferências de tarefas e problemas em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
* O Workfront remove todas as aprovações associadas a problemas durante a conversão.
* O Workfront substitui o Objeto de resolução do problema ao convertê-lo em uma tarefa ou em um projeto. A nova tarefa ou problema se torna o novo Objeto de resolução do problema após a conversão.
* Considere o seguinte:

   * Durante a conversão, você pode ser perguntado se deseja manter o problema e sua resolução vinculados ao projeto ou tarefa que está sendo criada.
   * Se você manter o problema, o status e o percentual concluído do projeto ou da tarefa atualizarão automaticamente o status e o percentual concluído do problema quando ocorrerem alterações no projeto, na tarefa ou no problema, ou quando a Workfront recalcular a linha do tempo.

* Ao converter um problema em uma tarefa ou um projeto, o problema é removido da área da página inicial do usuário atribuído ao problema.

* Ao converter um problema, as permissões para os problemas originais não são transferidas para o objeto convertido (tarefa ou projeto).

* Ao converter um problema em um projeto usando um modelo, a maioria das informações do modelo é transferida para o novo projeto. No entanto, algumas informações do problema também podem ser transferidas para o novo projeto. Para obter mais informações, consulte [Visão geral dos campos do projeto ao converter um problema em um projeto usando um modelo](#overview-of-project-fields-when-converting-an-issue-to-a-project-using-a-template) neste artigo.
* Ao converter um problema, nem todos os documentos ou suas informações são movidos para o novo objeto para o qual o problema é convertido. Os seguintes itens são incluídos quando você converte um problema que tem documentos ou links de documento anexados:

   * Documento
   * Links de documento para serviços de terceiros, como Google Drive ou SharePoint.
   * Versões
   * Provas são incluídas somente quando a opção **Conservar o problema original e vincular a sua resolução a esta tarefa** está desmarcada.
   * As aprovações de documentos não são incluídas ao converter um problema que tenha documentos e links de documentos anexados.

* Se você decidir manter o problema na conversão e ele tiver documentos anexados, o documento e suas versões serão copiados para o projeto ou para a tarefa. As provas e as aprovações de documentos não são copiadas para o projeto ou para a tarefa.
* Se você decidir não manter o problema na conversão e ele tiver documentos anexados, o documento, suas versões e as provas serão transferidos para o projeto ou a tarefa. As aprovações de documentos não serão transferidas para o projeto ou a tarefa.
* Se você tiver documentos e pastas vinculados ao problema original de serviços de terceiros, como o Google Drive, independentemente de você estar mantendo o problema ou não durante a conversão, esses links serão copiados para o novo objeto.
* Comentários de problemas também são copiados para a tarefa ou projeto convertidos a partir do problema, mas os usuários marcados não serão transferidos.
* Se você quiser transferir informações de formulário personalizadas do problema para o projeto ou tarefa para o qual está convertendo, verifique se você tem um formulário personalizado de projeto ou tarefa que inclua os mesmos campos que deseja transferir do problema. Para obter mais informações, consulte [Transferir dados de formulário personalizados ao converter um objeto](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md).

## Visão geral dos campos do projeto ao converter um problema em um projeto usando um modelo {#overview-of-project-fields-when-converting-an-issue-to-a-project-using-a-template}

Ao converter um problema em um projeto, você pode convertê-lo em um projeto em branco ou usar um modelo.

Para obter informações, consulte [Converter um problema em um projeto no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

Ao usar um modelo, alguns campos preenchidos no modelo são transferidos para o projeto criado a partir do problema convertido. Outros campos são transferidos para o projeto a partir do problema convertido.

A tabela a seguir lista as informações do projeto e se ele é transferido do modelo ou da ocorrência:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Descrição</td> 
   <td> <p>A Descrição do problema é transferida para o novo projeto. </p> <p> Se não houver descrição do problema, a Descrição do modelo será transferida para o projeto. </p> <p>Se o campo Descrição estiver vazio para o problema e para o modelo, o campo estará vazio no projeto. </p> </td> 
  </tr> 
  <tr> 
   <td>Status</td> 
   <td>Status padrão selecionado para o grupo no modelo. Se o modelo não estiver associado ao grupo, o status do projeto será definido como o status padrão definido pelo administrador do Workfront na área Preferências do projeto da Configuração. Para obter informações, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto em todo o sistema</a>.</td> 
  </tr> 
  <tr> 
   <td>Prioridade</td> 
   <td><p>Transferências da ocorrência.</p>
   <p>Ao usar um modelo para o projeto convertido, você tem a opção de alterar manualmente a Prioridade. Se você optar por não alterá-la, a prioridade do problema será transferida para o projeto. 
    </td> 
  </tr> 
  <tr> 
   <td>URL</td> 
   <td> <p>O URL do problema é transferido para o novo projeto. </p> <p> Se não houver um URL especificado no problema, o URL do modelo será transferido para o projeto. </p> <p>Se o campo URL estiver vazio para o problema e para o modelo, o campo estará vazio no projeto. </p> </td> 
  </tr> 
  <tr> 
   <td>Tipo de Condição do Projeto</td> 
   <td>Transferências do modelo.</td> 
  </tr> 
  <tr> 
   <td>Condição do projeto</td> 
   <td>Corresponde à preferência padrão em nível de sistema, conforme determinado pelo administrador do Workfront na área Configuração. Para obter informações, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref">Definir uma condição personalizada como padrão para projetos</a></td> 
  </tr> 
  <tr> 
   <td>Cronograma de</td> 
   <td>Transferências do modelo.</td> 
  </tr> 
  <tr> 
   <td>Datas do projeto</td> 
   <td> 
    <ul> 
     <li> <p><b>Data de Início Planejada</b>: O horário de trabalho mais próximo com base no horário de trabalho do agendamento do modelo deve ser pré-selecionado, de acordo com o fuso horário do agendamento do modelo. Este campo ficará desativado se o campo Agendar de estiver definido como Conclusão de. </p> </li> 
     <li> <p><b>Data de Término Planejada</b>: O horário de trabalho mais próximo com base no horário de trabalho do agendamento do modelo deve ser pré-selecionado, de acordo com o fuso horário do agendamento do modelo. Este campo estará desativado se o campo Agendar de estiver definido como Do início. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Portfólio</td> 
   <td>Transferências do modelo. Caso contrário, esse campo estará vazio.</td> 
  </tr> 
  <tr> 
   <td>Programa</td> 
   <td>Transferências do modelo. Caso contrário, esse campo estará vazio.</td> 
  </tr> 
  <tr> 
   <td>Grupo</td> 
   <td><p> Existem os seguintes cenários:</p>
     <ul><li>Se um grupo for especificado durante a conversão, ele será o grupo do projeto</li>
     <li>Se você converter em um projeto usando um modelo e houver um grupo no modelo e, durante a conversão, não especificar um grupo, o grupo do modelo se tornará o grupo do novo projeto</li>
      <li> Se não houver um grupo no modelo e você não especificar um grupo durante a conversão, o grupo do projeto original do problema se tornará o grupo do novo projeto</li> </ul>
      </td> 
  </tr> 
  <tr> 
   <td>Empresa</td>    
   <td>  Transferências do modelo. Caso contrário, esse campo estará vazio.</td>

</tr> 
  <tr> 
   <td>Proprietário do projeto</td> 
   <td>Transferências do campo Proprietário do modelo no modelo. Caso contrário, será definido como o usuário conectado que está executando a conversão. </td> 
  </tr> 
  <tr> 
   <td>Patrocinador do Projeto</td> 
   <td>Transferências do campo Patrocinador do modelo no modelo. Caso contrário, esse campo estará vazio.</td> 
  </tr> 
  <tr> 
   <td>Gerenciador de Recursos</td> 
   <td>Transferências do modelo. Caso contrário, esse campo estará vazio.</td> 
  </tr> 
  <tr> 
   <td>Configurações da tarefa</td> 
   <td>Transferir a partir do modelo.</td> 
  </tr> 
  <tr> 
   <td>Configurações do problema</td> 
   <td>Transferir a partir do modelo. </td> 
  </tr> 
  <tr> 
   <td>Acesso</td> 
   <td> <p>Transferências da seção Acesso no modelo. </p> </td> 
  </tr> 
  <tr> 
   <td>Aprovações</td> 
   <td>Transferir a partir do modelo. As aprovações associadas ao problema são removidas durante a conversão. </td> 
  </tr> 
 </tbody> 
</table>

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Convert an issue to a project</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article)</p>
-->
<!--
<ol>
<li value="1"> Click the <strong>Issues</strong> icon on a project. </li>
<li value="2"> <p>Click the issue to be converted to access the issue.</p> </li>
<li value="3"> <p> Click the <strong>More</strong> menu, then click <strong>Convert to Project</strong>. </p>  </li>
<li value="4"> <p>In the submenu that displays, do one of the following:</p>
<ul>
<li>Click <strong>New Project</strong></li>
<li>Under <strong>New from Template</strong>, click the name of a project template you want to use</li>
</ul> </li>
<li value="5"> <p>Specify a name for the project.</p> <p>The default name is the name of the issue you are converting.</p> </li>
<li value="6">(Optional and conditional) If you are creating this project from a template, update the available fields in the Convert to Project box.<br>For more information about editing fields on projects, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
<li value="7"> <p>(Optional and conditional) Under <strong>Options</strong>, select any of the available options:</p>
<ul>
<li> <p><strong>Keep the original issue and tie its resolution to the this project</strong>When deselected, the original issue is deleted.</p> <note type="note">
<p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p>
<ul>
<li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li>
<li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a> </p> </li>
</ul>
</note> </li>
<li><strong>Allow <User Name> to have access to this project</strong>If unselected, the user who entered the issue has no access to the new task.</li>
</ul> <note type="note">
<div>
<p>The options that are available here depend on how the Workfront administrator has configured them for everyone in the system or for your group. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p>
<p>Or, if the top-level groups in your organization configured them separately, the options available here depend on which group you selected for the new project in step 6. For more information, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md" class="MCXref xref">Configure task and issue preferences for a group</a><span class="preview">.</span></p>
</div>
</note> </li>
<li value="8">(Optional) In the <strong>Custom Forms</strong> section, attach any custom forms.<br>For more information about transferring information from the custom form of the issue to that of the new project, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md" class="MCXref xref">Transfer custom form data when converting an object</a>.</li>
<li value="9"> <p>Click <strong>Save Changes.</strong></p> <p> <img src="assets/qs-issue-convert-to-project-before-saving-ui-350x366.png" style="width: 350;height: 366;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> <p>The issue is now a project, if you decided to delete the original issue.<br>Or<br>The issue is now linked to the new project and it will complete when the project completes, if you decided to keep the original issue. </p> <p>Some issue fields transfer to the project. For information, see the <a href="#view-original-issue-information-on-projects-and-tasks" class="MCXref xref">View original issue information on projects and tasks</a> section in this article. </p> </li>
<li value="10"> <p>(Optional) Set any further project details ​(project owner, project dates) and tasks as necessary.</p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Convert an issue to a task</h2> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article)</p>
-->
<!--
<ol>
<li value="1"> Click the Issues icon on a project.  </li>
<li value="2"> <p>Click the issue you want to convert to go to the issue's landing page. </p> </li>
<li value="3"> <p> Click the <strong>More</strong> menu on the issue, then <strong>Convert to Task</strong>.  </p>  </li>
<li value="4"> <p>Name the task.</p> </li>
<li value="5"> <p>Identify the project where the task will reside. </p> <p>You can select a different project from the project that the issue is on.</p> </li>
<li value="6"> <p>In the <strong>Project</strong> box, start typing the name of the project where you want to put the new task, then press <strong>Enter</strong> when it appears.</p> <p>By default, this box the name of the project containing the issue that you are converting.</p> </li>
<li value="7"> <p>(Optional and conditional) Under <strong>Options</strong>, select any of the following options. </p> <p>The Workfront administrator or group administrator must enable these preferences before they are visible during the conversion of issues: </p>
<ul>
<li> <p><strong>Keep the original issue and tie its resolution to the this task</strong> </p> <p>If unselected, the original issue is deleted.</p> <note type="note">
<p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p>
<ul>
<li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li>
<li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a> </p> </li>
</ul>
</note> </li>
<li> <p><strong>Allow <User Name> to have access to this task</strong> </p> <p>If unselected, the user who entered the issue has no access to the new task.</p> </li>
<li> <p><strong>Keep the planned completion date of the issue</strong> </p> <p>If unselected, the Planned Completion Date of the new task is calculated from the Planned Start Date of the task. The Planned Start Date of the new task is set according to the system preferences for new tasks.</p> </li>
</ul> <note type="note">
<div>
<p>The options that display here depend on how the Workfront administrator configured them for everyone in the system. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p>
<p>Or, if the top-level groups in your organization configured them separately, the options that display here depend on which group is associated with the project you selected in step 6. For more information, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md" class="MCXref xref">Configure task and issue preferences for a group</a>.</p>
</div>
</note> </li>
<li value="8">(Optional) Attach custom forms.<br>For more information about transferring information from the custom form of the issue to that of the new task, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md" class="MCXref xref">Transfer custom form data when converting an object</a>.<br><p><img src="assets/qs-issue-convert-to-task-before-saving-ui-350x367.png" style="width: 350;height: 367;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></p></li>
<li value="9"> <p>Click <strong>Save Changes</strong> when all task settings are set.</p> <p>The issue is now a task on the designated project, if you decided to delete the original issue.</p> <p>Or</p> <p>The issue is now linked to the new task on the project you chose, and it will complete once the task completes, if you decided to keep the original issue.</p> <p>Some issue fields transfer to the task. For information, see the <a href="#view-original-issue-information-on-projects-and-tasks" class="MCXref xref">View original issue information on projects and tasks</a> section in this article. <br></p> </li>
<li value="10"> <p>(Optional) Continue editing the task (assignments, dates) as necessary. </p> </li>
</ol>
</div>
-->

## Exibir informações de problemas originais em projetos e tarefas {#view-original-issue-information-on-projects-and-tasks}

Você pode exibir as informações do problema original em listas de projetos e tarefas e relatórios ou na área Detalhes do Projeto. Para obter informações sobre a criação de relatórios, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

A tabela a seguir ilustra quais campos de problemas estão visíveis nas tarefas e nos projetos convertidos.

| Campos de problema | Campo de projeto ou tarefa | Lista ou relatório de projetos | Área Detalhes do projeto | Lista de tarefas ou relatório | Área Detalhes da tarefa |
|---|---|---|---|---|---|
| Nome do Problema | Nome do problema convertido | ✔ | ✔ | ✔ | ✔ |
| Contato Primário | Nome do originador do problema convertido | ✔ | `✔` | ✔ |  |
| Data de Entrada | Data de entrada do problema convertido | ✔ |  | ✔ |  |


>[!CAUTION]
>
>Se o contato primário de um problema mudar ou se o problema se tornar desvinculado do projeto ou da tarefa depois que o problema for convertido, o nome do originador do problema convertido não será atualizado e exibirá o contato primário original do problema no momento em que ele foi convertido.
