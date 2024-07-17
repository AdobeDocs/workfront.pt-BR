---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "View: exibir o resultado de um cálculo entre dois campos em uma coluna"
description: Você pode usar o modo de texto em uma coluna para exibir um cálculo entre dois campos.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---

# Exibir: exibir o resultado de um cálculo entre dois campos em uma coluna

Você pode usar o modo de texto em uma coluna para exibir um cálculo entre dois campos.

Por exemplo, se você quiser descobrir o número de dias da semana decorridos entre duas datas, poderá usar a sintaxe do modo de texto e as expressões de dados para calcular essa diferença.\
Por exemplo, você pode calcular a diferença de dia da semana entre a Data de conclusão planejada e a Data de conclusão real de uma tarefa e exibir o resultado em uma coluna.

Você pode usar quaisquer outras duas datas nesse cálculo (Início Efetivo, Conclusão Efetiva, Início Projetado, Conclusão Projetada etc.).\
Para obter mais informações sobre expressões de dados calculados, consulte [Visão geral de expressões de dados calculados](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitação para modificar uma exibição </p>
   <p>Planejar a modificação de um relatório</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar uma visualização</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Exibir o resultado de um cálculo entre dois campos em uma coluna

Para adicionar esta coluna a uma visualização de tarefa:

1. Ir para uma lista de tarefas.
1. No menu suspenso **Exibir**, clique em **Nova Exibição**.

1. Clique em **Adicionar Coluna** e em **Alternar para Modo de Texto**.

1. Passe o mouse sobre a área do modo de texto e clique em **Clicar para editar o texto**.
1. Remova o texto localizado na caixa **Modo de Texto** e substitua-o pelo seguinte código:
   <pre>displayname=Week Day Difference<br>textmode=true<br>valueexpression=WEEKDAYDIFF({plannedCompletionDate},{actualCompletionDate})<br>valueformat=HTML</pre>

1. (Opcional) Para agregar os valores exibidos na exibição em um agrupamento, siga as etapas descritas em [Agrupamento: exibir o resultado da agregação de vários valores calculados em um agrupamento](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. Clique em **Salvar** e depois em **Salvar exibição**.
