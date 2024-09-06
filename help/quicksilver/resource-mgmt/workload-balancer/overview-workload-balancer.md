---
content-type: overview
product-area: resource-management
navigation-topic: the-workload-balancer
title: Visão geral do Balanceador de carga de trabalho
description: Depois que os gerentes de projeto planejam o trabalho nos projetos criando tarefas e depois que os gerentes de recursos alocam os recursos da função de trabalho aos projetos no Planejador de Recursos, os proprietários de projetos e gerentes de equipe podem usar o Balanceador de carga de trabalho para atribuir itens de trabalho aos usuários.
author: Lisa
feature: Resource Management
exl-id: 9398bd04-9df7-4b77-8361-fdb5bdce6829
source-git-commit: db0aab0e6e7e896a8e7c0afe2da709de7c3c2a4e
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 0%

---

# Visão geral do Balanceador de carga de trabalho

<!--
<p>(NOTE: this is linked from the UI for the Workload Balancer page. DO NOT CHANGE TITLE OR LINK) </p>
-->

Depois que os gerentes de projeto planejam o trabalho nos projetos criando tarefas e depois que os gerentes de recursos alocam os recursos da função de trabalho aos projetos no Planejador de Recursos, os proprietários de projetos e gerentes de equipe podem usar o Balanceador de carga de trabalho para atribuir itens de trabalho aos usuários.

