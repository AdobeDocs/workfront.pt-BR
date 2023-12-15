---
content-type: overview
product-area: resource-management
navigation-topic: resource-management-overview
title: Introdução ao gerenciamento de recursos
description: O Gerenciamento de Recursos permite configurar o sistema para prever com precisão o uso dos recursos com base em sua disponibilidade, de modo que o trabalho que deve ser feito seja concluído no prazo e dentro do orçamento.
author: Alina
feature: Resource Management
exl-id: b10ef503-60ea-4450-b63e-b2918e9bcc11
source-git-commit: ca4da5302198d8fffc8b706baa3b3aeaa1f738e3
workflow-type: tm+mt
source-wordcount: '1171'
ht-degree: 0%

---

# Introdução ao gerenciamento de recursos

<!-- Audited: 12/2023 -->

<!--
<p>(NOTE: DO NOT DELETE THIS ARTICLE. MANY ARTICLES MENTIONING RES MANAGEMENT ARE AND STILL SHOULD / WILL BE LINKED TO IT.) </p>
<p>(NOTE: Alina: ***As functionality is removed from Legacy and added to Res Planning - this will be continually updated: remove the Legacy Res Planning when that functionality is removed from the system.) </p>
</div>
-->

O Gerenciamento de Recursos permite configurar o sistema para prever com precisão o uso dos recursos com base em sua disponibilidade, de modo que o trabalho que deve ser feito seja concluído no prazo e dentro do orçamento.

## Visão geral do gerenciamento de recursos no Adobe Workfront

O Gerenciamento de Recursos refere-se a todas as atividades realizadas pelo administrador do Adobe Workfront, pelo gerente de recursos e pelo Proprietário do Projeto para planejar (Planejamento de Recursos ou Cenários) e programar (Balanceador de Carga de Trabalho) os recursos de uma organização e atribuí-los ao trabalho que precisa ser feito, levando em conta sua disponibilidade. Além disso, o gerenciamento de recursos também se refere à exibição de informações sobre as alocações de recursos planejadas e reais em uma exibição de relatório (relatório de utilização).

O Workfront tem vários conjuntos de ferramentas usados para gerenciar recursos. Cada ferramenta tem um escopo individual. Atualmente, você pode usar as seguintes ferramentas de Gerenciamento de recursos no Workfront, dependendo do estágio do gerenciamento de recursos em que está:

* Para planejar como os recursos são alocados em um nível superior, antes do início do trabalho real nos projetos, use as seguintes ferramentas:

   * **O Planejador de Recursos**: Você pode usar o Planejador de recursos na primeira etapa do gerenciamento de recursos para estimar o tempo do projeto para seus recursos de acordo com a disponibilidade programada. Durante a fase de planejamento de recursos, é possível organizar usuários em conjuntos de recursos e atribuir vários conjuntos de recursos a um projeto.

     Para obter mais informações sobre o Planejamento de Recursos, consulte [Planejamento de recursos no Adobe Workfront](../../resource-mgmt/resource-planning/resource-planning-overview.md).

   * **O Planejador de cenários**: este é um planejamento de recursos de nível superior que permite gerenciá-los em várias iniciativas que podem abranger um plano de um, três ou cinco anos e incluir vários projetos. Você pode usar o melhor cenário para aproveitar ao máximo a disponibilidade e o orçamento.

     O Planejador de cenários requer uma licença separada, além da licença do Workfront. Para obter informações sobre o Planejador de cenários do Workfront, consulte [A visão geral do Planejador de cenários](../../scenario-planner/scenario-planner-overview.md).

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when more functionality is added, maybe we add that we recommend to start here if this is available for them?!) </p>   
     -->

