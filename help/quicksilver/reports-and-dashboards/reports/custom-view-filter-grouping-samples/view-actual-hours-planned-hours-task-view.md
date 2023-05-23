---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "View: Horas efetivas sobre horas planejadas na mesma coluna de uma View de tarefa"
description: Nesta visualização de tarefa, a quantidade real de horas registradas em uma tarefa são exibidas sobre as horas planejadas para cada tarefa.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1179283-dc2e-40d3-b8e0-4b1b79f83ad3
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# View: Horas Reais sobre Horas Planejadas na mesma coluna de uma View de tarefa

Nesta visualização de tarefa, a quantidade real de horas registradas em uma tarefa são exibidas sobre as horas planejadas para cada tarefa.

![atual_vs_planned_in_task_report.png](assets/actual-vs-planned-in-task-report-350x58.png)

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
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
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Visualizar Horas efetivas sobre horas planejadas em uma visualização de tarefa

Para aplicar esta exibição:

1. Ir para uma lista de tarefas.
1. No **Exibir** selecione **Nova visualização**.

1. No **Visualização da coluna** elimine todas as colunas, exceto uma.
1. Clique no cabeçalho da coluna restante e clique em **Alternar para modo de texto**.
1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar o texto**.
1. Remova o texto localizado na **Modo de texto** e substitua-o pelo seguinte código:
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=nome<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.viewalias=atribuições<br>column.1.displayname=<br>column.1.linkedname=direct<br>column.1.namekey=atribuições<br>column.1.valuefield=assiassignmentListString<br>column.1.valueformat=HTML<br>column.1.tile.name=component.assignmentslist<br>column.2.displayname=Horas Reais/ Planejadas<br>column.2.linkedname=direct<br>column.2.namekey=atualworkrequired<br>column.2.querysort=atualWork<br>column.2.textmode=true<br>column.2.valueexpression=CONCAT({atualWorkRequired}/60,' / ',{workRequired}/60)<br>column.2.valuefield=atualWorkRequired<br>column.2.valueformat=composto<br>column.2.viewalias=atualworkrequired<br>column.3.aggregator.function=SUM<br>column.3.aggregator.valueexpression=SUB({atualWork}, {workRequired})<br>column.3.aggregator.valueformat=composto<br>column.3.displayname=Variação de Horas<br>column.3.linkedname=direct<br>column.3.textmode=true<br>column.3.valueexpression=SUB({atualWork}, {workRequired})/60<br>column.3.valueformat=customNumberAsString</pre>

1. Clique em **Salvar visualização**.
