---
content-type: reference
product-area: projects
navigation-topic: financials
title: Calcular Custo Orçamentado
description: Calcular o andamento do projeto CostTracking Orçado com um Relatório de Utilização""
author: Alina
feature: Work Management
exl-id: e96fe38f-58c2-4938-9d2d-81d1109123fa
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 2%

---

# Calcular Custo Orçamentado

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: This article is linked from "Tracking Project Progress with a Utilization Report"</p>
<p>Keep the structure of this article similar to Calculating Budgeted Labor Cost)</p>
</div>
-->

O Custo orçado de um projeto é o custo total associado ao projeto, conforme estimado quando você planeja o projeto.

## Visão Geral do Custo Orçado em um projeto

Não é possível alterar manualmente o Custo Orçado de um projeto. O Adobe Workfront calcula o Custo Orçado usando a seguinte fórmula:

`Budgeted Cost = Resource Planner Budgeted Labor Cost + Budgeted Expenses Cost + Fixed Cost of the project`

* O **Custo de Mão-de-Obra Orçada do Planejador de Recursos** no cálculo acima está o custo associado às funções de trabalho no projeto.

   Você pode rastrear o Custo da Mão de Obra Orçada de um projeto na área Orçamento de Recursos do Caso de Negócios ou do Planejador de Recursos.

   >[!TIP]
   >
   >  O Custo da Mão-de-Obra Orçada de um projeto no Caso de Negócios é exibido como Custo da Mão-de-Obra Orçada pelo Planejador de Recursos em relatórios e listas.

   Para obter informações sobre Custos de Mão de obra Orçados, consulte o artigo [Entender o Custo da Mão de obra Orçada e as Horas Orçamentadas para Projetos](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* O **Custo de Despesas Orçamentadas** no cálculo acima está o Custo Planejado associado às despesas do projeto, como são calculadas na área Despesas do Caso de Negócios ou na guia Despesas do projeto.\
   Para obter mais informações sobre Despesas em um projeto, consulte o artigo [Gerenciar despesas do projeto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* O **Custo Fixo** no cálculo acima está o valor fixo associado ao Custo do projeto, conforme definido na área Finanças da seção Detalhes do projeto.\
   Para obter mais informações sobre a subguia Finanças de um projeto, consulte o artigo [Gerenciar informações na área de finanças do projeto](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

>[!NOTE]
>
>O Workfront calcula todas as informações de custo usando a moeda do projeto. Se você especificar Horas Orçadas para seus recursos no Planejador de Recursos, a opção para alterar a moeda do projeto será desativada.
>
>Para obter mais informações sobre como alterar a moeda de um projeto, consulte o artigo [Alterar a moeda do projeto](../../../manage-work/projects/project-finances/change-project-currency.md).

## Localizar o Custo Orçado de um projeto

O Custo Orçado conforme refletido na área Orçamento de Recursos do Caso de Negócios ou no Planejador de Recursos é exibido nas seguintes áreas do Workfront sob os seguintes nomes:

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>Nome de exibição de Custo orçado</strong></td> 
     <td><strong>Área do Workfront</strong></td> 
    </tr> 
    <tr> 
     <td>Custo Orçado</td> 
     <td> <p>Resumo de Business Case</p> <p> <img src="assets/business-case-summary-qs-350x453.png" style="width: 350;height: 453;"> </p> </td> 
    </tr> 
    <tr> 
     <td>Custo</td> 
     <td> <p>Portfolio Otimizer</p> <p>Dica: O total de todos os valores de Custo Orçado do projeto é o Custo Orçado do portfólio.</p> </td> 
    </tr> 
    <tr> 
     <td>Custo orçado do projeto</td> 
     <td> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (NOTE: this was removed with flash)</p>
      --> <p>Relatório de projeto</p> <p>Relatório do Projeto (Dados Financeiros)</p> <p>Relatório de tarefa</p> <p>Relatório de problemas</p> <p>Relatório de Hora Orçamentada</p> <p>Para obter mais informações sobre como criar um relatório, consulte o artigo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Criar um relatório personalizado</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>
