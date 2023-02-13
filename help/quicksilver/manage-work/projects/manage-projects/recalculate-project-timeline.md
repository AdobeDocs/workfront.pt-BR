---
product-area: projects
navigation-topic: manage-projects
title: Recalcular linhas do tempo do projeto
description: Recalcular Linhas do Tempo permite que os gerentes vejam como diferentes fatores relacionados ao projeto estão afetando a linha do tempo do projeto. A linha do tempo de um projeto refere-se às datas planejadas e projetadas.
author: Alina
feature: Work Management
exl-id: ec5d9a07-e45a-4aa2-9f41-9421ca5d5920
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '1017'
ht-degree: 0%

---

# Recalcular linhas do tempo do projeto

Recalcular Linhas do Tempo permite que os gerentes vejam como diferentes fatores relacionados ao projeto estão afetando a linha do tempo do projeto. A linha do tempo de um projeto refere-se às datas planejadas e projetadas.

Fazer alterações em agendamentos, tempo limite de pessoal e outros itens fora do escopo de um projeto não afeta a linha do tempo do projeto imediatamente. A linha do tempo do projeto é afetada quando a linha do tempo é recalculada. As influências externas não entrarão em vigor no projeto até que o recálculo ocorra.

Este artigo descreve as maneiras pelas quais o recálculo da linha do tempo acontece.

## Requisitos de acesso

<!--drafted for P&P: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>System administrator to recalculate timeline for all projects in the system</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
O recálculo automático da linha do tempo acontece sem acesso especial para qualquer um dos usuários envolvidos no trabalho no projeto.

No entanto, você deve ter o seguinte acesso para recalcular manualmente a linha do tempo de um projeto:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos</p> <p>Administrador do sistema para recalcular a linha do tempo de todos os projetos no sistema</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Recálculo automático

