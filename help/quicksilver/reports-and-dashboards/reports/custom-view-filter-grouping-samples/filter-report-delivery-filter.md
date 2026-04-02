---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: exibir relatórios agendados para entrega'
description: Este filtro de relatório exibe todos os relatórios agendados para serem entregues automaticamente no Adobe Workfront. É melhor usado com a exibição padrão.
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: 7b937384-80c9-4bc7-94be-5573cf86b35b
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 27%

---

# Filtro: exibir relatórios programados para entrega

<!--Audited: 10/2024-->

Este filtro de relatório exibe todos os relatórios agendados para serem entregues automaticamente no Adobe Workfront. É melhor usado com a exibição padrão.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Colaborador ou Solicitação para modificar um filtro </p>
   <p>Padrão ou Plano para modificar um relatório</p>
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

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtro de entrega de relatório

Para aplicar esse filtro:

1. Ir para uma lista de relatórios.

1. No menu suspenso **Filtro**, selecione **Novo Filtro**.

1. Clique em **Alternar para Modo de Texto**.

1. Na área **Definir regras de filtro para seu Relatório**, copie e cole o seguinte código:

   ```
    scheduledReportsOM:ID_Mod=notblank
   ```

1. Clique em **Salvar filtro**.
