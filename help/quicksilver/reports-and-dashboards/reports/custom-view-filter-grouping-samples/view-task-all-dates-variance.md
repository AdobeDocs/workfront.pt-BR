---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: Tarefa com Todas as Variações de Datas'
description: Essa exibição de tarefa é semelhante à exibição "Todas as datas" fornecida com sua conta da Adobe Workfront. Essa exibição específica inclui colunas de Variação, que calculam a diferença em dias entre datas.
author: Nolan
feature: Reports and Dashboards
exl-id: 20df7cd8-113e-4c0d-b3f5-1def7db968a5
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# View: tarefa com variação de Todas as Datas

<!--Audited: 11/2024-->

Essa exibição de tarefa é semelhante à exibição &quot;Todas as datas&quot; fornecida com sua conta da Adobe Workfront. Esta exibição específica inclui colunas de *Variação*, que calculam a diferença em dias entre as seguintes datas:

* Datas de Início Planejadas e Projetadas
* Datas de Início Planejadas e Efetivas
* Datas de Término Planejadas e Projetadas
* Datas de Término Planejadas e Efetivas

Essa exibição representa um exemplo de colunas calculadas, nas quais você pode obter os valores de duas colunas diferentes e conectá-los por um cálculo para obter um terceiro valor. Nesse caso, você subtrai a data 1 da data 2.

