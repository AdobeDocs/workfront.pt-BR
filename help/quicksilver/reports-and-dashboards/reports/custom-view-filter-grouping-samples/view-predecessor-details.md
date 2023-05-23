---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Exibir: detalhes do antecessor"
description: Esta exibição de tarefa mostra detalhes dos predecessores das tarefas usando uma exibição de coleção. Em uma exibição de coleção, é possível exibir informações sobre objetos que estão em uma relação "um para muitos". Nesse caso, cada tarefa (uma) pode ter várias predecessoras (muitas). A view exibe o nome das tarefas, bem como os Nomes dos Predecessores, os Nomes dos Projetos dos Predecessores, as Datas de Conclusão Planejadas dos Predecessores e os Status dos Predecessores.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 0187da94-4895-47b1-914f-284fed9e0fd0
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---

# Exibir: detalhes da predecessora

Esta exibição de tarefa mostra detalhes dos predecessores das tarefas usando uma exibição de coleção. Em uma exibição de coleção, é possível exibir informações sobre objetos que estão em uma relação &quot;um para muitos&quot;. Nesse caso, cada tarefa (uma) pode ter várias predecessoras (muitas). A view exibe o nome das tarefas, bem como os Nomes dos Predecessores, os Nomes dos Projetos dos Predecessores, as Datas de Conclusão Planejadas dos Predecessores e os Status dos Predecessores.

Para obter informações sobre como fazer referência a coleções nos relatórios, consulte [Coleções de referência em um relatório](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

![predecessor_details_task_view.png](assets/predecessor-details-task-view-350x34.png)

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

## Exibir detalhes da predecessora

1. Ir para uma lista de tarefas.
1. No **Exibir** selecione **Nova visualização**.

1. No **Visualização da coluna** elimine todas as colunas, exceto uma.
1. Clique no cabeçalho da coluna restante e clique em **Alternar para modo de texto**.
1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar o texto**.
1. Remova o texto localizado na **Modo de texto** e substitua-o pelo seguinte código:
   <pre>column.0.displayname=<br>column.0.linkedname=direct<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.valuefield=nome<br>column.0.valueformat=HTML<br>column.1.displayname=Números e Nomes dos Predecessores<br>column.1.listdelimititer=<br><br>column.1.listmethod=nested(predecessors).lists<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.valueexpression=CONCAT({antecessor}.{taskNumber},' - ',{antecessor}.{name})<br>column.1.valueformat=HTML<br>column.2.displayname=Nomes de Projetos Predecessores<br>column.2.listdelimititer=<br><br>column.2.listmethod=nested(predecessors).lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.valueexpression={predecessor}.{projeto}.{name}<br>column.2.valueformat=HTML<br>column.3.displayname=Datas de Conclusão de Predecessores<br>column.3.listdelimititer=<br><br>column.3.listmethod=nested(predecessors).lists<br>column.3.textmode=true<br>column.3.type=iterar<br>column.3.valueexpression={predecessor}.{plannedCompletionDate}<br>column.3.valueformat=HTML<br>column.4.displayname=Status dos Predecessores<br>column.4.listdelimititer=<br><br>column.4.listmethod=nested(predecessors).lists<br>column.4.textmode=true<br>column.4.type=iterate<br>column.4.valueexpression={predecessor}.{status}<br>column.4.valueformat=HTML</pre>

1. Clique em **Salvar visualização**.
