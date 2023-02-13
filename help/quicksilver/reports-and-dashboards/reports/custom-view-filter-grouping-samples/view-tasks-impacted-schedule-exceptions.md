---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Exibir: tarefas afetadas por exceções de agendamento'
description: Esta exibição de tarefa identifica tarefas que terão que ser concluídas com atraso devido aos finais de semana, Tempo Limite Pessoal ou outras exceções de programação.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7d7c77fa-d9a7-4e91-8dae-ad3aaca6f1da
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# Exibir: tarefas afetadas por exceções de agendamento

Esta exibição de tarefa identifica tarefas que terão que ser concluídas com atraso devido aos finais de semana, Tempo Limite Pessoal ou outras exceções de programação.

Essa exibição exibe o seguinte:

* A duração das tarefas
* As Datas de Início e Conclusão Planejadas das tarefas
* A duração das tarefas de acordo com o número de dias entre o Início Planejado e as Datas de Conclusão Planejadas das tarefas (Duração do Calendário)
* O número do dia no agendamento do projeto quando a tarefa é iniciada (Data de Início do Calendário)
* A Duração da Semana das tarefas de acordo com o número de dias da semana entre o Início Planejado e as Datas de Conclusão Planejadas das tarefas (Duração do Dia da Semana)
* Se a Duração do dia da semana for maior que a duração das tarefas, o que sugere que há dias de exceção na duração das tarefas, as tarefas são marcadas como uma &quot;Exceção&quot;.\
   ![tasks_with_calendar_exception.png](assets/tasks-with-calendar-exceptions-350x51.png)

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

## Exibir tarefas afetadas por exceções de programação

1. Vá para uma lista de tarefas.
1. No **Exibir** , selecione **Nova exibição**.

1. No **Visualização de coluna** , elimine todas as colunas, exceto uma.
1. Clique no cabeçalho da coluna restante e, em seguida, clique em **Alternar para o modo de texto**.
1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar texto**.
1. Remova o texto que você encontrar no **Modo de texto** e substitua-a pelo seguinte código:
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.value=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.estich=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=duration<br>column.1.linkedname=direct<br>column.1.listsort=intAsInt(durationMinutes)<br>column.1.namekey=duration.abbr<br>column.1.querysort=durationMinutes<br>column.1.shortview=false<br>column.1.alongch=0<br>column.1.valuefield=durationFieldLong<br>column.1.valueformat=composto<br>column.1.viewalias=duration<br>column.1.width=80<br>column.2.descriptionkey=plannedstartdate<br>column.2.linkedname=direct<br>column.2.listsort=atDateAsAtDate(planStartDate)<br>column.2.namekey=plannedstartdate.abbr<br>column.2.querysort=planStartDate<br>column.2.shortview=false<br>column.2.alongch=0<br>column.2.valuefield=planStartDate<br>column.2.valueformat=atDate<br>column.2.width=80<br>column.3.descriptionkey=plannedcompletiondate<br>column.3.linkedname=direct<br>column.3.listsort=atDateAsAtDate(planCompletionDate)<br>column.3.namekey=plannedcomplete.abbr<br>column.3.querysort=planCompletionDate<br>column.3.shortview=false<br>column.3.alongch=0<br>column.3.valuefield=planCompletionDate<br>column.3.valueformat=atDate<br>column.3.width=80<br>column.4.agregator.displayformat=int<br>column.4.agregator.function=SUM<br>column.4.agregator.namekey=id<br>column.4.agregator.valueexpression=DATEDIFF({planCompletionDate},<br>{planStartDate})+1<br>column.4.agregator.value=intAsInt<br>column.4.descriptionkey=id<br>column.4.linkedname=direct<br>column.4.listsort=intAsInt(ID)<br>column.4.name=Duração do calendário<br>column.4.querysort=ID<br>column.4.shortview=false<br>column.4.alongch=0<br>column.4.valueexpression=DATEDIFF({planCompletionDate},{planStartDate})+1<br>column.4.valueformat=int<br>column.4.width=80<br>column.5.agregator.displayformat=int<br>column.5.agregator.function=SUM<br>column.5.agregator.namekey=id<br>column.5.agregator.valueexpression=DATEDIFF({planStartDate},{project}.<br>{planStartDate})+0<br>column.5.agregator.value=intAsInt<br>column.5.descriptionkey=id<br>column.5.linkedname=direct<br>column.5.listsort=intAsInt(ID)<br>column.5.name=Data de início do calendário<br>column.5.querysort=ID<br>column.5.shortview=false<br>column.5.estich=0<br>column.5.valueexpression=DATEDIFF({planStartDate},{project}.{planStartDate})+0<br>column.5.valueformat=int<br>column.5.width=80<br>column.6.agregator.displayformat=int<br>column.6.agregator.function=SUM<br>column.6.agregator.namekey=id<br>column.6.agregator.valueexpression=WEEKDAYDIFF({planStartDate},<br>{planCompletionDate})+0<br>column.6.agregator.valueformat=HTML<br>column.6.descriptionkey=id<br>column.6.linkedname=direct<br>column.6.listsort=intAsInt(ID)<br>column.6.name=Week Day Duration<br>column.6.querysort=ID<br>column.6.shortview=false<br>column.6.estich=0<br>column.6.valueexpression=WEEKDAYDIFF({planStartDate},{planCompletionDate})+0<br>column.6.valueformat=int<br>column.6.width=80<br>column.7.agregator.displayformat=int<br>column.7.agregator.expression=IF((WEEKDAYDIFF({planStartDate},{planCompletionDate}))&gt;({duration}/480),"Exception",")<br>column.7.agregator.function=SUM<br>column.7.agregator.namekey=id<br>column.7.agregator.value=HTML<br>column.7.linkedname=direct<br>column.7.listsort=intAsInt(ID)<br>column.7.name=Schedule<br>column.7.querysort=ID<br>column.7.shortview=false<br>column.7.estich=0<br>column.7.valueexpression=IF((WEEKDAYDIFF({planStartDate},{planCompletionDate}))&gt;({duration}/480),"Exception",")<br>column.7.valueformat=HTML<br>column.7.width=80</pre>

1. Clique em **Salvar exibição**.
