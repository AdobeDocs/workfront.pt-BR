---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Exibir: problemas com informações de aprovação"
description: A visualização do problema a seguir mostra o processo de aprovação, a etapa, os nomes dos aprovadores e o status do problema antes da concessão da aprovação. Alguns desses campos não podem ser acessados por meio do construtor de interface padrão.
author: Nolan
feature: Reports and Dashboards
exl-id: 4e123844-a0d6-474b-87fb-d30ed391ad07
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# Exibir: problemas com informações de aprovação

<!--Audited: 11/2024-->

A visualização do problema a seguir mostra o processo de aprovação, a etapa, os nomes dos aprovadores e o status do problema antes da concessão da aprovação. Alguns desses campos não podem ser acessados por meio do construtor de interface padrão.

![custom_issue_view_with_approval_info.png](assets/custom-issue-view-with-approval-info-350x46.png)

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
   <td> <p>Novo:<ul><li>Colaborador para modificar uma visualização</li><li>Padrão para modificar um relatório</li></ul></p><p>Ou</p>Atual:<ul><li>Solicitação para modificar uma exibição</li><li>Planejar a modificação de um relatório</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
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

## Exibir problemas com informações de aprovação

1. Vá para uma lista de problemas.
1. No menu suspenso **Exibir**, selecione **Nova Exibição**.

1. Na área **Visualização da coluna**, elimine todas as colunas, exceto uma.
1. Clique no cabeçalho da coluna restante e clique em **Alternar para Modo de Texto** e em **Editar Modo de Texto**.
1. Remova o texto localizado na caixa **Editar Modo de Texto** e substitua-o pelo seguinte código:

   ```
   column.0.descriptionkey=name
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
   column.0.shortview=false
   column.0.stretch=40
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=220
   column.1.descriptionkey=assignedto
   column.1.linkedname=assignedTo
   column.1.listsort=nested(assignedTo).string(name)
   column.1.namekey=assignedto
   column.1.querysort=assignedTo:name
   column.1.shortview=true
   column.1.stretch=0
   column.1.valuefield=assignedTo:name
   column.1.valueformat=HTML
   column.1.width=150
   column.2.descriptionkey=role
   column.2.linkedname=role
   column.2.listsort=nested(role).string(name)
   column.2.namekey=role
   column.2.querysort=role:name
   column.2.shortview=false
   column.2.stretch=25
   column.2.valuefield=role:name
   column.2.valueformat=HTML
   column.2.width=150
   column.3.description=Approval Process Name
   column.3.linkedname=direct
   column.3.listsort=string(name)
   column.3.name=Approval Process Name
   column.3.querysort=name
   column.3.shortview=false
   column.3.stretch=35
   column.3.valuefield=approvalProcess:name
   column.3.valueformat=HTML
   column.3.width=220
   column.4.description=Approval Step Name
   column.4.linkedname=direct
   column.4.listsort=string(name)
   column.4.name=Approval Step Name
   column.4.querysort=name
   column.4.shortview=false
   column.4.stretch=0
   column.4.valuefield=currentApprovalStep:name
   column.4.valueformat=HTML
   column.4.width=220
   column.5.description=Previous Status
   column.5.linkedname=direct
   column.5.listsort=string(name)
   column.5.name=Previous Status
   column.5.querysort=name
   column.5.shortview=false
   column.5.stretch=0
   column.5.valuefield=previousStatus
   column.5.valueformat=HTML
   column.5.width=220
   column.6.linkedname=direct
   column.6.listsort=HTML(approversString)
   column.6.namekey=approver.plural.abbr
   column.6.querysort=approversString
   column.6.shortview=false
   column.6.stretch=0
   column.6.valuefield=approversString
   column.6.valueformat=HTML
   column.6.viewalias=approver.plural
   column.6.width=200
   ```

1. Clique em **Concluído** > **Salvar exibição**.
1. (Opcional) Atualize o nome da exibição e clique em **Salvar exibição**.
