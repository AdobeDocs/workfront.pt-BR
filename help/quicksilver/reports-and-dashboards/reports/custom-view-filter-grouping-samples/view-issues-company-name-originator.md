---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Exibir: problemas com o nome da empresa do originador"
description: Essa exibição de problema exibe o nome da empresa associado ao usuário que enviou o problema.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e628f7cf-4a7b-4125-bea6-348c72477bd7
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Exibir: problemas com o nome da empresa do originador

Essa exibição de problema exibe o nome da empresa associado ao usuário que enviou o problema.

![custom_view_for_issues_with_originator_company_name.png](assets/custom-view-for-issues-350x33.png)

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

## Exibir problemas com o nome da empresa do originador

Para aplicar esta exibição:

1. Acesse uma lista de problemas.
1. No **Exibir** , selecione **Nova exibição**.

1. No **Visualização de coluna** , elimine todas as colunas, exceto uma.
1. Clique no cabeçalho da coluna restante e, em seguida, clique em **Alternar para o modo de texto**.
1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar texto**.
1. Remova o texto que você encontrar no **Modo de texto** e substitua-a pelo seguinte código:
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=val<br>column.0.link.lookup=link.view<br>column.0.link.value=val(objCode)<br>column.0.listsort=string(name)<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=140<br>column.1.descriptionkey=originator<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=ownerID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup=link.view<br>column.1.link.valuefield=owner:objCode<br>column.1.link.value=val<br>column.1.listsort=nested(owner).string(name)<br>column.1.namekey=originator.abbr<br>column.1.querysort=owner:name<br>column.1.valuefield=owner:name<br>column.1.valueformat=HTML<br>column.1.width=151<br>column.2.descriptionkey=entrydate<br>column.2.listsort=atDateAsAtDate(entryDate)<br>column.2.namekey=entrydate.abbr<br>column.2.querysort=entryDate<br>column.2.valuefield=entryDate<br>column.2.valueformat=atDate<br>column.2.width=75<br>column.3.descriptionkey=age<br>column.3.listsort=doubleAsDouble(age)<br>column.3.namekey=age<br>column.3.querysort=age<br>column.3.valuefield=howOld<br>column.3.valueformat=val<br>column.3.width=80<br>column.4.viewalias=statusicons<br>column.4.displayname=Flags<br>column.4.linkedname=direct<br>column.4.namekey=statusicons<br>column.4.valuefield=<br>column.4.valueformat=HTML<br>column.4.querysort=<br>column.4.tile.name=component.issuestatusicons<br>column.4.tile.pdfcomponent=issueStatusIcons<br>column.4.delimiter=<br>column.4.tile.template=/WEB-INF/jsp/lists/components/issueStatusIcons.jsp<br>column.5.description=Nome da empresa do originador<br>column.5.link.linkproperty.0.name=ID<br>column.5.link.linkproperty.0.valuefield=owner:companyID<br>column.5.link.linkproperty.0.valueformat=int<br>column.5.link.lookup=link.view<br>column.5.link.value.field=owner:company:objCode<br>column.5.link.value.format=val<br>column.5.listsort=nested(owner:company).string(name)<br>column.5.name=Originator Company<br>column.5.querysort=owner:company:name<br>column.5.valuefield=owner:company:name<br>column.5.valueformat=HTML<br>column.5.width=151</pre>

1. Clique em **Salvar exibição**.
