---
navigation-topic: business-case-and-scorecards
title: Recursos de orçamento no Caso de negócios usando o Planejador de cenário
description: Como parte do planejamento de recursos, você pode usar o Planejador de Cenários da Adobe Workfront para orçar as funções de trabalho necessárias para concluir o trabalho em um projeto ao criar o caso comercial.
author: Alina
feature: Work Management
exl-id: d5f3e348-dc7d-4265-a5ce-8eef152db410
source-git-commit: ffd7a588c0c9449b7a6aa18e6df7baa7c9872926
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 0%

---

# Recursos de orçamento no Caso de negócios usando o Planejador de cenário

Como parte do planejamento de recursos, você pode usar o Planejador de Cenários da Adobe Workfront para orçar as funções de trabalho necessárias para concluir o trabalho em um projeto ao criar o caso comercial.

Para obter mais informações sobre como criar um caso comercial, consulte [Criar um caso de negócios para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>As informações de função de cargo para a iniciativa vinculada ao projeto inserido no Planejador de Cenário no nível do sistema são visíveis na área Orçamento de Recursos do caso comercial do projeto quando você publica a iniciativa. O Planejador de cenário está disponível somente na nova experiência do Adobe Workfront e requer uma licença adicional. Para obter informações sobre o Planejador de Cenário do Workfront, consulte [A visão geral do Planejador de cenário](../../../scenario-planner/scenario-planner-overview.md).

Você também pode orçar recursos no caso comercial usando o Planejador de Recursos. Para obter mais informações, consulte:

* [Recursos orçamentários no Caso de Negócios](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)

<!--* [Budget resources by project in the Resource Planner](../../../resource-mgmt/resource-planning/budget-by-project-resource-planner-d.md)-->

>[!NOTE]
>
>Recomendamos que você tome a decisão de usar o Planejador de Recursos ou o Planejador de Cenário quando começar a trabalhar em um projeto. A alternância frequente entre os dois durante a vida do projeto pode criar inconsistências na maneira como você orçou seus recursos para o projeto.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Empresa ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td> <p>Você deve comprar uma licença adicional para o Adobe Workfront Scenario Planner para acessar a funcionalidade descrita neste artigo.</p> <p>Para obter informações sobre como obter o Workfront Scenario Planner, consulte <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acesso necessário para usar o Planejador de cenário</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Edite o acesso ao seguinte: </p> 
    <ul> 
     <li> <p>Projetos</p> </li> 
     <li> <p>Dados financeiros</p> </li> 
     <li> <p>Planejador de cenários </p> </li> 
    </ul> <p>Para obter informações sobre o acesso necessário aos recursos do orçamento, consulte também <a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Acesso necessário para recursos de orçamento no Adobe Workfront</a>.</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Adobe Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões no projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Antes de começar, você deve fazer o seguinte:

* Crie um plano usando o Planejador de Cenário.

   Para obter mais informações, consulte [Criar e editar planos no Planejador de Cenário](../../../scenario-planner/create-and-edit-plans.md).

* Crie uma iniciativa no plano e a vincule a um projeto.

   Certifique-se de indicar as informações de funções de cargo necessárias para a iniciativa e atualizar o projeto vinculado com essas informações.

   Para obter mais informações, consulte os seguintes artigos:

   * [Criar e editar iniciativas no Planejador de Cenário](../../../scenario-planner/create-and-edit-initiatives.md)
   * [Importar projetos para planos no Planejador de Cenário](../../../scenario-planner/import-projects-to-plans.md)
   * [Atualize ou crie projetos publicando iniciativas no Planejador de Cenários](../../../scenario-planner/publish-scenarios-update-projects.md).

* Embora esses não sejam pré-requisitos, também recomendamos o seguinte:

   * Atribua tarefas no projeto às funções de cargo orçadas no Planejador de Cenário.
   * Indique o número de Horas Planejadas para as tarefas no projeto.

      Isso ajuda você a entender a quantidade de trabalho que uma tarefa pode precisar concluir, o que ajuda na decisão de quanto tempo os recursos devem ser orçados para concluir a tarefa.

      Para obter informações sobre como associar tarefas com Horas Planejadas, consulte [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Recursos de orçamento no Caso de negócios usando o Planejador de cenário para projetos vinculados a iniciativas

>[!IMPORTANT]
Você pode orçar seus recursos por um período de 15 anos. Se você orçar recursos para um projeto com uma duração superior a 15 anos, as informações de orçamento podem não ser precisas.
<!--
><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">>
>(is this still accurate for the Scenario Planner?)>
></MadCap:conditionalText>>
>-->


1. Vá para o projeto para o qual deseja orçar recursos.

   >[!TIP]
   Trata-se de um projeto vinculado a uma iniciativa no Planejador de Cenário cuja iniciativa vinculada foi publicada pelo menos uma vez.

1. Clique em **Caso de negócios** no painel esquerdo.
1. (Condicional) Na **Orçamentação de Recursos** siga um destes procedimentos:

   * Se você acabou de publicar informações do Planejador de Cenário, selecione Planejador de Cenário no **Escolha quais horas usar para calcular o Custo de Mão-de-Obra Orçada do projeto** na área do Orçamento de Recursos e clique em **Choose**.

      ![](assets/business-case-sp-selected-with-choose-button-350x121.png)

   * Se o Planejador de Recursos tiver sido selecionado anteriormente para recursos de orçamento do projeto, clique em **Alterar** > **Planejador de Cenário** > **Choose**.

      ![](assets/business-case-rp-selected-change-option-to-switch-to-sp-highlighted-350x37.png)

      O Workfront usa as horas necessárias da função de cargo a partir da iniciativa vinculada para calcular o Custo de Mão de obra Orçada do projeto. Essa é a opção recomendada. O custo é exibido no Caso de negócios na moeda do projeto.

      >[!IMPORTANT]
      Quando você usa o Planejador de Cenário para orçar recursos para o projeto, o Custo da Mão-de-Obra Orçada é exibido nas seguintes áreas do Workfront:
      * Área do Orçamento dos Recursos do Caso de Negócios
      * O Planejador de Cenário no nível do sistema como o Custo de Pessoas da iniciativa vinculada ao projeto. Para obter mais informações, consulte [Criar e editar iniciativas no Planejador de Cenário](../../../scenario-planner/create-and-edit-initiatives.md).


1. (Opcional) Clique em **Exibir no Planejador de Cenário** abrir o plano que contém a iniciativa ligada ao projeto. Isso abre o Planejador de cenário em uma nova guia do navegador.
1. (Opcional) Atualize as informações sobre a iniciativa. Para obter mais informações, consulte [Criar e editar iniciativas no Planejador de Cenário](../../../scenario-planner/create-and-edit-initiatives.md).

   >[!NOTE]
   Você deve publicar a iniciativa após cada alteração da área de Orçamento de Recursos no projeto a ser atualizado.
