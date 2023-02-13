---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Mostrar alocação de função para projetos e iniciativas no Balanceador de Carga de Trabalho
description: Depois de conectar projetos e iniciativas, você pode gerenciar a alocação de recursos lado a lado para garantir que eles
author: Alina
feature: Workfront Scenario Planner
exl-id: cdc3a1b0-7021-4853-9b51-c3682fd55430
source-git-commit: 82a5102d28700368a094502dcd6026462c149eb1
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 0%

---

# Mostrar alocação de função para projetos e iniciativas no [!DNL Workload Balancer]

>[!IMPORTANT]
>
>Sua organização deve comprar uma licença adicional para a [!DNL Adobe Workfront Scenario Planner] para que você possa visualizar as informações da iniciativa em um projeto. Para obter informações sobre como obter o [!DNL Workfront Scenario Planner], consulte [O acesso necessário para usar o [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Depois de conectar projetos e iniciativas, você pode gerenciar a alocação de recursos lado a lado para garantir a correspondência. Isto evita a atribuição excessiva ou a sua subutilização.

Este artigo descreve como reconciliar recursos usando o [!UICONTROL Alocação de função] no painel [!UICONTROL Balanceador de Carga de Trabalho] de um projeto.

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
   <td> <p>Você deve comprar uma licença adicional para a [!DNL Adobe Workfront Scenario Planner] para acessar a funcionalidade descrita neste artigo.</p> <p>Para obter informações sobre como obter o [!DNL Workfront Scenario Planner], consulte <a href="../scenario-planner/access-needed-to-use-sp.md">O acesso necessário para usar o [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configurações de nível de acesso*</strong> </td> 
   <td> <p>[!UICONTROL View] ou acesso superior a projetos </p> <p>Observação: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode alterar seu nível de acesso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Permissões de objeto</strong> </p> </td> 
   <td> <p>[!UICONTROL View] ou permissões superiores para o projeto</p> <p>Para obter informações sobre como solicitar acesso adicional a um plano, consulte <a href="../scenario-planner/request-access-to-plan.md">[!UICONTROL Solicitação] acesso a um plano na [!DNL Workfront Scenario Planner]</a>.</p> <p>Para obter informações sobre como solicitar acesso adicional a um projeto, consulte <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Mostrar alocação de função para projetos e iniciativas no [!DNL Workload Balancer]

Se sua empresa adquiriu um [!DNL Workfront Scenario Planner] , é possível reconciliar as alocações de recursos entre a iniciativa e o projeto vinculado a ela no nível do projeto [!DNL Workload Balancer].

1. (Condicional) Conecte um projeto com uma iniciativa usando um dos métodos descritos nos seguintes artigos:

   * [Importar projetos para planos na [!DNL Adobe Workfront Scenario Planner]](import-projects-to-plans.md).
   * [Atualize ou crie projetos publicando iniciativas no [!DNL Adobe Workfront Scenario Planner]](publish-scenarios-update-projects.md).

   >[!IMPORTANT]
   >
   >Se você fizer alterações nos recursos da iniciativa, deverá republicar o cenário ao qual a iniciativa pertence para que as últimas informações sobre recursos da iniciativa sejam atualizadas no projeto.

1. Vá para o projeto onde deseja revisar a alocação de funções de cargo para o projeto, bem como para a iniciativa associada.
1. Clique em [!DNL Workload Balancer] no painel esquerdo.

   Talvez seja necessário clicar em **[!UICONTROL Agendamento]**, em seguida **[!UICONTROL Alternar para Balanceador de Carga de Trabalho]**.

1. Siga um destes procedimentos:

   * Clique em **[!UICONTROL Mês]** para exibir o Balanceador de Carga de Trabalho por mês, clique no menu suspenso ao lado de um mês na linha do tempo ![](assets/drop-down-next-to-month-month-view-wb.png), depois clique em **[!UICONTROL Mais]**.
   * Clique no botão **[!UICONTROL Mostrar alocação de função]** ícone ![](assets/show-role-allocation-icon.png) no canto superior direito da barra de ferramentas.

   O [!UICONTROL Alocação de função] será exibido.

   ![](assets/role-allocation-panel-months-collapsed-350x319.png)

   >[!CAUTION]
   >
   >Embora seja possível visualizar a variável [!UICONTROL Alocação de função] painel mesmo se sua organização não tiver comprado um [!DNL Workfront Scenario Planner] não é possível exibir informações sobre as funções de trabalho das iniciativas.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. Revise as seguintes informações na **[!UICONTROL Totais do projeto]** Área do painel Alocação de funções:

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
   >   * Quando as tarefas ou problemas têm uma [!UICONTROL Duração] de zero.




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


1. (Opcional) Clique no ícone suspenso para expandir um dos meses no [!UICONTROL Alocação de função] ou na linha do tempo do [!UICONTROL Balanceador de Carga de Trabalho].

   ![](assets/month-expanded-highlighted-role-allocation-panel-wb-350x145.png)

   O mesmo tipo de informação exibida no [!UICONTROL Totais do projeto] também é exibida para cada mês.

   >[!TIP]
   >
   >Os meses listados na [!UICONTROL Alocação de função] são os meses na linha do tempo exibida na tela no [!UICONTROL Balanceador de Carga de Trabalho]. Role para trás e para a frente na linha do tempo para visualizar meses adicionais.

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p> </p> </li>
   -->