>[!IMPORTANT]
>
>Você pode usar o Balanceador de carga de trabalho para atribuir trabalho real (tarefas e problemas) aos usuários.
>
>Você deve usar o Planejador de recursos e não o Balanceador de carga de trabalho para estimar as alocações de funções de trabalho para seus projetos, em um nível superior. Para obter mais informações sobre o Planejador de recursos, consulte [Visão geral do Planejador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Este artigo descreve o objetivo geral do Balanceador de carga de trabalho e algumas práticas recomendadas para como você pode configurar seus projetos e recursos para usá-lo com êxito.

Para examinar os tutoriais em vídeo do Balanceador de carga de trabalho, acesse a página [Tutorials do Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=pt-BR). No menu esquerdo, selecione **Gerenciar recursos** > **Balanceador de carga de trabalho** e escolha um tutorial.

## Localize o Balanceador de carga de trabalho

<!--
<p>(NOTE: This will be taken out when all we will have is one tool - should be replaced by a blurb that says you can add this tool anywhere, in any custom tab, etc (long term dev promise)) </p>
-->

Recomendamos o uso do Balanceador de carga de trabalho nas seguintes áreas para agendar recursos:

* No nível do sistema, na área Recursos.
* No nível do projeto, na seção Balanceador de carga de trabalho de um projeto.
* No nível da equipe, na seção Balanceador de carga de trabalho de uma equipe.

Para obter mais informações sobre como localizar o Balanceador de carga de trabalho, consulte [Localizar o Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Benefícios do Balanceador de carga de trabalho

Considere os seguintes benefícios ao usar o Balanceador de carga de trabalho:

<!--
<p> Add about the what-if scenarios as a benefit when they become available </p>
-->

* Acessar um mapeamento visual claro de superalocação e subutilização de recursos que seja transparente para todas as partes interessadas.
* Como gerente de pessoas, você pode proteger seus funcionários contra esgotamento e capacitá-los a fazer seu melhor trabalho com mais foco, qualidade e envolvimento. Você pode garantir a utilização total, romper silos e habilitar o alinhamento do trabalho entre equipes.
* Ao atribuir um trabalho no nível de tarefa ou problema, você não tem visibilidade sobre o quão ocupado um usuário pode estar. Ao usar o Balanceador de carga de trabalho, você pode visualizar quais usuários têm disponibilidade em sua carga de trabalho para concluir a tarefa ou o problema no prazo. Isso inclui os detalhes de folga e exceções da programação.

  Para obter mais informações, consulte [Visão geral da atribuição de trabalho no Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

  Você também pode atribuir itens de trabalho em massa, o que facilita a distribuição de muitos itens de trabalho de uma vez, em vários projetos. Para obter mais informações, consulte [Atribuir trabalho em massa usando o Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

* Os executivos podem tomar decisões oportunas sobre a equipe por meio da transparência na forma como as pessoas em sua organização são utilizadas.
* Os membros da equipe se beneficiam de uma melhor colaboração, pois todos podem visualizar no que seus colegas de trabalho estão trabalhando a qualquer momento. Para obter informações sobre o acesso necessário para exibir ou gerenciar recursos no Balanceador de carga de trabalho, consulte [Acesso necessário para gerenciar recursos no Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
* Compartilhe-o com qualquer pessoa que não tenha acesso à área de Recursos, incorporando um link a ela em uma guia personalizada. Para obter informações, consulte [Compartilhar o Balanceador de Carga de Trabalho com um link](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md)
* Visualize e gerencie as cargas de trabalho e a demanda das pessoas em uma visualização no nível global, de projeto ou de equipe, dependendo da sua função. Ao gerenciar projetos, isso inclui não apenas a alocação de recursos para o projeto, mas também a visualização da alocação de recursos do Planejador de cenários do Adobe Workfront. Os gerentes de pessoas usam o Planejador de Cenários da Workfront para gerenciar habilidades de cargo na organização. O Planejador de cenários só está disponível na nova experiência do Adobe Workfront.

  >[!NOTE]
  >
  >  O Planejador de cenários requer uma licença adicional. Para obter informações sobre o Planejador de cenários do Workfront, consulte [A visão geral do Planejador de cenários](../../scenario-planner/scenario-planner-overview.md).


## Práticas recomendadas para usar o Balanceador de carga de trabalho

Recomendamos as seguintes práticas recomendadas para planejar projetos, configurar usuários e usar filtros antes de começar a agendar seus recursos usando o Balanceador de carga de trabalho.

* [Práticas recomendadas para exibir informações no Balanceador de carga de trabalho](#best-practices-for-displaying-information-in-the-workload-balancer)
* [Práticas recomendadas para configurar usuários](#best-practices-for-setting-up-users)
* [Práticas recomendadas para configurar tarefas e problemas](#best-practices-for-setting-up-tasks-and-issues)

### Práticas recomendadas para exibir informações no Balanceador de carga de trabalho {#best-practices-for-displaying-information-in-the-workload-balancer}

Recomendamos que você use filtros para exibir apenas as informações pertinentes a você, tanto para itens de trabalho não atribuídos quanto para itens de trabalho atribuídos.

Para obter informações sobre como criar e usar filtros no Balanceador de carga de trabalho, consulte [Informações de filtro no Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

### Práticas recomendadas para configurar usuários

* Como o usuário que agenda o trabalho para outros, você deve ter o acesso e as permissões corretas para agendar recursos para o trabalho.

  Para obter informações sobre o acesso necessário para gerenciar a carga de trabalho de seus recursos no Balanceador de carga de trabalho, consulte [Acesso necessário para gerenciar recursos no Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

* Os usuários cuja carga de trabalho você deseja gerenciar devem atender aos seguintes critérios para que as informações sobre sua disponibilidade e habilidades sejam precisas:

   * Têm Cronogramas e Funções de trabalho associados aos seus perfis.

     Para obter mais informações sobre como associar agendas e funções de trabalho a usuários, consulte [Adicionar usuários](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)
   * Se um usuário não estiver associado a um Cronograma, o Cronograma Padrão do seu sistema Workfront será associado ao usuário por padrão, para fins de gerenciamento de recursos.
   * Têm Exceções de Programação atualizadas em suas programações.

     Para obter mais informações sobre como criar agendas, consulte [Criar uma agenda](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

   * Atualize o calendário de Folga no perfil.

     Para obter informações sobre como atualizar o calendário de folga de um usuário, consulte [Configurar folga pessoal](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

     <!--   
     <div data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <p>(NOTE: Add another bullet for Costs, when this becomes available:</p>   
     <p>If you want to budget your resources by Cost, you must associate Job Roles with Cost/ Hr. rates. The cost associated with Job Roles assigned to users in your Resource Pools is used to calculate the Budgeted Labor Cost and the Budgeted Cost of the project.For more information about associating job roles with rates, see the article Creating and Managing Job Roles in the new Adobe Workfront experience.For more information about calculating Budgeted Labor Cost, see the article Calculating Budgeted Labor Cost in the new Adobe Workfront experience.For more information about calculating Budgeted Cost, see the article Calculating Budgeted Cost in .) </p>   
     </div>   
     -->

* O administrador do Workfront deve determinar como o Workfront calcula a disponibilidade do usuário. Eles podem decidir se o Workfront usa a Programação Padrão do Sistema ou a programação do usuário para calcular o tempo em que o usuário estará disponível para trabalhar ajustando as preferências do Gerenciamento de Recursos na área Configuração do Workfront.

  Para obter mais informações, consulte [Configurar preferências de Gerenciamento de Recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### Práticas recomendadas para configurar tarefas e problemas {#best-practices-for-setting-up-tasks-and-issues}

Verifique se a seguinte configuração de tarefa e problema existe antes de começar a atribuir trabalho aos usuários no Balanceador de carga de trabalho:

* As tarefas pai não são atribuídas a usuários ou funções. As tarefas pai não são exibidas no Balanceador de carga de trabalho.
* Tarefas e problemas têm um valor para Horas planejadas maior que zero.

* Tarefas e problemas têm um valor para a Duração maior que zero.
* As datas planejadas dos problemas estão dentro da linha do tempo do projeto.

## Antes de começar a usar o Balanceador de carga de trabalho

* Revise os seguintes artigos antes de começar a usar o Balanceador de carga de trabalho:

   * Este artigo mostra como navegar no Balanceador de carga de trabalho para executar estas ações: [Navegar pelo Balanceador de carga de trabalho](../workload-balancer/navigate-the-workload-balancer.md).

   * Os artigos a seguir o orientam sobre como atribuir trabalho e gerenciar alocações de usuário:

      * [Visão geral da atribuição de trabalho no Balanceador de carga de trabalho](../workload-balancer/assign-work-in-workload-balancer.md).
      * [Gerenciar alocações de usuário no Balanceador de Carga de Trabalho](../workload-balancer/manage-user-allocations-workload-balancer.md).

* O Balanceador de carga de trabalho pode ser encontrado em várias áreas diferentes do Workfront. Para obter informações sobre onde encontrar o Balanceador de carga de trabalho, consulte [Localizar o Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Acesso necessário para usar o Balanceador de carga de trabalho

Você deve ter o acesso e as permissões corretas do Workfront para projetos específicos para visualizar e usar o Balanceador de carga de trabalho no Workfront. Para obter informações sobre o acesso necessário para usar o Balanceador de carga de trabalho, consulte o artigo [Acesso necessário para gerenciar recursos no Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
