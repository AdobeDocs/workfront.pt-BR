---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Agrupamento: detalhamento percentual do projeto 1'''
description: Neste agrupamento de projeto personalizado, você pode exibir projetos agrupados por um intervalo de seus valores percentuais completos.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7cdc8e56-3486-4e78-b494-b2ba9389c1f7
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 3%

---

# Agrupamento: detalhamento percentual do projeto 1

Neste agrupamento de projeto personalizado, você pode exibir projetos agrupados por um intervalo de seus valores percentuais completos.

O agrupamento a seguir organiza os projetos pelo valor percentual completo em um desses agrupamentos:

* 0%
* 1-25%
* 26-50%
* 51-75%
* 76-99%
* 100%

![percent_complete_break_custom_project_grouping_25__increquirements.png](assets/percent-complete-breakdown-custom-350x56.png)

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

## Agrupar por detalhamento de porcentagem do projeto

Para aplicar este agrupamento:

1. Acesse uma lista de projetos.
1. No **Agrupamento** , selecione **Novo agrupamento**.

1. Clique em **Alternar para o modo de texto**.
1. Remova o texto na caixa e cole o seguinte código no espaço disponível:
   <pre>group.0.linkedname=direct<br>group.0.name=Detalhamento da porcentagem<br>group.0.notime=false<br>group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}&lt;=26,"0-25 %",IF({percentComplete}&lt;=51,"25-50 %",IF({percentComplete}&lt;=76,"50-75 %",IF({percentComplete} &lt;100,"75-99 %","100 %"))<br>group.0.valueformat=string</pre>

1. Clique em **Salvar Agrupamento**.
