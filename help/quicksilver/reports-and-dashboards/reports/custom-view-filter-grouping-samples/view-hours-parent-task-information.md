---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Exibir: horas com informações da tarefa pai'''
description: Essa exibição de hora exibe o nome da tarefa em que as horas foram registradas, bem como o nome da tarefa pai.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c24555fc-3bae-451b-8a44-28a8158199d1
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# Exibir: horas com informações da tarefa pai

Essa exibição de hora exibe o nome da tarefa em que as horas foram registradas, bem como o nome da tarefa pai.

![custom_hour_view_with_task_and_parent_task_info.png](assets/custom-hour-view-with-task-and-parent-task-info-350x55.png)

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

## Exibir horas com informações de tarefa pai

1. Vá para uma lista de horas.
1. No **Exibir** , selecione **Nova exibição**.

1. No **Visualização de coluna** , elimine todas as colunas, exceto uma.
1. Clique no cabeçalho da coluna restante e, em seguida, clique em **Alternar para o modo de texto**.
1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar texto**.
1. Remova o texto que você encontrar no **Modo de texto** e substitua-a pelo seguinte código:
   <pre>column.0.agregator.displayformat=doubleAsString<br>column.0.agregator.function=SUM<br>column.0.agregator.name=hours<br>column.0.agregator.valuefield=hours<br>column.0.agregator.valueformat=doubleAsDouble<br>column.0.descriptionkey=hours<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.value=val<br>column.0.linkedname=direct<br>column.0.listsort=doubleAsDouble(hours)<br>column.0.namekey=hours.abbr<br>column.0.querysort=hours<br>column.0.shortview=false<br>column.0.estich=100<br>column.0.valuefield=hours<br>column.0.valueformat=doubleAsString<br>column.0.width=150<br>column.1.descriptionkey=task<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=task:ID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup=link.view<br>column.1.link.valuefield=task:objCode<br>column.1.link.value=val<br>column.1.linkedname=task<br>column.1.listsort=nested(task).string(name)<br>column.1.namekey=task<br>column.1.querysort=task:name<br>column.1.shortview=false<br>column.1.alongch=0<br>column.1.valuefield=task:name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.description=Nome da tarefa pai<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=task:parent:ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.lookup=link.view<br>column.2.link.valuefield=task:objCode<br>column.2.link.value.format=val<br>column.2.linkedname=task<br>column.2.listsort=nested(task:parent).string(name)<br>column.2.name=Nome da tarefa pai<br>column.2.querysort=task:parent:name<br>column.2.shortview=false<br>column.2.alongch=0<br>column.2.valuefield=task:parent:name<br>column.2.valueformat=HTML<br>column.2.width=150</pre>

1. Clique em **Salvar exibição**.
