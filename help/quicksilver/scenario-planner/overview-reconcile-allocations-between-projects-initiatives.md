---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Visão geral da reconciliação de alocações de recursos entre projetos e iniciativas
description: Visão geral da reconciliação de alocações de recursos entre projetos e iniciativas
author: Alina
feature: Workfront Scenario Planner
exl-id: 82cd9641-1213-436c-935a-2f04a0425e9c
source-git-commit: 86ee649cdf0ac04230035a94a1326c45b67d36d2
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---

# Visão geral da reconciliação de alocações de recursos entre projetos e iniciativas

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: two more articles were added to split content from here according to where the reconciling can happen) </p>
-->

Você pode conectar projetos a iniciativas para garantir que seus planos estratégicos e o trabalho real estejam em sincronia. Ao destacar seus planos estratégicos e iniciativas no [!DNL Scenario Planner] e planejar o trabalho real em um projeto, você pode garantir que seus recursos sejam compatíveis com o projeto e com as iniciativas, evitando, assim, superalocar ou subutilizar esses recursos.

## Pré-requisitos

Antes de começar, você deve ter o seguinte:

* Um plano no [!DNL Scenario Planner] com uma iniciativa conectada a um projeto.
* Alocações de funções de trabalho necessárias para a iniciativa.
* Tarefas ou problemas no projeto que têm Horas planejadas e estão atribuídos a um dos seguintes itens:

   * Funções de trabalho
   * Usuários associados a funções de trabalho

## Conectar projetos e iniciativas

>[!NOTE]
>
>Você pode criar iniciativas e conectá-las a projetos somente se sua organização tiver comprado uma licença adicional para o [!DNL Workfront Scenario Planner].

Você pode conectar projetos a iniciativas seguindo um destes procedimentos:

* Importar projetos para um plano, como novas iniciativas

  Para obter mais informações, consulte [Importar projetos para planos na [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Publicar iniciativas nos projetos

  Para obter mais informações, consulte [Atualizar ou criar projetos publicando iniciativas em [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

Ambos os processos criam uma conexão entre os projetos e suas iniciativas correspondentes. Depois de conectá-los, é possível gerenciar as alocações de recursos comparando-os e garantindo a correspondência entre eles.

## Considerações sobre a reconciliação de recursos em projetos e iniciativas vinculados

>[!NOTE]
>
>Você pode exibir iniciativas, conectá-las a projetos e exibir suas alocações de recursos em um projeto somente se sua organização tiver comprado uma licença adicional para o [!DNL Workfront Scenario Planner].

* É possível atribuir usuários, equipes e funções de trabalho a itens de trabalho em um projeto e atribuir funções de trabalho a iniciativas. Como resultado, só é possível reconciliar funções de trabalho entre projetos e iniciativas.

  >[!TIP]
  >
  >Para reconciliar o tempo dos usuários em um projeto com as alocações de função nas iniciativas, você deve associar usuários com funções de trabalho.

* Você pode exibir a alocação de funções de trabalho da iniciativa em um projeto vinculado nas seguintes áreas do projeto:

   * Seção [!DNL Scenario Planner] da área [!UICONTROL Detalhes do projeto] em um projeto. Para obter mais informações, consulte os seguintes artigos:

      * [Atualizar ou criar projetos publicando iniciativas em [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)
      * [Gerenciar informações na área [!UICONTROL Visão geral] do projeto](../manage-work/projects/manage-projects/understand-project-overview-area.md)

     >[!TIP]
     >
     >Você não pode ver as informações de função de trabalho do projeto e da iniciativa lado a lado na seção [!DNL Scenario Planner] dos [!UICONTROL Detalhes do projeto].

   * O painel [!UICONTROL Alocação de Função] nas seguintes áreas:

      * [!UICONTROL Balanceador de carga de trabalho] do projeto

        Para obter informações sobre como visualizar e reconciliar as alocações de funções entre a iniciativa e o projeto vinculado no [!UICONTROL Balanceador de carga de trabalho], consulte [Mostrar alocação de funções para projetos e iniciativas no [!UICONTROL Balanceador de carga de trabalho]](../scenario-planner/show-role-allocation-workload-balancer.md).

      * Seção [!UICONTROL Tarefas]

        Para obter informações sobre como reconciliar as alocações de funções entre a iniciativa e o projeto vinculado na seção [!UICONTROL Tarefas], consulte [Mostrar alocação de funções para projetos e iniciativas na lista de tarefas](../scenario-planner/show-role-allocation-task-list-nwe.md).

     >[!TIP]
     >
     >Você pode ver as informações de função do trabalho do projeto e da iniciativa lado a lado no painel [!UICONTROL Alocação de função].

* Não é possível exibir a alocação de funções de trabalho para um projeto em uma iniciativa vinculada. Para obter mais informações, consulte [Importar projetos para planos na [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this might change - project job role visibility into initiative)
  </MadCap:conditionalText>
  -->
