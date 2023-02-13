---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Exibir e agrupar: exibir projeto Duração real agregada pela média em um Agrupamento'''
description: É possível adicionar a seguinte coluna em um relatório de projeto para mostrar a Duração real agregada como uma média em um agrupamento.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Exibir e agrupar: exibir o projeto Duração real agregada pela média em um Agrupamento

É possível adicionar a seguinte coluna em um relatório de projeto para mostrar a Duração real agregada como uma média em um agrupamento.

![project_with_aggregate_atual_duration_in_grouping_view.png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

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

## Exibir a Duração real do projeto agregada pela média em um Agrupamento

Para adicionar esta coluna a uma exibição de projeto:

1. (Recomendado) Para obter melhores resultados e ver o valor médio agregado da Duração real, é necessário adicionar um Agrupamento à lista ou ao relatório do projeto.\
   Para obter mais informações sobre como criar Agrupamentos, consulte o artigo [Visão geral dos agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Vá para uma visualização de projeto existente.
1. Expanda o menu suspenso Exibir e selecione **Personalizar exibição**.
1. Clique em **Adicionar coluna**.
1. Clique em **Alternar para o modo de texto**.
1. Passe o mouse sobre o **Mostrar nesta coluna** e clique em **Clique para editar texto**.

1. Remova todo o texto da caixa Modo de texto e substitua-o pelo seguinte código:

   <pre>agregator.displayformat=composto <br>aggregate.function=AVG <br>aggregate.namekey=view.related column <br>aggregate.namekeyargkey=atualduration <br>aggregate.valuefield=actualDurationMinutes <br>aggregate.valueformat=val <br>displayname=Duração real do projeto <br>durationunitfield=durationUnit.value <br>linkedname=project <br>namekey=atualduration <br>namekeyargkey=atualduration <br>querysort=atualDurationMinutes <br>textmode=true <br>valuefield=realDurationMinutes <br>valueformat=composta#M:D <br>viewalias=atualduration</pre>

1. Clique em **Salvar exibição**.
