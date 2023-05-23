---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Exibição: objetos resolvíveis em um relatório de tarefa ou de projeto"
description: Você pode exibir uma lista de todos os Objetos Resolvíveis em um projeto ou visualização de tarefa ou relatório.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2b0d8e7c-9211-44e5-9d92-c87a2fe4336d
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# Exibir: Objetos Resolvíveis em um relatório de tarefa ou de projeto

Você pode exibir uma lista de todos os Objetos Resolvíveis em um projeto ou visualização de tarefa ou relatório.

Para obter mais informações sobre Objetos Resolvíveis, consulte o artigo [Visão Geral de Objetos Resolventes e Resolvíveis](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

![list_of_resolvables_in_report.png](assets/list-of-resolvables-in-report-350x54.png)

A aplicação deste modo de exibição é idêntica para tarefas e projetos.

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

## Exibir Objetos Resolvíveis em um relatório de tarefa ou de projeto

1. Ir para uma lista de tarefas que foram convertidas de problemas.
1. No **Exibir** selecione **Nova visualização**.

1. No **Visualização da coluna** clique em **Adicionar coluna**.

1. Clique no cabeçalho da nova coluna e clique em **Alternar para modo de texto**.
1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar o texto**.
1. Remova o texto localizado na **Modo de texto** e substitua-o pelo seguinte código:

   <pre>displayname=Resolvables<br>delimitador de lista=<br><br>listmethod=nested(resolvables).lists<br>textmode=true<br>type=iterate<br>valuefield=nome<br>valueformat=HTML<br></pre>

1. Clique em **Salvar visualização**.\
   Uma lista de todos os Objetos Resolvíveis é exibida na nova coluna. Os nomes dos objetos na lista não podem ser vinculados diretamente aos objetos.
