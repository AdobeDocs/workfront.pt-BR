---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualização e agrupamento: exibir a duração real do projeto agregada pela média em um agrupamento"
description: Você pode adicionar a seguinte coluna em um relatório de projeto para mostrar a Duração real agregada como uma média em um agrupamento.
author: Nolan
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: ecce7484423419823effa2cb41da892ba3fb207c
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 1%

---

# Visualização e agrupamento: exibe a Duração real do projeto agregada pela média em um agrupamento

<!--Audited: 11/2024-->

Você pode adicionar a seguinte coluna em uma visualização do projeto para mostrar a Duração real agregada como uma média em um agrupamento.

![project_with_aggregate_atual_duration_in_grouping_view.png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

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
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> 
    <p>Novo:</p>
   <ul><li><p>Colaborador para modificar um filtro </p></li>
   <li><p>Padrão para modificar um relatório</p></li> </ul>

<p>Atual:</p>
   <ul><li><p>Solicitação para modificar um filtro </p></li>
   <li><p>Planejar a modificação de um relatório</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar um filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exibir a Duração Efetiva do projeto agregada pela média em um agrupamento

Para adicionar esta coluna a uma exibição de projeto:

1. Ir para uma lista de projetos.
1. (Obrigatório) Para ver o valor médio agregado da duração real do projeto, você deve ter um agrupamento adicionado à lista do projeto.\
   Para obter mais informações sobre como criar agrupamentos, consulte o artigo [Visão geral sobre agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
1. Expanda o menu suspenso **Exibir** e selecione **Personalizar exibição**.
1. Clique em **Adicionar coluna**.
1. Clique em **Alternar para Modo de Texto** e em **Editar Modo de Texto**.
1. Remova todo o texto da caixa **Editar Modo de Texto** e substitua-o pelo seguinte código:

   ```
   aggregator.displayformat=compound 
   aggregator.function=AVG 
   aggregator.namekey=view.relatedcolumn 
   aggregator.namekeyargkey=actualduration 
   aggregator.valuefield=actualDurationMinutes 
   aggregator.valueformat=val 
   displayname=Project Actual Duration 
   durationunitfield=durationUnit.value 
   linkedname=project 
   namekey=actualduration 
   namekeyargkey=actualduration 
   querysort=actualDurationMinutes 
   textmode=true 
   valuefield=actualDurationMinutes 
   valueformat=compound#M:D 
   viewalias=actualduration
   ```

1. Clique em **Concluído** e depois em **Salvar exibição**.
1. (Opcional) Atualize o nome da exibição e clique em **Salvar exibição**.
