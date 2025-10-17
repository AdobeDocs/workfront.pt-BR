---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Exibir: exibir o resultado de um cálculo entre dois campos em uma coluna'
description: Você pode usar o modo de texto em uma coluna para exibir um cálculo entre dois campos.
author: Lisa and Jenny
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# Exibir: exibir o resultado de um cálculo entre dois campos em uma coluna

<!--Audited: 11/2024-->

Você pode usar o modo de texto em uma coluna para exibir um cálculo entre dois campos.

Por exemplo, se você quiser descobrir o número de dias da semana decorridos entre duas datas, poderá usar a sintaxe do modo de texto e as expressões de dados para calcular essa diferença.\
Por exemplo, você pode calcular a diferença de dia da semana entre a Data de conclusão planejada e a Data de conclusão real de uma tarefa e exibir o resultado em uma coluna.

Você pode usar quaisquer outras duas datas nesse cálculo (Início Efetivo, Conclusão Efetiva, Início Projetado, Conclusão Projetada etc.).\
Para obter mais informações sobre expressões de dados calculados, consulte [Visão geral de expressões de dados calculados](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

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
   <p>Colaborador ou Solicitação para modificar um filtro </p>
   <p>Padrão ou Plano para modificar um relatório</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar um filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Exibir o resultado de um cálculo entre dois campos em uma coluna

Para adicionar esta coluna a uma visualização de tarefa:

1. Ir para uma lista de tarefas.
1. No menu suspenso **Exibir**, clique em **Nova Exibição**.

1. Clique em **Adicionar Coluna** e em **Alternar para Modo de Texto** > **Editar Modo de Texto**.
1. Remova o texto localizado na caixa **Modo de Texto** e substitua-o pelo seguinte código:

   ```
   displayname=Week Day Difference
   textmode=true
   valueexpression=WEEKDAYDIFF({plannedCompletionDate},{actualCompletionDate})
   valueformat=HTML
   ```

1. (Opcional) Para agregar os valores exibidos na exibição em um agrupamento, siga as etapas descritas em [Agrupamento: exibir o resultado da agregação de vários valores calculados em um agrupamento](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. Clique em **Concluído** e depois em **Salvar exibição**.
