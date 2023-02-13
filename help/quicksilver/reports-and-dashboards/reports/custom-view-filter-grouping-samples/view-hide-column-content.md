---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Exibir: ocultar o conteúdo de uma coluna'''
description: Talvez você queira ocultar as informações na coluna de uma exibição. Você pode fazer isso modificando o modo de texto da coluna.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Exibir: ocultar o conteúdo de uma coluna

Talvez você queira ocultar as informações na coluna de uma exibição. Você pode fazer isso modificando o modo de texto da coluna.

>[!TIP]
>
>* Você pode usar colunas ocultas para classificar por um determinado objeto que não deseja exibir na exibição.\
   >  Por exemplo, você pode classificar por Número da Tarefa em uma exibição de tarefa e ocultar as informações do Número da Tarefa na exibição. Nesse caso, o objeto referenciado na coluna ajuda a classificar a exibição, mas as informações desse objeto não são exibidas na exibição.
>* Ao ocultar uma coluna, observe que as informações na coluna estão ocultas, mas a coluna ainda existe na exibição.
>


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

## Exemplo: Classifique e oculte a coluna Número da Tarefa em uma exibição de tarefa:

1. Vá para uma lista de tarefas.
1. No **Exibir** , clique em **Nova exibição**.

1. Clique em **Adicionar coluna** e comece a digitar &quot;Número da tarefa&quot; no **Mostrar nesta coluna** em seguida, selecione-o quando for exibido na lista.

1. Clique em **Alternar para o modo de texto**.
1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar texto**.
1. Remova o texto que você encontrar no **Modo de texto** e substitua-a pelo seguinte código:

   <pre><strong>displayname=</strong>linkedname=direct<br>querysort=taskNumber<br>sortOrder=1<br>sortType=asc<br>textmode=true<br><strong>value=</strong>valueformat=int<br><strong>width=0</strong></pre>As alterações importantes nesse código que tornam a coluna oculta são:

   ```
   displayname
   ```

   esta linha deve estar em branco.

   ```
   valuefield
   ```

   Esse item foi substituído por *value* e devem estar em branco.

   ```
   width
   ```

   : Dependendo do campo , deve haver um valor de *0* ou *1*.

1. Clique em **Salvar**, em seguida **Salvar exibição**.
