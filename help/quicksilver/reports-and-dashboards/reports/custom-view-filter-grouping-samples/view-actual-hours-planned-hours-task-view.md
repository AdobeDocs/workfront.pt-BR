---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Exibir: Horas Reais sobre Horas Planejadas na mesma coluna de uma Exibição de tarefa'''
description: Nesta exibição de tarefa, a quantidade real de horas registradas em uma tarefa é exibida durante as horas planejadas para cada tarefa.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1179283-dc2e-40d3-b8e0-4b1b79f83ad3
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Exibir: Horas Reais sobre Horas Planejadas na mesma coluna de uma Exibição de tarefa

Nesta exibição de tarefa, a quantidade real de horas registradas em uma tarefa é exibida durante as horas planejadas para cada tarefa.

![real_vs_planejado_em_tarefa_relatório.png](assets/actual-vs-planned-in-task-report-350x58.png)

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

## Exibir Horas Reais sobre Horas Planejadas em uma exibição de tarefa

Para aplicar esta exibição:

1. Vá para uma lista de tarefas.
1. No **Exibir** , selecione **Nova exibição**.

1. No **Visualização de coluna** , elimine todas as colunas, exceto uma.
1. Clique no cabeçalho da coluna restante e, em seguida, clique em **Alternar para o modo de texto**.
1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar texto**.
1. Remova o texto que você encontrar no **Modo de texto** e substitua-a pelo seguinte código:
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.value=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.estich=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.viewalias=atribuições<br>column.1.displayname=<br>column.1.linkedname=direct<br>column.1.namekey=atribuições<br>column.1.valuefield=atribuiçõesListString<br>column.1.valueformat=HTML<br>column.1.tile.name=component.atribumentslist<br>column.2.displayname=Real/ Horas Planejadas<br>column.2.linkedname=direct<br>column.2.namekey=atualworkrequired<br>column.2.querysort=atualWork<br>column.2.textmode=true<br>column.2.valueexpression=CONCAT({actualWorkRequired}/60,' / ',{workRequired}/60)<br>column.2.valuefield=actualWorkRequired<br>column.2.valueformat=composto<br>column.2.viewalias=atualworkrequired<br>column.3.agregator.function=SUM<br>column.3.agregator.valueexpression=SUB({actualWork}, {workRequired})<br>column.3.agregator.valueformat=composto<br>column.3.displayname=Variação de horas<br>column.3.linkedname=direct<br>column.3.textmode=true<br>column.3.valueexpression=SUB({actualWork}, {workRequired})/60<br>column.3.valueformat=customNumberAsString</pre>

1. Clique em **Salvar exibição**.
