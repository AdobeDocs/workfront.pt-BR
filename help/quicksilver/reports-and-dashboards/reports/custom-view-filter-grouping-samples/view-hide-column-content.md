---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Exibição: ocultar o conteúdo de uma coluna"
description: Talvez você queira ocultar as informações na coluna de uma exibição. Você pode fazer isso modificando o modo de texto da coluna.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Exibir: ocultar o conteúdo de uma coluna

Talvez você queira ocultar as informações na coluna de uma exibição. Você pode fazer isso modificando o modo de texto da coluna.

>[!TIP]
>
>* Você pode usar colunas ocultas para classificar por um determinado objeto que não deseja exibir na visualização.\
   >  Por exemplo, você pode classificar por Número da Tarefa em uma exibição de tarefa e ocultar as informações de Número da Tarefa da exibição. Nesse caso, o objeto referenciado na coluna ajuda a classificar a view, mas as informações desse objeto não são exibidas na view.
>* Quando você oculta uma coluna, observe que as informações na coluna estão ocultas, mas a coluna ainda existe na exibição.
>


## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
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
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Exemplo: Classifique e oculte a coluna Número da Tarefa em uma exibição de tarefa:

1. Ir para uma lista de tarefas.
1. No **Exibir** clique em **Nova visualização**.

1. Clique em **Adicionar coluna** e comece digitando &quot;Número da tarefa&quot; no **Mostrar nesta coluna** e selecione-o quando ele for exibido na lista.

1. Clique em **Alternar para modo de texto**.
1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar o texto**.
1. Remova o texto localizado na **Modo de texto** e substitua-o pelo seguinte código:

   <pre><strong>displayname=</strong>linkedname=direct<br>querysort=taskNumber<br>sortOrder=1<br>sortType=asc<br>textmode=true<br><strong>value=</strong>valueformat=int<br><strong>width=0</strong></pre>As alterações importantes nesse código que tornam a coluna oculta são:

   ```
   displayname
   ```

   esta linha deve estar em branco.

   ```
   valuefield
   ```

   Esta disposição foi substituída por *value* e devem estar em branco.

   ```
   width
   ```

   : Dependendo do campo, deve ter um valor de *0* ou *1*.

1. Clique em **Salvar**, depois **Salvar visualização**.
