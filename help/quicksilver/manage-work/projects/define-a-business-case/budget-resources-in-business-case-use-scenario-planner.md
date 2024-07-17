---
navigation-topic: business-case-and-scorecards
title: Recursos de orçamento no Business Case usando o Planejador de Cenários
description: Como parte do planejamento de recursos, você pode usar o Planejador de cenários do Adobe Workfront para orçar as funções de trabalho necessárias para concluir o trabalho em um projeto ao criar o business case.
author: Alina
feature: Work Management
exl-id: d5f3e348-dc7d-4265-a5ce-8eef152db410
source-git-commit: 8420f65e84edd42204d91aa503ff0b95153a1e67
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 0%

---

# Recursos de orçamento no Business Case usando o Planejador de Cenários

Como parte do planejamento de recursos, você pode usar o Planejador de cenários do Adobe Workfront para orçar as funções de trabalho necessárias para concluir o trabalho em um projeto ao criar o business case.

Para obter mais informações sobre como criar um business case, consulte [Criar um business case para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>As informações de função de trabalho para a iniciativa vinculada ao projeto inserido no Planejador de Cenários no nível do sistema ficam visíveis na área Orçamento de Recursos do business case do projeto quando você publica a iniciativa. O Planejador de cenários está disponível somente na nova experiência do Adobe Workfront e requer uma licença adicional. Para obter informações sobre o Planejador de cenários do Workfront, consulte [A visão geral do Planejador de cenários](../../../scenario-planner/scenario-planner-overview.md).

Você também pode estimar recursos no business case usando o Planejador de recursos. Para obter mais informações, consulte o seguinte:

* [Recursos de orçamento no Business Case](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)
  <!--* [Budget resources by project in the Resource Planner](../../../resource-mgmt/resource-planning/budget-by-project-resource-planner-d.md)-->

>[!NOTE]
>
>Recomendamos que você tome a decisão de usar o Planejador de recursos ou o Planejador de cenários quando começar a trabalhar em um projeto. Alternar frequentemente entre os dois durante a vida útil do projeto pode criar inconsistências na maneira como você faz o orçamento de seus recursos para o projeto.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Business ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td> <p>Você deve adquirir uma licença adicional para que o Planejador de cenários da Adobe Workfront acesse a funcionalidade descrita neste artigo.</p> <p>Para obter informações sobre como obter o Planejador de cenários do Workfront, consulte <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acesso necessário para usar o Planejador de cenários</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso ao seguinte: </p> 
    <ul> 
     <li> <p>Projetos</p> </li> 
     <li> <p>Dados financeiros</p> </li> 
     <li> <p>Planejador de cenários </p> </li> 
    </ul> <p>Para obter informações sobre o acesso necessário aos recursos de orçamento, consulte também <a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Acesso necessário aos recursos de orçamento no Adobe Workfront</a>.</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Adobe Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões no projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Pré-requisitos

Antes de começar, você deve fazer o seguinte:

* Crie um plano usando o Planejador de cenários.

  Para obter informações, consulte [Criar e editar planos no Planejador de cenários](../../../scenario-planner/create-and-edit-plans.md).

* Crie uma iniciativa no plano e a vincule a um projeto.

  Indique as informações das funções de trabalho necessárias para a iniciativa e atualize o projeto vinculado com essas informações.

  Para obter mais informações, consulte os seguintes artigos:

   * [Criar e editar iniciativas no Planejador de cenários](../../../scenario-planner/create-and-edit-initiatives.md)
   * [Importar projetos para planos no Planejador de cenários](../../../scenario-planner/import-projects-to-plans.md)
   * [Atualize ou crie projetos publicando iniciativas no Planejador de cenários](../../../scenario-planner/publish-scenarios-update-projects.md).

* Embora esses não sejam pré-requisitos, também recomendamos o seguinte:

   * Atribua tarefas no projeto às funções de trabalho orçadas no Planejador de cenários.
   * Indique o número de Horas Planejadas para as tarefas no projeto.

     Isso ajuda a entender a quantidade de trabalho que uma tarefa pode precisar concluir, o que ajuda na decisão de quanto tempo os recursos devem ser orçados para concluir a tarefa.

     Para obter informações sobre como associar tarefas com Horas Planejadas, consulte [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Recursos de orçamento no Business Case usando o Planejador de cenários para projetos vinculados a iniciativas

>[!IMPORTANT]
>
>Você pode estimar seus recursos por um período de 15 anos. Se você orçar recursos para um projeto com duração superior a 15 anos, as informações de orçamento podem não ser precisas.
><!--
><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">>
>(is this still accurate for the Scenario Planner?)>
></MadCap:conditionalText>>
>-->

1. Vá para o projeto para o qual deseja orçar recursos.

   >[!TIP]
   >
   >Este é um projeto vinculado a uma iniciativa no Planejador de cenários cuja iniciativa vinculada foi publicada pelo menos uma vez.

1. Clique em **Business Case** no painel esquerdo.
1. (Condicional) Na seção **Estimativa de Recursos**, siga um destes procedimentos:

   * Se você acabou de publicar informações do Planejador de cenários, selecione o Planejador de cenários no **Escolha quais horas usar para calcular o Custo de mão de obra orçado do projeto** campo na área Orçamento de recursos, em seguida, clique em **Escolher**.

     ![](assets/business-case-sp-selected-with-choose-button-350x121.png)

   * Se o Planejador de Recursos foi selecionado anteriormente para recursos de orçamento para o projeto, clique em **Alterar** > **Planejador de Cenários** > **Escolher**.

     ![](assets/business-case-rp-selected-change-option-to-switch-to-sp-highlighted-350x37.png)

     O Workfront usa as horas de função de trabalho necessárias da iniciativa vinculada para calcular o Custo de mão de obra orçado e as horas orçadas do projeto. Esta é a opção recomendada. O custo é exibido no Business Case na moeda do projeto.

     Quando você copia um projeto e opta por copiar as Horas orçadas para o novo projeto, as horas orçadas usando o Planejador de cenários não são copiadas para o novo projeto. Somente as horas orçadas no Planejador de recursos são copiadas. Para obter mais informações, consulte [Copiar um projeto](../manage-projects/copy-project.md).

     >[!IMPORTANT]
     >
     >Quando você usa o Planejador de Cenários para orçar recursos para o projeto, o Custo de Mão de Obra Orçado é exibido nas seguintes áreas do Workfront:
     >
     >   
     >   
     >   * Área de orçamento de recursos do Business Case
     >   * O Planejador de cenários no nível do sistema como o Custo de pessoas da iniciativa vinculada ao projeto. Para obter mais informações, consulte [Criar e editar iniciativas no Planejador de cenários](../../../scenario-planner/create-and-edit-initiatives.md).
     >   
     >

1. (Opcional) Clique em **Exibir no Planejador de cenários** para abrir o plano que contém a iniciativa vinculada ao projeto. Isso abre o Planejador de cenários em uma nova guia do navegador.
1. (Opcional) Atualize as informações sobre a iniciativa. Para obter mais informações, consulte [Criar e editar iniciativas no Planejador de cenários](../../../scenario-planner/create-and-edit-initiatives.md).

   >[!NOTE]
   >
   >Você deve publicar a iniciativa após cada alteração na área Orçamento de recursos do projeto a ser atualizada.
