---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualização: visualização do projeto de várias linhas"
description: Saiba mais sobre a exibição de projeto de várias linhas nos relatórios.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 3c6028c0-2c9f-4f86-aa6c-bf089844bac8
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---

# Exibição: exibição de projeto de várias linhas

Nesta visualização de projeto você pode:

* Exibir informações do projeto em um formato de várias linhas.\
  A exibição usa o

  ```
  sharecol=true
  ```

  para combinar vários campos sob o mesmo cabeçalho de coluna. Para saber mais sobre esta marca, consulte [Exibir: mesclar informações de várias colunas em uma coluna compartilhada](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

* Use uma coluna de espaço reservado que contenha uma tag de quebra de linha de HTML (

  ```
  <br>
  ```

  ) para forçar a Descrição a ser exibida abaixo do nome do projeto, por exemplo.
* Exiba o Proprietário do projeto entre parênteses após o Nome do projeto.
* Exiba o Nome do projeto como um link para o projeto.

![](assets/project-multi-row-stacked-view-350x219.png)

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

## Criar uma exibição de projeto de várias linhas

1. Crie uma nova visualização do projeto. Para obter mais informações sobre como criar uma nova exibição, consulte [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
1. À medida que você constrói a exibição, exclua todas as colunas, exceto uma.
1. Selecione a coluna restante e clique em **Alternar para modo de texto**.
1. Copie e cole o modo de texto abaixo dentro da coluna:
   <pre>column.0.linkedname=direct<br>column.0.link.valueformat=val<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.valuefield=objCode<br>column.0.link.lookup=link.view<br>column.0.sharecol=true<br>column.0.descriptionkey=name<br>coluna.0.descriptionkey=name}column.0.width=150<br>column.0.querysort=name<br>column.0.valuefield=name<br>column.0.name=Nome do Projeto / Gerente / Descrição<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.textmode=true<br>column.0.listsort=string(name)<br>column.0.valueformat=HTML<br>column.1.valuevalueformat expression=CONCAT(" (",{owner}.{name},")")<br>coluna.1.listsort=nested(proprietário).string(nome)<br>coluna.1.width=1<br>coluna.1.linkedname=direct<br>coluna.1.querysort=owner:name<br>coluna.1.textmode=true<br>coluna.1.shortview=false<br>coluna.1.stretch=0<br>coluna.1.valueformat=HTML<br>coluna.1.sharecol=true<br>coluna.2.width=1<br>coluna .2.value=<br><br>column.2.shortview=false<br>column.2.sharecol=true<br>column.2.stretch=0<br>column.2.textmode=true<br>column.2.valueformat=HTML<br>column.3.styledef.style=font-color:#ccc;<br>column.3.descriptionkey=description<br>column.3.linkedname=direct<br>column.3.valuefield=description{2 1}column.3.listsort=string(description)<br>column.3.querysort=description<br>column.3.namekey=description.abbr<br>column.3.textmode=true<br>column.3.sharecol=true<br>column.3.stretch=0<br>column.3.shortview=false<br>column.3.valueformat=HTML<br>column.3.width=1<br>column.4.shortview=false<br>}column.4.value=<br><br>column.4.sharecol=true<br>column.4.width=1<br>column.4.textmode=true<br>column.4.valueformat=HTML\<br>column.4.stretch=0<br>column.5.name=Datas Planejadas / Duração<br>column.5.width=150<br>column.5.querysort=plannedStartDate<br>column.5.share=true 41}coluna.5.stretch=0<br>coluna.5.textmode=true<br>coluna.5.shortview=false<br>coluna.5.linkedname=direct<br>coluna.5.listsort=atDateAsAtDate(plannedStartDate)<br>coluna.5.valuefield=plannedStartDate<br>coluna.5.valueformat=atDate<br>coluna.6.sharecol=true<br>coluna.6.stretch=0 <br>coluna.6.largura=1<br>coluna.6.textmode=true<br>coluna.6.valor=-<br>coluna.6.valueformat=HTML<br>coluna.6.shortview=false<br>coluna.7.namekey=plannedcompletiondate.abbr<br>coluna.7.largura=1<br>coluna.7.sharecol=true<br>coluna.7.shortview=false<br>coluna.7.stretch=0{0 <br>column.7.listsort=atDateAsAtDate(plannedCompletionDate)<br>column.7.linkedname=direct<br>column.7.descriptionkey=plannedcompletiondate<br>column.7.textmode=true<br>column.7.querysort=plannedCompletionDate<br>column.7.valueformat=atDate<br>column.7.valuefield=plannedCompletionDate<br>column.7 .value=<br><br>coluna.8.width=1<br>coluna.8.textmode=true<br>coluna.8.sharecol=true<br>coluna.8.valueformat=HTML<br>coluna.8.stretch=0<br>coluna.9.textmode=true<br>coluna.9.listsort=intAsInt(durationMinutes)<br>coluna.9.stretch=0<br>coluna.9.valuefield=durationFieldLong<br>column.9.descriptionkey=duration<br>column.9.viewalias=duration<br>column.9.querysort=durationMinutes<br>column.9.sharecol=true<br>column.9.width=100<br>column.9.shortview=false<br>column.9.namekey=duration.abbr<br>column.9.linkedname=direct<br>column.9.valueformat=composto<br>column.10.txt mode=true<br>column.10.stretch=0<br><br></pre>

1. Clique em **Salvar visualização**.
