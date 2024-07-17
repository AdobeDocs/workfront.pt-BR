---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualização: URL externo usando campo de dados personalizado"
description: Você pode exibir um link para um URL personalizado interno usando um Campo personalizado calculado chamado "URL personalizado" em uma Exibição de tarefa.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---

# Exibição: URL externo usando campo de dados personalizado

Você pode exibir um link para uma URL personalizada interna usando um **Campo Personalizado Calculado** chamado &quot;URL Personalizado&quot; em uma **Exibição de Tarefa**.

Isso ajuda você a se vincular rapidamente de determinados objetos em uma exibição a determinadas áreas do aplicativo diretamente dos seus relatórios.

Ao criar um campo personalizado calculado, primeiro crie o campo e, em seguida, crie a Exibição.

As seções a seguir são um exemplo de um campo personalizado calculado para tarefas. O campo personalizado é chamado de URL personalizado. O modo de exibição personalizado mostra o valor do campo, bem como o campo **URL** para tarefas.

Usando as mesmas etapas, você pode criar campos personalizados calculados semelhantes e exibições personalizadas para todos os objetos no sistema que têm um Formulário personalizado.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitação para modificar uma exibição </p>
   <p>Planejar a modificação de um relatório</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar uma visualização</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Crie o campo personalizado calculado &quot;URL personalizado&quot;

Para obter informações sobre como criar um campo personalizado calculado, consulte o artigo [Adicionar dados calculados a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Se você tiver acesso para criar um formulário personalizado, poderá criar um campo personalizado calculado para tarefas chamadas &quot;URL personalizado&quot;. Este campo está vinculado diretamente à subguia **Visão Geral** da guia **Detalhes da Tarefa**.

1. Crie um campo personalizado calculado.
1. No campo Calculation, insira o seguinte código:

   CONCAT(&#39;&#39;https://`<domain>`.my.workfront.com&quot;,&quot;/&quot;,&quot;task/&quot;,ID,&quot;/overview&#39;&#39;)

1. Substitua &quot;`<domain>`&quot; pelo nome de domínio real, sem os colchetes.

   O

   ```
   /overview
   ```

   parte desta URL direciona o link para a seção **Visão geral** no painel esquerdo da tarefa.

1. Depois de criar seu **Campo Personalizado Calculado**, anexe o **Formulário Personalizado** com este campo a várias tarefas no Adobe Workfront que você deseja exibir no seu novo modo de exibição.

## Crie a exibição que mostra os campos &quot;URL personalizado&quot; e &quot;URL&quot; da tarefa

A tarefa **Exibir** no exemplo abaixo exibe o **Campo Personalizado Calculado** chamado de &quot;URL Personalizado&quot; como um link direto para a subguia **Visão Geral** na guia de tarefa **Detalhes**, bem como o campo **URL** da tarefa.

![](assets/task-view-with-custom-url-field-quicksilver-350x70.png)

Para personalizar esta exibição:

1. Ir para uma lista de tarefas.
1. Expanda o menu suspenso **Exibir** na parte superior da lista de tarefas.
1. Clique em **Personalizar exibição**.
1. Remova todas as colunas da exibição, exceto a primeira coluna.
1. Clique no cabeçalho da primeira coluna.
1. Clique em **Alternar para Modo de Texto** no canto superior direito da interface.
1. Clique em **Clique para editar o texto**.
1. Cole o modo de texto abaixo em uma coluna.\
   Neste exemplo, a &#39;column.1.&#39; exibe o valor no campo &#39;URL personalizado&#39; como um link na **Visão geral** da tarefa. &#39;Coluna.2.&#39; exibe o valor armazenado no **Campo de URL** da tarefa.
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat= int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield= objCode<br>column.0.link.valueformat= val<br>column.0.linkedname=direct<br>column.0.listsort=string(nome))<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.description=URL Personalizado<br>column.1.link.isnewwindow=true<br>column.1 link.url=customDataLabelsAsString(URL Personalizado)<br>column.1.linkedname=direct<br>column.1.listsort=customDataLabelsAsString(URL Personalizado)<br>column.1.name=URL Personalizado<br>column.1.querysort=URL<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=URL Personalizado<br>column.1.valuevalue format=customDataLabelsAsString<br>column.1.width=150<br>column.2.descriptionkey=url<br>column.2.linkedname=direct<br>column.2.listsort=string(URL)<br>column.2.namekey=url.abbr<br>column.2.querysort=URL<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2 .valuefield=URL<br>column.2.valueformat=HTML<br>column.2.width=150</pre>

1. Clique em **Salvar visualização**.
