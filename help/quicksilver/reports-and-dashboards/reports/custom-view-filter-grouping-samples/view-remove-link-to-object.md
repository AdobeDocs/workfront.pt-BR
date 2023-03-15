---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Exibir: remover link para um objeto em uma coluna'''
description: Alguns objetos exibidos em um link de exibição para a página Detalhes do objeto, por padrão. Por exemplo, a coluna que exibe o Nome de um projeto é um link para o projeto; a coluna que exibe o Nome de um usuário é um link para a página de perfil do usuário.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# Exibir: remover link para um objeto em uma coluna

Alguns objetos exibidos em um link de exibição para a página Detalhes do objeto, por padrão. Por exemplo, a coluna que exibe o Nome de um projeto é um link para o projeto; a coluna que exibe o Nome de um usuário é um link para a página de perfil do usuário.

Você pode remover esse link usando o modo de texto em colunas que são exibidas em todas as exibições.

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

## Exemplo: Remova o link para uma tarefa da coluna Nome da Tarefa em uma exibição de tarefa:

1. Vá para uma lista de tarefas.
1. No **Exibir** , clique em **Nova exibição** para criar uma nova visualização.

   Ou

   Clique no botão **Ícone Editar** ![](assets/edit-icon.png)

   para editar uma exibição existente, selecione-a.

1. Clique em **Adicionar coluna** para adicionar uma nova coluna.

   Ou

   Clique em uma coluna existente com um link para um objeto.

1. Clique em **Alternar para o modo de texto**.
1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar texto**.
1. Remova o texto que você encontrar no **Modo de texto** e substitua-a pelo seguinte código:

   <pre>displayname=Task Name<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br><strong>valueexpression={name}</strong><br>valueformat=Compound</pre>

   >[!TIP]
   >
   >Você pode usar um código semelhante para outros objetos ajustando o seguinte:
   >
   >   
   >   
   >   * Substitua o **campo de valor** linha do código com **valueexpression** e manter o mesmo nome incluído entre chaves depois do sinal de igual.
   >   
   >   
   >
   >   
   >   
   >   * Elimine todas as linhas que começam com >
   >   
      >     ```>   
      >     link.
      >     ```   >   
      >   
      >     from the original text of the column. For example, eliminate all the following lines:
      >     <pre>link.linkproperty.0.name=ID</pre><pre>link.linkproperty.0.valuefield=ID</pre><pre>link.linkproperty.0.valueformat=string</pre><pre>link.lookup=link.view</pre><pre>link.value=val(objCode)</pre>
      >   
      >   
      >



1. Clique em **Salvar**, em seguida **Salvar exibição**.
