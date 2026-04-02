---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Exibição: Ocultar o Conteúdo de uma Coluna'
description: Talvez você queira ocultar as informações na coluna de uma exibição. Você pode fazer isso modificando o modo de texto da coluna.
author: Courtney
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 13%

---

# Exibição: ocultar o conteúdo de uma coluna

<!--Audited: 11/2024-->

Talvez você queira ocultar as informações na coluna de uma exibição. Você pode fazer isso modificando o modo de texto da coluna.

>[!NOTE]
>
>* Você pode usar colunas ocultas para classificar por um determinado objeto que não deseja exibir na visualização.\
>  Por exemplo, você pode classificar por Número da Tarefa em uma exibição de tarefa e ocultar as informações de Número da Tarefa da exibição. Nesse caso, o objeto referenciado na coluna ajuda a classificar a view, mas as informações desse objeto não são exibidas na view.
>* Quando você oculta uma coluna, observe que as informações na coluna estão ocultas, mas a coluna ainda existe na exibição.

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
   <p>Colaborador ou Solicitação para modificar uma exibição </p>
   <p>Padrão ou Plano para modificar um relatório</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar uma visualização</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Exemplo: Classifique e oculte a coluna Número da Tarefa em uma exibição de tarefa:

1. Ir para uma lista de tarefas.
1. No menu suspenso **Exibir**, clique em **Nova Exibição**.

1. Clique em **Adicionar coluna** e comece a digitar &quot;Número da tarefa&quot; no campo **Mostrar nesta coluna** e, em seguida, selecione-o quando ele for exibido na lista.

1. Clique em **Alternar para Modo de Texto** e em **Editar Modo de Texto**.
1. Remova o texto localizado na caixa **Editar Modo de Texto** e substitua-o pelo seguinte código:

   ```
   displayname=
   linkedname=direct
   querysort=taskNumber
   sortOrder=1
   sortType=asc
   textmode=true
   value=
   valueformat=int
   width=0
   ```

   As alterações importantes nesse código que tornam a coluna oculta são:

   * `displayname=`: Esta linha deve estar em branco.
   * `valuefield=`: Esta linha deve ser substituída por `value=`, que deve estar em branco.
   * `width=`: Dependendo do campo, deve ter um valor de **0** ou **1**.

1. Clique em **Concluído** e depois em **Salvar exibição**.
