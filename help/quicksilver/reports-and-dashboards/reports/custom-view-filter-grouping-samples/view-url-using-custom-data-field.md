---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Exibição: URL Externo Usando Campo de Dados Personalizado'
description: Você pode exibir um link para um URL personalizado interno usando um Campo personalizado calculado chamado "URL personalizado" em uma Exibição de tarefa.
author: Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# Exibição: URL externo usando campo de dados personalizado

<!--Audited: 11/2024-->

Você pode exibir um link para uma URL personalizada interna usando um **Campo Personalizado Calculado** chamado &quot;URL Personalizado&quot; em uma **Exibição de Tarefa**.

Isso ajuda você a se vincular rapidamente de determinados objetos em uma exibição a determinadas áreas do aplicativo diretamente dos seus relatórios.

Ao criar um campo personalizado calculado, primeiro crie o campo e, em seguida, crie a Exibição.

As seções a seguir são um exemplo de um campo personalizado calculado para tarefas. O campo personalizado é chamado de URL personalizado. O modo de exibição personalizado mostra o valor do campo, bem como o campo **URL** para tarefas.

Usando as mesmas etapas, você pode criar campos personalizados calculados semelhantes e exibições personalizadas para todos os objetos no sistema que têm um Formulário personalizado.

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

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Crie o campo personalizado calculado &quot;URL personalizado&quot;

Para obter informações sobre como criar um campo personalizado calculado, consulte [Adicionar campos calculados a um formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Se você tiver acesso para criar um formulário personalizado, poderá criar um campo personalizado calculado para tarefas chamadas &quot;URL personalizado&quot;. Este campo está vinculado diretamente à subguia **Visão Geral** da guia **Detalhes da Tarefa**.

1. Crie um campo personalizado calculado.
1. No campo Calculation, insira o seguinte código:

   CONCAT(&#39;&#39;https://`<domain>`.my.workfront.com&quot;,&quot;/&quot;,&quot;task/&quot;,ID,&quot;/overview&#39;&#39;)

1. Substitua &quot;`<domain>`&quot; pelo nome de domínio real, sem os colchetes. A parte `/overview` desta URL direciona o link para a seção **Visão geral** do painel esquerdo da tarefa.

1. Depois de criar seu **Campo Personalizado Calculado**, anexe o **Formulário Personalizado** com este campo a várias tarefas no Adobe Workfront que você deseja exibir no seu novo modo de exibição.

## Crie a exibição que mostra os campos &quot;URL personalizado&quot; e &quot;URL&quot; da tarefa

A tarefa **Exibir** no exemplo abaixo exibe o **Campo Personalizado Calculado** chamado de &quot;URL Personalizado&quot; como um link direto para a subguia **Visão Geral** na guia de tarefa **Detalhes**, bem como o campo **URL** da tarefa.

(assets/task-view-with-custom-url-field-quicksilver-350x70.png)

Para personalizar esta exibição:

1. Ir para uma lista de tarefas.
1. Expanda o menu suspenso **Exibir** na parte superior da lista de tarefas.
1. Clique em **Personalizar exibição**.
1. Remova todas as colunas da exibição, exceto a primeira coluna.
1. Clique no cabeçalho da primeira coluna.
1. Clique em **Alternar para Modo de Texto** > **Editar Modo de Texto**.
1. Remova o texto da caixa **Editar Modo de Texto** e substitua-o pelo seguinte código:


   ```
   column.0.descriptionkey=name
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat= int
   column.0.link.lookup=link.view
   column.0.link.valuefield= objCode
   column.0.link.valueformat= val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.description=Custom URL
   column.1.link.isnewwindow=true
   column.1.link.url=customDataLabelsAsString(Custom URL)
   column.1.linkedname=direct
   column.1.listsort=customDataLabelsAsString(Custom URL)
   column.1.name=Custom URL
   column.1.querysort=URL
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=Custom URL
   column.1.valueformat=customDataLabelsAsString
   column.1.width=150
   column.2.descriptionkey=url
   column.2.linkedname=direct
   column.2.listsort=string(URL)
   column.2.namekey=url.abbr
   column.2.querysort=URL
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=URL
   column.2.valueformat=HTML
   column.2.width=150
   ```

   Neste exemplo, a &#39;column.1.&#39; as linhas exibem o valor no campo &#39;URL personalizado&#39; como um link na seção **Visão geral** da tarefa; &#39;coluna.2.&#39; exibe o valor armazenado no **Campo de URL** da tarefa.

1. Clique em **Concluído** > **Salvar exibição**.
