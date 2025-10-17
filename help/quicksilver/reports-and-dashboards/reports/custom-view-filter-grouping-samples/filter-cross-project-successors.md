---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: exibir sucessores incompletos entre projetos'
description: Este filtro de tarefa retorna sucessores de projetos cruzados incompletos.
author: Lisa and Jenny
feature: Reports and Dashboards
exl-id: aea955b1-581a-4ce0-8634-863ba1083c05
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '151'
ht-degree: 0%

---

# Filtro: exibir sucessores incompletos entre projetos

Este filtro de tarefa retorna sucessores de projetos cruzados incompletos.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

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

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrar sucessores entre projetos

Para aplicar esse filtro:

1. Ir para uma lista de tarefas.
1. No menu suspenso **Filtro**, selecione **Novo filtro**.

1. Clique em **Modo de texto**.
1. Na área exibida, cole o seguinte código:
   <pre>percentComplete=100<br>percentComplete_Mod=ne<br>sucessoresMM:projectID=FIELD:projectID<br>sucessoresMM:projectID_Mod=ne</pre>

1. Clique em **Aplicar** > **Salvar como novo**.
