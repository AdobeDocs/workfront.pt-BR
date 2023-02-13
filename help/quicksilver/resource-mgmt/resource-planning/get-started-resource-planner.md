---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: Visão geral do Planejador de recursos
description: Você pode estimar e orçar a alocação de seus recursos para os projetos aos quais eles são atribuídos e prever sua disponibilidade para trabalhos futuros usando o Planejador de Recursos.
author: Alina
feature: Resource Management
exl-id: 06cd2226-f94d-4b6a-8692-6d35210782f2
source-git-commit: ec49a7d3adeb24c1b8df0ff5fafe650d18d92280
workflow-type: tm+mt
source-wordcount: '2077'
ht-degree: 0%

---

# Visão geral do Planejador de recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: this used to be the beginning of Planning in the Resource Planner - consider restructuring it further? Merging some of this information with information about Understanding Navigation in the RP?!)</p>
-->

Você pode estimar e orçar a alocação de seus recursos para os projetos aos quais eles são atribuídos e prever sua disponibilidade para trabalhos futuros usando o Planejador de Recursos.

Para obter uma visão geral do planejamento de recursos no Adobe Workfront, consulte o artigo [Introdução ao planejamento de recursos](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## Visão geral do Planejador de recursos

Você pode usar o Planejador de Recursos para entender facilmente a disponibilidade de usuários e funções de cargo, bem como o tempo planejado necessário para concluir o trabalho nos projetos. Em seguida, você pode decidir como alocar seus usuários e suas funções de trabalho nos projetos aos quais eles são atribuídos com base em seu tempo disponível.

>[!IMPORTANT]
>
>Não é possível usar o Planejador de Recursos para atribuir trabalho real (tarefas e problemas) aos usuários. Você só pode estimar a quantidade de tempo necessária para que os usuários ou funções de trabalho concluam um projeto, independentemente das tarefas e problemas aos quais elas estão atribuídas.\
>Para atribuir trabalho real aos usuários, você deve usar o Balanceador de Carga de Trabalho. Para obter mais informações sobre o Balanceador de Carga de Trabalho, consulte [Visão Geral do Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Você pode exibir informações no Planejador de Recursos usando três exibições separadas. Você pode usar cada exibição para atender a um dos seguintes objetivos:

* Para orçar o tempo ou o custo de seus recursos para o trabalho que precisa ser realizado usando as exibições Projeto e Função. Esse é o principal objetivo do Planejador de Recursos.\
   Para obter mais informações sobre orçamento no Planejador de Recursos, consulte o artigo [Recursos de orçamento no Planejador de Recursos usando as exibições Projeto e Função](../resource-planning/budget-resources-project-role-views-resource-planner.md).

* Para exibir as seguintes informações usando a exibição Usuário:

   * a disponibilidade de seus usuários de acordo com seu cronograma
   * O período de tempo previsto necessário para concluir o trabalho de acordo com o plano do projeto.
   * o tempo que os usuários já efetuaram logon nos itens de trabalho reais.

   Para obter mais informações sobre como visualizar as Horas Disponíveis, Planejadas e Reais ou FTE para usuários no Planejador de Recursos, consulte o artigo [Exibir Horas Disponíveis, Planejadas e Reais ou FTE no Planejador de Recursos ao usar a exibição Usuário](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md#using).

## Considerações sobre o Planejador de recursos

* Você pode priorizar os projetos em que está trabalhando e orçar sua alocação de recursos de acordo com sua prioridade, para garantir que tenha recursos alocados primeiro para os projetos mais importantes.

   Para obter informações sobre priorização de projetos no Planejador de Recursos, consulte [Priorizar projetos no Planejador de Recursos](../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).

* Você pode exibir horas, FTE e informações de custo das tarefas e problemas dos projetos.

   >[!NOTE]
   >
   >Tarefas e problemas não são exibidos no Planejador de Recursos. No entanto, as informações de horas, FTE e custo das alocações de recursos nas tarefas são exibidas no Planejador de Recursos como um número total do projeto.

* As informações de hora, FTE e custo das tarefas principais são excluídas dos projetos exibidos no Planejador de Recursos. Recomendamos atribuir recursos somente a tarefas secundárias se você quiser gerenciar o tempo ou custo desses recursos no Planejador de Recursos.

   Para obter informações sobre tarefas pai, consulte os seguintes artigos:

   * [Visão geral das tarefas](../../manage-work/tasks/task-information/tasks-overview.md)
   * [Criar subtarefas](../../manage-work/tasks/create-tasks/create-subtasks.md)

   >[!TIP]
   >
   >As tarefas pai exibem um total de horas e custos das tarefas filho. Por causa disso, contar horas, FTE e o custo das tarefas secundárias e as tarefas pai contariam esses valores duas vezes. É por isso que as informações da tarefa pai são excluídas do Planejador de Recursos.

* Não é possível gerenciar a alocação de equipes nos projetos em que elas têm tarefas ou problemas no Planejador de Recursos.
* Você pode orçar recursos para vários projetos de cada vez usando o Planejador de Recursos ou para um único projeto usando a área de Orçamento de Recursos do Caso de Negócios. As informações orçadas para um projeto também são exibidas no Planejador de Recursos.

   Para obter informações sobre como você pode orçar recursos para um único projeto, consulte o artigo [Recursos orçamentários no Caso de Negócios](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

   Para obter informações sobre como você pode orçar recursos no Planejador de Recursos para vários projetos de cada vez, consulte a seção &quot;Recursos de orçamento no Planejador de Recursos&quot; no artigo [Recursos de orçamento no Planejador de Recursos usando as exibições Projeto e Função](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

## Pré-requisitos para trabalhar no Planejador de Recursos {#prerequisites-for-working-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(<b>THIS SECTION IS LINKED TO ALL RES PLANNING ARTICLES. DO NOT RENAME OF DELETE THIS!</b> - do NOT ADD the variable here, because it might break this link!)</p>
-->

Para usar o Planejador de Recursos com sucesso para orçar seus recursos, primeiro você deve garantir que, seus projetos e suas tarefas atendam a um conjunto de pré-requisitos. Esses pré-requisitos são obrigatórios para exibir as informações corretas no Planejador de Recursos e gerenciar com precisão seus recursos.

>[!IMPORTANT]
>
>Se algum dos pré-requisitos a seguir estiver ausente, você poderá descobrir que algumas das informações sobre a alocação ou a disponibilidade dos recursos estão ausentes ou têm um valor zero.\
>Para obter mais informações sobre por que os campos estão sem dados ou têm valores zero, passe o mouse sobre os campos.

![](assets/no-users-with-this-role-in-the-res-pool-350x57.png)

>[!NOTE]
>
>Os pré-requisitos a seguir são necessários apenas ao visualizar o Planejador de Recursos por projeto ou por função de cargo ou ao orçar recursos no Caso de Negócios de um projeto.

Os seguintes tipos de pré-requisitos são necessários para a funcionalidade correta do Planejador de Recursos ao exibi-lo por projeto ou por função:

* [Pré-requisitos do usuário](#user-prerequisites)
* [Pré-requisitos do projeto](#project-prerequisites)
* [Pré-requisitos de tarefas e problemas](#tasks-and-issues-prerequisites)
* [Pré-requisitos no nível do sistema](#system-level-prerequisites)

### Pré-requisitos do usuário {#user-prerequisites}

Certifique-se de que a seguinte configuração de usuário existe antes de começar a usar o Planejador de Recursos:

* Você tem o acesso correto aos recursos do orçamento.

   Para obter informações sobre o acesso necessário aos recursos do orçamento, consulte o artigo [Acesso necessário para recursos de orçamento no Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* Os usuários atribuídos a tarefas são adicionados aos pools de recursos associados ao projeto.

   Para obter informações sobre como adicionar usuários a pools de recursos, consulte [Associar pools de recursos a usuários](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md).

   >[!NOTE]
   >
   >Quando os usuários não são adicionados aos pools de recursos, os seguintes cenários podem existir:
   >
   >   
   >   
   >   * Os usuários não aparecem no Planejador de Recursos, embora possam ser atribuídos a tarefas nos projetos.
   >   * Se as tarefas às quais estão associadas tiverem Horas Planejadas, essas horas não aparecerão para o projeto no Planejador de Recursos, a menos que o usuário também esteja associado a uma função de trabalho nessas tarefas.
   >   * Se os usuários estiverem associados a uma função de trabalho em uma tarefa no projeto, as Horas Planejadas serão exibidas no Planejador de Recursos para a função de trabalho, mas a função de trabalho não poderá ser orçada.


* Os usuários atribuídos a pools de trabalho e recursos devem ter Agendamentos e Funções de Trabalho associados ao perfil.

   Para obter informações sobre como associar Programações e Funções de Job aos usuários, consulte [Editar o perfil de um usuário](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   >[!NOTE]
   >
   >Os usuários que não estão associados a um Agendamento, mas que estão no pool de recursos do projeto não podem ser orçados no Planejador de Recursos.

* Para obter informações precisas sobre as Horas disponíveis, verifique se os agendamentos associados aos usuários têm as exceções de agendamento e o tempo de folga atualizados.

   >[!NOTE]
   >
   >Se um usuário não estiver associado a uma Programação, a Programação Padrão do seu sistema Workfront será associada ao usuário por padrão, para fins do Planejador de Recursos.

   Para obter informações sobre como criar agendamentos, consulte o artigo [Criar um agendamento](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Se quiser orçar seus recursos por Custo, você deverá associar Funções de Ordem de Produção ao Custo/Hora. taxas. O custo associado às Funções de Job atribuídas aos usuários em seus pools de recursos é usado para calcular o Custo de Trabalho Orçado e o Custo Orçado do projeto.\
   Para obter informações sobre como associar funções de job a taxas, consulte o artigo [Criar e gerenciar funções de trabalho](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
   Para obter informações sobre o cálculo do Custo da Mão-de-Obra Orçada, consulte o artigo [Entender o Custo da Mão de obra Orçada e as Horas Orçamentadas para Projetos](../../manage-work/projects/project-finances/budgeted-labor-cost.md).\
   Para obter informações sobre o cálculo do Custo Orçamentado, consulte o artigo [Calcular Custo Orçamentado](../../manage-work/projects/project-finances/budgeted-cost.md).

### Pré-requisitos do projeto {#project-prerequisites}

Verifique se a configuração do projeto a seguir existe antes de começar a usar o Planejador de Recursos:

* Seus projetos estão associados a pools de recursos.\
   Para obter mais informações sobre como adicionar pools de recursos a projetos, consulte [Associar pools de recursos a projetos e modelos](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md).

   >[!IMPORTANT]
   >
   >Os projetos sem pools de recursos não exibem informações de Hora Planejada ou atribuições no Planejador de Recursos.

### Pré-requisitos de tarefas e problemas {#tasks-and-issues-prerequisites}

Embora não seja possível exibir tarefas e problemas no Planejador de Recursos, suas informações são transferidas para os projetos exibidos no Planejador de Recursos .

Verifique se a seguinte tarefa e configuração de emissão existe antes de iniciar a orçamentação de recursos no Planejador de Recursos:

* As tarefas ou problemas nos projetos para os quais você está orçando recursos são atribuídos a uma dessas entidades:

   * Usuários nos pools de recursos do projeto que também estão associados a Funções de Trabalho
   * Função no trabalho

   >[!NOTE]
   >
   >As Horas Planejadas de tarefas e os problemas atribuídos a funções de job são exibidos no Planejador de Recursos, mas essas horas não podem ser orçadas a menos que um usuário associado à função de job seja listado em um pool de recursos associado ao projeto.

* Você não deve atribuir tarefas pai a usuários ou funções.

   Para exibir informações de hora no Planejador de Recursos para usuários ou funções associadas às tarefas pai, você também deve atribuí-las às tarefas filho. O Planejador de Recursos não exibe informações de tarefas pai.

* Tarefas e problemas têm um valor para Horas Planejadas que é maior que zero.
* Tarefas e problemas têm um valor para a Duração, que é maior que zero.
* As Datas Planejadas dos problemas estão na linha do tempo do projeto.

### Pré-requisitos no nível do sistema {#system-level-prerequisites}

Você deve entender como sua instância do Workfront calcula a disponibilidade do usuário de acordo com as Preferências de gerenciamento de recursos em seu sistema. A Workfront pode calcular a disponibilidade do usuário usando o agendamento do usuário, conforme definido na página Perfil do usuário, ou o agendamento padrão do sistema.

![](assets/resource-management-preferences-section-in-setup-350x89.png)

O administrador do Workfront configura as Preferências de gerenciamento de recursos.

Para obter mais informações, consulte [Configurar preferências do Gerenciamento de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Localizar o Planejador de Recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This became another standalone article; drfat this section here when article is live.)</p>
-->

Você pode localizar o Planejador de Recursos em duas áreas do Workfront, dependendo se deseja orçar seus recursos para vários projetos ou para apenas um projeto.

Para obter informações sobre como localizar o Planejador de Recursos, consulte [Localizar o Planejador de Recursos](../../resource-mgmt/resource-planning/locate-resource-planner.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(this is drafted and moved to its own article: locate-resource-planner) </p>
<p>Ensure that all prerequisites are met before starting to use the Resource Planner. This way, you ensure that the Resource Planner displays the correct information before you start budgeting your resources.<br>For information about the prerequisites that must be met before you can start using the Resource Planner, see the <a href="#prerequisites-for-working-in-the-resource-planner" class="MCXref xref">Prerequisites for working in the Resource Planner</a> section in this article. </p>
<p>You can locate the Resource Planner in two areas of Workfront, depending on whether you want to budget your resources for multiple projects, or for just one project.</p>
<ul>
<li><a href="#use-the-resource-planner-for-multiple-projects" class="MCXref xref">Use the Resource Planner for multiple projects</a> </li>
<li> <p><a href="#use-the-resource-planner-for-one-project" class="MCXref xref">Use the Resource Planner for one project</a> </p> </li>
</ul>
<p><strong>Use the Resource Planner for multiple projects</strong></p>
<p>When using the Resource Planner for multiple projects, the allocation numbers for your resources represent numbers across multiple projects. </p>
<p>To access the  Planner section  in the  Resourcing area: </p>
<ol>
<li value="1">  Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.  </li>
<li value="2"> <p>  Click <strong>Resourcing</strong>. The Resource Planner displays by default.  For information about budgeting resources in the Resource Planner, see the article <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a>. </p> <p> <img src="assets/qs-resource-management-area-with-planner-as-default-350x152.png" style="width: 350;height: 152;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">  Hover over the left panel, and click <strong>Resource Pools</strong>. <br>For information about creating new resource pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md" class="MCXref xref">Create resource pools</a>.</li>
</ol>
<p><strong>Use the Resource Planner for one project</strong></p>
<p>When using the Resource Planner for one project, the allocation numbers for your resources represent numbers for the selected project. </p>
<ol>
<li value="1"> <p>Go to a project you want to budget resources for.</p> </li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Business Case</strong> in the left panel.</p> </li>
<li value="3"> <p>Scroll to the <strong>Resource Budgeting</strong> section of the Business Case.</p> </li>
<li value="4"> <p>Click <strong>Edit Resource Budgeting</strong> to add resource pools to your project and start budgeting your resources. </p> <note type="tip">
You can only add a resource pool in the Resource Budgeting area of the Business Case when the project has no resource pools associated with it. When the project already has a resource pool, the users in the pool and their job roles display in the Resource Budgeting area by default.
</note> <p> <img src="assets/resource-budgeting-area-on-project-350x70.png" style="width: 350;height: 70;"> </p> <p>For information about budgeting resources for one project, see the article <a href="../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md" class="MCXref xref">Budget resources in the Business Case</a>.</p> </li>
</ol>
</div>
-->

## As áreas do Planejador de Recursos

Você pode exibir as seguintes informações ou executar as seguintes ações no Planejador de Recursos:

* Informações sobre os recursos atribuídos aos seus projetos no Planejador de Recursos em uma linha do tempo geral.
* Alocação ou subutilização de seus recursos no Planejador de Recursos.
* Faça o orçamento dos recursos de forma manual ou automática.

Para obter mais informações sobre quais áreas são exibidas no Planejador de Recursos e como configurar quais informações serão exibidas nessas áreas, consulte o artigo [Visão geral da navegação do Planejador de recursos](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Limitações na exibição de informações no Planejador de Recursos

Para melhorar o desempenho, o Workfront limita a quantidade de itens que você pode exibir no Planejador de Recursos.

Para obter mais informações sobre essas limitações, consulte o artigo [Limitações de exibição do Planejador de recursos](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md) .

## Calcular FTE no Planejador de Recursos

Você pode exibir valores de disponibilidade, alocação e planejado no Planejador de Recursos em Horas, FTE ou Custo.

Para obter mais informações sobre como alterar as informações exibidas no Planejador de Recursos, consulte a seção [Exibir informações por Hora, FTE ou Custo](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#display-by-hour-or-fte-menu) no artigo [Revise a disponibilidade e alocação de recursos usando o Adobe Workfront Resource Planner](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

Para obter mais informações sobre como as Horas e o FTE para usuários e funções são calculados no Workfront, consulte o artigo [Visão geral do cálculo de horas e FTE para usuários e funções no Planejador de Recursos](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

## Calcular Custos no Planejador de Recursos

Você deve ter acesso de Exibição aos Dados Financeiros e permissões de Exibição Financeira nos projetos para ver as informações por Custo no Planejador de Recursos.

Além de exibir a disponibilidade, alocação e valores planejados no Planejador de Recursos em Horas e FTE, você também pode exibi-los por Custo.

>[!TIP]
>
>Você deve associar seus usuários e suas funções de cargo às taxas de Custo por Hora para exibir as informações por Custos no Planejador de Recursos.

Para obter mais informações sobre como associar as taxas de Custo por Hora às funções de cargo, consulte o artigo [Criar e gerenciar funções de trabalho](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
Para obter mais informações sobre como associar as taxas de Custo por Hora aos usuários, consulte o artigo [Editar o perfil de um usuário](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Considere o seguinte ao exibir informações por Custo no Planejador de Recursos:

* O Custo de cada tipo de hora (Planejado, Disponível, Orçado, Real para Usuários, Funções ou Projetos) é calculado usando uma Taxa de Custo diferente.
* O Custo Planejado é afetado pelo Tipo de Custo das tarefas nos projetos.
* Ao aplicar a Exibição de Usuário ao Planejador de Recursos, você não pode exibir as informações de alocação e disponibilidade por Custo.

Para obter mais informações sobre como os Custos são calculados no Planejador de Recursos para usuários e funções, consulte o artigo [Calcular custos no Planejador de Recursos](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the User View to view Available, Planned, and Actual Hours or FTE </h2>
<p>(this information is repeated from above where it exists in shorter form. Drafted to simplify the amount of info of this article.) </p>
<p>You can use the User View of the Resource Planner to display information about the Planned, Available, and Actual Hours or FTE values for projects and resources. </p>
<p>For information about using the Resource Planner to review the Available, Planned, and Actual Hours and FTE for resources, see the article <a href="../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md" class="MCXref xref">View Available, Planned, and Actual Hours or FTE in the Resource Planner when using the User view</a>.</p>
<p><strong>Use the Project and Role Views to budget resources </strong></p>
<p> The main function of the Resource Planner is to budget your resources for the work that needs to be completed on the projects that you can manage. </p>
<p> You can budget your resources only if you apply the <strong>View by Project</strong> or <strong>View by Role</strong> views to the Resource Planner.</p>
<p>For information about budgeting resources using the Project and Role views in the Resource Planner, see the article <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md"><a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a></a>.</p>
</div>
-->

## Filtrar informações no Planejador de Recursos

Você pode reduzir o número de projetos, funções ou usuários exibidos no Planejador de Recursos criando um filtro.\
Para obter mais informações, consulte o artigo [Filtrar informações no Planejador de Recursos](../../resource-mgmt/resource-planning/filter-resource-planner.md).
