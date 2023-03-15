---
content-type: overview
product-area: resource-management
navigation-topic: resource-management-overview
title: Introdução ao Gerenciamento de recursos
description: O Gerenciamento de Recursos permite configurar seu sistema para prever com precisão o uso de seus recursos com base em sua disponibilidade, de modo que o trabalho que deve ser feito seja concluído a tempo e no orçamento.
author: Alina
feature: Resource Management
exl-id: b10ef503-60ea-4450-b63e-b2918e9bcc11
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1171'
ht-degree: 0%

---

# Introdução ao Gerenciamento de recursos

<!--
<p>(NOTE: DO NOT DELETE THIS ARTICLE. MANY ARTICLES MENTIONING RES MANAGEMENT ARE AND STILL SHOULD / WILL BE LINKED TO IT.) </p>
<p>(NOTE: Alina: ***As functionality is removed from Legacy and added to Res Planning - this will be continually updated: remove the Legacy Res Planning when that functionality is removed from the system.) </p>
</div>
-->

O Gerenciamento de Recursos permite configurar seu sistema para prever com precisão o uso de seus recursos com base em sua disponibilidade, de modo que o trabalho que deve ser feito seja concluído a tempo e no orçamento.

## Visão geral do gerenciamento de recursos no Adobe Workfront

O Gerenciamento de Recursos refere-se a todas as atividades executadas pelo administrador do Adobe Workfront, pelo gerente de recursos e pelo Proprietário do Projeto para planejar (Planejamento de Recursos ou Cenário) e programar (Balanceador de Carga de Trabalho) os recursos de uma organização e atribuí-los ao trabalho que precisa ser feito, levando em conta sua disponibilidade. Além disso, o gerenciamento de recursos também se refere à exibição de informações sobre as alocações de recursos programadas e reais em uma exibição de relatório (relatório Utilização ).

A Workfront tem vários conjuntos de ferramentas usados para gerenciar recursos. Cada ferramenta tem um escopo individual. Atualmente, você pode usar as seguintes ferramentas de Gerenciamento de Recursos no Workfront, dependendo de qual estágio do gerenciamento de recursos você está:

* Para planejar como os recursos são alocados em um nível superior, antes do início do trabalho real nos projetos, use as seguintes ferramentas:

   * **O Planejador de recursos**: Você pode usar o Planejador de Recursos no primeiro estágio do gerenciamento de recursos para orçar o tempo do projeto para seus recursos de acordo com sua disponibilidade programada. Durante a fase de planejamento de recursos, você pode organizar usuários em pools de recursos e atribuir vários pools de recursos a um projeto.

      Para obter mais informações sobre o Planejamento de Recursos, consulte a seção [Planejamento de recursos no Adobe Workfront](../../resource-mgmt/resource-planning/resource-planning-overview.md).

   * **O Planejador de Cenário**: Esse é um planejamento de nível superior de recursos que permite gerenciá-los em várias iniciativas que podem abranger um plano de um, três ou cinco anos e incluir vários projetos. Você pode usar o melhor cenário para aproveitar ao máximo a disponibilidade e o orçamento.

      O Planejador de Cenário requer uma licença separada, além da licença da Workfront. Para obter informações sobre o Planejador de Cenário do Workfront, consulte [A visão geral do Planejador de cenário](../../scenario-planner/scenario-planner-overview.md).

      <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when more functionality is added, maybe we add that we recommend to start here if this is available for them?!) </p>   
     -->

* Para agendar ou atribuir recursos ao trabalho real (tarefas e problemas), use a seguinte ferramenta:

   * **O Balanceador de Carga de Trabalho**: Isso pertence a um estágio inferior do gerenciamento de recursos, em que você pode atribuir seus recursos ao trabalho real (tarefas e problemas) que eles devem concluir, com base na quantidade de horas necessárias para concluí-los e sua disponibilidade. Usando o Balanceador de Carga de Trabalho, você pode atribuir usuários ao trabalho real que está atualmente não atribuído ou atribuído a funções de job.

      Para obter informações sobre o Balanceador de Workfront, consulte a seção [O Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/workload-balancer.md).

<!--

  * **Scheduling** (deprecated <span class="preview">and removed from the Preview environment</span>): Refers to assigning actual work to users by matching the job roles assigned to the tasks and issues with the job roles they can fulfill, or assigning actual work to users on tasks and issues which are currently unassigned. This happens at a lower-level in the process of managing resources, where you can assign your resources to the actual work (tasks and issues) that they must fulfill, according to the hours needed in the project plan to fulfill them.  

     For more information about resource scheduling, see the section [Resource Scheduling](../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md).

    >[!CAUTION]
    >
    >
    >We are no longer supporting the Resource Scheduling tools and they will be removed from Workfront in **January 2023**. We recommend that you use the Workload Balancer for scheduling your resources. 
    >
    >
    >* For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).
    >
    >
    >* For more information about the timeline for removing the Resource Scheduling tools and replacing them with the Workload Balancer, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

