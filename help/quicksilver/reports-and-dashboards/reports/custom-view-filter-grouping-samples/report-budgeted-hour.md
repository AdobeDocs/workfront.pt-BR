---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Relatório: Hora do Orçamento'''
description: '"Relatório: Hora do Orçamento'''
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 1%

---

# Relatório: Hora do Orçamento

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resouce Management and it is super important.) </p>
-->

Quando quiser compartilhar informações de Hora do Orçamento com outros usuários que não têm acesso ao Planejador de Recursos, crie um relatório de Hora do Orçamento. É possível compartilhar o relatório com eles.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This info is also added and drafted in the article "View Budget Hours in a report" in the Resource Planning section. Consider deleting this article?!)</p>
-->

>[!IMPORTANT]
>
>As Horas Orçadas são atualizadas a cada hora no banco de dados do Adobe Workfront. Atualizar o relatório não necessariamente atualiza as informações de hora nele. Você pode visualizar o tempo decorrido desde a última atualização no canto superior direito de cada relatório de Hora do orçamento. Atualizar o relatório atualiza as informações nele somente quando houver mais de uma hora desde a última atualização.
>
>![](assets/budgeted-hour-report-time-sync-warning-350x74.png)>

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

## Criar um relatório de Hora do Orçamento

1. Clique no botão **Menu principal** ![](assets/main-menu-icon.png) no canto superior direito, em seguida, clique em **Relatórios**.

1. Clique em **Novo Relatório > Hora do Orçamento**.

   A exibição padrão é aplicada ao relatório.

1. (Opcional) Para facilitar a leitura do relatório, clique no botão **Horas Orçamentadas** coluna, em seguida **Alternar para o modo de texto** em seguida, altere a

   ```
   valuefield
   ```

   linha para

   ```
   valueexpreesion
   ```

   e insira a expressão de arredondamento.

   Isso arredonda o número de Horas Orçadas para um número de decimais especificado.

   Para obter informações sobre como arredondar um número no Workfront, consulte o artigo [Expressões de dados calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. (Opcional) Clique em **Adicionar coluna** para adicionar outras colunas.
1. (Opcional) Para facilitar a leitura do relatório, recomendamos que você adicione um agrupamento a ele. Sugerimos o seguinte agrupamento:

   Clique no botão **Agrupamentos** em seguida, execute um ou vários dos seguintes procedimentos:

   1. Clique em **Adicionar agrupamento** e comece a digitar &quot;Nome do projeto&quot;, em seguida, selecione-o quando ele for exibido na lista.
   1. Clique em **Adicionar agrupamento** e comece a digitar &quot;Nome da função do trabalho&quot;, em seguida, selecione-o quando ele for exibido na lista.
   1. Clique em **Adicionar agrupamento** e começar a digitar **Data de alocação**, selecione-o quando ele for exibido na lista e, em seguida, selecione o período que deseja agrupar no **Agrupar datas por** campo.

1. (Opcional) Clique em **Filtros** para adicionar filtros ao relatório.
1. (Opcional) Clique em **Gráfico** para adicionar um gráfico ao relatório.
1. Clique em **Salvar + Fechar**.

## Revisão do relatório de Horas Orçamentadas

As seguintes informações estão disponíveis no relatório Hora do orçamento por padrão:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Projeto </td> 
   <td>Este é o nome do projeto associado à Hora Orçada.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Função da Tarefa</p> </td> 
   <td>Este é o nome da função de trabalho associada à Hora Orçada. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Usuário</td> 
   <td>Este é o nome do usuário associado à Hora do Orçamento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Dt Aloc</td> 
   <td> <p>Esta é a Data de alocação. É o primeiro dia (um domingo) da semana para a qual você orçou as horas.</p> <p>Dica:  <p>Se uma semana se estender por dois meses, isso gera duas linhas no relatório: um correspondente ao primeiro dia da semana (o domingo da semana que ocorre durante o primeiro mês) e um segundo correspondente ao primeiro dia do segundo mês (e que pode ser qualquer dia da semana).</p> <p>Por exemplo, se você orçar 8 horas para um usuário na semana de 30 de junho (domingo) a 6 de julho (sábado), as duas linhas mostrarão uma Data de alocação de 30 de junho e 1º de julho.</p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Hrs Orç</td> 
   <td>Essas são as Horas Orçadas alocadas ao Usuário no Planejador de Recursos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pln. Hrs Orç</td> 
   <td>São as Horas Orçamentadas alocadas para a Função do Trabalho ou o Projeto no Planejador de Recursos.</td> 
  </tr> 
 </tbody> 
</table>
