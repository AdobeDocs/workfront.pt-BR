---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Agrupamento: tarefas por portfólio, programa e projeto'''
description: Use esse agrupamento de tarefas para agrupar tarefas pelo portfólio, por programa e, em seguida, pelo projeto ao qual elas estão associadas.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8fdad6a1-54b3-4d3e-8f21-4f2efc2dc27a
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# Agrupamento: tarefas por portfólio, programa e projeto

Use esse agrupamento de tarefas para agrupar tarefas pelo portfólio, por programa e, em seguida, pelo projeto ao qual elas estão associadas.

![](assets/portfolio-program-project-grouping-for-tasks-350x120.png)

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

## Agrupar tarefas por portfólio, programa e projeto

Para aplicar este agrupamento:

1. Vá para uma lista de tarefas.
1. No **Agrupamento** , selecione **Novo agrupamento**.

1. Clique em **Alternar para o modo de texto**.
1. Remova o texto na **Agrupar seu relatório** área.
1. Substitua o texto pelo seguinte código:

   <pre>group.0.linkedname=project<br>group.0.namekey=portfólio<br>group.0.notime=false<br>group.0.valuefield=project:portfolio:name<br>group.0.valueformat=string<br>group.1.linkedname=project<br>group.1.namekey=program<br>group.1.notime=false<br>group.1.valuefield=project:program:name<br>group.1.valueformat=string<br>group.2.name=Project<br>group.2.valuefield=project:name<br>group.2.valueformat=HTML<br>textmode=true<br></pre>

1. Clique em **Salvar Agrupamento**.
