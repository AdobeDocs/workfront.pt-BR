---
navigation-topic: business-case-and-scorecards
title: Recursos de orçamento no Caso de negócios usando o Planejador de recursos
description: Como parte do planejamento de recursos, você pode usar o Planejador de Recursos no nível do projeto para orçar as funções de trabalho necessárias para concluir o trabalho em um projeto ao criar o caso comercial.
author: Alina
feature: Work Management
exl-id: 51ebb940-111c-442f-a8a6-287a04d2db68
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1249'
ht-degree: 0%

---

# Recursos de orçamento no Caso de negócios usando o Planejador de recursos

Como parte do planejamento de recursos, você pode usar o Planejador de Recursos no nível do projeto para orçar as funções de trabalho necessárias para concluir o trabalho em um projeto ao criar o caso comercial.

Para obter mais informações sobre como criar um caso comercial, consulte [Criar um caso de negócios para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>As informações inseridas no Planejador de Recursos no nível do projeto também são visíveis no Planejador de Recursos no nível do sistema. O contrário também é verdade. Para obter informações sobre o Planejador de Recursos, consulte [Visão geral do Planejador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Você também pode orçar recursos no caso comercial usando o Adobe Workfront Scenario Planner. Para obter mais informações, consulte [Recursos de orçamento no Caso de negócios usando o Planejador de cenário](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Plano Adobe Workfront</a>*</td> 
   <td> <p>Pro ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Visão geral das licenças do Adobe Workfront</a>*</td> 
   <td> <p>Revisar ou superior</p> <p>Importante: Você deve ter uma licença do Plan para modificar as informações de orçamento de recursos. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Edite o acesso ao seguinte: </p> 
    <ul> 
     <li> <p>Projetos</p> </li> 
     <li> <p>Gerenciamento de recursos</p> </li> 
     <li> <p>Dados financeiros</p> </li> 
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

* Satisfazer todos os pré-requisitos para o planejamento de recursos no Adobe Workfront. Para obter mais informações, consulte [Visão geral do Planejador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Associar Grupos de Recursos ao projeto.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:(you must have tasks assigned to job roles and users on the project - this is optional because the users and their roles come from the pools))</p>
  -->

   >[!NOTE]
   Não é possível orçar recursos atribuídos a problemas no Caso de negócios. Você pode orçá-los no Planejador de Recursos no nível do sistema. Para obter mais informações sobre o Planejador de Recursos, consulte [Visão geral do Planejador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Embora isso não seja um pré-requisito, também recomendamos que você indique Horas Planejadas para as tarefas no projeto. Isso ajuda você a entender a quantidade de trabalho que uma tarefa pode precisar concluir, o que ajuda com a decisão de muito tempo em que os recursos devem ser orçados para concluir a tarefa. Para obter informações sobre como associar tarefas com Horas Planejadas, consulte [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Aplicar pools de recursos a um projeto e recursos de orçamento no Caso de negócios

>[!IMPORTANT]
Você pode orçar seus recursos por um período de 15 anos. Se você orçar recursos para um projeto com uma duração superior a 15 anos, as informações de orçamento podem não ser precisas.

Para aplicar Pools de Recursos e recursos de projeto de orçamento no Caso de Negócios para um projeto sem Pool de Recursos:

1. Vá para o projeto para o qual deseja orçar recursos.
1. Clique em **Caso de negócios** no painel esquerdo.
1. (Condicional) Se sua empresa não tiver uma licença para o Workfront Scenario Planner, clique em **Editar Orçamento de Recurso** no **Orçamentação de Recursos** e continue com a etapa 5.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">(NOTE: ensure it stays right - this is 5 instead of 6 because step 2 won't print for nwe)</p>
   -->

1. (Opcional e condicional) Se as informações do projeto tiverem sido publicadas por uma iniciativa sobre o Planejador de Cenário, siga um destes procedimentos:

   * Selecione o Planejador de Recursos no **Escolha quais horas usar para calcular o Custo de Mão-de-Obra Orçada do projeto** e clique em **Escolha > Editar Orçamento de Recurso**.

      ![](assets/business-case-rp-selected-with-choose-button-350x120.png)

   * Se o Planejador de Cenário tiver sido selecionado para recursos de orçamento para o projeto, clique em **Alterar** > **Editar Orçamento de Recurso**.

      ![](assets/business-case-sp-selected-change-option-to-switch-to-rp-highlighted-350x88.png)
   Usa as Horas Orçadas do projeto para calcular o Custo da Mão de Obra Orçada para o projeto.

   O Planejador de cenário está disponível somente na nova experiência do Adobe Workfront e requer uma licença adicional. Para obter informações sobre o Planejador de Cenário do Workfront, consulte [A visão geral do Planejador de cenário](../../../scenario-planner/scenario-planner-overview.md).

   >[!NOTE]
   Recomendamos que você tome a decisão de usar o Planejador de Recursos ou o Planejador de Cenário quando começar a trabalhar em um projeto. A alternância frequente entre os dois durante a vida do projeto pode criar inconsistências na maneira como você orçou seus recursos para o projeto.

1. No **Selecionar Pool de Recursos** , especifique um ou vários **Pools de Recursos**.

   Você deve especificar somente os Pools de Recursos que são preenchidos com usuários ativos.

   >[!TIP]
   Se o projeto já estiver associado a Pools de Recursos, o Planejador de Recursos será exibido por padrão. Para adicionar mais Pools de Recursos ao projeto, edite o projeto. Para obter informações sobre como editar um projeto, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Clique em **Aplicar**.

   O Planejador de Recursos é exibido para o projeto selecionado.

   Por padrão, as primeiras 20 funções de cargo associadas a este projeto são listadas na seção Orçamento de Recurso em ordem alfabética. 

   Para obter mais informações sobre o Planejador de Recursos, consulte [Visão geral do Planejador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   ![BC_resource_budgeting_area.png](assets/bc-resource-budgeting-area-350x276.png)

1. (Opcional e condicional) Expanda as funções do trabalho para ver os usuários associados a elas.

   >[!NOTE]
   Os usuários ativos são exibidos nas funções de trabalho associadas a eles somente se atenderem aos seguintes critérios:
   * Eles pertencem a um dos Pools de Recursos do projeto.
   * Eles orçamentaram horas atribuídas a eles.
   * Eles estão associados a uma das funções do projeto.


    

1. Clique em **Hoje** para voltar ao período atual.
1. (Opcional) Clique em **Semana**, **Mês** ou **Trimestre** para exibir informações do projeto em diferentes intervalos de tempo.
1. (Opcional) Clique no botão **Horas** e selecione **Horas**,**FTE** ou **Custo** para alterar como as informações são exibidas no Planejador de Recursos. As horas são exibidas por padrão.

1. (Opcional) Clique em **Exportar** para exportar o Planejador de Recursos para um arquivo Excel.

   >[!NOTE]
   É possível exportar dados por até 12 períodos de cada vez.

1. (Opcional) Clique no botão **Tela cheia** ícone ![full_screen_RP_in_BC.png](assets/full-screen-rp-in-bc.png) para exibir o Planejador de recursos no modo de tela cheia.

1. Atualize o **BDG** Campo (Horas Orçadas) com valores de Hora, FTE ou Custo para os usuários, funções ou o projeto, executando um dos seguintes procedimentos:

   * Estimar manualmente a quantidade de valores de Horas, FTE ou Custo para funções, usuários ou o projeto.

      Ou

   * Clique no botão **Opções** ícone para o projeto ou as funções do trabalho e selecione uma opção para orçar automaticamente as horas para funções, usuários ou o projeto.
   Para obter mais informações sobre orçamento na Exibição de Projeto do Planejador de Recursos, consulte [Recursos de orçamento no Planejador de Recursos usando as exibições Projeto e Função](../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   >[!NOTE]
   Você pode orçar horas, FTEs ou custos para seus recursos por qualquer período exibido na área de Orçamento de Recursos, independentemente da linha do tempo do projeto. Por exemplo, se você quiser indicar que seus recursos podem não estar disponíveis durante a linha do tempo do projeto (onde estão associados às Horas Planejadas), mas podem estar disponíveis durante outro tempo, faça isso orçando-os para períodos de tempo em que as Horas Planejadas sejam zero, se isso for quando estiverem disponíveis para trabalhar.

1. (Opcional) Para entender se você pode mover as Horas, FTEs ou Custos orçados para outro período, clique no botão **Opções** ícone , em seguida **Ajustar datas de orçamento**.

   Para obter mais informações sobre o ajuste de datas orçadas, consulte [Ajustar datas de orçamento no Planejador de Recursos](../../../resource-mgmt/resource-planning/adjust-budgeting-dates.md).

1. Clique em **Salvar**.

   Se você tiver as taxas de Custo por Hora associadas às suas funções de cargo, o orçamento dos recursos na área de Orçamento de Recurso calculará o valor de **Custo de Mão-de-Obra Orçada** do projeto. O Custo da Mão-de-Obra Orçada é exibido na área Orçamento de Recursos do Caso de Negócios e no Sumário do Caso de Negócios.

   >[!TIP]
   O custo é exibido no Caso de negócios na moeda do projeto.

   As informações de orçamento especificadas no Caso de Negócios também são exibidas no Planejador de Recursos.
