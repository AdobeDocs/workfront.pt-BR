---
content-type: overview
product-area: projects;user-management
navigation-topic: plan-a-project
title: Visão geral dos proprietários e patrocinadores do projeto
description: Você pode designar um proprietário de projeto e um patrocinador de projeto para um projeto.
author: Alina
feature: Work Management
exl-id: e3e8be3f-105f-4702-8c93-ae8092f5d5d3
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 0%

---

# Visão geral dos proprietários e patrocinadores do projeto

Você pode designar um proprietário de projeto e um patrocinador de projeto para um projeto.

O proprietário do projeto é o responsável pela conclusão do projeto a tempo e no orçamento.

O Patrocinador do Projeto é uma parte importante do projeto que possui recursos investidos no projeto. A conclusão do projeto geralmente beneficia o patrocinador do projeto.

Para obter informações sobre como atualizar o Proprietário ou Patrocinador do Projeto para um projeto, consulte [Atualizar proprietários e patrocinadores do projeto](../../../manage-work/projects/planning-a-project/update-project-owners-and-sponsors.md).

## Proprietários do projeto

Você pode designar o gerente de um projeto especificando um Proprietário do projeto em um projeto ou modelo.

Você pode definir somente um Proprietário do projeto para um projeto.

Os itens a seguir são possíveis usando o campo Proprietário do projeto :

* Você pode designar apenas um usuário como Proprietário do projeto.
* Você pode designar Proprietários de projeto como aprovador de horas do projeto.
* Você pode designar o Proprietário do projeto como um aprovador genérico ao definir processos de aprovação de projeto, tarefa ou emissão. Para obter informações sobre aprovações, consulte [Editar um processo de aprovação](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

   >[!IMPORTANT]
   >
   >Quando você atribui uma aprovação ao Proprietário do projeto e ninguém é designado como o proprietário de um projeto, a aprovação é reatribuída ao administrador principal do Workfront, conforme indicado na seção Informações do cliente na área Configuração . Para obter mais informações, consulte [Configurar informações básicas para seu sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).


* Você pode ativar determinadas notificações que são entregues somente ao Proprietário do projeto.

   Para obter mais informações sobre notificações por email, consulte a seção [Configurar notificações de evento para todos no sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md#modify) no artigo [Configurar notificações de evento para todos no sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* Você pode exibir o campo Proprietário do projeto em um relatório ou lista.

   Também é possível exibir o campo Proprietário do projeto em uma visualização, agrupamento ou prompt.

   Por exemplo, você pode copiar a seguinte expressão de modo de texto em um filtro para exibir projetos de propriedade do usuário conectado: 

   ```
   ownerID=$$USER.ID
   ```

Para obter mais informações sobre como criar relatórios, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Owner of a project</h2>
<p>(NOTE:&nbsp;drafted and moved to its own article)</p>
<ol>
<li value="1">Go to the project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click&nbsp;the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;<strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Owner</strong> field.</p> <p>Only active users can be specified as Project Owners.</p> </li>
<li value="5"> Click&nbsp;<strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## Patrocinadores de projetos

Você pode designar qualquer usuário do sistema como patrocinador de projeto. O patrocinador do projeto geralmente é um gerente, executivo ou parte interessada que precisa saber o que está acontecendo com o projeto.

Considere o seguinte ao atribuir um patrocinador de projeto:

* O Patrocinador de projeto não obtém acesso adicional ao projeto, mas é adicionado às notificações por email do projeto. Para obter informações sobre notificações, consulte o artigo [Configurar notificações de evento para todos no sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* Você pode designar apenas um patrocinador de projeto.
* Você pode designar o Patrocinador de projeto como um aprovador genérico ao definir processos de aprovação de projeto, tarefa ou emissão. Para obter informações sobre aprovações, consulte [Editar um processo de aprovação](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

   >[!IMPORTANT]
   >
   >Quando você atribui uma aprovação ao Patrocinador do Projeto e ninguém é designado como patrocinador de um projeto, a aprovação é reatribuída ao Proprietário do Projeto. Se ninguém for designado como proprietário do projeto, a aprovação será atribuída ao administrador do Workfront.

* Você pode exibir o campo Patrocinador de projeto em um relatório ou lista.

   Também é possível exibir o campo Patrocinador do projeto em uma visualização, agrupamento ou prompt.

   Por exemplo, você pode copiar a seguinte expressão de modo de texto em um filtro para exibir projetos patrocinados pelo usuário conectado:

   ```
   sponsorID=$$USER.ID
   ```

    

   Para obter mais informações sobre como criar relatórios, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Sponsor of a project </h2>
<p>(NOTE: drafted and moved to its own article) </p>
<ol>
<li value="1">Go to the Project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click&nbsp;the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;<strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Sponsor</strong> field.</p> <p>Only active users can be specified as Project Sponsors.</p> </li>
<li value="5"> Click&nbsp;<strong>Save Changes</strong>. </li>
</ol>
</div>
-->
