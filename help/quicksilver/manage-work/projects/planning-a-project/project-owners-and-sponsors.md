---
content-type: overview
product-area: projects;user-management
navigation-topic: plan-a-project
title: Visão Geral dos Proprietários e Patrocinadores do Projeto
description: Você pode designar um Proprietário do projeto e um Patrocinador do projeto.
author: Alina
feature: Work Management
exl-id: e3e8be3f-105f-4702-8c93-ae8092f5d5d3
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 0%

---

# Visão geral dos proprietários e patrocinadores do projeto

<!-- Audited: 1/2024 -->

Você pode designar um Proprietário do projeto e um Patrocinador do projeto.

O Proprietário do Projeto é o indivíduo responsável pela conclusão do projeto no prazo e dentro do orçamento.

O Patrocinador do projeto é uma parte interessada importante para o projeto que tem recursos investidos no projeto. A conclusão do projeto normalmente beneficia o Patrocinador do Projeto.

Para obter informações sobre como atualizar o Proprietário ou Patrocinador do Projeto, consulte [Atualizar proprietários e patrocinadores do projeto](../../../manage-work/projects/planning-a-project/update-project-owners-and-sponsors.md).

## Proprietários do projeto

Você pode designar o gerente de um projeto especificando um Proprietário do projeto em um projeto ou modelo.

Você pode definir apenas um Proprietário de projeto para um projeto.

Os itens a seguir são possíveis usando o campo Proprietário do projeto:

* Você pode designar somente um usuário como Proprietário do projeto.
* Você pode designar Proprietários do Projeto como aprovadores de horas para o projeto.
* Você pode designar o Proprietário do projeto como um aprovador genérico ao definir processos de aprovação de projetos, tarefas ou problemas. Para obter informações sobre aprovações, consulte [Editar um processo de aprovação](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

  >[!IMPORTANT]
  >
  >Quando você atribui uma aprovação ao Proprietário do projeto e ninguém é designado como o proprietário de um projeto, a aprovação é reatribuída ao administrador principal do Workfront, conforme indicado na seção Informações do cliente na área Configuração. Para obter informações, consulte [Configurar informações básicas do sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).
  >


* Você pode ativar determinadas notificações que são entregues somente ao Proprietário do projeto.

  Para obter mais informações sobre notificações por email, consulte a seção [Configurar notificações de eventos para todos no sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md#modify) no artigo [Configurar notificações de eventos para todos no sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* É possível exibir o campo Proprietário do projeto em um relatório ou lista.

  Você também pode exibir o campo Proprietário do projeto em uma visualização, agrupamento ou prompt.

  Por exemplo, você pode copiar a seguinte expressão de modo de texto em um filtro para exibir projetos pertencentes ao usuário conectado:

  ```
  ownerID=$$USER.ID
  ```

Para obter mais informações sobre como criar relatórios, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Owner of a project</h2>
<p>(NOTE: drafted and moved to its own article)</p>
<ol>
<li value="1">Go to the project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project Details area, then click <strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Owner</strong> field.</p> <p>Only active users can be specified as Project Owners.</p> </li>
<li value="5"> Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## Patrocinadores do projeto

Você pode designar qualquer usuário no sistema como um Patrocinador do projeto. O Patrocinador do projeto geralmente é um gerente, executivo ou participante que precisa saber o que está acontecendo com o projeto.

Considere o seguinte ao atribuir um Patrocinador do projeto:

* O Patrocinador do Projeto não obtém acesso adicional ao projeto, mas é adicionado às notificações por email do projeto. Para obter informações sobre notificações, consulte o artigo [Configurar notificações de eventos para todos no sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* Você pode designar somente um Patrocinador do Projeto.
* Você pode designar o Patrocinador do Projeto como um aprovador genérico ao definir processos de aprovação de projetos, tarefas ou problemas. Para obter informações sobre aprovações, consulte [Editar um processo de aprovação](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

  >[!IMPORTANT]
  >
  >Quando você atribui uma aprovação ao Patrocinador do Projeto e ninguém é designado como patrocinador de um projeto, a aprovação é reatribuída ao Proprietário do Projeto. Se ninguém for designado como o proprietário do projeto, a aprovação será atribuída ao administrador do Workfront.

* Você pode exibir o campo Patrocinador do projeto em um relatório ou lista.

  Você também pode exibir o campo Patrocinador do projeto em uma visualização, agrupamento ou prompt.

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
<li value="3"> Click the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project Details area, then click <strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Sponsor</strong> field.</p> <p>Only active users can be specified as Project Sponsors.</p> </li>
<li value="5"> Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
