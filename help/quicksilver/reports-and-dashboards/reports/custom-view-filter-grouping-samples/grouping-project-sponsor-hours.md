---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Agrupamento: Patrocinador do projeto para horas'''
description: Esse agrupamento de hora organiza horas pelo patrocinador do projeto em que as horas são registradas. A interface padrão do Construtor de relatórios para agrupamentos de hora não fornece um mapeamento para o campo Patrocinador do projeto. Você deve usar a interface do Modo de texto para acessar esse campo.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6b35b0ef-18b7-4121-ae39-d7957d76c04b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# Agrupamento: Patrocinador de Projeto para horas

Esse agrupamento de hora organiza horas pelo patrocinador do projeto em que as horas são registradas. A interface padrão do Construtor de relatórios para agrupamentos de hora não fornece um mapeamento para o campo Patrocinador do projeto. Você deve usar a interface do Modo de texto para acessar esse campo.

![hour_report_group_by_esponsor.png](assets/hour-report-grouped-by-sponsor-350x39.png)

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

## Agrupar por Patrocinador de Projeto por horas

Para aplicar este agrupamento:

1. Vá para uma lista de horas.
1. No **Agrupamento** , selecione **Novo agrupamento**.

1. Clique em **Alternar para o modo de texto**.
1. Remova o texto na **Agrupar seu relatório** área.

1. Substitua o texto pelo seguinte código:

   <pre>group.0.linkedname=project:sponsor:name<br>group.0.name=<br>group.0.valuefield=project:sponsor:name<br>group.0.value.format=HTML<br>textmode=true<br></pre>

1. Clique em **Salvar Agrupamento**.