-->
* Para analisar alocações orçadas, planejadas e reais em vários projetos, use a seguinte ferramenta:

   * **Relatório de utilização**: Use este relatório para visualizar a utilização de recursos para projetos. Você pode comparar alocações orçadas, planejadas e reais para seus projetos e seu impacto no custo e na receita dos projetos.

      Para obter informações sobre o Relatório de Utilização, consulte [Exibir informações de utilização de recursos](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Os componentes do processo de gerenciamento de recursos

>[!NOTE]
>
>O Gerenciamento de recursos nunca é um processo estagnado no Workfront. Conforme as programações de seus projetos, a disponibilidade de seus usuários ou suas funções mudam, você deve ajustar continuamente as informações sobre seus recursos, atribuições e alocações para projetos, tarefas e problemas.

O processo de gerenciamento de recursos no Workfront inclui as seguintes etapas:

* **Configuração**: Como administrador de sistema, gerente de recursos ou proprietário do projeto, você deve configurar determinados campos e objetos na instância do Workfront antes de gerenciar os recursos. Para obter mais informações sobre os pré-requisitos necessários para iniciar o gerenciamento de recursos no Workfront, consulte o [Pré-requisitos para um gerenciamento preciso de recursos](#prerequisites-for-accurate-resource-management) neste artigo.\
   Além de ter projetos com itens de trabalho, você deve configurar os seguintes itens no Workfront:

   * Usuários\
      Para obter mais informações sobre como criar usuários, consulte o artigo [Adicionar usuários](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   * Função no trabalho\
      Para obter mais informações sobre a criação de funções, consulte o artigo [Criar e gerenciar funções de trabalho](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

   * Cronogramas\
      Para obter mais informações sobre como criar programações, consulte o artigo [Criar um agendamento](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   * Preferências do projeto

      >[!TIP]
      >
      >Somente um administrador de sistema ou de grupo pode modificar as Preferências do projeto para seu sistema ou para seu grupo.

      Para obter mais informações sobre como definir Preferências do projeto, consulte o artigo [Configurar preferências de projeto em todo o sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * Conjuntos de Recursos

      Para obter mais informações sobre a criação de pools de recursos, consulte [Criar pools de recursos](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

   * Preferências do Gerenciamento de recursos

      Como sistema, você deve decidir como a Workfront calcula a disponibilidade do usuário no nível do sistema, usando o agendamento do usuário ou o agendamento padrão de seu sistema.

      Para obter mais informações, consulte [Configurar preferências do Gerenciamento de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **Alocação de recursos**: Como gerente de recursos ou Proprietário do projeto, você pode definir a alocação de recursos para seus projetos, bem como atribuir trabalho. Para esta etapa, você pode gerenciar a estimativa da alocação de seus recursos usando o Planejador de Recursos ou o Planejador de Cenários e atribuir trabalho real aos usuários no Balanceador de Carga de Trabalho.

   Para obter mais informações sobre planejamento de recursos e atribuição de trabalhos, consulte as seguintes seções:

   * [Planejamento de recursos no Adobe Workfront](../../resource-mgmt/resource-planning/resource-planning-overview.md)
   * [Planejador de cenário do Adobe Workfront](../../scenario-planner/scenario-planning.md)
   * [O Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/workload-balancer.md)

<!--
* **Resource scheduling**: After generally planning for resources to use on your projects at a high level, you can start assigning work items (tasks and issues) to users based on their job roles using the Workload Balancer.

  For more information, see [Overview of the Workload Balancer](../workload-balancer/overview-workload-balancer.md). 
-->

* **Análise**: Como gerente de recursos, proprietário do projeto ou gerente de pessoas, revise o Relatório de Utilização para entender como as alocações orçadas e planejadas de seus recursos se comparam às reais. Revise as informações por horas, custo ou receita. Para obter informações sobre o relatório Utilização, consulte [Exibir informações de utilização de recursos](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Acesso necessário para visualizar e gerenciar recursos usando as ferramentas de Gerenciamento de Recursos no Workfront

Os seguintes usuários têm acesso às ferramentas de Gerenciamento de Recursos no Workfront:

Você deve ser um dos seguintes usuários e ter o seguinte acesso e permissões para acessar as ferramentas de gerenciamento de recursos:

* O administrador do sistema.
* Um usuário com uma licença de Plano.

   Um usuário com uma licença de Trabalho pode usar o Balanceador de Carga de Trabalho de um projeto e gerenciar atribuições e alocações.

   Além de ter uma licença do Work ou superior, você deve ter o seguinte para usar ferramentas específicas de gerenciamento de recursos:

   * Editar acesso ao Gerenciamento de Recursos (não é necessário para fazer atribuições no Balanceador de Carga de Trabalho)
   * Edite o acesso a Dados Financeiros para exibir informações de Custo no Planejador de Recursos
   * Exibir o acesso aos Dados Financeiros para exibir informações de Custo e Receita no Relatório de Utilização (somente usuários com licença de Plano)

* Contribua ou permissões superiores que incluem Fazer atribuições nos projetos para os quais você deseja gerenciar recursos.

<!--
* Designated as a Resource Manager for projects to use the Scheduling tool (the Scheduling tool is deprecated).

  >[!TIP]
  >
  >You do not have to be a Resource Manager to use the Resource Planner, Scenario Planner, or the Workload Balancer. 
-->

Para obter informações sobre o acesso necessário aos recursos do orçamento, consulte o artigo [Acesso necessário aos recursos orçamentais](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

Para obter informações sobre o acesso necessário para gerenciar recursos no Balanceador de Carga de Trabalho, consulte [Acesso necessário para gerenciar recursos no Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

## Pré-requisitos para um gerenciamento preciso de recursos  {#prerequisites-for-accurate-resource-management}

Você deve atender a um conjunto de requisitos para usar com eficiência as ferramentas de gerenciamento de recursos no Workfront.

Para obter informações sobre quais são os requisitos para cada ferramenta de gerenciamento de recursos no Workfront, consulte o seguinte:

* A seção &quot;Pré-requisitos para trabalhar no Planejador de Recursos&quot; no artigo [Visão geral do Planejador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md).
   <!--remove this at production: * The section "Prerequisites" in the article [Get started with Resource Scheduling](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).-->
* A seção &quot;Práticas recomendadas para usar o Balanceador de carga de trabalho&quot; no artigo [Visão Geral do Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).
* [Acesso necessário para recursos de orçamento no Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).
* [Acesso necessário para gerenciar recursos no Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted and replaced with the links to each prerequisites instead) </p>
<p> We recommend that the following settings exist before starting to manage resources for your organization: </p>
<ul>
<li> You must have users in the system who have active accounts. </li>
<li> You must assign a Plan or a Worker license to the users whose work allocation you want to manage. <note type="note">
Although you can assign work to a Reviewer or a Requestor, they cannot complete it.
<br>We recommend against assigning work to Reviewers or Requestors. For information about access levels in Workfront, see
<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref" xrefformat="{para}">Access levels overview</a>.
</note></li>
<li> You must have job roles configured in the system.<br>For information about adding job roles to Workfront, see the article <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" xrefformat="{para}">Create and manage job roles</a>.</li>
<li> (Optional) If you want to budget cost for your work, your job roles and your users must also have rates associated with them.<br></li>
<li> You must associate at least one job role with your users. </li>
<li> You must specify a valid value for the FTE field of all users when you use the User's Schedule instead of The Default Schedule in your Resource Management system preferences. <br>For information about editing users to ensure they have a job role, FTE, or cost associated with them, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" xrefformat="{para}">Edit a user's profile</a>. For information about editing the Resource Management preferences in your system, see <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref" xrefformat="{para}">Configure Resource Management preferences</a>.</li>
<li>You must associate accurate schedules with your users and they should include schedule exceptions.<br>For information about creating and editing schedules, see the article <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" xrefformat="{para}">Create a schedule</a>.</li>
<li>The Time Off calendar of the users must be up to date. </li>
<li> <p>The following is recommended for the Resource Planner when applying the Project and Role views: </p>
<ul>
<li> <p>You must associate projects with Resource Pools.<br>For information about associating projects with Resource Pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md" class="MCXref xref" xrefformat="{para}">Associate resource pools with projects and templates</a>.</p> </li>
</ul> </li>
<li> <p>Your must designate a Resource Manager on your projects and they must have the correct access to budget resources when using the Scheduling tools. </p> <p>For information about the access needed to budget resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref" xrefformat="{para}">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p> </li>
<li> <p>You must assign the tasks and issues in your system to job roles, teams, or users.</p> </li>
<li>You must specify a valid value for Planned Hours and Duration for all tasks in your system.<br>For information about Planned Hours, see the article <a href="../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref" xrefformat="{para}">Planned Hours overview</a>.<br>For information about Duration, see the article <a href="../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref" xrefformat="{para}">Overview of Task Duration and Duration Type</a>.</li>
</ul>
</div>
-->
