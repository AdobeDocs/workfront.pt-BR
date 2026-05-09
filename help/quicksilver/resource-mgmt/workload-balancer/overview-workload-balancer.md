---
content-type: overview
product-area: resource-management
navigation-topic: the-workload-balancer
title: Visão geral do balanceador de carga de trabalho
description: Depois que gerentes de projeto planejam o trabalho nos projetos criando tarefas e gerentes de recursos alocam recursos de funções de trabalho aos projetos no planejador de recursos, os proprietários do projeto e gerentes de equipe podem usar o Balanceador de carga de trabalho para atribuir itens de trabalho aos usuários.
author: Lisa
feature: Resource Management
exl-id: 9398bd04-9df7-4b77-8361-fdb5bdce6829
source-git-commit: 9e217d36d5aeb36761a9a433b84e73ac2b7a114b
workflow-type: tm+mt
source-wordcount: '1202'
ht-degree: 100%

---

# Visão geral do Balanceador de carga de trabalho {#workload-balancer-overview}

>[!CONTEXTUALHELP]
>id="wf-resourcing-workload-balancer"
>title="Balanceador de carga de trabalho"
>abstract="Os proprietários do projeto e os gerentes de equipe podem usar o Balanceador de carga de trabalho para atribuir itens de trabalho aos usuários."

<!--
<p>(NOTE: this is linked from the UI for the Workload Balancer page. DO NOT CHANGE TITLE OR LINK) </p>
-->

Depois que gerentes de projeto planejam o trabalho nos projetos criando tarefas e gerentes de recursos alocam recursos de funções de trabalho aos projetos no planejador de recursos, os proprietários do projeto e gerentes de equipe podem usar o Balanceador de carga de trabalho para atribuir itens de trabalho aos usuários.