Por padrão, as linhas do tempo do projeto são automaticamente recalculadas diariamente quando o escopo do projeto é alterado ou todas as noites. O administrador do Workfront determina se as linhas do tempo devem ser calculadas automaticamente todas as noites ou com cada alteração de escopo gerenciando as configurações de Linhas do tempo na área Preferências do projeto da Configuração. Para obter mais informações, consulte [Configurar recálculos de linha do tempo para projetos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

>[!NOTE]
>
>Se a linha do tempo de um projeto for superior a 15 anos, o recálculo automático será desativado para esse projeto. Você só pode selecionar um Tipo de Atualização do Manual para um projeto com mais de 15 anos. Se você alterar as datas do projeto para menos de 15 anos, será necessário recalcular manualmente a linha do tempo uma vez antes de ela ser calculada automaticamente.

* [Recálculo automático de linhas do tempo do projeto](#automatic-recalculation-of-project-timelines)
* [Ações que acionam um recálculo automático de linhas do tempo do projeto](#actions-that-trigger-an-automatic-recalculation-of-project-timelines)

### Recálculo automático de linhas do tempo do projeto {#automatic-recalculation-of-project-timelines}

O Adobe Workfront recalcula as linhas do tempo diariamente apenas para projetos em que todas as condições a seguir são atendidas:

* Ter um status de Atual
* O Tipo de Atualização do projeto é definido como Automático ou Automático e On Change

   Para obter informações sobre o tipo de Tipo de Atualização do projeto, consulte [Visão geral do Tipo de atualização do projeto](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

* Ter uma última data de atualização nos últimos três meses\
   O administrador do Workfront pode alterar essa funcionalidade padrão, conforme descrito em [Configurar recálculos de linha do tempo para projetos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

* A última data de cálculo da linha do tempo do projeto não está no dia de calendário atual. Isso significa que a última data de cálculo da linha do tempo do projeto é antes de 00:00 do dia atual.

Você pode configurar a frequência com que a linha do tempo do seu projeto é atualizada. Quando a linha do tempo do projeto é atualizada, ela é recalculada com base nas alterações feitas no projeto.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
or changes made to another project that the timeline is dependent on
</MadCap:conditionalText>
-->


<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: above, the last part is drafted because of this: I don't think this is right because we told people that in the case of cross-project predecessors, the timeline must be calculated manually for the successor to see the updates in the predecessor's project. Drafting for now.)</p>
-->

Para obter mais informações, consulte [Selecione o Tipo de Atualização do projeto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;content moved to the article linked above)</p>
<p>You can configure how the timeline for your project is updated:</p>
<ol>
<li value="1">Go to the project for which you want to configure how the timeline is updated.</li>
<li value="2"> <p>  Click the <strong>More</strong> icon <img src="assets/more-icon.png"> to the right of the project name, then click&nbsp; <strong>Edit</strong>. </p> <p>The <strong>Edit Project</strong> dialog box is displayed.</p> </li>
<li value="3"> <p>Click<strong>Settings.</strong><br><img src="assets/screen-shot-2013-09-18-at-10.36.16-am-350x347.png" alt="" style="width: 350;height: 347;"></p> </li>
<li value="4">In the <strong>Update Type</strong> drop-down list, select from the following options:<br><strong>- Automatic and On Change:</strong> (Default setting) The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on. The project timeline is also updated each night. <br>This is the recommended setting for this field because it ensures that the project timeline is always up to date.<br>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed.
<div>
<p><img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"></p>
</div><br>This indicates that the recalculation is not yet finished, and the dates are subject to change. <br><strong>- Change Only:</strong> The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur.<br>You might want to select this option if changes rarely occur in the project or in other projects that the timeline is dependent on.<br><strong>- Automatic Only:</strong> The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if many changes occur each day in the project or in other projects that the timeline is dependent on.<br><note type="note">
A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
</note><br><strong>- Manual Only:</strong> The project timeline is updated only when you select the option to Recalculate Timelines, as described in <a href="#manual-recalculation" class="MCXref xref">Manual recalculation</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).<br>For more information about the project Update Type, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a><note type="note">
If the timeline of a project is longer than 15 years, the automatic recalculation is disabled. If you change the dates on the project to less than 15 years, you must manually recalculate your timeline one time before it is calculated automatically.
</note></li>
<li value="5">Click <strong>Save Changes.</strong></li>
</ol>
</div>
-->

### Ações que acionam um recálculo automático de linhas do tempo do projeto {#actions-that-trigger-an-automatic-recalculation-of-project-timelines}

Várias alterações de escopo na vida de um projeto recalcular automaticamente a linha do tempo do projeto, incluindo as seguintes ações:

* Atualizando o status da tarefa.
* Movimentação de uma tarefa para um projeto diferente.
* Atualizando a Data Planejada ou as Datas de Conclusão Planejadas das tarefas.
* Atualizar o Tipo de Duração, a Restrição de Tarefa ou o número de destinatários nas tarefas.
* Atualizando relações do antecessor da tarefa.
* Adicionar uma aprovação a uma tarefa que também adicione tempo à Data de conclusão planejada da tarefa.\
   Para obter mais informações sobre configurações de aprovação, consulte [Definir configurações de aprovação global](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

## Recálculo manual {#manual-recalculation}

Como proprietário do projeto, você pode recalcular manualmente as linhas do tempo de projetos individuais. O administrador do Workfront pode recalcular manualmente todas as linhas do tempo no Workfront.

* [Recalcular linhas do tempo de projetos individuais ou em massa](#recalculate-timelines-for-individual-projects-or-in-bulk)
* [Recalcular manualmente as linhas do tempo em massa na caixa Editar projetos](#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box)
* [Recalcular linhas do tempo para todos os projetos no sistema (somente administradores do Workfront)](#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only)

### Recalcular linhas do tempo de projetos individuais ou em massa {#recalculate-timelines-for-individual-projects-or-in-bulk}

Você pode recalcular a linha do tempo de um projeto no Workfront a partir da página do projeto ou de uma lista de projetos ou relatório.

1. Vá para o projeto para o qual deseja recalcular a linha do tempo e clique no link **Mais** ícone ![](assets/qs-more-menu.png) à esquerda do nome do projeto

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   Ou

   Vá para uma lista de projetos ou relatório, selecione um ou vários projetos e clique no botão **Mais** ícone ![](assets/qs-more-menu.png) na parte superior da lista.

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >Dependendo da complexidade de seus projetos, recomendamos não selecionar um grande número de projetos ao recalcular suas linhas do tempo em massa para garantir desempenho ideal. Algumas coisas que podem tornar um projeto muito complexo podem ser várias dependências ou atribuições, ou um grande número de campos personalizados.

1. Clique em **Recalcular Linha do Tempo**.

   Depois que a linha do tempo é recalculada, você vê uma mensagem indicando que o recálculo foi bem-sucedido.

   >[!TIP]
   >
   >Antes de concluir o recálculo da linha do tempo, algumas datas planejadas ou projetadas podem ser exibidas como esmaecidas. Isso significa que o recálculo ainda não foi concluído e que as datas estão sujeitas a alterações.

### Recalcular manualmente as linhas do tempo em massa na caixa Editar projetos {#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box}

Você pode recalcular manualmente as linhas do tempo de vários projetos editando-os em massa.

>[!TIP]
>
>Dependendo da complexidade de seus projetos, recomendamos não selecionar um grande número de projetos ao editá-los em massa para garantir um desempenho ideal. Algumas coisas que podem tornar um projeto muito complexo podem ser várias dependências ou atribuições ou um grande número de campos personalizados.

1. Acesse uma lista de projetos.
1. Selecione vários projetos na lista e clique em **Editar**.
1. Clique em **Configurações**, em seguida selecione **Recalcular Linhas do Tempo**.

1. Clique em **Salvar alterações**.

### Recalcular linhas do tempo para todos os projetos no sistema (somente administradores do Workfront) {#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only}

Os administradores do Workfront podem executar o diagnóstico Recalcular linha do tempo para recalcular imediatamente todas as linhas do tempo no sistema Workfront. Isso permite que todos os Gerentes de projeto vejam a influência das alterações externas imediatamente nas datas planejadas e projetadas.

Para obter mais informações sobre o recálculo de linhas do tempo para todo o site do Workfront, consulte a seção &quot;Recalcular linhas do tempo para toda a instância do Workfront&quot; em [Configurar recálculos de linha do tempo para projetos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Project Update Types</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and moved to thisa rticle: /Content/Manage work/Projects/Planning a Project/project-update-type-overview.htm)</p>
<p>For information about how to update the project's Update Type, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>. </p> <note type="important">
If the timeline of a project is longer than 15 years, Workfront does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual.
</note>
<p>You can select how each project calculates its timeline by choosing between the following Update Types:</p> <note type="important">
If the timeline of a project is longer than 15 years, Workfront does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual.
</note>
<ul>
<li> <p><strong>Automatic and On Change:</strong>&nbsp;This is the default setting. The project timeline is updated each time a change occurs&nbsp;in the project or in another project that the timeline is dependent on. The project timeline is also updated each night.&nbsp; <br>This is the recommended setting as it ensures that the project timeline is always up to date.</p> <p>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed. </p> <p> <img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"> </p> <p>This indicates that the recalculation is not yet finished, and the dates are subject to change. </p> </li>
<li><strong>Change Only:</strong>&nbsp;The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur. <br>You might want to select this option if you are concerned about system performance and if&nbsp;changes rarely occur in the project or in other projects that the timeline is dependent on.</li>
<li> <p><strong>Automatic Only:</strong>&nbsp;The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if you are concerned about system performance and if many changes occur each day in the project or in other projects that the timeline is dependent on.</p> <note type="note">
A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
</note> </li>
<li><strong>Manual Only:</strong>&nbsp;The project timeline is updated only&nbsp;when you select the option to <strong>Recalculate Timelines</strong>, as described in the section "Manual Recalculation" in&nbsp;the article <a href="#" class="MCXref xref selected">Recalculate project timelines</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).</li>
</ul>
</div>
-->
