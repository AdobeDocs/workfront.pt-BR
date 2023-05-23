---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Exibição: problemas com informações de aprovação"
description: A visualização do problema a seguir mostra o processo de aprovação, a etapa, os nomes dos aprovadores e o status do problema antes da concessão da aprovação. Alguns desses campos não podem ser acessados por meio do construtor de interface padrão.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4e123844-a0d6-474b-87fb-d30ed391ad07
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 0%

---

# Exibir: problemas com informações de aprovação

A visualização do problema a seguir mostra o processo de aprovação, a etapa, os nomes dos aprovadores e o status do problema antes da concessão da aprovação. Alguns desses campos não podem ser acessados por meio do construtor de interface padrão.

![custom_issue_view_with_approval_info.png](assets/custom-issue-view-with-approval-info-350x46.png)

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

## Exibir problemas com informações de aprovação

1. Vá para uma lista de problemas.
1. No **Exibir** selecione **Nova visualização**.

1. No **Visualização da coluna** elimine todas as colunas, exceto uma.
1. Clique no cabeçalho da coluna restante e clique em **Alternar para modo de texto**.
1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar o texto**.
1. Remova o texto localizado na **Modo de texto** e substitua-o pelo seguinte código:
   <pre style="font-style: normal;">column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=40<br>column.0.valuefield=nome<br>column.0.valueformat=HTML<br>column.0.width=220<br>column.1.descriptionkey=assignedto<br>column.1.linkedname=assignedTo<br>column.1.listsort=nested(assignedTo).string(name)<br>column.1.namekey=assigned<br>column.1.querysort=assignedTo:name<br>column.1.shortview=true<br>column.1.stretch=0<br>column.1.valuefield=assignedTo:name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.descriptionkey=função<br>column.2.linkedname=função<br>column.2.listsort=nested(role).string(name)<br>column.2.namekey=função<br>column.2.querysort=role:name<br>column.2.shortview=false<br>column.2.stretch=25<br>column.2.valuefield=função:nome<br>column.2.valueformat=HTML<br>column.2.width=150<br>column.3.description=Nome do processo de aprovação<br>column.3.linkedname=direct<br>column.3.listsort=string(name)<br>column.3.name=Nome do processo de aprovação<br>column.3.querysort=name<br>column.3.shortview=false<br>column.3.stretch=35<br>column.3.valuefield=approvalProcess:name<br>column.3.valueformat=HTML<br>column.3.width=220<br>column.4.description=Nome da etapa de aprovação<br>column.4.linkedname=direct<br>column.4.listsort=string(name)<br>column.4.name=Nome da etapa de aprovação<br>column.4.querysort=name<br>column.4.shortview=false<br>column.4.stretch=0<br>column.4.valuefield=currentApprovalStep:name<br>column.4.valueformat=HTML<br>column.4.width=220<br>column.5.description=Status anterior<br>column.5.linkedname=direct<br>column.5.listsort=string(name)<br>column.5.name=Status anterior<br>column.5.querysort=name<br>column.5.shortview=false<br>column.5.stretch=0<br>column.5.valuefield=previousStatus<br>column.5.valueformat=HTML<br>column.5.width=220<br>column.6.linkedname=direct<br>column.6.listsort=HTML(approversString)<br>column.6.namekey=approver.plural.abbr<br>column.6.querysort=approversString<br>column.6.shortview=false<br>column.6.stretch=0<br>column.6.valuefield=approversString<br>column.6.valueformat=HTML<br>column.6.viewalias=approver.plural<br>column.6.width=200<br></pre>

1. Clique em **Salvar visualização**.
