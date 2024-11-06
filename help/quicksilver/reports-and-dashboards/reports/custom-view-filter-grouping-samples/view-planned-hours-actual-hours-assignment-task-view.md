---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "View: Horas planejadas vs. Horas efetivas por atribuição em uma view de tarefa"
description: Esta view de tarefa exibe o total de Horas Planejadas de uma tarefa, o número de Horas Planejadas alocadas para cada designado (quando a tarefa é atribuída a vários usuários), o total de Horas Reais da tarefa e o número de Horas Reais registradas por cada designado.
author: Nolan
feature: Reports and Dashboards
exl-id: f249ff57-50c7-4aa9-a563-cb7f5562b96a
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# Exibição: Horas Planejadas vs. Horas Efetivas por atribuição em uma exibição de tarefa

<!--Audited: 11/2024-->

Esta view de tarefa exibe o total de Horas Planejadas de uma tarefa, o número de Horas Planejadas alocadas para cada designado (quando a tarefa é atribuída a vários usuários), o total de Horas Reais da tarefa e o número de Horas Reais registradas por cada designado.

![multi_assignment_budget_vs_atual_for_tasks.png](assets/multi-assignment-budget-vs-actual-for-tasks-350x66.png)

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

## Exibir Horas Planejadas vs. Horas Efetivas por atribuição em uma tarefa Exibir

1. Ir para uma lista de tarefas.
1. No menu suspenso **Exibir**, selecione **Nova Exibição**.

1. Na área **Visualização da coluna**, elimine todas as colunas, exceto uma.
1. Clique no cabeçalho da coluna restante e clique em **Alternar para Modo de Texto** > **Editar Modo de Texto**.
1. Remova o texto localizado na caixa **Editar Modo de Texto** e substitua-o pelo seguinte código:

   ```
   column.0.descriptionkey=name
   column.0.isInlineEditable=false
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat=int
   column.0.link.lookup=link.view
   column.0.link.valuefield=objCode
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.section=0
   column.0.shortview=false
   column.0.stretch=0
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.descriptionkey=workrequired
   column.1.isInlineEditable=false
   column.1.linkedname=direct
   column.1.listsort=doubleAsDouble(workRequired)
   column.1.namekey=workrequired.abbr
   column.1.querysort=workRequired
   column.1.section=0
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=workFieldLong
   column.1.valueformat=compound
   column.1.viewalias=workrequired
   column.1.width=100
   column.2.listdelimiter=
   column.2.listmethod=nested(assignments).lists
   column.2.name=Wrk Assignment(s)
   column.2.stretch=0
   column.2.type=iterate
   column.2.valueexpression=CONCAT(right(CONCAT('~~~',{assignmentPercent}),3),'% (', {workRequired}/60 ,' Hours) - ',{assignedTo}.{name})
   column.2.valueformat=HTML
   column.2.width=300
   column.3.descriptionkey=actualworkrequired
   column.3.isInlineEditable=false
   column.3.linkedname=direct
   column.3.listsort=intAsInt(actualWorkRequired)
   column.3.namekey=actualworkrequired.abbr
   column.3.querysort=actualWork
   column.3.section=0
   column.3.shortview=false
   column.3.stretch=100
   column.3.valuefield=actualWorkFieldLong
   column.3.valueformat=compound
   column.3.viewalias=actualworkrequired
   column.3.width=100
   column.4.listdelimiter=
   column.4.listmethod=nested(hours).lists
   column.4.name=Actual Hours
   column.4.stretch=0
   column.4.type=iterate
   column.4.valueexpression=CONCAT('(', {hours} ,' Hours) - ',{owner}.{name})
   column.4.valueformat=HTML
   column.4.width=300
   ```

1. Clique em **Concluído** > **Salvar exibição**.
