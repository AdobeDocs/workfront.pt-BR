---
content-type: reference
product-area: projects
navigation-topic: financials
title: Entender o custo do trabalho orçado e as horas orçadas dos projetos
description: Entender o custo do trabalho orçado e as horas orçadas dos projetos
author: Alina
feature: Work Management
exl-id: 01020bbb-7cf9-4461-b0b6-dcbbc537c616
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 0%

---

# Entender o custo do trabalho orçado e as horas orçadas dos projetos

<!--
<(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)</p>
-->

Você pode estimar seus recursos para o trabalho usando o Planejador de recursos da Adobe Workfront.

À medida que você faz o orçamento de seus recursos para trabalhar em projetos, o Workfront calcula o Custo de mão de obra orçado para as funções, os projetos e os usuários com base nos valores de custo por hora.

O Custo do Trabalho Orçado pelo Planejador de Recursos de um projeto é um cálculo entre o custo associado às funções de trabalho atribuídas para concluir o trabalho no projeto e a quantidade de horas estimadas (Horas Orçadas do Planejador de Recursos) que podem levar cada função para concluir o trabalho.

>[!IMPORTANT]
>
>O Custo do Trabalho Orçado pelo Planejador de Recursos para os usuários não afeta o do projeto. Somente o custo de mão de obra para funções de trabalho afeta o custo do projeto.

## Visão Geral do Custo de Trabalho Orçado para Funções de Trabalho e do Projeto

O Workfront usa o Custo de Trabalho Orçado das funções de trabalho no projeto para calcular o Custo de Trabalho Orçado do projeto.

>[!TIP]
>
>O Custo de Mão de Obra Orçado de um projeto no Business Case é exibido como Custo de Mão de Obra Orçado do Planejador de Recursos em relatórios e listas.

O **Custo do Trabalho Orçado** (ou Custo do Trabalho Orçado pelo Planejador de Recursos) de um projeto é calculado pela seguinte fórmula:

`Resource Planner Budgeted Labor Cost = SUM ( Resource Planner Budgeted Hours for each job role on the project * Cost per Hour rate of each job role on the project)`

Os campos usados no cálculo acima se referem ao seguinte:

