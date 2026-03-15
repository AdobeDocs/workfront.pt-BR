---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Exibir: Objetos Resolvíveis em um Relatório de Tarefa ou Projeto'
description: Você pode exibir uma lista de todos os Objetos Resolvíveis em um relatório ou exibição de projeto ou de tarefa.
author: Courtney
feature: Reports and Dashboards
exl-id: 2b0d8e7c-9211-44e5-9d92-c87a2fe4336d
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 18%

---

# Exibição: objetos resolvíveis em um relatório de tarefa ou projeto

<!--Audited: 11/2024-->

Você pode exibir uma lista de todos os Objetos Resolvíveis em um relatório ou exibição de projeto ou de tarefa.

Para obter mais informações sobre Objetos Resolvíveis, consulte o artigo [Visão Geral de Resolvendo e Objetos Resolvíveis](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

![list_of_resolvables_in_report.png](assets/list-of-resolvables-in-report-350x54.png)

A aplicação deste modo de exibição é idêntica para tarefas e projetos.

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
   <p>Colaborador ou Solicitação de modificação de uma exibição </p>
   <p>Padrão ou Plano para modificar um relatório</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso de edição a relatórios, painéis e calendários para modificar um relatório</p> <p>Acesso de edição a filtros, visualizações, agrupamentos para modificar uma visualização</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Exibir Objetos Resolvíveis em um relatório de tarefa ou projeto

1. Vá para uma lista de tarefas ou projetos que foram convertidos de problemas.
1. No menu suspenso **Exibição**, clique em **Nova Exibição**.

1. Na área **Visualização da Coluna**, clique em **Adicionar Coluna**.

1. Clique no cabeçalho da nova coluna e clique em **Alternar para o Modo de Texto** > **Editar Modo de Texto**.
1. Remova o texto encontrado na caixa **Editar Modo de Texto** e substitua-o pelo seguinte código:

   ```
   displayname=Resolvables
   listdelimiter=<br>
   listmethod=nested(resolvables).lists
   textmode=true
   type=iterate
   valuefield=name
   valueformat=HTML
   ```

1. Clique em **Concluído** > **Salvar Exibição**.\
   Uma lista de todos os Objetos resolvíveis é exibida na nova coluna. Os nomes dos objetos na lista não podem ser vinculados diretamente aos objetos.
