---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: Exibir Relatórios Agendados para Entrega'
description: Este filtro de relatório exibe todos os relatórios agendados para entrega automática no Adobe Workfront. É melhor usá-la com a exibição padrão.
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: 7b937384-80c9-4bc7-94be-5573cf86b35b
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 27%

---

# Filtro: exibir relatórios programados para entrega

<!--Audited: 10/2024-->

Este filtro de relatório exibe todos os relatórios agendados para entrega automática no Adobe Workfront. É melhor usá-la com a exibição padrão.

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
   <p>Colaborador ou solicitação para modificar um filtro </p>
   <p>Padrão ou Plano para modificar um relatório</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso de edição a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a filtros, exibições e agrupamentos para modificar um filtro</p> </td> 
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

Para aplicar este filtro:

1. Ir para uma lista de relatórios.

1. No menu suspenso **Filtro**, selecione **Novo Filtro**.

1. Clique em **Alternar para o Modo de Texto**.

1. Na área **Definir Regras de Filtro para o Relatório**, copie e cole o seguinte código:

   ```
    scheduledReportsOM:ID_Mod=notblank
   ```

1. Clique em **Salvar filtro**.