* As horas orçadas para funções de trabalho na área Orçamento de Recursos do projeto ou no Planejador de Recursos.

  Para obter mais informações sobre recursos de orçamento no Planejador de recursos, consulte a seção &quot;Budgeting Resources in the Resource Planner&quot; no artigo [Resource Planner overview](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

  Para obter mais informações sobre recursos de orçamento na área Orçamento de Recursos do Business Case, consulte [Recursos de orçamento no Business Case](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

* A **taxa de Custo por Hora de uma função de trabalho** no cálculo acima refere-se ao custo associado a cada função de trabalho no projeto.\
  Para obter mais informações sobre como criar e gerenciar funções de trabalho e associá-las a Taxas de custo, consulte o artigo [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

>[!NOTE]
>
>O Workfront calcula todas as informações de custo usando a moeda do projeto. Se você especificar Horas orçadas para seus recursos no Planejador de recursos, a opção para alterar a moeda do projeto será desativada.\
>Para obter mais informações sobre como alterar a moeda de um projeto, consulte o artigo [Alterar a moeda do projeto](../../../manage-work/projects/project-finances/change-project-currency.md).

## Visão Geral do Custo de Mão de Obra Orçado para Usuários

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Update the following section in the Create a Business Case article, as well, when you update it here.)</p>
-->

>[!IMPORTANT]
>
>O Custo do Trabalho Orçado pelo Usuário não afeta o Custo do Trabalho Orçado do projeto. Somente o custo de mão de obra das funções de trabalho em um projeto afeta o Custo de Mão de Obra Orçado do Planejador de Recursos do projeto.
> 
>O total de todos os custos de mão de obra de todos os usuários pode ou não ser igual ao Custo do Trabalho Orçado pelo Planejador de Recursos das funções de trabalho associadas aos usuários.
>
>Se você estimar Horas orçadas para usuários no Planejador de recursos, os custos associados a eles serão os das funções de trabalho associadas aos usuários. Eles não são custos associados aos usuários ou a suas taxas.

Se os usuários estiverem associados às funções de trabalho no projeto e suas horas forem orçadas no Planejador de Recursos, seu Custo de Mão-de-Obra Orçado será exibido pelos seguintes nomes, dependendo de onde você visualizá-los no Workfront:

* [!UICONTROL **Custo do Trabalho Orçado**]: a área de orçamento de recursos do Business Case nas respectivas funções.

  ![](assets/budgeted-labor-cost-for-users-in-business-case-highlighted-350x73.png)

* [!UICONTROL **BDG**]: o Planejador de Recursos ao visualizar informações na exibição Projeto e Função por Custo.

  ![](assets/budgeted-labor-cost-for-users-in-rp-project-view-cost--highlighted-350x115.png)

Os usuários são exibidos na área Orçamento de recursos do Business Case nas respectivas funções ou no Planejador de recursos se atenderem aos seguintes requisitos:

* Eles estão associados a uma das funções de trabalho no projeto.
* Eles têm horas orçadas especificadas no Planejador de recursos.
* Eles têm uma Taxa de custo por hora associada ao seu perfil.

  Para obter mais informações sobre como adicionar taxas de Custo por hora aos usuários, consulte o artigo [Editar perfil de usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* O usuário faz parte de um dos Conjuntos de recursos associados ao projeto.

O Custo do Trabalho Orçado de um usuário é calculado pela seguinte fórmula:

`User Budgeted Labor Cost = Budgeted hours for the user on the project * Cost per Hour rate of the user`

## Localizar o Custo do Trabalho Orçado de um projeto

O Custo de Mão-de-Obra Orçado, conforme refletido na área Orçamento de Recursos do Business Case ou do Planejador de Recursos, é exibido nas seguintes áreas do Workfront com os seguintes nomes:

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>Nome de exibição do Custo de Trabalho Orçado</strong></td> 
     <td><strong>Área do Workfront</strong></td> 
    </tr> 
    <tr> 
     <td>Custo do Trabalho Orçado</td> 
     <td>Área de orçamento de recursos do Business Case</td> 
    </tr> 
    <tr> 
     <td>Custo Orçado</td> 
     <td><p>Visualização de Custo do relatório de utilização</p><p>Para obter mais informações, consulte <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">Exibir informações de utilização</a>.</p></td> 
    </tr> 
    <tr> 
     <td>BDG </td> 
     <td>Visualizações de Projeto ou Função do Planejador de Recursos, por Custo</td> 
    </tr> 
    <tr> 
     <td>Custo do Trabalho Orçado do Projeto do Planejador de Recursos</td> 
     <td> <p>Relatório do projeto</p> <p>Relatório de Projeto (Dados Financeiros)</p> <p>Relatório de tarefa</p> <p>Relatório de problema</p> <p>Relatório de horas orçadas</p> <p>Para obter informações sobre como criar um relatório, consulte o artigo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Criar um relatório personalizado</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>

>[!NOTE]
>
>Se você usar o Planejador de Cenários do Adobe Workfront para orçar recursos do projeto, o Custo de Mão-de-Obra Orçado na área Orçamento de Recursos do Business Case será o mesmo que os Custos de Pessoas da iniciativa vinculada ao projeto. O Planejador de cenários está disponível somente na nova experiência do Adobe Workfront e requer uma licença adicional. Para obter informações sobre o Planejador de cenários do Workfront, consulte [A visão geral do Planejador de cenários](../../../scenario-planner/scenario-planner-overview.md). Para obter informações sobre recursos de orçamento usando o Planejador de cenários, consulte [Recursos de orçamento no Business Case usando o Planejador de cenários](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## Localizar as horas orçadas de um projeto

<!--
(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)
-->

As Horas Orçadas afetam o valor do Custo de Trabalho Orçado (ou o Custo Orçado do Planejador de Recursos) do projeto.

O Custo de Trabalho Orçado de um projeto é o custo associado às funções de trabalho atribuídas para concluir o trabalho no projeto e a quantidade de horas estimadas (Horas Orçadas) que podem levar cada função para concluir o trabalho.

Você pode visualizar as Horas orçadas no Workfront nos campos listados na tabela abaixo.

>[!NOTE]
>
>Qualquer outra menção de &quot;Horas orçadas&quot; no Workfront se refere às horas orçadas usando recursos obsoletos que foram removidos do Workfront. Esses são campos somente para visualização e não são atualizados com as informações atuais quando você usa as ferramentas atuais de orçamento de recursos.

As horas orçadas na área Orçamento de recursos do Business Case ou do Planejador de recursos são exibidas nas seguintes áreas do Workfront e sob os seguintes nomes:

* **Horas**: área de orçamento de recursos do Business Case
* **BDG**:Planejador de recursos visualizado por Horas
* **Horas Orçadas**: exibição das Horas do relatório de utilização
Para obter informações, consulte [Exibir informações sobre a utilização de recursos](../../../resource-mgmt/resource-utilization/view-utilization-information.md).
* **Bud. Horas**: relatório de horas orçadas

  O objeto Hora orçada no relatório Hora orçada refere-se às informações relacionadas a uma ferramenta de gerenciamento de recursos obsoleta. Apenas o &quot;Bud. O campo &quot;Horas&quot; neste relatório refere-se às horas orçadas no Planejador de recursos ou na área de orçamento de recursos do Business Case do projeto.

  Para obter mais informações sobre como criar um relatório, consulte o artigo **Criar um relatório personalizado**.
* **Horas orçadas do Planejador de recursos**: nos seguintes relatórios:

   * Relatório do projeto
   * Relatório de Projeto (Dados Financeiros)
   * Relatório de tarefa
   * Relatório de problema
   * Relatório de horas orçadas
