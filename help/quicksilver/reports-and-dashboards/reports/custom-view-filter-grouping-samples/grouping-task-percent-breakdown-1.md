---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Agrupamento: Detalhamento Percentual da Tarefa 1'
description: 'Neste agrupamento de projeto personalizado, você pode exibir projetos agrupados por um intervalo de seus valores de porcentagem concluída. Os detalhamentos mostram o valor percentual concluído de incrementos de 25%: 0-25%, 25-50%, etc.'
author: Nolan
feature: Reports and Dashboards
exl-id: ddb9496c-9347-4dc9-a4ce-b9017abd0bb2
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 0%

---

# Agrupamento: detalhamento de percentual de tarefa 1

<!--Audited: 10/2024-->

Neste agrupamento de projeto personalizado, você pode exibir projetos agrupados por um intervalo de seus valores de porcentagem concluída. Os detalhamentos mostram o valor percentual concluído de incrementos de 25%: 0-25%, 25-50%, etc.

O agrupamento a seguir organiza tarefas pelo valor de percentual concluído em 6 agrupamentos diferentes:

* 0%
* 1-25%
* 26-50%
* 51-75%
* 76-99%
* 100%

![tarefa_25_detalhamento_agrupamento.png](assets/task-25--breakdown-grouping-350x412.png)

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

## Agrupar por detalhamento de percentual de tarefa

Para aplicar esse agrupamento:

1. Ir para uma lista de tarefas.
1. No menu suspenso **Agrupamento**, selecione **Novo agrupamento**.
1. Clique em **Adicionar agrupamento**.

1. Clique em **Alternar para Modo de Texto**.
1. Remover o texto da área **Agrupar por**.
1. Substitua o texto pelo seguinte código:

   ```
   group.0.linkedname=direct
   group.0.name=Percent Breakdown
   group.0.notime=false
   group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}<=26,"0-25 %",IF({percentComplete}<=51,"26-50 %",IF({percentComplete}<=76,"51-75 %",IF({percentComplete}<100,"76-99 %","100 %")))))
   group.0.valueformat=string
   ```

1. Clique em **Concluído** > **Salvar agrupamento**.
1. (Opcional) Atualize o nome do agrupamento e clique em **Salvar agrupamento**.
