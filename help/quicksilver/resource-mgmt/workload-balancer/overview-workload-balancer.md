---
content-type: overview
product-area: resource-management
navigation-topic: the-workload-balancer
title: Visão Geral do Balanceador de Carga de Trabalho
description: Depois que os gerentes de projeto planejarem o trabalho em projetos e criarem tarefas, você poderá usar o Balanceador de Carga de Trabalho para atribuir esse trabalho aos usuários em suas equipes.
author: Alina
feature: Resource Management
exl-id: 9398bd04-9df7-4b77-8361-fdb5bdce6829
source-git-commit: 11c87d8a97261c24d063fbc824f2e907d07f8217
workflow-type: tm+mt
source-wordcount: '1122'
ht-degree: 0%

---

# Visão Geral do Balanceador de Carga de Trabalho

<!--
<p>(NOTE: this is linked from the UI for the Workload Balancer page. DO NOT CHANGE TITLE OR LINK) </p>
-->

Depois que os gerentes de projeto planejarem o trabalho em projetos e criarem tarefas, você poderá usar o Balanceador de Carga de Trabalho para atribuir esse trabalho aos usuários.

>[!IMPORTANT]
>
>Você pode usar o Balanceador de Carga de Trabalho para atribuir trabalho real (tarefas e problemas) aos usuários.
>
>Você deve usar o Planejador de Recursos e não o Balanceador de Carga de Trabalho para estimar alocações de função de cargo para seus projetos, em um nível alto. Para obter mais informações sobre o Planejador de Recursos, consulte [Visão geral do Planejador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Este artigo descreve o propósito geral do Balanceador de carga de trabalho e algumas das práticas recomendadas para a configuração de projetos e recursos para usá-lo com sucesso.

## Localizar o Balanceador de Carga de Trabalho

<!--
<p>(NOTE: This will be taken out when all we will have is one tool - should be replaced by a blurb that says you can add this tool anywhere, in any custom tab, etc (long term dev promise)) </p>
-->

Recomendamos usar o Balanceador de Carga de Trabalho nas seguintes áreas para agendar recursos:

* No nível do sistema, na área Recursos.
* No nível do projeto, na seção Balanceador de Carga de Trabalho de um projeto.
* No nível da equipe, na seção Balanceador de Carga de Trabalho de uma equipe.

Para obter mais informações sobre como localizar o Balanceador de Carga de Trabalho, consulte [Localizar o Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Benefícios do Balanceador de Carga de Trabalho

Considere os seguintes benefícios ao usar o Balanceador de Carga de Trabalho:

<!--
<p> Add about the what-if scenarios as a benefit when they become available </p>
-->

* Acesse um mapeamento visual claro da atribuição excessiva de recursos e da subutilização, transparente para todas as partes interessadas.
* Como gerente de pessoas, você pode proteger seu pessoal contra queimadas e capacitá-lo a fazer seu melhor trabalho com melhor foco, qualidade e envolvimento. Você pode garantir sua utilização total, quebrar silos e habilitar o alinhamento do trabalho entre as equipes.
* Ao atribuir trabalho no nível da tarefa ou da ocorrência, você não tem visibilidade sobre como um usuário pode estar ocupado. Ao usar o Balanceador de Carga de Trabalho, você pode visualizar quais usuários têm disponibilidade em sua carga de trabalho para concluir a tarefa ou o problema a tempo. Isso inclui os detalhes de tempo limite e de exceções de programação.

   Para obter mais informações, consulte [Visão Geral da atribuição de trabalho no Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

   Também é possível atribuir itens de trabalho em massa, o que facilita a distribuição de um grande número de itens de trabalho de uma vez, em vários projetos. Para obter mais informações, consulte [Atribua trabalho em massa usando o Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

* Os executivos podem tomar decisões oportunas sobre a equipe por meio da transparência sobre como as pessoas em sua organização são utilizadas.
* Os membros da equipe se beneficiam de uma melhor colaboração, já que todos podem ver em que ponto os seus colegas de trabalho estão trabalhando a qualquer momento. Para obter informações sobre o acesso necessário para visualizar ou gerenciar recursos no Balanceador de Carga de Trabalho, consulte [Acesso necessário para gerenciar recursos no Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
* Compartilhe-o com qualquer pessoa que não tenha acesso à área Recursos ao incorporar um link a ela em uma guia personalizada. Para obter mais informações, consulte [Compartilhar o Balanceador de Carga de Trabalho com um link](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md)
* Visualize e gerencie as cargas de trabalho e a demanda de pessoas em uma única visualização no nível global, de projeto ou de equipe, dependendo da sua função. Ao gerenciar projetos, isso inclui não apenas a alocação de recursos para o projeto, mas também a visualização da alocação de recursos do Adobe Workfront Scenario Planner. Os gerentes de pessoas usam o Workfront Scenario Planner para gerenciar as habilidades de trabalho na organização. O Planejador de cenário só está disponível na nova experiência do Adobe Workfront.

   >[!NOTE]
   >
   >  O Planejador de Cenário requer uma licença adicional. Para obter informações sobre o Planejador de Cenário do Workfront, consulte [A visão geral do Planejador de cenário](../../scenario-planner/scenario-planner-overview.md).


## Práticas recomendadas para usar o Balanceador de carga de trabalho

Recomendamos as seguintes práticas recomendadas para planejar projetos, configurar usuários e usar filtros antes de começar a programar seus recursos usando o Balanceador de Carga de Trabalho.

* [Práticas recomendadas para exibir informações no Balanceador de Carga de Trabalho](#best-practices-for-displaying-information-in-the-workload-balancer)
* [Práticas recomendadas para configurar usuários](#best-practices-for-setting-up-users)
* [Práticas recomendadas para configurar tarefas e problemas](#best-practices-for-setting-up-tasks-and-issues)

### Práticas recomendadas para exibir informações no Balanceador de Carga de Trabalho {#best-practices-for-displaying-information-in-the-workload-balancer}

Recomendamos usar filtros para exibir apenas as informações pertinentes a você para os itens de trabalho não atribuídos e atribuídos.

Para obter informações sobre como criar e usar filtros no Balanceador de Carga de Trabalho, consulte [Filtrar informações no Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

### Práticas recomendadas para configurar usuários

* Como o usuário que agendou o trabalho para outras pessoas, você deve ter o acesso e as permissões corretas para agendar recursos para o trabalho.

   Para obter informações sobre o acesso necessário para gerenciar a carga de trabalho de seus recursos no Balanceador de Carga de Trabalho, consulte [Acesso necessário para gerenciar recursos no Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

* Os usuários cuja carga de trabalho você deseja gerenciar precisam atender aos seguintes critérios para que as informações sobre sua disponibilidade e habilidades sejam precisas:

   * Ter Agendamentos e Funções de Trabalho associadas ao seu perfil.
   * Para obter mais informações sobre como associar Programações e Funções de Job a usuários, consulte [Adicionar usuários](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)
   * Se um usuário não estiver associado a uma Programação, a Programação Padrão do seu sistema Workfront será associada ao usuário por padrão, para fins de gerenciamento de recursos.
   * Ter Exceções de Programação atualizadas em suas programações.\
      Para obter mais informações sobre como criar programações, consulte [Criar um agendamento](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

   * Faça com que o calendário Tempo limite seja atualizado em seu perfil.\
      Para obter informações sobre como atualizar o calendário Tempo desligado de um usuário, consulte [Configurar o horário pessoal no Adobe Workfront](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

      <!--   
     <div data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <p>(NOTE: Add another bullet for Costs, when this becomes available:</p>   
     <p>If you want to budget your resources by Cost, you must associate Job Roles with Cost/ Hr. rates. The cost associated with Job Roles assigned to users in your Resource Pools is used to calculate the Budgeted Labor Cost and the Budgeted Cost of the project.For more information about associating job roles with rates, see the article Creating and Managing Job Roles in the new Adobe Workfront experience.For more information about calculating Budgeted Labor Cost, see the article Calculating Budgeted Labor Cost in the new Adobe Workfront experience.For more information about calculating Budgeted Cost, see the article Calculating Budgeted Cost in .) </p>   
     </div>   
     -->

* O administrador do Workfront deve determinar como o Workfront calcula a disponibilidade do usuário. Eles podem decidir se o Workfront usa a Programação Padrão do Sistema ou a programação do usuário para calcular o tempo em que o usuário está disponível para trabalhar. Para obter mais informações, consulte [Configurar preferências do Gerenciamento de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### Práticas recomendadas para configurar tarefas e problemas {#best-practices-for-setting-up-tasks-and-issues}

Verifique se a seguinte configuração de tarefa e problema existe antes de começar a atribuir trabalho aos usuários no Balanceador de Carga de Trabalho:

* As tarefas pai não são atribuídas a usuários ou funções. Eles não são exibidos no Balanceador de Carga de Trabalho.
* Tarefas e problemas têm um valor para Horas Planejadas que é maior que zero.

* Tarefas e problemas têm um valor para a Duração, que é maior que zero.
* As Datas Planejadas dos problemas estão na linha do tempo do projeto.

## Antes de começar a usar o Balanceador de Carga de Trabalho

* Você pode usar o Balanceador de Carga de Trabalho para atribuir trabalho e gerenciar alocações diárias para usuários em sua organização.

   Este artigo aborda como navegar pelo Balanceador de Carga de Trabalho para executar estas ações: [Navegar pelo Balanceador de Carga de Trabalho](../workload-balancer/navigate-the-workload-balancer.md).

   Os artigos a seguir o orientam sobre como você atribui trabalhos e gerencia alocações de usuários:

   * [Visão Geral da atribuição de trabalho no Balanceador de Carga de Trabalho](../workload-balancer/assign-work-in-workload-balancer.md).
   * [Gerenciar alocações de usuários no Balanceador de Carga de Trabalho](../workload-balancer/manage-user-allocations-workload-balancer.md).

* O Balanceador de carga de trabalho pode ser localizado em várias áreas diferentes do Workfront. Para obter informações sobre onde você pode encontrar o Balanceador de Carga de Trabalho, consulte [Localizar o Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Acesso necessário para usar o Balanceador de Carga de Trabalho

Você deve ter o acesso e as permissões corretas do Workfront para projetos específicos para visualizar e usar o Balanceador de carga de trabalho no Workfront. Para obter informações sobre o acesso necessário para usar o Balanceador de Carga de Trabalho, consulte o artigo [Acesso necessário para gerenciar recursos no Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
