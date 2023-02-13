---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Exibir: URL externo usando campo de dados personalizado'''
description: Você pode exibir um link para um URL personalizado interno usando um Campo personalizado calculado chamado "URL personalizado" em uma Exibição de tarefa.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 0%

---

# Exibir: URL externo usando campo de dados personalizado

Você pode exibir um link para um URL personalizado interno usando um **Campo personalizado calculado** chamado de &quot;URL personalizado&quot; em um **Exibição de tarefa**.

Isso ajuda a vincular rapidamente de determinados objetos em uma visualização a determinadas áreas do aplicativo, diretamente dos relatórios.

Ao criar um campo personalizado calculado, primeiro crie o campo e depois crie a Exibição.

As seções a seguir são um exemplo de um campo personalizado calculado para tarefas. O campo personalizado é chamado de URL personalizado. A exibição personalizada exibe o valor do campo, bem como a variável **URL** para tarefas.

Usando as mesmas etapas, é possível criar campos personalizados calculados e exibições personalizadas semelhantes para todos os objetos no sistema que têm um Formulário personalizado.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Relatórios, Painéis, Calendários</p> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Crie o campo personalizado &quot;URL personalizado&quot; calculado

Para obter informações sobre como criar um campo personalizado calculado, consulte o artigo [Adicionar dados calculados a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Se você tiver acesso para criar um formulário personalizado, poderá criar um campo personalizado calculado para tarefas chamado &quot;URL personalizado&quot;. Esse campo vincula diretamente à variável **Visão geral** na subguia **Detalhes da tarefa** guia .

1. Crie um campo personalizado calculado.
1. No campo Calculation , digite o seguinte código:

   CONCAT(&#39;&#39;https://`<domain>`.my.workfront.com&quot;,&quot;/&quot;,&quot;task/&quot;,ID,&quot;/overview&#39;&#39;)

1. Substituir &quot;`<domain>`&quot; com seu nome de domínio real, sem os colchetes.

   O

   ```
   /overview
   ```

   parte desse URL direciona o link para a variável **Visão geral** no painel esquerdo da tarefa.

1. Depois de criar o **Campo personalizado calculado**, anexe o **Formulário personalizado** com esse campo para várias tarefas no Adobe Workfront que você deseja exibir na nova visualização.

## Crie a exibição que exibe os campos &quot;URL personalizado&quot; e &quot;URL&quot; da tarefa

A tarefa **Exibir** no exemplo abaixo exibe a variável **Campo personalizado calculado** chamado de &quot;URL personalizado&quot; como um link direto para o **Visão geral** subguia dentro da tarefa **Detalhes** , bem como a guia **URL** da tarefa.

![](assets/task-view-with-custom-url-field-quicksilver-350x70.png)

Para personalizar esta exibição:

1. Vá para uma lista de tarefas.
1. Expanda o **Exibir** na parte superior da lista de tarefas.
1. Clique em **Personalizar exibição**.
1. Remova todas as colunas dentro da exibição, exceto a primeira coluna.
1. Clique no cabeçalho da primeira coluna.
1. Clique em **Alternar para o modo de texto** no canto superior direito da interface.
1. Clique em **Clique para editar texto**.
1. Cole o modo de texto abaixo em uma coluna.\
   Neste exemplo, o &#39;column.1.&#39; exibe o valor no campo &quot;URL personalizado&quot; como um link no campo da tarefa **Visão geral**. &quot;Coluna.2.&quot; exibe o valor armazenado no **Campo de URL** da tarefa.
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat= int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield= objCode<br>column.0.link.value.format= val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.estich=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.description=URL personalizado<br>column.1.link.isnewwindow=true<br>column.1.link.url=customDataLabelsAsString(URL personalizado)<br>column.1.linkedname=direct<br>column.1.listsort=customDataLabelsAsString(URL personalizado)<br>column.1.name=Custom URL<br>column.1.querysort=URL<br>column.1.shortview=false<br>column.1.alongch=0<br>column.1.value.field=URL personalizada<br>column.1.valueformat=customDataLabelsAsString<br>column.1.width=150<br>column.2.descriptionkey=url<br>column.2.linkedname=direct<br>column.2.listsort=string(URL)<br>column.2.namekey=url.abbr<br>column.2.querysort=URL<br>column.2.shortview=false<br>column.2.alongch=0<br>column.2.valuefield=URL<br>column.2.valueformat=HTML<br>column.2.width=150</pre>

1. Clique em **Salvar exibição**.
