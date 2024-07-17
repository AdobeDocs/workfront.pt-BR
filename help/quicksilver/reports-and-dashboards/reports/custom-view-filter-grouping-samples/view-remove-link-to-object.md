---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualização: remover link de um objeto em uma coluna"
description: Alguns objetos exibidos em uma view são vinculados à página Detalhes do objeto, por padrão. Por exemplo, a coluna que exibe o Nome de um projeto é um link para o projeto; a coluna que exibe o Nome de um usuário é um link para a página de perfil do usuário.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 5480d6b5e97c4c2e21080bb92ffe255f60ed6f60
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---

# Exibir: remover link de um objeto em uma coluna

Alguns objetos exibidos em uma view são vinculados à página Detalhes do objeto, por padrão. Por exemplo, a coluna que exibe o Nome de um projeto é um link para o projeto; a coluna que exibe o Nome de um usuário é um link para a página de perfil do usuário.

Você pode remover esse link usando o modo de texto em colunas exibidas em todas as exibições.

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

## Exemplo: Remova o link para uma tarefa da coluna Nome da Tarefa em uma exibição de tarefa:

1. Ir para uma lista de tarefas.
1. No menu suspenso **Exibir**, clique em **Nova Exibição** para criar uma nova exibição.

   Ou

   Clique no **ícone Editar** ![](assets/edit-icon.png)

   para editar uma exibição existente, selecione-a.

1. Clique em **Adicionar coluna** para adicionar uma nova coluna.

   Ou

   Clique em uma coluna existente com um link para um objeto.

1. Clique em **Alternar para Modo de Texto**.
1. Passe o mouse sobre a área do modo de texto e clique em **Clicar para editar o texto**.
1. Remova o texto localizado na caixa **Modo de Texto** e substitua-o pelo seguinte código:
   <pre>displayname=Task Name<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br><strong>valueexpression={name}</strong><br>valueformat=Compound</pre>

   >[!TIP]
   >
   >Você pode usar um código semelhante para outros objetos ajustando o seguinte:
   >
   >* Substitua a linha **valuefield** do código por **valueexpression** e mantenha o mesmo nome incluído entre chaves após o sinal de igual.
   >* Eliminar todas as linhas que começam com `link.` do texto original da coluna. Por exemplo, elimine todas as linhas a seguir:
   >
   >  ```
   >  link.linkproperty.0.name=ID
   >  link.linkproperty.0.valuefield=ID
   >  link.linkproperty.0.valueformat=string
   >  link.lookup=link.view
   >  link.value=val(objCode)
   >  ```
   >

1. Clique em **Salvar** e depois em **Salvar exibição**.
