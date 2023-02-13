---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Exibir: exibir recuos da tarefa em uma lista de tarefas'''
description: Nesta visualização de tarefa, é possível adicionar código à coluna Nome da Tarefa para exibir as tarefas recuadas de acordo com a Estrutura de Detalhamento do Trabalho do projeto.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f7f43e1e-db32-48b8-9a23-ff9fa6195386
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Exibir: exibir recuos de tarefas em uma lista de tarefas

Nesta visualização de tarefa, é possível adicionar código à coluna Nome da Tarefa para exibir as tarefas recuadas de acordo com a Estrutura de Detalhamento do Trabalho do projeto.

![](assets/view-text-mode-indentation-task-list-350x171.png)

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

## Exibir recuos de tarefas em uma coluna de uma lista de tarefas

1. Vá para uma lista de tarefas.
1. No **Exibir** , clique em **Nova exibição**.

1. Clique em **Adicionar coluna** e comece a digitar &quot;Nome da tarefa&quot; no **Mostrar nesta coluna** em seguida, selecione-o quando for exibido na lista.

1. Na nova coluna, clique em **Alternar para o modo de texto**.
1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar texto**.
1. Remova o texto que você encontrar no

   ```
   valuefield=
   ```

   e substitua-a pelo seguinte código:

   ```
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(' - ',{name}),IF({indent}<3,CONCAT(' - - ',{name}),IF({indent}<4,CONCAT(' - - - ',{name}),CONCAT(' - - - - ',{name})))))
   ```

1. Clique em **Salvar**, em seguida **Salvar exibição**.
