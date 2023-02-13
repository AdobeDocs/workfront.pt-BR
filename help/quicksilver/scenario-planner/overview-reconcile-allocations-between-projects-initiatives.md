---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Visão geral da reconciliação das alocações de recursos entre projetos e iniciativas
description: Visão geral da reconciliação das alocações de recursos entre projetos e iniciativas
author: Alina
feature: Workfront Scenario Planner
exl-id: 82cd9641-1213-436c-935a-2f04a0425e9c
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# Visão geral da reconciliação das alocações de recursos entre projetos e iniciativas

>[!IMPORTANT]
>
>Sua organização deve comprar uma licença adicional para a [!DNL Adobe Workfront Scenario Planner] para que você possa visualizar as informações da iniciativa em um projeto. Para obter informações sobre como obter o [!DNL Workfront Scenario Planner], consulte [Acesso necessário para usar o Planejador de cenário](../scenario-planner/access-needed-to-use-sp.md) .

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: two more articles were added to split content from here according to where the reconciling can happen) </p>
-->

Você pode conectar projetos com iniciativas para garantir que seus planos estratégicos e o trabalho real estejam sincronizados. Conforme você esboça seus planos estratégicos e iniciativas na [!DNL Scenario Planner] e você planeja o trabalho real em um projeto, você pode garantir que os recursos no projeto e nas iniciativas correspondam, de modo que você não irá realocá-los ou subutilizá-los.

## Pré-requisitos

Antes de começar, você deve ter o seguinte:

* Um plano no [!DNL Scenario Planner] com uma iniciativa ligada a um projeto.
* Atribuições de funções de emprego necessárias para a iniciativa.
* Tarefas ou problemas no projeto que têm Horas Planejadas e são atribuídos a um dos seguintes:

   * Funções de trabalho
   * Usuários associados a funções de trabalho

## Conectar projetos e iniciativas

>[!NOTE]
>
>Você pode criar iniciativas e conectá-las a projetos somente se sua organização tiver comprado uma licença adicional para a [!DNL Workfront Scenario Planner].

Você pode conectar projetos a iniciativas seguindo um destes procedimentos:

* Importar projetos para um plano como novas iniciativas

   Para obter mais informações, consulte [Importar projetos para planos na [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Publicar iniciativas em projetos

   Para obter mais informações, consulte [Atualize ou crie projetos publicando iniciativas no [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) .

Ambos os processos criam uma conexão entre os projetos e suas iniciativas correspondentes. Depois de conectá-las, você poderá gerenciar suas alocações de recursos comparando-as e garantindo a correspondência.

## Considerações sobre a reconciliação de recursos em projetos e iniciativas vinculadas

>[!NOTE]
>
>Você pode visualizar iniciativas, conectá-las a projetos e exibir suas alocações de recursos em um projeto somente se sua organização tiver comprado uma licença adicional para a [!DNL Workfront Scenario Planner].

* Você pode atribuir usuários, equipes e funções de trabalho a itens de trabalho em um projeto e pode atribuir funções de trabalho a iniciativas. Como resultado, você só pode reconciliar funções de trabalho entre projetos e iniciativas.

   >[!TIP]
   >
   >Para reconciliar o tempo dos usuários em um projeto com alocações de função nas iniciativas, você deve associar os usuários com funções de cargo.

* Você pode visualizar a alocação de função de trabalho de iniciativa em um projeto vinculado nas seguintes áreas do projeto:

   * [!DNL Scenario Planner] da seção [!UICONTROL Detalhes do projeto] em um projeto. Para obter mais informações, consulte os seguintes artigos:

      * [Atualize ou crie projetos publicando iniciativas no [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)
      * [Gerenciar informações no projeto [!UICONTROL Visão geral] area](../manage-work/projects/manage-projects/understand-project-overview-area.md)

      >[!TIP]
      >
      >Você não pode ver informações de função de emprego do projeto e da iniciativa lado a lado no [!DNL Scenario Planner] da seção [!UICONTROL Detalhes do projeto].

   * O [!UICONTROL Alocação de função] nas seguintes áreas:

      * [!DNL Workload Balancer] do projeto

         Para obter informações sobre como visualizar e reconciliar as atribuições entre a iniciativa e o projeto vinculado na [!DNL Workload Balancer], consulte [Mostrar alocação de função para projetos e iniciativas no [!DNL Workload Balancer]](../scenario-planner/show-role-allocation-workload-balancer.md).

      * [!UICONTROL Tarefas] seção

         Para obter informações sobre como reconciliar as atribuições entre a iniciativa e o projeto vinculado na [!UICONTROL Tarefas] seção , consulte [Mostrar alocação de funções para projetos e iniciativas na lista de tarefas](../scenario-planner/show-role-allocation-task-list-nwe.md).
      >[!TIP]
      >
      >Você pode ver informações sobre a função no trabalho do projeto e da iniciativa lado a lado no [!UICONTROL Alocação de função] painel.



* Não é possível visualizar a alocação de função de cargo para um projeto em uma iniciativa vinculada. Para obter mais informações, consulte [Importar projetos para planos na [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this might change - project job role visibility into initiative)
  </MadCap:conditionalText>
  -->
