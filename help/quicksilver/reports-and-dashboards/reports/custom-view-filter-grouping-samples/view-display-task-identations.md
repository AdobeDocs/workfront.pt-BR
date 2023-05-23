---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: "Exibir: exibir recuos de tarefas em uma lista de tarefas"
description: Nesta visualização de tarefa, você pode adicionar código à coluna Nome da tarefa para exibir as tarefas recuadas de acordo com a Estrutura de divisão de trabalho do projeto.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f7f43e1e-db32-48b8-9a23-ff9fa6195386
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# Exibição: exibir recuos de tarefas em uma lista de tarefas

Nesta visualização de tarefa, você pode adicionar código à coluna Nome da tarefa para exibir as tarefas recuadas de acordo com a Estrutura de divisão de trabalho do projeto.

![](assets/view-text-mode-indentation-task-list-350x171.png)

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

## Exibir recuos de tarefas em uma coluna de uma lista de tarefas

1. Ir para uma lista de tarefas.
1. No **Exibir** clique em **Nova visualização**.

1. Clique em **Adicionar coluna** e comece digitando &quot;Nome da tarefa&quot; no campo **Mostrar nesta coluna** e selecione-o quando ele for exibido na lista.

1. Na nova coluna, clique em **Alternar para modo de texto**.
1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar o texto**.
1. Remova o texto localizado na

   ```
   valuefield=
   ```

   e substitua-o pelo seguinte código:

   ```
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(' - ',{name}),IF({indent}<3,CONCAT(' - - ',{name}),IF({indent}<4,CONCAT(' - - - ',{name}),CONCAT(' - - - - ',{name})))))
   ```

1. Clique em **Salvar**, depois **Salvar visualização**.
