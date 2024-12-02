---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Exibição: Mostrar Nome de Tarefas Pai como Todas em Maiúsculas'
description: É possível adicionar essa coluna a uma visualização de tarefa para exibir o nome das tarefas pai em todas as letras maiúsculas.
author: Nolan
feature: Reports and Dashboards
exl-id: bb489920-6b17-4689-b432-b0c28bcb5d10
source-git-commit: a7cdee912e5047f1c8ef224aff6a41eaa3633df6
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Modo de exibição: mostrar nome de tarefas pai como todas em maiúsculas

<!--Audited: 10/2024-->

É possível adicionar essa coluna a uma visualização de tarefa para exibir o nome das tarefas pai em todas as letras maiúsculas.

![](assets/column-task-with-all-caps-parent-350x112.png)

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

## Mostrar nome das tarefas pai como todas em maiúsculas

Para criar essa coluna em uma exibição de tarefa:

1. Ir para uma lista de tarefas.
1. No menu suspenso **Exibir**, selecione um modo de exibição e clique no ícone ![](assets/edit-icon.png) de **Editar**.
Ou\
   No menu suspenso **Exibir**, selecione **Nova Exibição**.

1. Na área **Visualização da coluna**, clique no cabeçalho da coluna que mostra o nome da tarefa na lista.
1. Clique em **Alternar para Modo de Texto** e em **Editar Modo de Texto**.
1. Remova o texto localizado na caixa **Modo de Texto** e substitua-o pelo seguinte código:

   ```
   linkedname=direct
   namekey=name
   querysort=name
   styledef.case.0.comparison.icon=false
   styledef.case.0.comparison.leftmethod=numberOfChildren
   styledef.case.0.comparison.lefttext=numberOfChildren
   styledef.case.0.comparison.operator=gt
   styledef.case.0.comparison.operatortype=int
   styledef.case.0.comparison.righttext=0
   styledef.case.0.comparison.trueproperty.0.name=fontstyle
   styledef.case.0.comparison.trueproperty.0.value=bold
   valueexpression=IF({numberOfChildren}>"0",UPPER({name}),{name})
   valueformat=HTML
   ```

1. Clique em **Concluído** e em **Salvar exibição**.
