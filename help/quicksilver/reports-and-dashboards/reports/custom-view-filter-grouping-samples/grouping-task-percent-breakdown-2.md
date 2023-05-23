---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Agrupamento: detalhamento de percentual de tarefa 2"
description: 'Neste agrupamento de tarefa personalizado, você pode exibir tarefas agrupadas por um intervalo de seus valores de porcentagem concluída. Os detalhamentos mostram o valor percentual concluído de incrementos de 10% pontos: 1-10%, 11-20%, etc.'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7d5a40dd-d451-48c7-9323-af52aa387709
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 4%

---

# Agrupamento: detalhamento de percentual de tarefa 2

Neste agrupamento de tarefa personalizado, você pode exibir tarefas agrupadas por um intervalo de seus valores de porcentagem concluída. Os detalhamentos mostram o valor percentual concluído de incrementos de 10% pontos: 1-10%, 11-20%, etc.

O agrupamento a seguir organiza projetos pelo valor percentual concluído em um desses agrupamentos:

* 0%
* 1 - 10%
* 11-20%
* 21-30%
* 31-40%
* 41-50%
* 51-60%
* 61-70%
* 71-80%
* 81-90%
* 91-99%
* 100%

![task_10_detalhamento_agrupamento.png](assets/task-10--breakdown-grouping-350x547.png)

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
   <td> <p>Solicitação para modificar um agrupamento </p>
   <p>Planejar a modificação de um relatório</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar um agrupamento</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Agrupar por detalhamento de percentual de tarefa

Para aplicar esse agrupamento:

1. Ir para uma lista de tarefas.
1. No **Agrupamento** selecione **Novo Agrupamento**.

1. Clique em **Alternar para modo de texto**.
1. Remova o texto da **Agrupar seu relatório** área.
1. Substitua o texto pelo seguinte código:

   <pre>group.0.linkedname=direct<br>group.0.name=Detalhamento percentual<br>group.0.notime=false<br>group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}&lt;=11,"1-10 %",IF({percentComplete}&lt;=21,"11-20 %",IF({percentComplete}&lt;=31,"21-30 %",IF({percentComplete}&lt;41,"31-40 %",IF({percentComplete}&lt;51,"41-50 %",IF ({percentComplete}&lt;61,"51-60 %",IF({percentComplete}&lt;71,"61-70 %",IF({percentComplete}&lt;81,"71-80 %",IF({percentComplete}&lt;91,"81-90 %",IF({percentComplete}&lt;100,"91-99 %","100 %"))))))))))))))<br>textmode=true</pre>

1. Clique em **Salvar Agrupamento**.