>[!IMPORTANT]
>
>Você pode usar o Balanceador de carga de trabalho para atribuir tarefas reais (tarefas e problemas) aos usuários.
>
>Você deve usar o planejador de recursos e não o Balanceador de carga de trabalho para estimar as alocações de funções de trabalho para seus projetos em nível geral. Para obter mais informações sobre o planejador de recursos, consulte [Visão geral do planejador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Este artigo descreve a finalidade geral do Balanceador de carga de trabalho e algumas das práticas recomendadas para configurar seus projetos e recursos, a fim de usá-lo de forma eficiente.

Para examinar os tutoriais em vídeo do Balanceador de carga de trabalho, acesse a página [Tutoriais do Workfront](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home?lang=pt-BR). No menu esquerdo, selecione **Gerenciar recursos** > **Balanceador de carga de trabalho** e escolha um tutorial.

## Localize o Balanceador de carga de trabalho

<!--
<p>(NOTE: This will be taken out when all we will have is one tool - should be replaced by a blurb that says you can add this tool anywhere, in any custom tab, etc (long term dev promise)) </p>
-->

Recomendamos o uso do Balanceador de carga de trabalho nas seguintes áreas para agendar recursos:

* No nível do sistema, na área de Recursos.
* No nível do projeto, na seção Balanceador de carga de trabalho de um projeto.
* No nível da equipe, na seção Balanceador de carga de trabalho de uma equipe.

Para obter mais informações sobre como localizar o Balanceador de carga de trabalho, consulte [Localizar o Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Benefícios do Balanceador de carga de trabalho

Considere os seguintes benefícios ao usar o Balanceador de carga de trabalho:

<!--
<p> Add about the what-if scenarios as a benefit when they become available </p>
-->

* Acesso a uma visão geral clara da alocação excessiva e subutilização de recursos, que é transparente para todas as partes interessadas.
* Como gestor de pessoas, você pode proteger funcionários(as) contra o esgotamento e capacitá-los(as) a realizar seu trabalho com mais foco, qualidade e engajamento. Você pode garantir sua plena utilização, quebrar silos e habilitar o alinhamento do trabalho entre as equipes.
* Ao atribuir trabalhos no nível da tarefa ou do problema, você não pode ver o nível de ocupação de um usuário. Por meio do Balanceador de carga de trabalho, é possível visualizar quais usuários têm disponibilidade em sua carga de trabalho para concluir a tarefa ou o problema no prazo. Isso inclui detalhes sobre suas folgas e exceções de cronograma.

  Para obter mais informações, consulte [Visão geral da atribuição de trabalho no Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

  Você também pode atribuir itens de trabalho em massa, o que facilita a distribuição de muitos itens de trabalho de uma vez, para vários projetos. Para obter mais informações, consulte [Atribuir trabalho em massa usando o Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

* A equipe executiva pode tomar decisões oportunas sobre funcionários(as) por meio da transparência na forma como as pessoas em sua organização são utilizadas.
* Membros da equipe se beneficiam de uma melhor colaboração, pois qualquer pessoa pode ver em que seus colegas estão trabalhando a qualquer momento. Para obter informações sobre o acesso necessário para exibir ou gerenciar recursos no Balanceador de carga de trabalho, consulte [Acesso necessário para gerenciar recursos no Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
* Compartilhe-o com qualquer pessoa que não tenha recursos no menu principal, incorporando um link para ele em uma guia personalizada. Para obter informações, consulte [Compartilhar o Balanceador de carga de trabalho por meio de um link](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md).
* Visualize e gerencie as cargas de trabalho e a demanda das pessoas em uma visualização de nível global, de projeto ou de equipe, dependendo da sua função. Ao gerenciar projetos, isso inclui não apenas a alocação de recursos para o projeto, mas também a visualização da alocação de recursos do planejador de cenários do Adobe Workfront. Gerentes de pessoas usam o planejador de cenários do Workfront para gerenciar habilidades de trabalho na organização. O planejador de cenários só está disponível na nova experiência do Adobe Workfront.

  >[!NOTE]
  >
  >  O planejador de cenários requer uma licença adicional. Para obter informações sobre o planejador de cenários do Workfront, consulte [Visão geral do planejador de cenários](../../scenario-planner/scenario-planner-overview.md).


## Práticas recomendadas para usar o Balanceador de carga de trabalho

Estas são as práticas recomendadas para planejar projetos, configurar usuários e usar filtros antes de começar a programar seus recursos por meio do Balanceador de carga de trabalho.

* [Práticas recomendadas para exibir informações no Balanceador de carga de trabalho](#best-practices-for-displaying-information-in-the-workload-balancer)
* [Práticas recomendadas para configurar usuários](#best-practices-for-setting-up-users)
* [Práticas recomendadas para configurar tarefas e problemas](#best-practices-for-setting-up-tasks-and-issues)

### Práticas recomendadas para exibir informações no Balanceador de carga de trabalho {#best-practices-for-displaying-information-in-the-workload-balancer}

Recomendamos que você use filtros para exibir apenas as informações pertinentes a você, tanto para itens de trabalho não atribuídos quanto para itens de trabalho atribuídos.

Para obter informações sobre como criar e usar filtros no Balanceador de carga de trabalho, consulte [Informações de filtro no Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

### Práticas recomendadas para configurar usuários

* Como usuário responsável por programar o trabalho de outras pessoas, você deve ter o acesso e as permissões corretas para programar recursos para o trabalho.

  Para obter informações sobre o acesso necessário para gerenciar a carga de trabalho dos seus recursos no Balanceador de carga de trabalho, consulte [Acesso necessário para gerenciar recursos no Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

* Os usuários cuja carga de trabalho você deseja gerenciar devem atender aos seguintes critérios para que as informações sobre sua disponibilidade e habilidades sejam precisas:

   * Ter horários e funções de trabalho associados ao seu perfil.

     Para obter mais informações sobre como associar programações e funções de trabalho a usuários, consulte [Adicionar usuários](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)
   * Se um usuário não estiver associado a um cronograma, o cronograma padrão do seu sistema do Workfront será associado ao usuário por padrão, para fins de gerenciamento de recursos.
   * Ter exceções de cronograma atualizadas em seus cronogramas.

     Para obter mais informações sobre como criar cronogramas, consulte [Criar um cronograma](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

   * Ter seu calendário de folgas atualizado no perfil.

     Para obter informações sobre como atualizar o calendário de folgas de um usuário, consulte [Configurar folga pessoal](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

     <!--   
     <div data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <p>(NOTE: Add another bullet for Costs, when this becomes available:</p>   
     <p>If you want to budget your resources by Cost, you must associate Job Roles with Cost/ Hr. rates. The cost associated with Job Roles assigned to users in your Resource Pools is used to calculate the Budgeted Labor Cost and the Budgeted Cost of the project.For more information about associating job roles with rates, see the article Creating and Managing Job Roles in the new Adobe Workfront experience.For more information about calculating Budgeted Labor Cost, see the article Calculating Budgeted Labor Cost in the new Adobe Workfront experience.For more information about calculating Budgeted Cost, see the article Calculating Budgeted Cost in .) </p>   
     </div>   
     -->

* O(a) admin do Workfront deve determinar como o Workfront calcula a disponibilidade do usuário. É possível definir se o Workfront usa o cronograma padrão do sistema ou o cronograma do usuário para calcular o tempo disponível para trabalhar ajustando as preferências de gerenciamento de recursos na área de configuração do Workfront.

  Para obter mais informações, consulte [Configurar preferências de gerenciamento de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### Práticas recomendadas para configurar tarefas e problemas {#best-practices-for-setting-up-tasks-and-issues}

Certifique-se de que a seguinte configuração de tarefas e problemas exista antes de começar a atribuir trabalhos aos usuários no Balanceador de carga de trabalho:

* As tarefas principais não são atribuídas a usuários ou funções. As tarefas principais não são exibidas no Balanceador de carga de trabalho.
* Tarefas e problemas têm um valor de Horas planejadas maior que zero.

* Tarefas e problemas têm um valor de Duração é maior que zero.
* As Datas planejadas dos problemas estão dentro da linha do tempo do projeto.

## Antes de começar a usar o Balanceador de carga de trabalho

* Revise os seguintes artigos antes de começar a usar o Balanceador de carga de trabalho:

   * Este artigo mostra como navegar no Balanceador de carga de trabalho para executar estas ações: [Navegar pelo Balanceador de carga de trabalho](../workload-balancer/navigate-the-workload-balancer.md).

   * Os artigos a seguir fornecem instruções sobre como atribuir trabalhos e gerenciar alocações de usuário:

      * [Visão geral da atribuição de trabalhos no Balanceador de carga de trabalho](../workload-balancer/assign-work-in-workload-balancer.md).
      * [Gerenciar alocações de usuários no Balanceador de carga de trabalho](../workload-balancer/manage-user-allocations-workload-balancer.md).

* O Balanceador de carga de trabalho pode ser encontrado em várias áreas diferentes do Workfront. Para obter informações sobre onde encontrar o Balanceador de carga de trabalho, consulte [Localizar o Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Acesso necessário para usar o Balanceador de carga de trabalho

Você deve ter o acesso e as permissões corretas do Workfront para projetos específicos para visualizar e usar o Balanceador de carga de trabalho no Workfront. Para obter informações sobre o acesso necessário para usar o Balanceador de carga de trabalho, consulte o artigo [Acesso necessário para gerenciar recursos no Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
