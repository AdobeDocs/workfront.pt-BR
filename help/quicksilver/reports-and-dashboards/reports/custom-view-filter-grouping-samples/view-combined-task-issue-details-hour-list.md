---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Exibir: detalhes combinados de tarefas e problemas em uma lista de Horas"
description: Esta hora visualização combina as colunas Tarefa e Nome do problema, bem como as Horas Planejadas de Tarefa e Problema usando o sharecol tag. Como uma entrada de hora só pode pertencer a uma tarefa ou problema, ambos os objetos não podem aparecer na mesma coluna ao mesmo tempo. Cada linha do visualização é preenchida com as informações de uma Tarefa ou de um Problema.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cf1137fd-c26a-4907-afe9-2373d3434631
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 0%

---

# Exibir: detalhes combinados de tarefa e edição em uma lista hora

Esta hora visualização combina as colunas Tarefa e Nome do problema, bem como as Horas planejadas da Tarefa e do Problema usando o

```
sharecol
```

tag. Como uma entrada de hora só pode pertencer a uma tarefa ou problema, ambos os objetos não podem aparecer na mesma coluna ao mesmo tempo. Cada linha da visualização é preenchida com as informações de uma Tarefa ou um Problema.

Para saber mais sobre o

```
sharecol
```

marca, consulte [Exibir: mesclar informações de várias colunas em uma coluna compartilhada](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).\
![custom_view_hours_with_task_and_issue_information.png](assets/custom-view-hours-with-350x48.png)

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Systems plano da Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Systems licença da Workfront*</td> 
   <td> <p>Solicitação para modificar um visualização </p>
   <p>Planejar a modificação de um relatório</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar uma visualização</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões em um relatório</p> <p>Para obter informações sobre a solicitação de acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Exibir detalhes combinados de tarefas e problemas em uma lista de Horas

Para aplicar esta exibição:

1. Ir para uma lista de horas.
1. No menu suspenso **Exibir**, selecione **Nova Exibição**.

1. Na área **Visualização da coluna**, elimine todas as colunas, exceto uma.
1. Clique no cabeçalho da coluna restante e em **Alternar para Modo de Texto**.
1. Passe o mouse sobre a área de modo de texto e clique em **Clicar para editar o texto**.
1. Remova o texto localizado na caixa **Modo de Texto** e substitua-o pelo seguinte código:
   <pre>column.1.querysort=project:name column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=project:name<br>column.1.valueformat=HTML<br>column.1.width=100<br>column.2.description=Task or Issue<br>column.2.link.linkproperty.0.name=ID column.2.link.linkproperty.0.valuefield=tarefa:ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.lookup=link.visualização<br>column.2.link.valuefield=tarefa:objCode<br><br><br>column.2.link.valueformat=val<br>column.2.linkedname=tarefa<br>column.2.listsort=nested(tarefa).string(name)<br>column.2.name=Task or Issue<br>column.2.querysort=tarefa:name column.2.sharecol=true column..2.querysort=tarefa:name column.2.sharecol=true column..2.querysort=tarefa:name column.2.sharecol=true column..2.querysort=tarefa:name column.2.sharecol=true column.2.querysort=tarefa:name column.2.sharecol=true column.2.querysort=tarefa:name column.2.sharecol=true column.2.querysort=tarefa:name column.2.sharecol=true<br>column.2.querysort=tarefa:name<br>column.2.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=tarefa:name<br>column.2.valueformat=HTML<br>column.2.width=100<br>column.3.descriptionkey=optask<br>column.3.link.linkproperty.0.name=ID<br>column.3.link.linkproperty.0.valuefield=opTask:ID<br>column.3.link.linkproperty.0.valueformat=int<br>column.3.link.lookup=link.visualização<br>column.3.link.valuefield=opTask:objCode column.3.visualização column.3.link.valuefield=opTask:objCode column.3.visualização column.3.link.valuefield=opTask:objCode column.3.visualização column.3.link.valuefield=opTask:objCode<br>column.3.link visualização.valueformat=val<br>column.3.linkedname=optask<br>column.3.listsort=nested(opTask).string(name)<br>column.3.namekey=opTask<br>column.3.querysort=opTask:name<br>column.3.shortview=false<br>column.3.stretch=0<br>column.3.valuefield=opTask: name<br>column.3.valueformat=HTML<br>column.3.width=1<br>column.4.valuefield=tarefa:work<br>column.4.sharecol=true<br>column.4.linkedname=tarefa<br>column.4.valueformat=doubleAsInt<br>column.4.namekey=visualização.relatedcolumn<br>column.4.querysort=tarefa:work<br>column.4.textmode=true<br>column.4.namekeyargkey.0=tarefa<br>column.4.namekeyargkey.1=work<br>column.4.displayname=Planned Effort<br>column.5.displayname=Planned Effort<br>column.5.viewalias=opTask:workrequired column.5.linkedname=opTask<br>column.5.valuefield=opTask:workRequired<br>column.5.valueformat=compound<br>column.5.querysort=opTask:workRequired<br>column.5.namekeyargkey.2 0=opTask<br>column.5.namekeyargkey.1=workrequired<br>column.5.namekey=visualização.relatedcolumn<br>column.5.textmode=true<br>column.6.descriptionkey=hours<br>column.6.linkedname=direct<br>column.6.listsort=doubleAsDouble<br>( hours)<br>column.6.namekey=hours.abbr<br>column.6.querysort=hours<br>column.6.shortview=false<br>column.6.stretch=0<br>column.6.valuefield=hours column.6.valueformat=doubleAsString column.6.width=75 column.6.valuefield=hours<br>column.6.valueformat=doubleAsString<br>column.6.width=75<br>column.6 7.descriptionkey=entrydate<br>column.7.linkedname=direct<br>column.7.listsort=atDateAsAtDate(entryDate)<br>column.7.namekey=entrydate.abbr<br>column.7.querysort=entryDate<br>column.7.shortview=false<br>column.7.stretch=0<br>column.7.valuefield=entryDate<br>column.7.valueformat=atDate<br>column.7.width=75<br>column.8.descriptionkey=description<br>column.8.linkedname=direct<br>column.8.listsort=string(description)<br>column.8.namekey=description.abbr<br>column.8.querysort=description<br>column.8.shortview=false<br>column.8.stretch=0<br>column.8.valuefield=description<br>column.8.valueformat=HTML<br>column.8.width=150</pre>

1. Clique em **Salvar visualização**.