* Para agendar ou atribuir recursos ao trabalho real (tarefas e problemas), use a seguinte ferramenta:

   * **O Balanceador de carga de trabalho**: pertence a um estágio de nível inferior do gerenciamento de recursos, em que você pode atribuir seus recursos ao trabalho real (tarefas e problemas) que devem ser concluídos, com base na quantidade de horas necessárias para concluí-los e sua disponibilidade. Usando o Balanceador de carga de trabalho, você pode atribuir usuários ao trabalho real que não está atribuído ou atribuído a funções de trabalho no momento.

     Para obter informações sobre o Workfront Balancer, consulte [O Balanceador de carga de trabalho: índice do artigo](../../resource-mgmt/workload-balancer/workload-balancer.md).

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
* Para analisar alocações previstas em orçamento, planejadas e reais entre vários projetos, use a seguinte ferramenta:

   * **Relatório de Utilização**: use este relatório para exibir a utilização dos recursos de projetos. É possível comparar alocações previstas em orçamento, planejadas e reais para seus projetos e seu impacto no custo e na receita dos projetos.

     Para obter informações sobre o Relatório de Utilização, consulte [Exibir informações de utilização de recursos](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Os componentes do processo de gerenciamento de recursos

>[!NOTE]
>
>O gerenciamento de recursos nunca é um processo estagnado no Workfront. À medida que o cronograma de seus projetos, a disponibilidade de seus usuários ou suas funções mudam, você deve ajustar continuamente as informações sobre os recursos, suas atribuições e suas alocações para projetos, tarefas e problemas.

O processo de gerenciamento de recursos no Workfront inclui as seguintes etapas:

* **Configuração**: Como administrador do sistema, gerente de recursos ou Proprietário do projeto, você deve configurar determinados campos e objetos na instância do Workfront antes de gerenciar os recursos. Para obter mais informações sobre os pré-requisitos necessários para iniciar o gerenciamento de recursos no Workfront, consulte [Pré-requisitos para o gerenciamento preciso de recursos](#prerequisites-for-accurate-resource-management) neste artigo.\
  Além de ter projetos com itens de trabalho, você deve configurar os seguintes itens no Workfront:

   * Usuários\
     Para obter mais informações sobre como criar usuários, consulte o artigo [Adicionar usuários](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   * Função no trabalho\
     Para obter mais informações sobre como criar funções de trabalho, consulte o artigo [Criar e gerenciar funções de trabalho](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

   * Cronogramas\
     Para obter mais informações sobre como criar cronogramas, consulte o artigo [Criar um agendamento](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   * Preferências do projeto

     >[!TIP]
     >
     >Somente um administrador de sistema ou de grupo pode modificar as Preferências de Projeto do seu sistema ou do seu grupo.

     Para obter mais informações sobre como definir Preferências de Projeto, consulte o artigo [Configurar preferências de projeto em todo o sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * Conjuntos de Recursos

     Para obter mais informações sobre a criação de conjuntos de recursos, consulte [Criar conjuntos de recursos](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

   * Preferências de gerenciamento de recursos

     Como um sistema, você deve decidir como o Workfront calcula a disponibilidade do usuário no nível do sistema, seja usando a programação do usuário ou a Programação Padrão do seu sistema.

     Para obter mais informações, consulte [Configurar preferências de gerenciamento de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **Alocação de recursos**: Como um gerente de recursos ou um Proprietário do projeto, você pode definir a alocação de recursos para seus projetos, bem como atribuir trabalho. Para esta etapa, é possível gerenciar a estimativa da alocação de recursos usando o Planejador de Recursos ou o Planejador de Cenários e atribuir o trabalho real aos usuários no Balanceador de carga de trabalho.

  Para obter mais informações sobre o planejamento de recursos e a atribuição de trabalho, consulte as seguintes seções:

   * [Planejamento de recursos no Adobe Workfront](../../resource-mgmt/resource-planning/resource-planning-overview.md)
   * [Planejador de cenários do Adobe Workfront](../../scenario-planner/scenario-planning.md)
   * [O Balanceador de carga de trabalho: índice do artigo](../../resource-mgmt/workload-balancer/workload-balancer.md)

<!--
* **Resource scheduling**: After generally planning for resources to use on your projects at a high level, you can start assigning work items (tasks and issues) to users based on their job roles using the Workload Balancer.

  For more information, see [Overview of the Workload Balancer](../workload-balancer/overview-workload-balancer.md). 
-->

* **Análise**: Como um gerente de recursos, Proprietário do projeto ou gerente de pessoas, revise o Relatório de Utilização para entender como as alocações previstas e previstas em orçamento de seus recursos se comparam às reais. Revise as informações por horas, custo ou receita. Para obter informações sobre o relatório de Utilização, consulte [Exibir informações de utilização de recursos](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Acesso necessário para exibir e gerenciar recursos usando as ferramentas de Gerenciamento de recursos no Workfront

Os seguintes usuários têm acesso às ferramentas de Gerenciamento de recursos no Workfront:

Você deve ser um dos usuários a seguir e ter o seguinte acesso e permissões para acessar as ferramentas de gerenciamento de recursos:

* O administrador do sistema.
* Um usuário com uma licença de Plano.

  Um usuário com uma licença de Trabalho pode usar o Balanceador de carga de trabalho de um projeto e gerenciar atribuições e alocações.

  Além de ter uma licença de Trabalho ou superior, você deve ter o seguinte para usar ferramentas de gerenciamento de recursos específicas:

   * Editar o acesso ao Gerenciamento de recursos (não necessário para fazer atribuições no Balanceador de carga de trabalho)
   * Editar o acesso aos Dados Financeiros para exibir as informações de Custo no Planejador de Recursos
   * Acesso aos Dados Financeiros para exibir as informações de Custo e Receita no Relatório de Utilização (somente usuários com uma licença de Plano)

* Permissões do Contribute ou superior que incluem Fazer atribuições nos projetos para os quais você deseja gerenciar recursos.

<!--
* Designated as a Resource Manager for projects to use the Scheduling tool (the Scheduling tool is deprecated).

  >[!TIP]
  >
  >You do not have to be a Resource Manager to use the Resource Planner, Scenario Planner, or the Workload Balancer. 
-->

Para obter informações sobre o acesso necessário aos recursos de orçamento, consulte o artigo [Acesso necessário aos recursos do orçamento](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

Para obter informações sobre o acesso necessário para gerenciar recursos no Balanceador de carga de trabalho, consulte [Acesso necessário para gerenciar recursos no Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

## Pré-requisitos para o gerenciamento preciso de recursos  {#prerequisites-for-accurate-resource-management}

Você deve atender a um conjunto de requisitos antes de usar com eficiência as ferramentas de gerenciamento de recursos no Workfront.

Para obter informações sobre quais são os requisitos de cada ferramenta de gerenciamento de recursos no Workfront, consulte o seguinte:

* A seção [Pré-requisitos para trabalhar no Planejador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md#prerequisites-for-working-in-the-resource-planner) no artigo [Visão geral do Planejador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md).
  <!--remove this at production: * The section "Prerequisites" in the article [Get started with Resource Scheduling](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).-->
* A seção [Práticas recomendadas para usar o Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/overview-workload-balancer.md#best-practices-for-using-the-workload-balancer) no artigo [Visão geral do Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).
* [Acesso necessário para orçar recursos no Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).
* [Acesso necessário para gerenciar recursos no Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

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
