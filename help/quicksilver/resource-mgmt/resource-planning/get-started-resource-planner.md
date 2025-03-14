---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: Visão geral do Planejador de recursos
description: Você pode estimar e orçar a alocação dos recursos para os projetos aos quais estão atribuídos e prever sua disponibilidade para trabalho futuro usando o Planejador de Recursos.
author: Lisa
feature: Resource Management
exl-id: 06cd2226-f94d-4b6a-8692-6d35210782f2
source-git-commit: 696d656816a4c1c2edef4347567b2fc553f489f7
workflow-type: tm+mt
source-wordcount: '2113'
ht-degree: 0%

---

# Visão geral do Planejador de recursos {#resource-planner-overview}

>[!CONTEXTUALHELP]
>id="wf-resourcing-planner"
>title="Planejador de recursos"
>abstract="Você pode usar o Planejador de Recursos para estimar e orçar a alocação dos recursos para os projetos aos quais estão atribuídos e prever sua disponibilidade para trabalho futuro."

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: this used to be the beginning of Planning in the Resource Planner - consider restructuring it further? Merging some of this information with information about Understanding Navigation in the RP?!)</p>
-->

Você pode estimar e orçar a alocação dos recursos para os projetos aos quais estão atribuídos e prever sua disponibilidade para trabalho futuro usando o Planejador de Recursos.

