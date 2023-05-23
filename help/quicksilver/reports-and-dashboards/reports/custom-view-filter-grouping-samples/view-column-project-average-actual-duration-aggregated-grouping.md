---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualização e agrupamento: exibir a duração real do projeto agregada pela média em um agrupamento"
description: Você pode adicionar a seguinte coluna em um relatório de projeto para mostrar a Duração real agregada como uma média em um agrupamento.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---

# Visualização e agrupamento: exibe a Duração real do projeto agregada pela média em um agrupamento

Você pode adicionar a seguinte coluna em um relatório de projeto para mostrar a Duração real agregada como uma média em um agrupamento.

![project_with_aggregate_atual_duration_in_grouping_view.png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

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

## Exibir a Duração Efetiva do projeto agregada pela média em um Agrupamento

Para adicionar esta coluna a uma exibição de projeto:

1. (Recomendado) Para obter melhores resultados e visualizar o valor médio agregado da duração real, é necessário adicionar um agrupamento à lista ou ao relatório do projeto.\
   Para obter mais informações sobre como criar agrupamentos, consulte o artigo [Visão geral de agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Ir para uma visualização de projeto existente.
1. Expanda o menu suspenso Exibir e selecione **Personalizar visualização**.
1. Clique em **Adicionar coluna**.
1. Clique em **Alternar para modo de texto**.
1. Passe o mouse sobre a **Mostrar nesta coluna** e clique em **Clique para editar o texto**.

1. Remova todo o texto na caixa Modo de texto e substitua-o pelo seguinte código:

   <pre>agregador.displayformat=composto <br>aggregator.function=AVG <br>aggregator.namekey=view.relatedcolumn <br>aggregator.namekeyargkey=atualduration <br>aggregator.valuefield=atualDurationMinutes <br>aggregator.valueformat=val <br>displayname=Duração Efetiva do Projeto <br>durationunitfield=durationUnit.value <br>linkedname=project <br>namekey=atualduration <br>namekeyargkey=atualduration <br>querysort=atualDurationMinutes <br>textmode=true <br>valuefield=atualDurationMinutes <br>valueformat=composto#M:D <br>viewalias=atualduration</pre>

1. Clique em **Salvar visualização**.
