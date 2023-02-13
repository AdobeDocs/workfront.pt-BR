---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Exibir: adicionar uma lista de sucessores de tarefas em uma coluna'''
description: É possível adicionar uma coluna a uma exibição de tarefa para mostrar uma lista dos sucessores das tarefas. A coluna Sucessores de tarefa inclui o número do sucessor, bem como o nome.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Exibir: adicionar uma lista de sucessores de tarefas em uma coluna

É possível adicionar uma coluna a uma exibição de tarefa para mostrar uma lista dos sucessores das tarefas. O **Sucessores da Tarefa** inclui o número do sucessor, bem como o nome.

![task_view_with_a_list_of_success_png](assets/task-view-with-a-list-of-successors--350x118.png)

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

## Adicionar uma lista de sucessores de tarefas em uma coluna

Para adicionar esta coluna a uma exibição de tarefa:

1. Vá para uma visualização de tarefa existente.
1. Expanda o menu suspenso Exibir e selecione **Personalizar exibição**.
1. Clique em **Adicionar coluna**.
1. Clique em **Alternar para o modo de texto**.
1. Passe o mouse sobre o **Mostrar nesta coluna** e clique em **Clique para editar texto**.

1. Remova todo o texto da caixa Modo de texto e substitua-o pelo seguinte código:

   <pre>displayname=Task Successors<br>listdelimiter=<br><br>listmethod=nested(sucessors).lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({sucessor}.{taskNumber},' - ',{sucessor}.{name})<br>valueformat=HTML</pre>

1. Clique em **Salvar exibição**.
