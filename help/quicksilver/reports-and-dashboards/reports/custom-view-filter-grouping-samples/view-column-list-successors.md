---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Exibição: adicionar uma lista de tarefas sucessoras em uma coluna"
description: É possível adicionar uma coluna a uma visualização de tarefa para mostrar uma lista de sucessores das tarefas. A coluna Sucessores da Tarefa inclui o número do sucessor e o nome.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 2%

---

# Exibição: adicionar uma lista de tarefas sucessoras em uma coluna

É possível adicionar uma coluna a uma visualização de tarefa para mostrar uma lista de sucessores das tarefas. A coluna **Sucessoras da Tarefa** inclui o número da sucessora e o nome.

![exibição_tarefa_com_uma_lista_de_sucessores_.png](assets/task-view-with-a-list-of-successors--350x118.png)

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

## Adicionar uma lista de tarefas sucessoras em uma coluna

Para adicionar esta coluna a uma visualização de tarefa:

1. Ir para uma visualização de tarefa existente.
1. Expanda o menu suspenso Exibir e selecione **Personalizar exibição**.
1. Clique em **Adicionar coluna**.
1. Clique em **Alternar para Modo de Texto**.
1. Passe o mouse sobre a área **Mostrar nesta coluna** e clique em **Clicar para editar texto**.

1. Remova todo o texto na caixa Modo de texto e substitua-o pelo seguinte código:
   <pre>displayname=Task Successors<br>listdelimititer=<br><br>listmethod=nested(sucessores).lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({successor}.{taskNumber},' - ',{successor}.{name})<br>valueformat=HTML</pre>

1. Clique em **Salvar visualização**.
