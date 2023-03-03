---
navigation-topic: business-case-and-scorecards
title: Estimativa de recursos no Business Case usando o Planejador de recursos
description: Como parte do planejamento de recursos, você pode usar o Planejador de recursos no nível do projeto para fazer o orçamento das funções de trabalho necessárias para concluir o trabalho em um projeto ao criar o business case.
author: Alina
feature: Work Management
exl-id: 51ebb940-111c-442f-a8a6-287a04d2db68
source-git-commit: 8420f65e84edd42204d91aa503ff0b95153a1e67
workflow-type: tm+mt
source-wordcount: '1284'
ht-degree: 0%

---

# Estimativa de recursos no Business Case usando o Planejador de recursos

Como parte do planejamento de recursos, você pode usar o Planejador de recursos no nível do projeto para fazer o orçamento das funções de trabalho necessárias para concluir o trabalho em um projeto ao criar o business case.

Para obter mais informações sobre como criar um business case, consulte [Criar um Business Case para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>As informações inseridas no Planejador de Recursos no nível do projeto também estão visíveis no Planejador de Recursos no nível do sistema. O inverso também é verdadeiro. Para obter informações sobre o Planejador de recursos, consulte [Visão geral do Planejador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Você também pode estimar recursos no business case usando o Planejador de cenários do Adobe Workfront. Para obter mais informações, consulte [Recursos de orçamento no Business Case usando o Planejador de Cenários](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">plano do Adobe Workfront</a>*</td> 
   <td> <p>Pro ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Visão geral das licenças do Adobe Workfront</a>*</td> 
   <td> <p>Revisar ou superior</p> <p>Importante: é necessário ter uma licença de Plano para modificar as informações de orçamento de recursos. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso ao seguinte: </p> 
    <ul> 
     <li> <p>Projetos</p> </li> 
     <li> <p>Gerenciamento de recursos</p> </li> 
     <li> <p>Dados financeiros</p> </li> 
    </ul> <p>Para obter informações sobre o acesso necessário aos recursos do orçamento, consulte também <a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Acesso necessário para orçar recursos no Adobe Workfront</a>.</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Adobe Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões no projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Pré-requisitos

Antes de começar, você deve fazer o seguinte:

* Atenda a todos os pré-requisitos para o planejamento de recursos na Adobe Workfront. Para obter informações, consulte [Visão geral do Planejador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Associar Conjuntos de Recursos ao projeto.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:(you must have tasks assigned to job roles and users on the project - this is optional because the users and their roles come from the pools))</p>
  -->

   >[!NOTE]
   Não é possível estimar recursos atribuídos a problemas no Business Case. Você pode fazer o orçamento deles no Planejador de recursos no nível do sistema. Para obter mais informações sobre o Planejador de recursos, consulte [Visão geral do Planejador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Embora isso não seja um pré-requisito, também recomendamos que você indique as Horas planejadas para as tarefas no projeto. Isso ajuda a entender a quantidade de trabalho que uma tarefa pode precisar concluir, o que ajuda na decisão de quanto tempo os recursos devem ser orçados para a conclusão da tarefa. Para obter informações sobre como associar tarefas com Horas Planejadas, consulte [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Aplicar Conjuntos de Recursos a um projeto e recursos de orçamento no Business Case

>[!IMPORTANT]
Você pode estimar seus recursos por um período de 15 anos. Se você orçar recursos para um projeto com duração superior a 15 anos, as informações de orçamento podem não ser precisas.

Para aplicar Conjuntos de Recursos e prever recursos do projeto no Business Case de um projeto sem Conjunto de Recursos:

1. Vá para o projeto para o qual deseja orçar recursos.
1. Clique em **Business Case** no painel esquerdo.
1. (Condicional) Se sua empresa não tiver uma licença do Planejador de cenários do Workfront, clique em **Editar orçamento de recursos** no **Estimativa de Recursos** e prossiga com a etapa 5.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">(NOTE: ensure it stays right - this is 5 instead of 6 because step 2 won't print for nwe)</p>
   -->

1. (Opcional e condicional) Se as informações do projeto tiverem sido publicadas de uma iniciativa no Planejador de cenários, execute um dos seguintes procedimentos:

   * Selecione o Planejador de recursos na **Escolha quais horas usar para calcular o Custo de Trabalho Orçado do projeto** e clique em **Escolha > Editar orçamento de recursos**.

      ![](assets/business-case-rp-selected-with-choose-button-350x120.png)

   * Se o Planejador de cenários foi selecionado para recursos de orçamento para o projeto, clique em **Alterar** > **Editar orçamento de recursos**.

      ![](assets/business-case-sp-selected-change-option-to-switch-to-rp-highlighted-350x88.png)
   Usa as Horas Orçadas do projeto para calcular o Custo de Mão-de-Obra Orçado do projeto.

   O Planejador de cenários está disponível somente na nova experiência do Adobe Workfront e requer uma licença adicional. Para obter informações sobre o Planejador de cenários do Workfront, consulte [A visão geral do Planejador de cenários](../../../scenario-planner/scenario-planner-overview.md).

   >[!NOTE]
   Recomendamos que você tome a decisão de usar o Planejador de recursos ou o Planejador de cenários quando começar a trabalhar em um projeto. Alternar frequentemente entre os dois durante a vida útil do projeto pode criar inconsistências na maneira como você faz o orçamento de seus recursos para o projeto.

1. No **Selecionar Conjunto de Recursos** especifique um ou vários **Conjuntos de recursos**.

   Você deve especificar apenas Conjuntos de recursos que são preenchidos com usuários ativos.

   >[!TIP]
   Se o projeto já estiver associado a Conjuntos de recursos, o Planejador de recursos será exibido por padrão. Para adicionar mais Conjuntos de recursos ao projeto, edite o projeto. Para obter informações sobre como editar um projeto, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Clique em **Aplicar**.

   O Planejador de recursos é exibido para o projeto selecionado.

   Por padrão, as primeiras 20 funções de cargo associadas a esse projeto são listadas na seção Orçamento de Recursos em ordem alfabética. 

   Para obter mais informações sobre o Planejador de recursos, consulte [Visão geral do Planejador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   ![BC_resource_budgeting_area.png](assets/bc-resource-budgeting-area-350x276.png)

1. (Opcional e condicional) Expanda as funções de trabalho para ver os usuários associados a elas.

   >[!NOTE]
   Os usuários ativos são exibidos nas funções de trabalho associadas a eles somente se atenderem aos seguintes critérios:
   * Eles pertencem a um dos Conjuntos de recursos do projeto.
   * Eles têm horas orçadas atribuídas a eles.
   * Eles estão associados a uma das funções de trabalho do projeto.


    

1. Clique em **Hoje** para retornar ao período atual.
1. (Opcional) Clique em **Semana**, **Month** ou **Trimestre** para exibir informações do projeto em diferentes períodos.
1. (Opcional) Clique no link **Horas** e selecione **Horas**,**FTE** ou **Custo** para alterar como as informações são exibidas no Planejador de recursos. As horas são exibidas por padrão.

1. (Opcional) Clique em **Exportar** para exportar o Planejador de recursos para um arquivo do Excel.

   >[!NOTE]
   É possível exportar dados para até 12 períodos de tempo por vez.

1. (Opcional) Clique no link **Tela cheia** ícone ![full_screen_RP_in_BC.png](assets/full-screen-rp-in-bc.png) para exibir o Planejador de recursos no modo de tela cheia.

1. Atualize o **BDG** (Horas orçadas) com valores de Hora, FTE ou Custo para os usuários, funções ou o projeto, seguindo um destes procedimentos:

   * Estime manualmente a quantidade de valores de Horas, FTE ou Custo para funções, usuários ou o projeto.

      Ou

   * Clique em **Opções** ícone do projeto ou das funções de trabalho e selecione uma opção para orçar automaticamente as horas para funções, usuários ou o projeto.
   Para obter mais informações sobre orçamento na Visualização de projeto do Planejador de recursos, consulte [Recursos de orçamento no Planejador de recursos usando as visualizações Projeto e Função](../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   >[!NOTE]
   Você pode estimar horas, FTEs ou custos dos recursos para qualquer período exibido na área Orçamento de recursos, independentemente da linha do tempo do projeto. Por exemplo, se você quiser indicar que seus recursos podem não estar disponíveis durante a linha do tempo do projeto (em que estão associados às Horas planejadas), mas podem estar disponíveis durante outro tempo, você pode fazer isso orçando-os para períodos em que as Horas planejadas são zero, se for quando elas estiverem disponíveis para trabalhar.

1. (Opcional) Para entender se você pode mover as Horas orçadas, os FTEs ou os Custos para outro intervalo de tempo, clique no link **Opções** ícone, depois **Ajustar Datas de Orçamento**.

   Para obter mais informações sobre o ajuste de datas previstas em orçamento, consulte [Ajustar datas de orçamento no Planejador de recursos](../../../resource-mgmt/resource-planning/adjust-budgeting-dates.md).

1. Clique em **Salvar**.

   Se você tiver taxas de Custo por Hora associadas às suas funções de trabalho, o orçamento dos recursos na área Orçamento de Recursos calculará as **Custo do Trabalho Orçado** do projeto. O Custo de Mão-de-Obra Orçado é exibido na área Orçamento de Recursos do Business Case e no Resumo de Business Case.

   >[!TIP]
   O custo é exibido no Business Case na moeda do projeto.

   As informações de orçamento especificadas no Business Case também são exibidas no Planejador de Recursos.

   Ao copiar um projeto, você tem a opção de também copiar as Horas orçadas para o novo projeto. Somente as horas orçadas no Planejador de recursos são copiadas. Para obter mais informações, consulte [Copiar um projeto](../manage-projects/copy-project.md).
