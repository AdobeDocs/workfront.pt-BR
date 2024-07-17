---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualização: empresa e grupo padrão do usuário atribuído"
description: Esta exibição de tarefa mostra a Empresa e o Grupo inicial do Proprietário principal da tarefa. Esses são valores que não estão disponíveis na interface padrão, mas são acessíveis por meio do modo de texto.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 818c1f3a-4e82-4dc3-af86-4f9dcf5c11a4
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# Visualização: Empresa e grupo padrão do usuário atribuído

Esta exibição de tarefa mostra a Empresa e o Grupo inicial do Proprietário principal da tarefa. Esses são valores que não estão disponíveis na interface padrão, mas são acessíveis por meio do modo de texto.

![](assets/view--assigned-user-s-company-and-home-group-350x80.png)

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

## Visualizar Empresa e Grupo Inicial do usuário atribuído

1. Ir para uma lista de tarefas.
1. No menu suspenso **Exibir**, selecione **Nova Exibição**.

1. Na área **Visualização da coluna**, elimine todas as colunas, exceto uma.
1. Clique no cabeçalho da coluna restante e em **Alternar para Modo de Texto**.
1. Passe o mouse sobre a área de modo de texto e clique em **Clicar para editar o texto**.
1. Remova o texto localizado na caixa **Modo de Texto** e substitua-o pelo seguinte código:
   <pre>column.0.descriptionkey=name<br> column.0.link.linkproperty.0.name=ID<br> column.0.link.linkproperty.0.valuefield=ID<br> column.0.link.linkproperty.0.valueformat=int<br> column.0.link.lookup=link.view<br> column.0.link.valuefield=objCode<br> column.0.link.valueformat=val<br> column.0.linkedname=direct<br> column.0.listsort=string(nome)<br> column.0.namekey=name.abbr<br> column.0.querysort=name<br> column.0.shortview=false<br> column.0.stretch=100<br> column.0.valuefield=name<br> column.0.valueformat=HTML<br> column.0.width=150<br> column.1.descriptionkey=assignedto<br> column.1.link.linkproperty.0.name=ID 17} coluna.1.link.linkproperty.0.valuefield=assignedTo:ID<br> coluna.1.link.linkproperty.0.valueformat=int<br> coluna.1.link.lookup=link.view<br> coluna.1.link.valuefield=assignedTo:objCode<br> coluna.1.link.valueformat=val<br> coluna.1.linkedname=assignedTo<br> coluna.1.listsort=nested(assignedTo) .string(name)<br> column.1.namekey=assignedto<br> column.1.querysort=assignedTo:name<br> column.1.shortview=false<br> column.1.stretch=0<br> column.1.valuefield=assignedTo:name<br> column.1.valueformat=HTML<br> column.1.width=150<br> column.2.description=Assigned To Company<br> column.2.string=Atribuído à Empresa<br> coluna.2.linkedname=assignedTo:company<br> coluna.2.listsort=nested(assignedTo:company).string(name)<br> coluna.2.namekey=assignedto<br> coluna.2.querysort=assignedTo:company:nome<br> coluna.2.shortview=false<br> coluna.2.stretch=0<br> coluna.2.valuefield=assignedTo:company:nome<br>} column.2.valueformat=HTML<br> column.2.width=150<br> column.3.description=Atribuído ao Grupo Inicial<br> column.3.displayname=Atribuído ao Grupo Inicial<br> column.3.linkedname=assignedTo:homeGroup<br> column.3.listsort=nested(assignedTo:homeGroup).string(name)<br> column.3.namekey=assignedto<br> column.3.querysort=Para:homeGroup:nome<br> coluna.3.shortview=falso<br> coluna.3.stretch=0<br> coluna.3.valuefield=assignedTo:homeGroup:nome<br> coluna.3.valueformat=HTML<br> coluna.3.width=150<br></pre>

1. Clique em **Salvar alterações**.
