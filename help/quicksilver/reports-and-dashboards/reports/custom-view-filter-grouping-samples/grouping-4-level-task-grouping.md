---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Agrupamento: Agrupamento de tarefas em 4 níveis para Proprietário do Portfolio, Proprietário do Programa, Proprietário do Projeto e Status do Projeto'''
description: Este agrupamento de tarefas fornece quatro níveis de agrupamento. Nesse caso, as tarefas são agrupadas por Proprietário do Portfolio, Proprietário do programa, Proprietário do projeto e Status do projeto. Você só pode ter até três níveis de Agrupamento usando a interface padrão. Para adicionar um quarto nível, você deve usar o Modo de texto. Não é possível agrupar relatórios por mais de quatro critérios ao mesmo tempo.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# Agrupamento: Agrupamento de tarefas em 4 níveis para Proprietário do Portfolio, Proprietário do Programa, Proprietário do Projeto e Status do Projeto

Este agrupamento de tarefas fornece quatro níveis de agrupamento. Nesse caso, as tarefas são agrupadas por Proprietário do Portfolio, Proprietário do programa, Proprietário do projeto e Status do projeto. Você só pode ter até três níveis de Agrupamento usando a interface padrão. Para adicionar um quarto nível, você deve usar o Modo de texto. Não é possível agrupar relatórios por mais de quatro critérios ao mesmo tempo.

![four_tier_grouping_for_tasks.png](assets/four-tier-grouping-for-tasks-350x239.png)

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

## Crie um Agrupamento de tarefa de 4 níveis para Proprietário do Portfolio, Proprietário do programa, Proprietário do projeto e Status do projeto

Para aplicar este agrupamento:

1. Vá para uma lista de tarefas.
1. No **Agrupamento** , selecione **Novo agrupamento**.

1. Clique em **Alternar para o modo de texto**.
1. Remova o texto na **Agrupar seu relatório** área.
1. Substitua o texto pelo seguinte código:

   <pre>group.0.linkedname=project<br>group.0.name=Proprietário do Portfolio<br>group.0.notime=false<br>group.0.valuefield=project:portfolio:proprietário:nome<br>group.0.valueformat=string<br>group.1.linkedname=project<br>group.1.name=Proprietário do Programa<br>group.1.notime=false<br>group.1.valuefield=project:program:proprietário:nome<br>group.1.valueformat=string<br>group.2.linkedname=projectOwnerMM<br>group.2.listgrouingparsedmethod=nested(project).nested(owner).string(name)<br>group.2.namekey=projectownermm<br>group.2.notime=false<br>group.2.valuefield=projectOwnerMM:name<br>group.2.valueformat=string<br>group.3.enumerclass=com.attask.common.constants.ProjectStatusEnum<br>group.3.linkedname=project<br>group.3.namekey=view.related column<br>group.3.namekeyargkey.0=project<br>group.3.namekeyargkey.1=status<br>group.3.notime=false<br>group.3.valuefield=project:status<br>group.3.value.format=val</pre>

1. Clique em **Salvar Agrupamento**.
