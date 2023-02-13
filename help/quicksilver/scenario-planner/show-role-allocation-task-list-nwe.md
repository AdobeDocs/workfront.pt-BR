---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Mostrar alocação de funções para projetos e iniciativas na lista de tarefas
description: Depois de conectar projetos e iniciativas, você pode gerenciar a alocação de recursos lado a lado para garantir a correspondência. Isto evita a atribuição excessiva ou a sua subutilização.
author: Alina
feature: Workfront Scenario Planner
exl-id: 77152e46-0b7b-4937-9d16-1a20c2a7fdf1
source-git-commit: 82a5102d28700368a094502dcd6026462c149eb1
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# Mostrar alocação de funções para projetos e iniciativas na lista de tarefas

>[!IMPORTANT]
>
>Sua organização deve comprar uma licença adicional para a [!DNL Adobe Workfront Scenario Planner] para que você possa visualizar as informações da iniciativa em um projeto. Para obter informações sobre como obter o [!DNL Workfront Scenario Planner], consulte [O acesso necessário para usar o [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Depois de conectar projetos e iniciativas, você pode gerenciar a alocação de recursos lado a lado para garantir a correspondência. Isto evita a atribuição excessiva ou a sua subutilização.

Este artigo descreve como reconciliar recursos usando o [!UICONTROL Alocação de função] na lista de tarefas de um projeto.

Para obter informações gerais sobre como reconciliar recursos entre projetos e iniciativas, incluindo pré-requisitos, consulte [Visão geral da reconciliação das alocações de recursos entre projetos e iniciativas](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## Requisitos de acesso

É necessário:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plano*</b> </p> </td> 
   <td>[!UICONTROL Business] ou superior</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> licença*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td><b>Produto</b> </td> 
   <td> <p>Você deve comprar uma licença adicional para a [!DNL Adobe Workfront Scenario Planner] para acessar a funcionalidade descrita neste artigo.</p> <p>Para obter informações sobre como obter o [!DNL Workfront Scenario Planner], consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">O acesso necessário para usar o [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configurações de nível de acesso*</strong> </td> 
   <td> <p>[!UICONTROL View] ou acesso superior a projetos </p> <p>Observação: Se você ainda não tiver acesso, pergunte ao administrador da [!UICONTROL Workfront] se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador da [!UICONTROL Workfront] pode alterar seu nível de acesso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Permissões de objeto</strong> </p> </td> 
   <td> <p>[!UICONTROL View] ou permissões superiores para o projeto</p> <p>Para obter informações sobre como solicitar acesso adicional a um plano, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acesso a um plano na [!DNL Scenario Planner]</a>.</p> <p>Para obter informações sobre como solicitar acesso adicional a um projeto, consulte <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Mostrar alocação de funções para projetos e iniciativas na lista de tarefas

Se sua empresa adquiriu um [!DNL Workfront Scenario Planner] , é possível reconciliar as alocações de recursos entre a iniciativa e o projeto vinculado a ela na [!UICONTROL Tarefas] seção do projeto.

1. (Condicional) Conecte um projeto com uma iniciativa usando um dos métodos descritos no [Mostrar alocação de funções para projetos e iniciativas na lista de tarefas](#Connect) deste artigo.

   >[!IMPORTANT]
   >
   >Se você fizer alterações nos recursos da iniciativa, deverá republicar o cenário ao qual a iniciativa pertence para que as últimas informações sobre recursos da iniciativa sejam atualizadas no projeto.

1. Vá para o projeto onde deseja revisar a alocação de funções de cargo para o projeto, bem como para a iniciativa associada.
1. Clique em **[!UICONTROL Tarefas]** no painel esquerdo.
1. Clique no botão **[!UICONTROL Mostrar alocação de função]** ícone ![](assets/show-role-allocation-icon.png) no canto superior direito da barra de ferramentas.

   O [!UICONTROL Alocação de função] será exibido.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. Revise as seguintes informações na **[!UICONTROL Totais do projeto]** área do [!UICONTROL Alocação de função] painel:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Função do trabalho]</td> 
      <td> <p>Os nomes das funções de trabalho associadas a qualquer um dos seguintes itens:</p> 
       <ul> 
        <li> <p>tarefas no projeto</p> </li> 
        <li> <p>problemas do projeto</p> </li> 
        <li> <p>iniciativa ligada ao projeto</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Horas da iniciativa]</td> 
      <td>O número de horas necessárias associadas a cada função de emprego na iniciativa para a duração total da iniciativa. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Horas planejadas]</td> 
      <td>O número de Horas Planejadas associadas a cada função de cargo nas tarefas ou problemas no projeto pela duração total do projeto. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Variação]</td> 
      <td> <p>A diferença entre as horas necessárias na iniciativa e as horas planejadas associadas ao trabalho no projeto. [!DNL Workfront] O calcula a [!UICONTROL Variance] usando esta fórmula:</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>Quando os recursos são planejados por mais horas do que o necessário na iniciativa, a [!UICONTROL Variance] é negativa e é exibida em vermelho. Isso significa que seus recursos estão sobrealocados. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >As Horas Planejadas do projeto não são exibidas nos seguintes cenários:
   >
   >   
   >   
   >   * Quando tarefas ou problemas não são atribuídos a funções de trabalho ou usuários com uma função de trabalho associada a elas.
   >   * Quando tarefas ou problemas têm uma Duração de zero.




1. (Opcional) Se a variável [!UICONTROL Variação] mostra que seus recursos estão sobrealocados, ajuste uma das opções a seguir:

   * Diminua o número de Horas Planejadas para uma função de cargo que mostra o sobrealocado ou adicione mais recursos às tarefas e distribua mais Horas Planejadas para os novos recursos. Você pode atualizar atribuições ou o número de Horas Planejadas em tarefas ou problemas ao editá-las. Para obter mais informações, consulte os seguintes artigos:

      * [Editar tarefas](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [Editar problemas](../manage-work/issues/manage-issues/edit-issues.md)

      >[!NOTE]
      >
      >Você deve ter acesso e permissões adicionais para editar tarefas e problemas.

   * Aumente o número de horas necessárias para a função que mostra a atribuição excessiva na iniciativa. Para obter mais informações, consulte [Crie e edite iniciativas na [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md).

      >[!NOTE]
      >
      >Você deve ter acesso e permissões adicionais para editar planos.



