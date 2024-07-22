---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Mostrar alocação de funções para projetos e iniciativas na lista de tarefas
description: Depois de conectar projetos e iniciativas, é possível gerenciar a alocação de recursos lado a lado para garantir que eles correspondam. Isso evita a superalocação ou a subutilização deles.
author: Alina
feature: Workfront Scenario Planner
exl-id: 77152e46-0b7b-4937-9d16-1a20c2a7fdf1
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 0%

---

# Mostrar alocação de funções para projetos e iniciativas na lista de tarefas

<!--Audited: 07/2024-->

Depois de conectar projetos e iniciativas, é possível gerenciar a alocação de recursos lado a lado para garantir que eles correspondam. Isso evita a superalocação ou a subutilização deles.

Este artigo descreve como reconciliar recursos usando o painel [!UICONTROL Alocação de função] na lista de tarefas de um projeto.

Para obter informações gerais sobre como reconciliar recursos entre projetos e iniciativas, incluindo pré-requisitos, consulte [Visão geral da reconciliação de alocações de recursos entre projetos e iniciativas](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plano*</p> </td> 
   <td> <p>Atual: [!UICONTROL Business] ou superior</p>
   <p>Novo: Ultimate </p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licença*</p> </td> 
   <td> <p>Novo: Claro ou superior</p> 
   <p>Atual: [!UICONTROL Review] ou posterior</p> </td> 
  </tr> 
  <tr> 
   <td>Produto* </td> 
   <td> 
   <p>Para os planos atuais do Workfront: </p>
   <p>Você deve comprar uma licença adicional para o [!DNL Adobe Workfront Scenario Planner] acessar a funcionalidade descrita neste artigo.</p> <p>Para obter informações sobre acesso e permissões para o [!DNL Workfront Scenario Planner], consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acesso necessário para usar o [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Nível de acesso </td> 
   <td> <p>[!UICONTROL Exibir] ou acesso superior a [!UICONTROL Projetos]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Permissões de objeto </p> </td> 
   <td> <p>[!UICONTROL Exibir] permissões para um projeto</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso à documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Mostrar alocação de funções para projetos e iniciativas na lista de tarefas

Se sua empresa adquiriu uma licença [!DNL Workfront Scenario Planner], é possível reconciliar as alocações de recursos entre a iniciativa e o projeto vinculado a ela na seção [!UICONTROL Tarefas] do projeto.

1. (Condicional) Conecte um projeto a uma iniciativa usando um dos métodos descritos em [Mostrar alocação de função para projetos e iniciativas na lista de tarefas](#Connect) deste artigo.

   >[!IMPORTANT]
   >
   >Se você fizer alterações em recursos da iniciativa, deverá republicar o cenário ao qual a iniciativa pertence para que as informações de recurso mais recentes da iniciativa sejam atualizadas no projeto.

1. Acesse o projeto em que deseja revisar a alocação de funções de trabalho para o projeto, bem como para a iniciativa associada.
1. Clique em **[!UICONTROL Tarefas]** no painel esquerdo.
1. Clique no ícone ![](assets/show-role-allocation-icon.png) da **[!UICONTROL Mostrar alocação de função]**, no canto superior direito da barra de ferramentas.

   O painel [!UICONTROL Alocação de função] é exibido.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. Revise as seguintes informações na área **[!UICONTROL Totais do Projeto]** do painel [!UICONTROL Alocação de Função]:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Função de Trabalho]</td> 
      <td> <p>Os nomes das funções de trabalho associadas a qualquer uma das seguintes opções:</p> 
       <ul> 
        <li> <p>tarefas no projeto</p> </li> 
        <li> <p>problemas no projeto</p> </li> 
        <li> <p>iniciativa vinculada ao projeto</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Horas da Iniciativa]</td> 
      <td>O número de horas necessárias associadas a cada função de trabalho na iniciativa durante a duração total da iniciativa. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Horas Planejadas]</td> 
      <td>O número de Horas Planejadas associadas a cada função de trabalho nas tarefas ou problemas no projeto pela duração total do projeto. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Variação]</td> 
      <td> <p>A diferença entre as horas necessárias para a iniciativa e as horas planejadas associadas ao trabalho no projeto. [!DNL Workfront] calcula a [!UICONTROL Variance] usando esta fórmula:</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>Quando os recursos são planejados para mais horas do que o necessário na iniciativa, a [!UICONTROL Variance] é negativa e é exibida em vermelho. Isso significa que seus recursos estão superalocados. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >As horas planejadas do projeto não são exibidas nos seguintes cenários:
   >
   >   
   >   
   >   * Quando tarefas ou problemas não são atribuídos a funções de trabalho ou usuários com uma função de trabalho associada a eles.
   >   * Quando as tarefas ou problemas tiverem uma Duração zero.
   >   
   >



1. (Opcional) Se a coluna [!UICONTROL Variação] mostrar que seus recursos estão superalocados, ajuste uma das seguintes opções:

   * Reduza o número de Horas Planejadas para uma função de trabalho que mostra estar superalocada ou adicione mais recursos às tarefas e distribua mais Horas Planejadas para os novos recursos. Você pode atualizar as atribuições ou o número de Horas planejadas nas tarefas ou problemas ao editá-las. Para obter mais informações, consulte os seguintes artigos:

      * [Editar tarefas](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [Editar problemas](../manage-work/issues/manage-issues/edit-issues.md)

     >[!NOTE]
     >
     >Você deve ter acesso e permissões adicionais para editar tarefas e problemas.

   * Aumente o número de horas necessárias para a função que mostra a superalocação na iniciativa. Para obter mais informações, consulte [Criar e editar iniciativas no [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md).

     >[!NOTE]
     >
     >Você deve ter acesso e permissões adicionais para editar planos.


