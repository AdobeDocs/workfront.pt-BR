---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Agrupamento: detalhamento percentual da tarefa 1'''
description: 'Neste agrupamento de projeto personalizado, você pode exibir projetos agrupados por um intervalo de seus valores percentuais completos. Os detalhamentos mostram o valor percentual completo de incrementos de ponto percentual: 0-25%, 25-50%, etc.'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ddb9496c-9347-4dc9-a4ce-b9017abd0bb2
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 2%

---

# Agrupamento: detalhamento percentual de tarefa 1

Neste agrupamento de projeto personalizado, você pode exibir projetos agrupados por um intervalo de seus valores percentuais completos. Os detalhamentos mostram o valor percentual completo de incrementos de ponto percentual: 0-25%, 25-50%, etc. 

O agrupamento a seguir organiza tarefas pelo valor percentual completo em 6 agrupamentos diferentes:

* 0%
* 1-25%
* 26-50%
* 51-75%
* 76-99%
* 100%

![task_25__break_grouping.png](assets/task-25--breakdown-grouping-350x412.png)

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

## Detalhamento por porcentagem de grupo por tarefa

Para aplicar este agrupamento:

1. Vá para uma lista de tarefas.
1. No **Agrupamento** , selecione **Novo agrupamento**.

1. Clique em **Alternar para o modo de texto**.
1. Remova o texto na **Agrupar seu relatório** área.
1. Substitua o texto pelo seguinte código:

   <pre>group.0.linkedname=direct<br>group.0.name=Detalhamento da porcentagem<br>group.0.notime=false<br>group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}&lt;=26,"0-25 %",IF({percentComplete}&lt;=51,"25-50 %",IF({percentComplete}&lt;=76,"50-75 %",IF({percentComplete} &lt;100,"75-99 %","100 %"))<br>group.0.valueformat=string</pre>

1. Clique em **Salvar Agrupamento**.
