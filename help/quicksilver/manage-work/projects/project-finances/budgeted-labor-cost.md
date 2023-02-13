---
content-type: reference
product-area: projects
navigation-topic: financials
title: Entender o Custo da Mão de obra Orçada e as Horas Orçamentadas para Projetos
description: Entender o Custo da Mão de obra Orçada e as Horas Orçamentadas para Projetos
author: Alina
feature: Work Management
exl-id: 01020bbb-7cf9-4461-b0b6-dcbbc537c616
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 0%

---

# Entender o Custo da Mão de obra Orçada e as Horas Orçamentadas para Projetos

<!--
<(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)</p>
-->

Você pode orçar seus recursos para trabalhar usando o Adobe Workfront Resource Planner.

À medida que você faz o orçamento de seus recursos para trabalhar em projetos, a Workfront calcula o Custo da Mão de Obra Orçada para as funções, projetos e usuários com base nos valores de custo por hora.

O Custo da Mão de obra Orçada do Planejador de Recursos de um projeto é um cálculo entre o custo associado às funções do job atribuídas para concluir o trabalho no projeto e a quantidade de horas estimadas (Horas Orçadas do Planejador de Recursos) que podem tomar cada função para concluir o trabalho.

>[!IMPORTANT]
>
>O Custo da Mão de obra Orçada pelo Planejador de Recursos para usuários não afeta o do projeto. Apenas o custo da mão de obra para funções de emprego afeta o custo do projeto.

## Visão Geral do Custo da Mão-de-Obra Orçada para Funções de Cargo e do Projeto

O Workfront usa o Custo da Mão-de-Obra Orçada das funções de cargo no projeto para calcular o Custo da Mão-de-Obra Orçada do projeto.

>[!TIP]
>
>O Custo da Mão-de-Obra Orçada de um projeto no Caso de Negócios é exibido como Custo da Mão-de-Obra Orçada pelo Planejador de Recursos em relatórios e listas.

O **Custo de Mão-de-Obra Orçada** (ou Custo de Mão-de-Obra Orçada do Planejador de Recursos) de um projeto é calculado pela seguinte fórmula:

`Resource Planner Budgeted Labor Cost = SUM ( Resource Planner Budgeted Hours for each job role on the project * Cost per Hour rate of each job role on the project)`

Os campos usados no cálculo acima se referem ao seguinte:

