---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Exibir: detalhes de emissão originada para tarefas e projetos'
description: Quando um problema é convertido em uma tarefa ou projeto, uma relação de objeto de resolução é estabelecida entre a tarefa ou projeto e o problema. Essa exibição exibe os seguintes campos do problema que é concluído automaticamente quando a tarefa ou projeto é concluído - EDITAR-ME.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5fefb174-3a18-408f-aa12-3f4aff23acfa
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 3%

---

# Exibir: detalhes de emissão originada para tarefas e projetos

Quando um problema é convertido em uma tarefa ou projeto, uma relação de objeto de resolução é estabelecida entre a tarefa ou projeto e o problema. Essa exibição exibe os seguintes campos do problema que é concluído automaticamente quando a tarefa ou projeto é concluído:

* Nome
* Data de Entrada
* Data de conclusão planejada
* Data de Término Efetivo
* Tipo de requisição
* Nome do Originador
* Atribuído ao usuário

![task_with_resolving_issue_fields.png](assets/task-with-resolving-issue-fields-350x38.png)

Para obter mais informações, consulte também [Exibir: exibir informações de problema originais em listas de tarefas e projetos](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

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

## Exibir detalhes de problemas originados para tarefas e projetos

1. Acesse uma lista de tarefas ou uma lista de projetos.
1. No **Exibir** , selecione **Nova exibição**.

1. No **Visualização de coluna** , elimine todas as colunas, exceto uma.
1. Clique no cabeçalho da coluna restante e, em seguida, clique em **Alternar para o modo de texto**.
1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar texto**.
1. Remova o texto que você encontrar no **Modo de texto** e substitua-a pelo seguinte código:

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Clique em **Salvar exibição**.
