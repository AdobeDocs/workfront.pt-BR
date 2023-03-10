---
content-type: reference
product-area: reporting;projects
keywords: calculado,agregações,avançado,exibições
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Agrupamento: exibir o resultado da agregação de vários valores calculados em um agrupamento'''
description: Você pode usar o modo de texto em uma coluna para exibir um cálculo entre dois campos na visualização de um relatório ou lista. Cada linha exibe o cálculo para cada objeto no relatório ou na lista.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# Agrupamento: exibir o resultado da agregação de vários valores calculados em um agrupamento

Você pode usar o modo de texto em uma coluna para exibir um cálculo entre dois campos na visualização de um relatório ou lista. Cada linha exibe o cálculo para cada objeto no relatório ou na lista.

Por exemplo, você pode exibir a diferença entre Horas Reais e Horas Planejadas em uma terceira coluna chamada Saldo de Trabalho para cada tarefa em um relatório de tarefa. Para obter mais informações sobre expressões de dados calculados, consulte [Expressões de dados calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

É possível exibir o valor agregado de vários itens de exibição calculados na mesma coluna de um agrupamento adicionando um cálculo ao `aggregator` da coluna que contém o valor calculado. Por exemplo, você pode agregar (exibir a soma de) a quantidade de horas de Saldo de Trabalho de todas as tarefas no agrupamento do relatório ou a lista da coluna Saldo de Trabalho. Este artigo descreve como fazer isso.

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

## Exibir o resultado da agregação de vários valores calculados em um agrupamento

1. Vá para um relatório de tarefa, clique em **Ações de Relatório** > **Editar**.
1. No **Agrupamentos** clique em **Adicionar agrupamento** e comece a digitar **Nome do projeto** no **Agrupar seu relatório** > **Primeiro a** e, em seguida, selecione-o quando for exibido na lista.

1. No **Colunas (Exibir)** clique em **Adicionar coluna**, em seguida, comece a digitar **Horas Planejadas** no **Mostrar nesta coluna** e, em seguida, selecione-o quando for exibido na lista.

   >[!TIP]
   >
   >Sempre comece a adicionar quantas informações usando a interface Padrão antes de editar informações no modo de texto. Adicione campos que estão mais próximos ou contêm a maior quantidade de informações que você está tentando fazer para o cálculo.

1. No **Resumir esta coluna por** , selecione **Soma**, depois clique em **Concluído**.
1. Clique em **Alternar para o modo de texto** na coluna adicionada.
1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar texto**.
1. Substitua o `valuefield ` e `aggregator.valuefield` linhas com as linhas realçadas no seguinte exemplo de modo de texto:

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
   valueexpression=CONCAT(ROUND(({workRequired}-{actualWorkRequired})/60,2)," Hours") viewalias=workrequired displayname=Work Balance
   ```

   >[!TIP]
   >
   >Para obter o valor agregado no agrupamento para exibir a diferença agregada entre os campos Horas Planejadas e Horas Reais, insira a mesma equação no `aggregator.valuefield` linha. O `aggregator.displayformat` usado para a coluna Horas planejadas converte minutos em horas. Como o campo Horas Planejadas foi usado como espaço reservado, essa linha não precisa ser ajustada.
   >
   >
   >O `minutesAsHoursString` definição da `aggregator.displayformat` linha significa que não há necessidade de dividir cada campo por 60, conforme feito na variável `valueexpression` para os resultados. Neste `aggregator.valuefield=workRequired` torna-se: `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`.

1. Clique em **Salvar+Fechar**.
