---
product-area: projects
navigation-topic: manage-projects
title: Recalcular Linhas de Tempo do Projeto
description: Recalcular as linhas do tempo permite que os gerentes vejam como diferentes fatores relacionados ao projeto estão afetando a linha do tempo do projeto. A linha do tempo de um projeto se refere às datas planejadas e projetadas.
author: Alina
feature: Work Management
exl-id: ec5d9a07-e45a-4aa2-9f41-9421ca5d5920
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1066'
ht-degree: 2%

---

# Recalcular linhas do tempo do projeto

<!--Audited: 06/2025-->

Recalcular as linhas do tempo permite que os gerentes vejam como diferentes fatores relacionados ao projeto estão afetando a linha do tempo do projeto. A linha do tempo de um projeto se refere às datas planejadas e projetadas.

Fazer alterações em cronogramas, folga da equipe e outros itens fora do escopo de um projeto não afeta a linha do tempo do projeto imediatamente. A linha do tempo do projeto é afetada quando a linha do tempo é recalculada. As influências externas não entrarão em vigor no projeto até que o recálculo ocorra.

Este artigo descreve as maneiras como ocorre o recálculo da linha do tempo.

O recálculo automático da linha do tempo ocorre sem acesso especial para qualquer um dos usuários envolvidos no trabalho no projeto. Além disso, é possível recalcular manualmente a linha do tempo.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Padrão</p> 
    <p>Plano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a projetos</p> <p>O administrador do sistema deve recalcular a linha de tempo de todos os projetos no sistema</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um projeto</p>  </td> 
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
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Standard </p> 
    <p>Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> <p>System administrator to recalculate timeline for all projects in the system</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Recálculo automático

