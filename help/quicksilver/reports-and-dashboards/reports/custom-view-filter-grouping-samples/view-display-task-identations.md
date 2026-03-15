---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Exibir: Exibir Recuos de Tarefas em uma Lista de Tarefas'
description: Nesta exibição de tarefa, você pode adicionar código à coluna Nome da Tarefa para exibir as tarefas recuadas de acordo com a Estrutura Analítica de Projeto do projeto.
author: Courtney
feature: Reports and Dashboards
exl-id: f7f43e1e-db32-48b8-9a23-ff9fa6195386
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 19%

---

# Exibição: exibir recuos de tarefas em uma lista de tarefas

<!--Audited: 11/2024-->

Nesta exibição de tarefa, você pode adicionar código à coluna Nome da Tarefa para exibir as tarefas recuadas de acordo com a Estrutura Analítica de Projeto do projeto.

![Exibir recuo da tarefa](assets/view-text-mode-indentation-task-list-350x171.png)

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

## Exibir recuos de tarefas em uma coluna de uma lista de tarefas

1. Ir para uma lista de tarefas.
1. No menu suspenso **Exibição**, clique em **Nova Exibição**.

1. Clique em **Adicionar coluna** e comece a digitar “Nome da tarefa” no campo **Mostrar nesta coluna** e selecione-o quando for exibido na lista.

1. Na nova coluna, clique em **Alternar para o Modo de Texto** > **Editar Modo de Texto**.
1. Remova o texto encontrado na linha `valuefield=` e substitua-o pelo seguinte código:

   ```
   displayname=Task hierarchy
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(' - ',{name}),IF({indent}<3,CONCAT(' - - ',{name}),IF({indent}<4,CONCAT(' - - - ',{name}),CONCAT(' - - - - ',{name})))))
   ```

1. Clique em **Concluído** e depois em **Salvar exibição**.
1. (Opcional) Atualize o nome da exibição e clique em **Salvar Exibição**.
