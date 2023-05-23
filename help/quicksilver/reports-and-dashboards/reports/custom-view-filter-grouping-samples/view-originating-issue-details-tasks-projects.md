---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Exibir: detalhes de problemas de origem para tarefas e projetos"
description: Quando um problema é convertido em uma tarefa ou um projeto, uma relação de objeto de resolução é estabelecida entre a tarefa ou o projeto e o problema. Essa exibição exibe os seguintes campos do problema que é concluído automaticamente quando a tarefa ou o projeto é concluído - EDIT ME.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5fefb174-3a18-408f-aa12-3f4aff23acfa
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 3%

---

# Exibir: detalhes de problemas de origem para tarefas e projetos

Quando um problema é convertido em uma tarefa ou um projeto, uma relação de objeto de resolução é estabelecida entre a tarefa ou o projeto e o problema. Essa exibição exibe os seguintes campos da ocorrência que é concluída automaticamente quando a tarefa ou o projeto é concluído:

* Nome
* Data de Entrada
* Data de conclusão planejada
* Data de Término Efetivo
* Tipo de requisição
* Nome do Originador
* Atribuído para usuário

![task_with_resolving_issue_fields.png](assets/task-with-resolving-issue-fields-350x38.png)

Para obter mais informações, consulte também [Exibir: exibir informações sobre a emissão original em listas de tarefas e projetos](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

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

## Exibir detalhes de problemas de origem para tarefas e projetos

1. Ir para uma lista de tarefas ou uma lista de projetos.
1. No **Exibir** selecione **Nova visualização**.

1. No **Visualização da coluna** elimine todas as colunas, exceto uma.
1. Clique no cabeçalho da coluna restante e clique em **Alternar para modo de texto**.
1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar o texto**.
1. Remova o texto localizado na **Modo de texto** e substitua-o pelo seguinte código:

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Clique em **Salvar visualização**.