* As horas orçadas para funções de cargo na área Orçamento de Recursos do projeto ou no Planejador de Recursos.

   Para obter mais informações sobre como orçar recursos no Planejador de Recursos, consulte a seção &quot;Recursos de Orçamento no Planejador de Recursos&quot; no artigo [Visão geral do Planejador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   Para obter mais informações sobre como orçamentar recursos na área Orçamento de Recursos do Caso de Negócios, consulte [Recursos orçamentários no Caso de Negócios](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

* O **Custo por Hora taxa de uma função de cargo** no cálculo acima refere-se ao custo associado a cada função de cargo no projeto.\
   Para obter mais informações sobre como criar e gerenciar funções de cargo e associá-las a taxas de Custo, consulte o artigo [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

>[!NOTE]
>
>O Workfront calcula todas as informações de custo usando a moeda do projeto. Se você especificar Horas Orçadas para seus recursos no Planejador de Recursos, a opção para alterar a moeda do projeto será desativada.\
>Para obter mais informações sobre como alterar a moeda de um projeto, consulte o artigo [Alterar a moeda do projeto](../../../manage-work/projects/project-finances/change-project-currency.md).

## Visão Geral do Custo da Mão-de-Obra Orçada para Usuários

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Update the following section in the Create a Business Case article, as well, when you update it here.)</p>
-->

>[!IMPORTANT]
>
>O Custo da Mão-de-Obra Orçada pelo Usuário não afeta o Custo da Mão-de-Obra Orçada do projeto. Somente o custo da mão de obra das funções de cargo em um projeto afeta o Custo da Mão de obra Orçada pelo Planejador de Recursos do projeto.
> 
>O total de todos os custos de mão de obra de todos os usuários pode ou não ser igual ao Custo de Trabalho Orçado do Planejador de Recursos das funções de cargo associadas aos usuários.
>
>Se você estimar Horas Orçadas para usuários no Planejador de Recursos, os custos associados a eles serão os das funções de job associadas aos usuários. Eles não são custos associados aos usuários ou suas taxas.

Se os usuários estiverem associados às funções do trabalho no projeto e suas horas forem orçadas no Planejador de Recursos, o Custo da Mão-de-Obra Orçada será exibido pelos seguintes nomes, dependendo de onde você os exibir no Workfront:

* [!UICONTROL **Custo de Mão-de-Obra Orçada**]: A área do Orçamento de Recursos do Caso de Negócios, sob as respectivas funções.

   ![](assets/budgeted-labor-cost-for-users-in-business-case-highlighted-350x73.png)

* [!UICONTROL **BDG**]: O Planejador de Recursos ao exibir informações na exibição Projeto e Função por Custo.

   ![](assets/budgeted-labor-cost-for-users-in-rp-project-view-cost--highlighted-350x115.png)

Os usuários são exibidos na área Orçamento de Recursos do Caso de Negócios em suas respectivas funções ou no Planejador de Recursos se atenderem aos seguintes requisitos:

* Eles estão associados a uma das funções do trabalho no projeto.
* Eles orçamentaram Horas especificadas no Planejador de Recursos.
* Eles têm uma Taxa de Custo por Hora associada ao perfil.

   Para obter mais informações sobre como adicionar as taxas de Custo por Hora aos usuários, consulte o artigo [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* O usuário faz parte de um dos Grupos de Recursos associados ao projeto.

O Custo de Mão-de-Obra Orçado de um usuário é calculado pela seguinte fórmula:

`User Budgeted Labor Cost = Budgeted hours for the user on the project * Cost per Hour rate of the user`

## Localizar o Custo de Mão-de-Obra Orçado de um projeto

O Custo da Mão-de-Obra Orçada conforme refletido na área Orçamento de Recursos do Caso de Negócios ou no Planejador de Recursos é exibido nas seguintes áreas do Workfront sob os seguintes nomes:

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>Nome de exibição Custo de mão de obra orçada</strong></td> 
     <td><strong>Área do Workfront</strong></td> 
    </tr> 
    <tr> 
     <td>Custo do Trabalho Orçado</td> 
     <td>Área do Orçamento dos Recursos do Caso de Negócios</td> 
    </tr> 
    <tr> 
     <td>Custo Orçado</td> 
     <td><p>Relatório de utilização - Vista de custo</p><p>Para obter mais informações, consulte <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">Exibir informações de utilização</a> .</p></td> 
    </tr> 
    <tr> 
     <td>BDG </td> 
     <td>Exibições de Projeto ou Função do Planejador de Recursos, por Custo</td> 
    </tr> 
    <tr> 
     <td>Custo de Mão-de-Obra Orçada do Projeto do Planejador de Recursos</td> 
     <td> <p>Relatório de projeto</p> <p>Relatório do Projeto (Dados Financeiros)</p> <p>Relatório de tarefa</p> <p>Relatório de problemas</p> <p>Relatório de Hora Orçamentada</p> <p>Para obter informações sobre como criar um relatório, consulte o artigo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Criar um relatório personalizado</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>

>[!NOTE]
>
>Se você usar o Planejador de Cenário do Adobe Workfront para orçar os recursos do projeto, o Custo da Mão-de-Obra Orçada na área de Orçamento de Recursos do Caso de Negócios será o mesmo que os Custos de Pessoas da iniciativa vinculada ao projeto. O Planejador de cenário está disponível somente na nova experiência do Adobe Workfront e requer uma licença adicional. Para obter informações sobre o Planejador de Cenário do Workfront, consulte [A visão geral do Planejador de cenário](../../../scenario-planner/scenario-planner-overview.md). Para obter informações sobre como orçar recursos usando o Planejador de Cenário, consulte [Recursos de orçamento no Caso de negócios usando o Planejador de cenário](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## Localizar as Horas Orçadas de um projeto

<!--
(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)
-->

As Horas Orçadas afetam o valor do Custo da Mão-de-Obra Orçada (ou o Custo Orçado do Planejador de Recursos) do projeto.

O Custo da Mão-de-Obra Orçada de um projeto é o custo associado às funções de cargo atribuídas para concluir o trabalho no projeto e a quantidade de horas estimadas (Horas Orçadas) que podem tomar cada função para concluir o trabalho.

Você pode exibir as Horas Orçadas no Workfront nos campos listados na tabela abaixo.

>[!NOTE]
>
>Qualquer outra menção de &quot;Horas orçadas&quot; no Workfront se refere às horas orçadas usando recursos obsoletos que foram removidos do Workfront. Esses são campos somente visualização e não são atualizados com as informações atuais quando você usa as ferramentas de orçamento de recursos atuais.

As horas orçadas na área Orçamento de Recursos do Caso de Negócios ou do Planejador de Recursos são exibidas nas seguintes áreas do Workfront e sob os seguintes nomes:

* **Horas**: Área do Orçamento dos Recursos do Caso de Negócios
* **BDG**:Planejador de recursos exibido por Horas
* **Horas Orçamentadas**: Exibição de Horas do relatório de Utilização Para obter informações, consulte [Exibir informações de utilização de recursos](../../../resource-mgmt/resource-utilization/view-utilization-information.md).
* **Bud. Horas**: Relatório de Hora Orçamentada

   O objeto Hora do Orçamento no relatório Hora do Orçamento refere-se a informações relacionadas a uma ferramenta de gerenciamento de recursos obsoleta. Apenas o &quot;Bud&quot;. O campo Horas neste relatório refere - se às horas orçadas no Planejador de Recursos ou na área de Orçamento de Recursos do Caso de Negócios do projeto.

   Para obter mais informações sobre como criar um relatório, consulte o artigo **Criar um relatório personalizado**.
* **Horas Orçadas do Planejador de Recursos**: nos seguintes relatórios:

   * Relatório de projeto
   * Relatório do Projeto (Dados Financeiros)
   * Relatório de tarefa
   * Relatório de problemas
   * Relatório de Hora Orçamentada
