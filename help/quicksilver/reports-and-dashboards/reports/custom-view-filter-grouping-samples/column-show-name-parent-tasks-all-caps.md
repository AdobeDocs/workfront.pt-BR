---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Exibição: Mostrar Nome de Tarefas Pai como Todas em Maiúsculas'
description: É possível adicionar essa coluna a uma visualização de tarefa para exibir o nome das tarefas pai em todas as letras maiúsculas.
author: Nolan
feature: Reports and Dashboards
exl-id: bb489920-6b17-4689-b432-b0c28bcb5d10
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---

# Modo de exibição: mostrar nome de tarefas pai como todas em maiúsculas

<!--Audited: 10/2024-->

É possível adicionar essa coluna a uma visualização de tarefa para exibir o nome das tarefas pai em todas as letras maiúsculas.

![Coluna com tarefa pai em todas as maiúsculas](assets/column-task-with-all-caps-parent-350x112.png)

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

## Mostrar nome das tarefas pai como todas em maiúsculas

Para criar essa coluna em uma exibição de tarefa:

1. Ir para uma lista de tarefas.
1. No menu suspenso **Exibir**, selecione um modo de exibição e clique no ícone **Editar** ![Ícone Editar](assets/edit-icon.png).
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