Por padrão, as linhas do tempo do projeto são recalculadas automaticamente diariamente quando o escopo do projeto é alterado ou todas as noites. O administrador do Workfront determina se as linhas do tempo devem ser calculadas automaticamente todas as noites ou com cada alteração de escopo gerenciando as configurações de Linhas do Tempo na área Preferências do projeto da Configuração. Para obter mais informações, consulte [Configurar recálculos de linha de tempo para projetos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

>[!IMPORTANT]
>
>* Se a linha do tempo de um projeto tiver mais de 15 anos, o recálculo automático será desativado para esse projeto e você só poderá selecionar um tipo de atualização Manual. Se você alterar as datas no projeto para menos de 15 anos, será necessário recalcular manualmente a linha do tempo uma vez antes de calculá-la automaticamente.
>* Para os ambientes Pré-visualização e Atualização personalizada da Sandbox, o recálculo noturno é desativado e as linhas de tempo do projeto não são recalculadas automaticamente. Você deve recalcular manualmente a linha do tempo do projeto para os ambientes Pré-visualização e Atualização personalizada da sandbox.
>* Se um projeto for complexo, o recálculo automático da linha do tempo talvez não ocorra.
> Um exemplo de um projeto complexo pode ser um projeto com várias dependências, grande número de tarefas, vários predecessores entre projetos ou vários recuos de tarefas.
> O Workfront coloca um aviso à direita do nome do projeto na página do projeto para avisar aos usuários que a linha do tempo do projeto deve ser recalculada manualmente. Somente os usuários com permissões para Gerenciar o projeto podem recalcular manualmente a linha do tempo.
>
>   ![](assets/project-warning-to-manually-recalculate-timeline.png)
>

* [Recálculo automático das linhas de tempo do projeto](#automatic-recalculation-of-project-timelines)
* [Ações que acionam um recálculo automático de linhas de tempo do projeto](#actions-that-trigger-an-automatic-recalculation-of-project-timelines)



### Recálculo automático de linhas de tempo do projeto {#automatic-recalculation-of-project-timelines}

O Workfront recalcula as linhas do tempo diariamente somente para projetos em que todas as condições a seguir sejam atendidas:

* Têm um status Atual.
* O tipo de atualização do projeto está definido como Automático ou Automático e Mediante alteração.

  Para obter informações, consulte [Visão geral do Tipo de Atualização de Projeto](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

* Ter uma data de última atualização nos últimos 3 meses. Um administrador do Workfront pode alterar essa funcionalidade padrão. Para obter mais informações, consulte [Configurar recálculos de linha de tempo para projetos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

* A data do último cálculo da linha do tempo do projeto não está dentro do dia atual do calendário. Isso significa que a última data de cálculo da linha de tempo do projeto é anterior a 00:00 do dia atual.

Você pode configurar a frequência com que a linha do tempo do seu projeto é atualizada. Quando a linha do tempo do projeto é atualizada, ela é recalculada com base nas alterações feitas no projeto.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
or changes made to another project that the timeline is dependent on
</MadCap:conditionalText>
-->


<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: above, the last part is drafted because of this: I don't think this is right because we told people that in the case of cross-project predecessors, the timeline must be calculated manually for the successor to see the updates in the predecessor's project. Drafting for now.)</p>
-->

Para obter informações, consulte [Selecionar o Tipo de Atualização do projeto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: content moved to the article linked above)</p>
<p>You can configure how the timeline for your project is updated:</p>
<ol>
<li value="1">Go to the project for which you want to configure how the timeline is updated.</li>
<li value="2"> <p>  Click the <strong>More</strong> icon <img src="assets/more-icon.png"> to the right of the project name, then click  <strong>Edit</strong>. </p> <p>The <strong>Edit Project</strong> dialog box is displayed.</p> </li>
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

### Ações que acionam um recálculo automático de linhas de tempo do projeto {#actions-that-trigger-an-automatic-recalculation-of-project-timelines}

Várias alterações de escopo na vida útil de um projeto recalculam automaticamente a linha do tempo do projeto, incluindo as seguintes ações:

* Atualizando status da tarefa.
* Mover uma tarefa para um projeto diferente.
* Atualizando a Data Planejada ou as Datas de Conclusão Planejadas das tarefas.
* Atualizar o Tipo de Duração, a Restrição de Tarefa ou o número de atribuídos nas tarefas.
* Atualizando relações de predecessoras da tarefa.
* Adicionar uma aprovação a uma tarefa que também adicione horas à Data de conclusão planejada da tarefa.\
  Para obter mais informações sobre configurações de aprovação, consulte [Definir configurações de aprovação globais](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

## Recálculo manual {#manual-recalculation}

Como proprietário de um projeto, você pode recalcular manualmente as linhas do tempo de projetos individuais. O administrador do Workfront pode recalcular manualmente todas as linhas do tempo no Workfront.

* [Recalcular linhas do tempo para projetos individuais ou em massa](#recalculate-timelines-for-individual-projects-or-in-bulk)
* [Recalcular manualmente as linhas do tempo em massa na caixa Editar Projetos](#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box)
* [Recalcular linhas do tempo para todos os projetos no sistema (somente administradores do Workfront)](#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only)

### Recalcular linhas do tempo de projetos individuais ou em massa {#recalculate-timelines-for-individual-projects-or-in-bulk}

Você pode recalcular a linha do tempo de um projeto no Workfront a partir da página do projeto ou de uma lista de projetos ou relatório.

1. Vá para o projeto para o qual você deseja recalcular a linha do tempo e clique no ícone **Mais** ![Mais menu](assets/qs-more-menu.png) à esquerda do nome do projeto.

   Ou

   Vá para uma lista de projetos ou relatório, selecione um ou vários projetos e clique no ícone **Mais** ![Mais menu](assets/qs-more-menu.png) na parte superior da lista.

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >Dependendo da complexidade de seus projetos, recomendamos não selecionar um grande número de projetos ao recalcular suas linhas do tempo em massa para garantir o desempenho ideal. Alguns itens que podem tornar um projeto muito complexo podem ser várias dependências ou atribuições, ou um grande número de campos personalizados.

1. Clique em **Recalcular Linha do Tempo**. A linha do tempo é recalculada e uma mensagem de sucesso é exibida na tela.

   >[!TIP]
   >
   >Antes da conclusão do recálculo do cronograma, algumas datas planejadas ou projetadas podem ser exibidas esmaecidas. Isso significa que o recálculo ainda não foi concluído e as datas estão sujeitas a alterações.

### Recalcular manualmente as linhas do tempo em massa na caixa Editar projetos {#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box}

Você pode recalcular manualmente as linhas do tempo de vários projetos editando-os em massa.

>[!TIP]
>
>Dependendo da complexidade de seus projetos, recomendamos não selecionar um grande número de projetos ao editá-los em massa para garantir o desempenho ideal. Alguns itens que podem tornar um projeto muito complexo podem ser várias dependências ou atribuições, ou um grande número de campos personalizados.

1. Ir para uma lista de projetos.
1. Selecione vários projetos na lista e clique em **Editar**.
1. Clique em **Configurações** e selecione **Recalcular Linhas de Tempo**.

1. Clique em **Salvar alterações**.

### Recalcular linhas do tempo para todos os projetos no sistema (somente administradores do Workfront) {#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only}

Os administradores do Workfront podem executar o diagnóstico Recalcular linha do tempo para recalcular imediatamente todas as linhas do tempo no sistema Workfront. Isso permite que todos os gerentes de projeto vejam a influência das alterações externas imediatamente nas datas planejadas e projetadas.

Para obter mais informações sobre como recalcular linhas do tempo para todo o site do Workfront, consulte a seção Recalcular linhas do tempo para toda a instância do Workfront em [Configurar recálculos de linha do tempo para projetos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

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
<li> <p><strong>Automatic and On Change:</strong> This is the default setting. The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on. The project timeline is also updated each night.  <br>This is the recommended setting as it ensures that the project timeline is always up to date.</p> <p>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed. </p> <p> <img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"> </p> <p>This indicates that the recalculation is not yet finished, and the dates are subject to change. </p> </li>
<li><strong>Change Only:</strong> The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur. <br>You might want to select this option if you are concerned about system performance and if changes rarely occur in the project or in other projects that the timeline is dependent on.</li>
<li> <p><strong>Automatic Only:</strong> The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if you are concerned about system performance and if many changes occur each day in the project or in other projects that the timeline is dependent on.</p> <note type="note">
A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
</note> </li>
<li><strong>Manual Only:</strong> The project timeline is updated only when you select the option to <strong>Recalculate Timelines</strong>, as described in the section "Manual Recalculation" in the article <a href="#" class="MCXref xref selected">Recalculate project timelines</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).</li>
</ul>
</div>
-->
