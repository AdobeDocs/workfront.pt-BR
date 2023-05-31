---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Mostrar alocação de funções para projetos e iniciativas no Balanceador de carga de trabalho
description: Depois de conectar projetos e iniciativas, é possível gerenciar a alocação de recursos lado a lado para garantir que eles
author: Alina
feature: Workfront Scenario Planner
exl-id: cdc3a1b0-7021-4853-9b51-c3682fd55430
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 0%

---

# Mostrar alocação de funções para projetos e iniciativas na [!UICONTROL Balanceador de carga de trabalho]

>[!IMPORTANT]
>
>Sua organização deve comprar uma licença adicional para o [!DNL Adobe Workfront Scenario Planner] para que você possa exibir as informações da iniciativa em um projeto. Para obter mais informações sobre como obter a [!DNL Workfront Scenario Planner], consulte [Acesso necessário para usar o [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Depois de conectar projetos e iniciativas, é possível gerenciar a alocação de recursos lado a lado para garantir que eles correspondam. Isso evita a superalocação ou a subutilização deles.

Este artigo descreve como reconciliar recursos usando o [!UICONTROL Alocação de função] painel no [!UICONTROL Balanceador de carga de trabalho] de um projeto.

Para obter informações gerais sobre como reconciliar recursos entre projetos e iniciativas, incluindo pré-requisitos, consulte [Visão geral da reconciliação de alocações de recursos entre projetos e iniciativas](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## Requisitos de acesso

Você precisa seguir:

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
   <td> <p>Você deve adquirir uma licença adicional para o [!DNL Adobe Workfront Scenario Planner] para acessar a funcionalidade descrita neste artigo.</p> <p>Para obter mais informações sobre como obter a [!DNL Workfront Scenario Planner], consulte <a href="../scenario-planner/access-needed-to-use-sp.md">Acesso necessário para usar o [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configurações de nível de acesso*</strong> </td> 
   <td> <p>[!UICONTROL View] ou acesso superior a Projetos </p> <p>Observação: se você ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais no seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode alterar seu nível de acesso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Permissões de objeto</strong> </p> </td> 
   <td> <p>[!UICONTROL Exibir] ou permissões superiores para o projeto</p> <p>Para obter informações sobre como solicitar acesso adicional a um plano, consulte <a href="../scenario-planner/request-access-to-plan.md">[!UICONTROL Solicitação] acesso a um plano na [!DNL Workfront Scenario Planner]</a>.</p> <p>Para obter informações sobre como solicitar acesso adicional a um projeto, consulte <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

## Mostrar alocação de funções para projetos e iniciativas na [!UICONTROL Balanceador de carga de trabalho]

Se sua empresa adquiriu um [!DNL Workfront Scenario Planner] é possível reconciliar as alocações de recursos entre a iniciativa e o projeto vinculado a ela no nível do projeto [!UICONTROL Balanceador de carga de trabalho].

1. (Condicional) Conecte um projeto a uma iniciativa usando um dos métodos descritos nos seguintes artigos:

   * [Importar projetos para planos na [!DNL Adobe Workfront Scenario Planner]](import-projects-to-plans.md).
   * [Atualizar ou criar projetos publicando iniciativas no [!DNL Adobe Workfront Scenario Planner]](publish-scenarios-update-projects.md).

   >[!IMPORTANT]
   >
   >Se você fizer alterações em recursos da iniciativa, deverá republicar o cenário ao qual a iniciativa pertence para que as informações de recurso mais recentes da iniciativa sejam atualizadas no projeto.

1. Acesse o projeto em que deseja revisar a alocação de funções de trabalho para o projeto, bem como para a iniciativa associada.
1. Clique em [!UICONTROL Balanceador de carga de trabalho] no painel esquerdo.

   Talvez seja necessário clicar em **[!UICONTROL Agendamento]**, depois **[!UICONTROL Alternar para o Balanceador de carga de trabalho]**.

1. Siga um destes procedimentos:

   * Clique em **[!UICONTROL Month]** para exibir o Balanceador de carga de trabalho por mês, clique no menu suspenso ao lado de um mês na linha do tempo ![](assets/drop-down-next-to-month-month-view-wb.png)e, em seguida, clique em **[!UICONTROL Mais]**.
   * Clique em **[!UICONTROL Mostrar alocação de funções]** ícone ![](assets/show-role-allocation-icon.png) no canto superior direito da barra de ferramentas.

   A variável [!UICONTROL Alocação de função] é exibido.

   ![](assets/role-allocation-panel-months-collapsed-350x319.png)

   >[!CAUTION]
   >
   >Embora você possa visualizar as [!UICONTROL Alocação de função] mesmo se sua organização não tiver comprado um [!DNL Workfront Scenario Planner] licença, não será possível exibir informações sobre as funções de trabalho das iniciativas.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. Revise as seguintes informações no **[!UICONTROL Totais do projeto]** área do painel Alocação de função:

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
   >   * Quando tarefas ou problemas têm um [!UICONTROL Duração] de zero.




1. (Opcional) Se a variável [!UICONTROL Variação] mostra que os recursos estão superalocados e ajuste uma das opções a seguir:

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


1. (Opcional) Clique no ícone suspenso para expandir um dos meses na [!UICONTROL Alocação de função] ou na linha do tempo do [!UICONTROL Balanceador de carga de trabalho].

   ![](assets/month-expanded-highlighted-role-allocation-panel-wb-350x145.png)

   O mesmo tipo de informação exibida na variável [!UICONTROL Totais do projeto] também é exibida para cada mês.

   >[!TIP]
   >
   >Os meses listados na variável [!UICONTROL Alocação de função] são os meses na linha do tempo exibidos na tela no painel [!UICONTROL Balanceador de carga de trabalho]. Role para trás e para frente na linha do tempo para visualizar os meses adicionais.

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p> </p> </li>
   -->


