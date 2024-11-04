---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Exibição: adicionar uma lista de tarefas sucessoras em uma coluna"
description: É possível adicionar uma coluna a uma visualização de tarefa para mostrar uma lista de sucessores das tarefas. A coluna Sucessores da Tarefa inclui o número do sucessor e o nome.
author: Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: ecce7484423419823effa2cb41da892ba3fb207c
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 1%

---

# Exibição: adicionar uma lista de tarefas sucessoras em uma coluna

<!--Audited: 11/2024-->

É possível adicionar uma coluna a uma visualização de tarefa para mostrar uma lista de sucessores das tarefas. A coluna **Sucessoras da Tarefa** inclui o número da sucessora e o nome.

![exibição_tarefa_com_uma_lista_de_sucessores_.png](assets/task-view-with-a-list-of-successors--350x118.png)

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


## Adicionar uma lista de tarefas sucessoras em uma coluna

Para adicionar esta coluna a uma visualização de tarefa:

1. Ir para uma lista de tarefas.
1. Expanda o menu suspenso **Exibir** e clique em **Nova Exibição**.
1. Clique em **Adicionar coluna**.
1. Clique em **Alternar para Modo de Texto** e em **Editar Modo de Texto**.
1. Remova todo o texto da caixa **Editar Modo de Texto** e substitua-o pelo seguinte código:

   ```
   displayname=Task Successors
   listdelimiter=
   listmethod=nested(successors).lists
   textmode=true
   type=iterate
   valueexpression=CONCAT({successor}.{taskNumber},' - ',{successor}.{name})
   valueformat=HTML
   ```

1. Clique em **Concluído** e depois em **Salvar exibição**.
