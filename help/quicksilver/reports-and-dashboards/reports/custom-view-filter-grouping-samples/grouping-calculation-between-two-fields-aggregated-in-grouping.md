---
content-type: reference
product-area: reporting;projects
keywords: calculado,agregações,avançado,exibições
navigation-topic: custom-view-filter-and-grouping-samples
title: "Agrupamento: exibir o resultado da agregação de vários valores calculados em um agrupamento"
description: Você pode usar o modo texto em uma coluna para exibir um cálculo entre dois campos na exibição de um relatório ou lista. Cada linha exibe o cálculo de cada objeto no relatório ou lista.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---

# Grouping: exibe o resultado da agregação de vários valores calculados em um agrupamento

Você pode usar o modo texto em uma coluna para exibir um cálculo entre dois campos na exibição de um relatório ou lista. Cada linha exibe o cálculo de cada objeto no relatório ou lista.

Por exemplo, você pode exibir a diferença entre as Horas Reais e as Horas Planejadas em uma terceira coluna chamada Saldo de Trabalho para cada tarefa em um relatório de tarefa. Para obter mais informações sobre expressões de dados calculados, consulte [Visão geral de expressões de dados calculados](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Você pode exibir o valor agregado de vários itens de exibição calculados na mesma coluna em um agrupamento adicionando um cálculo à linha `aggregator` da coluna que contém o valor calculado. Por exemplo, você pode agregar (exibir a soma de) a quantidade de horas de Saldo de Trabalho de todas as tarefas no agrupamento do relatório ou na lista para a coluna Saldo de Trabalho. Este artigo descreve como fazer isso.

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
   <td> <p>Solicitação para modificar um agrupamento </p>
   <p>Planejar a modificação de um relatório</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar um agrupamento</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Exibir o resultado da agregação de vários valores calculados em um agrupamento

1. Vá para um relatório de tarefa, clique em **Ações de Relatório** > **Editar**.
1. Na guia **Agrupamentos**, clique em **Adicionar Agrupamento** e comece a digitar o **Nome do Projeto** no campo **Agrupar seu Relatório** > **Primeiro por** e selecione-o quando ele for exibido na lista.

1. Na guia **Colunas(Modo de Exibição)**, clique em **Adicionar Coluna** e comece a digitar **Horas Planejadas** no campo **Mostrar nesta coluna**. Em seguida, selecione-a quando ela for exibida na lista.

   >[!TIP]
   >
   >Sempre comece a adicionar o máximo de informações usando a interface Padrão antes de editar as informações no modo de texto. Adicione campos que estejam mais próximos ou que contenham a maior quantidade de informações que você está tentando fazer para o cálculo.

1. No campo **Resumir esta coluna por**, selecione **Soma** e clique em **Concluído**.
1. Clique em **Alternar para Modo de Texto** na coluna adicionada.
1. Passe o mouse sobre a área do modo de texto e clique em **Clicar para editar o texto**.
1. Substitua as linhas `valuefield ` e `aggregator.valuefield` pelas linhas realçadas no seguinte exemplo de modo de texto:

   ```
   valueformat=compound
   aggregator.displayformat=minutesAsHoursString
   aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2)
   aggregator.function=SUM
   aggregator.valueformat=val
   aggregator.namekey=workrequired
   linkedname=direct
   textmode=true
   valuefield=workRequired
   namekey=workrequired
   valueexpression=CONCAT(ROUND(({workRequired}-{actualWorkRequired})/60,2)," Hours") 
   viewalias=workrequired 
   displayname=Work Balance
   ```

   >[!TIP]
   >
   >Para obter o valor agregado no agrupamento e exibir a diferença agregada entre os campos Horas Planejadas e Horas Efetivas, insira a mesma equação na linha `aggregator.valuefield`. O `aggregator.displayformat` usado para a coluna Horas Planejadas converte minutos em horas. Como o campo Horas planejadas foi usado como um espaço reservado, essa linha não precisa ser ajustada.
   >
   >
   >A definição `minutesAsHoursString` da linha `aggregator.displayformat` significa que não há necessidade de dividir cada campo por 60, como concluído em `valueexpression` para os resultados. Neste `aggregator.valuefield=workRequired` torna-se: `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`.

1. Clique em **Salvar+Fechar**.
