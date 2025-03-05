---
product-area: resource-management
keywords: trabalho,equipe,equipe,recursos
navigation-topic: the-workload-balancer
title: Localize o Balanceador de carga de trabalho
description: Você pode usar o Balanceador de carga de trabalho para agendar recursos para trabalho ou revisar sua disponibilidade e alocações atuais.
author: Lisa
feature: Resource Management
exl-id: 88029c9d-b588-4d33-801a-04f49b12a6e8
source-git-commit: 496420d1c74b7c29d0fb2ff7109ea8478680d117
workflow-type: tm+mt
source-wordcount: '724'
ht-degree: 1%

---

# Localize o Balanceador de carga de trabalho

Você pode usar o Balanceador de carga de trabalho para agendar recursos para trabalho ou revisar sua disponibilidade e alocações atuais.

Você pode acessar o Balanceador de carga de trabalho das seguintes maneiras:

* De várias áreas predefinidas pelo Adobe Workfront
* Ao adicioná-lo a uma seção personalizada

Este artigo descreve as áreas em que você pode acessar o Balanceador de carga de trabalho.

>[!NOTE]
>
>Independentemente do método usado para acessar o Balanceador de carga de trabalho, navegá-lo e gerenciar recursos é idêntico.
>
>Para obter informações sobre o Balanceador de carga de trabalho e como usá-lo para gerenciar e programar seus recursos para trabalho, consulte os seguintes artigos:
>
>* [Visão geral do Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)
>* [Navegar pelo Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)
>* [Visão geral da atribuição de trabalho no Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)
>* [Gerenciar alocações de usuário no Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Novo: Padrão</p>
       <p>ou</p>
       <p>Atual: plano, ao usar o Balanceador de Carga de Trabalho na área Recursos;</br>
       Trabalhar, ao usar o Balanceador de carga de trabalho de uma equipe ou projeto</p></td>
  </tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Visualize ou tenha acesso superior ao seguinte:</p> 
    <ul> 
     <li>Gerenciamento de recursos</li> 
     <li>Projetos</li> 
     <li>Tarefas</li> 
     <li>Problemas</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td>Exibir permissões ou permissões superiores para projetos, tarefas e problemas</td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Acessar o Balanceador de carga de trabalho em áreas predefinidas

As seções a seguir ilustram onde você pode acessar o Balanceador de carga de trabalho no Workfront.

### Acesse o Balanceador de carga de trabalho para vários projetos na área Recursos

{{step1-to-resourcing}}

1. Clique em **Balanceador de carga de trabalho** no painel esquerdo.

   ![Balanceador de carga de trabalho](assets/nwe-balancer-global.png)

   O Balanceador de carga de trabalho exibe as seguintes informações na área Recursos, por padrão:

   * **Trabalho não atribuído**: nenhum item de trabalho não atribuído.
   * **Trabalho atribuído**: todos os usuários ativos no sistema.

     Recomendamos o uso de filtros ao exibir usuários na área Trabalho atribuído. Para obter mais informações, consulte [Informações de filtro no Balanceador de carga de trabalho](../workload-balancer/filter-information-workload-balancer.md).

### Acessar o Balanceador de carga de trabalho de uma equipe

Para obter mais informações sobre equipes no Workfront, consulte [Visão geral das equipes](/help/quicksilver/people-teams-and-groups/create-and-manage-teams/teams-overview.md).

{{step1-to-team}}

A página da sua equipe inicial é exibida.

1. Clique em **Balanceador de carga de trabalho** no painel esquerdo.

   ![Balanceador de carga de trabalho para a equipe](assets/nwe-balancer-team-350x172.png)

   O Balanceador de carga de trabalho de uma equipe exibe as seguintes informações, por padrão:

   * **Trabalho não atribuído**: itens atribuídos à equipe e não atribuídos a usuários.
   * **Trabalho atribuído**: todos os membros da equipe com todas as suas atribuições.

     >[!TIP]
     >
     >Os membros da equipe podem ser atribuídos a trabalhos também atribuídos à equipe ou a trabalhos atribuídos a outras equipes ou funções.

### Acessar o Balanceador de carga de trabalho de um projeto

{{step1-to-projects}}

1. Clique no nome de um projeto para abrir a página.
1. Clique em **Balanceador de carga de trabalho** no painel esquerdo. Talvez seja necessário clicar em **Mostrar Mais** e depois em **Balanceador de Carga de Trabalho**.

   O Balanceador de carga de trabalho do projeto é exibido.

   ![Balanceador de carga de trabalho para o projeto](assets/nwe-balancer-project-350x152.png)

   O Balanceador de carga de trabalho de um projeto exibe as seguintes informações por padrão:

   * **Trabalho não atribuído**: itens do projeto que são atribuídos a funções de trabalho ou equipes e não são atribuídos a usuários.
   * **Trabalho atribuído**: usuários atribuídos a itens no projeto.

     >[!TIP]
     >
     >Você pode exibir todos os usuários no sistema em vez de somente os do projeto (na área Trabalho atribuído ) ativando a opção Mostrar todos os usuários. Para obter informações, consulte [Navegar pelo Balanceador de Carga de Trabalho](../workload-balancer/navigate-the-workload-balancer.md).


## Adicionar o Balanceador de carga de trabalho a uma seção personalizada

Você pode adicionar o Balanceador de carga de trabalho a qualquer seção personalizada.

A maioria das personalizações já aplicadas ao Balanceador de carga de trabalho é preservada ao adicioná-lo a uma seção personalizada.

1. Acesse o Balanceador de carga de trabalho indo para qualquer uma das seguintes áreas:

   * A área Recursos
   * Uma equipe
   * Um projeto

1. Obtenha um link compartilhável e copie-o para a área de transferência conforme descrito em [Compartilhar o Balanceador de carga de trabalho com um link](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md).
1. Crie um painel com uma página externa conforme descrito em [Incorporar uma página da Web externa em um painel](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md). Use o link compartilhável obtido na Etapa 2 para a página externa.

   <!--
      (NOTE: ensure this stays correct)
      -->

1. Crie uma seção personalizada conforme descrito em [Criar guias ou seções personalizadas](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md) para colocar o painel na guia personalizada.

   Ao acessar o Balanceador de carga de trabalho na seção personalizada, você pode visualizá-lo como se o estivesse acessando diretamente de uma de suas áreas originais listadas na Etapa 1.

   <!--
      (NOTE: ensure this stays correct)
     -->

1. (Opcional) Compartilhe a guia personalizada em um Modelo de layout conforme descrito em [Personalizar o painel esquerdo usando um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).


<!--
For a team:

* From the Workload Balancer section of a team.

  You can adjust allocations and review or assign work from multiple projects to individual team members.

For a project:

  You can do the following when you use the Workload Balancer within a project:

   * Assign work on the project to users already assigned other work on the project.
   * Assign work to any user that might not be on the project.

   * View additional work that users are assigned to on other projects.
   * Adjust user allocations to work items.-->