Para obter mais informações sobre o uso de cálculos em uma Exibição, consulte a seção [Visão Geral dos usos comuns do Modo de Texto](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md) em  [Visão geral dos usos comuns do Modo de Texto](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

![Exibir tarefa com todas as datas](assets/view-task-with-all-dates-variance.png)

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p> Atual: 
   <ul>
   <li>Solicitação para modificar uma exibição</li> 
   <li>Planejar a modificação de um relatório</li>
   </ul>
     </p>
     <p> Novo: 
   <ul>
   <li>Colaborador para modificar uma visualização</li> 
   <li>Padrão para modificar um relatório</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar uma visualização</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exibir tarefas com variação de Todas as Datas

1. Ir para uma lista de tarefas.
1. No menu suspenso **Exibir**, selecione **Nova Exibição**.

1. Na área **Visualização da coluna**, elimine todas as colunas, exceto uma.
1. Clique no cabeçalho da coluna restante e em **Alternar para Modo de Texto** > **Editar Modo de Texto**.
1. Remova o texto localizado na caixa **Editar Modo de Texto** e substitua-o pelo seguinte código:

   ```
   column.1.descriptionkey=name
   column.1.link.linkproperty.0.name=ID
   column.1.link.linkproperty.0.valuefield=ID
   column.1.link.linkproperty.0.valueformat=int
   column.1.link.lookup=link.view
   column.1.link.valuefield=objCode
   column.1.link.valueformat=val
   column.1.linkedname=direct
   column.1.listsort=string(name)
   column.1.namekey=name.abbr
   column.1.querysort=name
   column.1.shortview=false
   column.1.stretch=95
   column.1.styledef.case.0.comparison.attribute=css
   column.1.styledef.case.0.comparison.isrowcase=true
   column.1.styledef.case.0.comparison.leftmethod=intAsInt(numberOfChildren)
   column.1.styledef.case.0.comparison.lefttext=numberOfChildren
   column.1.styledef.case.0.comparison.operator=gt
   column.1.styledef.case.0.comparison.operatortype=int
   column.1.styledef.case.0.comparison.righttext=0
   column.1.styledef.case.0.comparison.trueproperty.0.name=fontstyle
   column.1.styledef.case.0.comparison.trueproperty.0.value=bold
   column.1.styledef.case.0.comparison.truetext=
   column.1.styledef.case.0.comparison.usefield=false
   column.1.valuefield=name
   column.1.valueformat=HTML
   column.1.width=150
   column.2.descriptionkey=plannedstartdate
   column.2.linkedname=direct
   column.2.listsort=atDateAsAtDate(plannedStartDate)
   column.2.namekey=plannedstartdate.abbr
   column.2.querysort=plannedStartDate
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=plannedStartDate
   column.2.valueformat=atDate
   column.2.width=75
   column.3.descriptionkey=projectedstartdate
   column.3.linkedname=direct
   column.3.listsort=atDateAsAtDate(projectedStartDate)
   column.3.namekey=projectedstartdate.abbr
   column.3.querysort=projectedStartDate
   column.3.shortview=false
   column.3.stretch=0
   column.3.valuefield=projectedStartDate
   column.3.valueformat=atDate
   column.3.width=75
   column.4.descriptionkey=plannedstartdate
   column.4.displayname=Projected Start Variance
   column.4.linkedname=direct
   column.4.listsort=atDateAsAtDate(plannedStartDate)
   column.4.namekey=plannedstartdate.abbr
   column.4.querysort=plannedStartDate
   column.4.shortview=false
   column.4.stretch=0
   column.4.styledef.case.0.comparison.attribute=css
   column.4.styledef.case.0.comparison.isrowcase=false
   column.4.styledef.case.0.comparison.leftmethod=atDateAsAtDate(plannedStartDate)
   column.4.styledef.case.0.comparison.lefttext=plannedStartDate
   column.4.styledef.case.0.comparison.operator=notnull
   column.4.styledef.case.0.comparison.operatortype=date
   column.4.styledef.case.0.comparison.righttext=
   column.4.styledef.case.0.comparison.trueproperty.0.name=bgcolor
   column.4.styledef.case.0.comparison.trueproperty.0.value=E1E1E1
   column.4.styledef.case.0.comparison.truetext=
   column.4.styledef.case.0.comparison.usefield=false
   column.4.valueexpression=ROUND(DATEDIFF({projectedStartDate},{plannedStartDate}))
   column.4.valueformat=HTML
   column.4.width=75
   column.5.descriptionkey=plannedstartdate
   column.5.linkedname=direct
   column.5.listsort=atDateAsAtDate(plannedStartDate)
   column.5.namekey=plannedstartdate.abbr
   column.5.querysort=plannedStartDate
   column.5.shortview=false
   column.5.stretch=0
   column.5.valuefield=plannedStartDate
   column.5.valueformat=atDate
   column.5.width=75
   column.6.descriptionkey=actualstartdate
   column.6.linkedname=direct
   column.6.listsort=atDateAsAtDate(actualStartDate)
   column.6.namekey=actualstartdate.abbr
   column.6.querysort=actualStartDate
   column.6.shortview=false
   column.6.stretch=0
   column.6.valuefield=actualStartDate
   column.6.valueformat=atDate
   column.6.width=75
   column.7.descriptionkey=plannedstartdate
   column.7.displayname=Actual Start Variance
   column.7.linkedname=direct
   column.7.listsort=atDateAsAtDate(plannedStartDate)
   column.7.namekey=plannedstartdate.abbr
   column.7.querysort=plannedStartDate
   column.7.shortview=false
   column.7.stretch=0
   column.7.styledef.case.0.comparison.attribute=css
   column.7.styledef.case.0.comparison.isrowcase=false
   column.7.styledef.case.0.comparison.leftmethod=atDateAsAtDate(plannedStartDate)
   column.7.styledef.case.0.comparison.lefttext=plannedStartDate
   column.7.styledef.case.0.comparison.operator=notnull
   column.7.styledef.case.0.comparison.operatortype=date
   column.7.styledef.case.0.comparison.righttext=
   column.7.styledef.case.0.comparison.trueproperty.0.name=bgcolor
   column.7.styledef.case.0.comparison.trueproperty.0.value=E1E1E1
   column.7.styledef.case.0.comparison.truetext=
   column.7.styledef.case.0.comparison.usefield=false
   column.7.valueexpression=ROUND(DATEDIFF({actualStartDate},{plannedStartDate}))
   column.7.valueformat=HTML
   column.7.width=75
   column.8.descriptionkey=plannedcompletiondate
   column.8.linkedname=direct
   column.8.listsort=atDateAsAtDate(plannedCompletionDate)
   column.8.namekey=plannedcompletiondate.abbr
   column.8.querysort=plannedCompletionDate
   column.8.shortview=false
   column.8.stretch=0
   column.8.valuefield=plannedCompletionDate
   column.8.valueformat=atDate
   column.8.width=75
   column.9.descriptionkey=projectedcompletiondate
   column.9.linkedname=direct
   column.9.listsort=atDateAsAtDate(projectedCompletionDate)
   column.9.namekey=projectedcompletiondate.abbr
   column.9.querysort=projectedCompletionDate
   column.9.shortview=false
   column.9.stretch=0
   column.9.valuefield=projectedCompletionDate
   column.9.valueformat=atDate
   column.9.width=75
   column.10.descriptionkey=plannedcompletiondate
   column.10.displayname=Projected Completion Variance
   column.10.linkedname=direct
   column.10.listsort=atDateAsAtDate(plannedCompletionDate)
   column.10.namekey=plannedcompletiondate.abbr
   column.10.querysort=plannedCompletionDate
   column.10.shortview=false
   column.10.stretch=0
   column.10.styledef.case.0.comparison.attribute=css
   column.10.styledef.case.0.comparison.isrowcase=false
   column.10.styledef.case.0.comparison.leftmethod=atDateAsAtDate(plannedCompletionDate)
   column.10.styledef.case.0.comparison.lefttext=plannedCompletionDate
   column.10.styledef.case.0.comparison.operator=notnull
   column.10.styledef.case.0.comparison.operatortype=date
   column.10.styledef.case.0.comparison.righttext=
   column.10.styledef.case.0.comparison.trueproperty.0.name=bgcolor
   column.10.styledef.case.0.comparison.trueproperty.0.value=E1E1E1
   column.10.styledef.case.0.comparison.truetext=
   column.10.styledef.case.0.comparison.usefield=false
   column.10.valueexpression=ROUND(DATEDIFF({projectedCompletionDate},{plannedCompletionDate}))
   column.10.valueformat=HTML
   column.10.width=75
   column.11.descriptionkey=plannedcompletiondate
   column.11.linkedname=direct
   column.11.listsort=atDateAsAtDate(plannedCompletionDate)
   column.11.namekey=plannedcompletiondate.abbr
   column.11.querysort=plannedCompletionDate
   column.11.shortview=false
   column.11.stretch=0
   column.11.valuefield=plannedCompletionDate
   column.11.valueformat=atDate
   column.11.width=75
   column.12.descriptionkey=actualcompletiondate
   column.12.linkedname=direct
   column.12.listsort=atDateAsAtDate(actualCompletionDate)
   column.12.namekey=actualcompletiondate.abbr
   column.12.querysort=actualCompletionDate
   column.12.shortview=false
   column.12.stretch=0
   column.12.valuefield=actualCompletionDate
   column.12.valueformat=atDate
   column.12.width=75
   column.13.descriptionkey=plannedcompletiondate
   column.13.displayname=Actual Completion Variance
   column.13.linkedname=direct
   column.13.listsort=atDateAsAtDate(plannedCompletionDate)
   column.13.namekey=plannedcompletiondate.abbr
   column.13.querysort=plannedCompletionDate
   column.13.shortview=false
   column.13.stretch=0
   column.13.styledef.case.0.comparison.attribute=css
   column.13.styledef.case.0.comparison.isrowcase=false
   column.13.styledef.case.0.comparison.leftmethod=atDateAsAtDate(plannedCompletionDate)
   column.13.styledef.case.0.comparison.lefttext=plannedCompletionDate
   column.13.styledef.case.0.comparison.operator=notnull
   column.13.styledef.case.0.comparison.operatortype=date
   column.13.styledef.case.0.comparison.righttext=
   column.13.styledef.case.0.comparison.trueproperty.0.name=bgcolor
   column.13.styledef.case.0.comparison.trueproperty.0.value=E1E1E1
   column.13.styledef.case.0.comparison.truetext=
   column.13.styledef.case.0.comparison.usefield=false
   column.13.valueexpression=ROUND(DATEDIFF({actualCompletionDate},{plannedCompletionDate}))
   column.13.valueformat=HTML
   column.13.width=75
   row.0.styledef.applyallcases=true
   row.0.styledef.case.0.comparison.attribute=css
   row.0.styledef.case.0.comparison.isrowcase=true
   row.0.styledef.case.0.comparison.leftmethod=intAsInt(numberOfChildren)
   row.0.styledef.case.0.comparison.lefttext=numberOfChildren
   row.0.styledef.case.0.comparison.operator=gt
   row.0.styledef.case.0.comparison.operatortype=int
   row.0.styledef.case.0.comparison.righttext=0
   row.0.styledef.case.0.comparison.trueproperty.0.name=fontstyle
   row.0.styledef.case.0.comparison.trueproperty.0.value=bold
   row.0.styledef.case.0.comparison.truetext=
   row.0.styledef.case.0.comparison.usefield=false
   ```

1. Clique em **Concluído** > **Salvar exibição**.
