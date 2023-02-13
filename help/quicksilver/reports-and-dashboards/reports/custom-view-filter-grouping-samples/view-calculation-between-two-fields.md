---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Exibir: exibir o resultado de um cálculo entre dois campos em uma coluna'''
description: Você pode usar o modo de texto em uma coluna para exibir um cálculo entre dois campos.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# Exibir: exibir o resultado de um cálculo entre dois campos em uma coluna

Você pode usar o modo de texto em uma coluna para exibir um cálculo entre dois campos.

Por exemplo, se você quiser descobrir o número de dias da semana decorridos entre duas datas, é possível usar a sintaxe do modo de texto e as expressões de dados para calcular essa diferença.\
Por exemplo, você pode calcular a diferença de dia da semana entre a Data de Conclusão Planejada e a Data de Conclusão Real de uma tarefa e exibir o resultado em uma coluna.

Você pode usar quaisquer outras duas datas neste cálculo (Início Real, Conclusão Real, Início Projetado, Conclusão Projetada etc.).\
Para obter mais informações sobre expressões de dados calculados, consulte [Expressões de dados calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Relatórios, Painéis, Calendários</p> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Exibir o resultado de um cálculo entre dois campos em uma coluna

Para adicionar esta coluna a uma exibição de tarefa:

1. Vá para uma lista de tarefas.
1. No **Exibir** , clique em **Nova exibição**.

1. Clique em **Adicionar coluna**, em seguida **Alternar para o modo de texto**.

1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar texto**.
1. Remova o texto que você encontrar no **Modo de texto** e substitua-a pelo seguinte código:
   <pre>displayname=Semana de diferença de dia<br>textmode=true<br>valueexpression=WEEKDAYDIFF({planCompletionDate},{actualCompletionDate})<br>valueformat=HTML</pre>

1. (Opcional) Para agregar os valores exibidos na visualização em um agrupamento, siga as etapas descritas em [Agrupamento: exibir o resultado da agregação de vários valores calculados em um agrupamento](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. Clique em **Salvar**, em seguida **Salvar exibição**.
