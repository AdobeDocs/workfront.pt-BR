---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Exibir: exibe o resultado de um cálculo entre dois campos em uma coluna'
description: You can use text mode in a column to display a calculation between two fields.
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 20%

---

# Exibir: exibe o resultado de um cálculo entre dois campos em uma coluna

<!--Audited: 11/2024-->

You can use text mode in a column to display a calculation between two fields.

For example, if you want to find out the number of week days that elapsed between two dates, you can use text mode syntax and data expressions to calculate this difference.\
For example, you can calculate the week day difference between the Planned Completion Date and the Actual Completion Date of a task and display the result in a column.

You can use any other two dates in this calculation (Actual Start, Actual Completion, Projected Start, Projected Completion, etc).\
For more information about calculated data expressions, see [Overview of calculated data expressions](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Colaborador ou solicitação para modificar um filtro </p>
   <p>Padrão ou Plano para modificar um relatório</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso de edição a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a filtros, exibições e agrupamentos para modificar um filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Display the result of a calculation between two fields in a column

To add this column to a task view:

1. Ir para uma lista de tarefas.
1. No menu suspenso **Exibição**, clique em **Nova Exibição**.

1. Click **Add Column**, then **Switch to Text Mode** > **Edit Text Mode**.
1. Remove the text you find in the **Text Mode** box, and replace it with the following code:

   ```
   displayname=Week Day Difference
   textmode=true
   valueexpression=WEEKDAYDIFF({plannedCompletionDate},{actualCompletionDate})
   valueformat=HTML
   ```

1. (Optional) To aggregate the values displayed in the view in a grouping, follow the steps described in [Grouping: display the result of aggregating multiple calculated values in a grouping](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. Clique em **Concluído** e depois em **Salvar exibição**.
