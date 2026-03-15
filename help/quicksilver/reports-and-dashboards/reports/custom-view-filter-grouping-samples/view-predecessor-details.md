---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Exibir: Detalhes do Antecessor'
description: Esta exibição de tarefa mostra detalhes dos predecessores das tarefas que usam uma exibição de coleção. Em uma exibição de coleção, é possível exibir informações sobre objetos que estão em uma relação “um para muitos”. Nesse caso, cada tarefa (uma) pode ter vários predecessores (muitos). A view exibe o nome das tarefas, bem como os Nomes dos Antecessores, os Nomes dos Projetos dos Antecessores, as Datas de Conclusão Planejadas dos Antecessores e os Status dos Antecessores.
author: Courtney
feature: Reports and Dashboards
exl-id: 0187da94-4895-47b1-914f-284fed9e0fd0
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 14%

---

# Exibição: detalhes do predecessor

<!--Audited: 11/2024-->

Esta exibição de tarefa mostra detalhes dos predecessores das tarefas que usam uma exibição de coleção. Em uma exibição de coleção, é possível exibir informações sobre objetos que estão em uma relação “um para muitos”. Nesse caso, cada tarefa (uma) pode ter vários predecessores (muitos). A view exibe o nome das tarefas, bem como os Nomes dos Antecessores, os Nomes dos Projetos dos Antecessores, as Datas de Conclusão Planejadas dos Antecessores e os Status dos Antecessores.

Para obter informações sobre como fazer referência a coleções em relatórios, consulte [Fazer referência a coleções em um relatório](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

![predecessores_details_task_view.png](assets/predecessor-details-task-view-350x34.png)

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

## Exibir detalhes do antecessor

1. Ir para uma lista de tarefas.
1. No menu suspenso **Exibição**, selecione **Nova Exibição**.

1. Na área **Visualização da coluna**, elimine todas as colunas, exceto uma.
1. Clique no cabeçalho da coluna restante e clique em **Alternar para o Modo de Texto** > **Editar Modo de Texto**.
1. Remova o texto encontrado na caixa **Editar Modo de Texto** e substitua-o pelo seguinte código:

   ```
   column.0.displayname=
   column.0.linkedname=direct
   column.0.namekey=name
   column.0.querysort=name
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.1.displayname=Predecessors Numbers & Names
   column.1.listdelimiter=
   column.1.listmethod=nested(predecessors).lists
   column.1.textmode=true
   column.1.type=iterate
   column.1.valueexpression=CONCAT({predecessor}.{taskNumber},' - ',{predecessor}.{name})
   column.1.valueformat=HTML
   column.2.displayname=Predecessors Project Names
   column.2.listdelimiter=
   column.2.listmethod=nested(predecessors).lists
   column.2.textmode=true
   column.2.type=iterate
   column.2.valueexpression={predecessor}.{project}.{name}
   column.2.valueformat=HTML
   column.3.displayname=Predecessors Completion Dates
   column.3.listdelimiter=
   column.3.listmethod=nested(predecessors).lists
   column.3.textmode=true
   column.3.type=iterate
   column.3.valueexpression={predecessor}.{plannedCompletionDate}
   column.3.valueformat=HTML
   column.4.displayname=Predecessors Status
   column.4.listdelimiter=
   column.4.listmethod=nested(predecessors).lists
   column.4.textmode=true
   column.4.type=iterate
   column.4.valueexpression={predecessor}.{status}
   column.4.valueformat=HTML
   ```

1. Clique em **Concluído** > **Salvar Exibição**.