Para obter uma visão geral do planejamento de recursos no Adobe Workfront, consulte o artigo [Introdução ao Planejamento de Recursos](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## Visão geral do Planejador de recursos

Você pode usar o Planejador de recursos para entender facilmente a disponibilidade de usuários e funções de trabalho, bem como o tempo planejado necessário para concluir o trabalho nos projetos. Você pode decidir como alocar os usuários e suas funções de trabalho nos projetos aos quais eles estão atribuídos com base no tempo disponível.

>[!IMPORTANT]
>
>Você não pode usar o Planejador de recursos para atribuir trabalho real (tarefas e problemas) aos usuários. Você só pode estimar a quantidade de tempo necessária para que os usuários ou funções de trabalho concluam um projeto, independentemente das tarefas e problemas aos quais estão atribuídos.\
>Para atribuir o trabalho real aos usuários, você deve usar o Balanceador de carga de trabalho. Para obter mais informações sobre o Balanceador de carga de trabalho, consulte [Visão geral do Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Você pode exibir informações no Planejador de recursos usando três visualizações separadas. Você pode usar cada exibição para atender a uma das seguintes finalidades:

* Para prever o tempo ou custo de seus recursos para o trabalho que precisa ser realizado usando as visualizações Projeto e Função. Este é o objetivo principal do Planejador de recursos.\
  Para obter mais informações sobre orçamento no Planejador de recursos, consulte o artigo [Recursos de orçamento no Planejador de recursos usando as exibições de Projeto e Função](../resource-planning/budget-resources-project-role-views-resource-planner.md).

* Para exibir as seguintes informações usando a view Usuário:

   * A disponibilidade de seus usuários de acordo com a programação deles
   * O tempo planejado necessário para concluir o trabalho de acordo com o plano do projeto
   * O tempo que os usuários já fizeram logon em itens de trabalho reais

  Para obter mais informações sobre como exibir as Horas Disponíveis, Planejadas e Reais ou FTE para usuários no Planejador de Recursos, consulte o artigo [Exibir Horas Disponíveis, Planejadas e Reais ou FTE no Planejador de Recursos ao usar o modo de exibição Usuário](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md#using).

## Considerações do Planejador de Recursos

* É possível priorizar os projetos em que está trabalhando e orçar sua alocação de recursos de acordo com a prioridade, para garantir que você tenha recursos alocados primeiro para os projetos mais importantes.

  Para obter informações sobre a priorização de projetos no Planejador de recursos, consulte [Priorizar projetos no Planejador de recursos](../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).

* Você pode exibir horas, FTE e informações de custo das tarefas e problemas dos projetos.

  >[!NOTE]
  >
  >Tarefas e problemas não são exibidos no Planejador de recursos. No entanto, as informações de horas, FTE e custo das alocações de recursos nas tarefas são exibidas no Planejador de recursos como um número total para o projeto.

* As informações de hora, FTE e custo de tarefas pai são excluídas dos projetos exibidos no Planejador de recursos. Recomendamos atribuir recursos somente a tarefas secundárias se você quiser gerenciar o tempo ou custo desses recursos no Planejador de recursos.

  Para obter informações sobre tarefas pai, consulte os seguintes artigos:

   * [Visão geral das tarefas](../../manage-work/tasks/task-information/tasks-overview.md)
   * [Criar subtarefas](../../manage-work/tasks/create-tasks/create-subtasks.md)

  >[!TIP]
  >
  >As tarefas pai exibem um total de horas e custos das tarefas filho. Por causa disso, contar horas, FTE e custo das tarefas filhas e das tarefas pai contaria esses valores duas vezes. É por isso que as informações da tarefa pai são excluídas do Planejador de recursos.

* Você não pode gerenciar a alocação de equipes nos projetos nos quais elas têm tarefas ou problemas no Planejador de recursos.
* Você pode estimar recursos para vários projetos de uma vez usando o Planejador de Recursos ou para um único projeto usando a área Orçamento de Recursos do Business Case. As informações orçadas para um projeto também são exibidas no Planejador de recursos.

  Para obter informações sobre como é possível orçar recursos para um único projeto, consulte o artigo [Recursos de orçamento no Business Case](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

  Para obter informações sobre como fazer o orçamento de recursos no Planejador de Recursos para vários projetos ao mesmo tempo, consulte a seção &quot;Budget resources in the Resource Planner&quot; no artigo [Budget resources in the Resource Planner using the Project and Role views](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

## Pré-requisitos para trabalhar no Planejador de recursos {#prerequisites-for-working-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(<b>THIS SECTION IS LINKED TO ALL RES PLANNING ARTICLES. DO NOT RENAME OF DELETE THIS!</b> - do NOT ADD the variable here, because it might break this link!)</p>
-->

Para usar com êxito o Planejador de recursos para fazer o orçamento de seus recursos, você deve primeiro garantir que você, seus projetos e suas tarefas atendam a um conjunto de pré-requisitos. Esses pré-requisitos são obrigatórios para exibir as informações corretas no Planejador de recursos e para gerenciar com precisão seus recursos.

>[!IMPORTANT]
>
>Se qualquer um dos pré-requisitos a seguir estiver ausente, você poderá descobrir que algumas informações sobre a alocação ou a disponibilidade dos recursos estão ausentes ou têm um valor zero.\
>Para saber mais sobre por que os campos estão sem dados ou têm valores zero, passe o mouse sobre os campos.

![Nenhum usuário com esta função](assets/no-users-with-this-role-in-the-res-pool-350x57.png)

>[!NOTE]
>
>Os seguintes pré-requisitos são necessários somente ao exibir o Planejador de Recursos por projeto ou por função de trabalho ou ao estimar recursos no Business Case de um projeto.

Os seguintes tipos de pré-requisitos são necessários para a funcionalidade correta do Planejador de recursos ao visualizá-lo por projeto ou por função:

* [Pré-requisitos de usuário](#user-prerequisites)
* [Pré-requisitos do projeto](#project-prerequisites)
* [Pré-requisitos de tarefas e problemas](#tasks-and-issues-prerequisites)
* [Pré-requisitos no nível do sistema](#system-level-prerequisites)

### Pré-requisitos do usuário {#user-prerequisites}

Verifique se a seguinte configuração de usuário existe antes de começar a usar o Planejador de recursos:

* Você tem o acesso correto aos recursos do orçamento.

  Para obter informações sobre o acesso necessário aos recursos de orçamento, consulte o artigo [Acesso necessário aos recursos de orçamento no Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* Os usuários atribuídos a tarefas são adicionados ao conjunto de recursos associado ao projeto.

  Para obter informações sobre como adicionar usuários aos pools de recursos, consulte [Associar pools de recursos a usuários](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md).

  >[!NOTE]
  >
  >Quando os usuários não são adicionados ao conjunto de recursos, os seguintes cenários podem existir:
  >
  >   
  >   
  >   * Os usuários não aparecem no Planejador de recursos, embora possam ser atribuídos a tarefas nos projetos.
  >   * Se as tarefas às quais estão associados tiverem Horas planejadas, essas horas não aparecerão para o projeto no Planejador de recursos, a menos que o usuário também esteja associado a uma função de trabalho nessas tarefas.
  >   * Se os usuários estiverem associados a uma função de trabalho em uma tarefa do projeto, as Horas Planejadas serão exibidas no Planejador de Recursos para a função de trabalho, mas a função de trabalho não poderá ser orçada.
  >   
  >

* Os usuários atribuídos a grupos de trabalho e recursos devem ter Agendamentos e Funções de trabalho associadas ao seu perfil.

  Para obter informações sobre como associar agendas e funções de trabalho a usuários, consulte [Editar perfil de usuário](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

  >[!NOTE]
  >
  >Os usuários que não estão associados a um Cronograma, mas estão no conjunto de recursos do projeto, não podem ser orçados no Planejador de recursos.

* Para obter informações precisas sobre Horas Disponíveis, verifique se os cronogramas associados aos usuários têm as exceções de cronograma e folga atualizadas.

  >[!NOTE]
  >
  >Se um usuário não estiver associado a um Cronograma, o Cronograma Padrão do seu sistema Workfront será associado ao usuário por padrão, para fins do Planejador de Recursos.

  Para obter informações sobre como criar agendas, consulte o artigo [Criar uma agenda](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Se quiser estimar seus recursos por Custo, você deverá associar Funções de Cargo a Custo/Hr. taxas. O custo associado às Funções de Trabalho atribuídas aos usuários nos conjuntos de recursos é usado para calcular o Custo de Trabalho Orçado e o Custo Orçado do projeto.\
  Para obter informações sobre como associar funções de trabalho a taxas, consulte o artigo [Criar e gerenciar funções de trabalho](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
  Para obter informações sobre como calcular o Custo do Trabalho Orçado, consulte o artigo [Entender o Custo do Trabalho Orçado e as Horas Orçadas dos projetos](../../manage-work/projects/project-finances/budgeted-labor-cost.md).\
  Para obter informações sobre como calcular o Custo Orçado, consulte o artigo [Calcular Custo Orçado](../../manage-work/projects/project-finances/budgeted-cost.md).

### Pré-requisitos do projeto {#project-prerequisites}

Verifique se a seguinte configuração de projeto existe antes de começar a usar o Planejador de recursos:

* Seus projetos estão associados a conjuntos de recursos.\
  Para obter mais informações sobre como adicionar conjuntos de recursos a projetos, consulte [Associar conjuntos de recursos a projetos e modelos](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md).

  >[!IMPORTANT]
  >
  >Projetos sem conjunto de recursos não exibem informações de Hora planejada ou atribuições no Planejador de recursos.

### Pré-requisitos de tarefas e problemas {#tasks-and-issues-prerequisites}

Embora não seja possível exibir tarefas e problemas no Planejador de recursos, suas informações são transferidas para os projetos exibidos no Planejador de recursos.

Certifique-se de que a seguinte configuração de tarefa e problema existe antes de iniciar os recursos de orçamento no Planejador de Recursos:

* As tarefas ou problemas nos projetos para os quais você está orçando recursos são atribuídos a uma destas entidades:

   * Usuários no conjunto de recursos do projeto que também estão associados a Funções de trabalho
   * Função no trabalho

  >[!NOTE]
  >
  >As horas planejadas de tarefas e problemas atribuídas às funções de trabalho são exibidas no Planejador de recursos, mas essas horas não podem ser orçadas a menos que um usuário que esteja associado à função de trabalho seja listado em um conjunto de recursos associado ao projeto.

* Você não deve atribuir tarefas pai a usuários ou funções.

  Para exibir informações sobre horas no Planejador de Recursos para usuários ou funções associados a tarefas pai, você também deve atribuí-las às tarefas filho. O Planejador de recursos não exibe informações de tarefas pai.

* Tarefas e problemas têm um valor para Horas planejadas maior que zero.
* Tarefas e problemas têm um valor para a Duração maior que zero.
* As datas planejadas dos problemas estão dentro da linha do tempo do projeto.

### Pré-requisitos no nível do sistema {#system-level-prerequisites}

Você deve entender como sua instância do Workfront calcula a disponibilidade de usuários de acordo com as Preferências de gerenciamento de recursos em seu sistema. O Workfront pode calcular a disponibilidade do usuário usando a programação do usuário conforme definido na página Perfil do usuário, ou a Programação padrão do seu sistema.

![Preferências de gerenciamento](assets/resource-management-preferences-section-in-setup-350x89.png)

O administrador do Workfront configura as Preferências de gerenciamento de recursos.

Para obter mais informações, consulte [Configurar preferências de Gerenciamento de Recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Localizar o Planejador de recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This became another standalone article; drfat this section here when article is live.)</p>
-->

Você pode localizar o Planejador de recursos em duas áreas do Workfront, dependendo se deseja fazer o orçamento de seus recursos para vários projetos ou para apenas um projeto.

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

## As áreas do Planejador de recursos

Você pode exibir as seguintes informações ou executar as seguintes ações no Planejador de Recursos:

* Informações sobre os recursos atribuídos aos seus projetos no Planejador de recursos em uma linha do tempo geral.
* Superalocação ou subutilização de recursos no Planejador de recursos.
* Estimativa dos recursos para o trabalho manual ou automático.

Para obter mais informações sobre quais áreas são exibidas no Planejador de recursos e como configurar quais informações são exibidas nessas áreas, consulte o artigo [Visão geral da navegação do Planejador de recursos](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Limitações na exibição de informações no Planejador de recursos

Para melhorar o desempenho, o Workfront limita a quantidade de itens que podem ser exibidos no Planejador de recursos.

Para obter mais informações sobre essas limitações, consulte o artigo [Limitações de exibição do Planejador de recursos](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md).

## Calcular FTE no Planejador de recursos

Você pode exibir os valores de disponibilidade, alocação e planejamento no Planejador de Recursos em Horas, FTE ou Custo.

Para obter mais informações sobre como alterar as informações exibidas no Planejador de Recursos, consulte a seção [Exibir informações por hora, FTE ou Custo](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#display-by-hour-or-fte-menu) no artigo [Revisar a disponibilidade e a alocação de recursos usando o Planejador de Recursos da Adobe Workfront](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

Para obter mais informações sobre como as Horas e o FTE de usuários e funções são calculados no Workfront, consulte o artigo [Visão geral do cálculo de horas e FTE de usuários e funções no Planejador de recursos](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

## Calcular Custos no Planejador de Recursos

Você deve ter acesso de Visualização de Dados Financeiros e permissões de Visualização de Finanças nos projetos para ver as informações por Custo no Planejador de Recursos.

Além de exibir os valores de disponibilidade, alocação e planejamento no Planejador de Recursos em Horas e FTE, você também pode exibi-los por Custo.

>[!TIP]
>
>Você deve associar seus usuários e suas funções de trabalho às taxas de Custo por Hora para exibir informações por Custos no Planejador de Recursos.

Para obter mais informações sobre como associar taxas de Custo por hora a funções de trabalho, consulte o artigo [Criar e gerenciar funções de trabalho](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
Para obter mais informações sobre como associar taxas de Custo por hora a usuários, consulte o artigo [Editar perfil de usuário](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Considere o seguinte ao exibir informações por Custo no Planejador de Recursos:

* O Custo de cada tipo de horas (Planejadas, Disponíveis, Orçadas, Reais para Usuários, Funções ou Projetos) é calculado usando uma Taxa de Custo diferente.
* O Custo Planejado é afetado pelo Tipo de Custo das tarefas nos projetos.
* Ao aplicar a Exibição do Usuário ao Planejador de Recursos, você não pode exibir as informações sobre alocação e disponibilidade por Custo.

Para obter mais informações sobre como os custos são calculados no Planejador de recursos para usuários e funções, consulte o artigo [Calcular custos no Planejador de recursos](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

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

## Filtrar informações no Planejador de recursos

Você pode reduzir o número de projetos, funções ou usuários exibidos no Planejador de recursos criando um filtro.\
Para obter mais informações, consulte o artigo [Filtrar informações no Planejador de Recursos](../../resource-mgmt/resource-planning/filter-resource-planner.md).
