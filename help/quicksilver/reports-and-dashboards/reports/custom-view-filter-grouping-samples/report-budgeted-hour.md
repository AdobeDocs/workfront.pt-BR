---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Relatório: Hora orçada"
description: "Relatório: Hora orçada"
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 1%

---

# Relatório: Hora orçada

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resouce Management and it is super important.) </p>
-->

Quando você deseja compartilhar informações de Hora orçada com outros usuários que não têm acesso ao Planejador de recursos, é possível fazê-lo criando um relatório de Hora orçada. Você pode compartilhar o relatório com eles.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This info is also added and drafted in the article "View Budget Hours in a report" in the Resource Planning section. Consider deleting this article?!)</p>
-->

>[!IMPORTANT]
>
>As horas orçadas são atualizadas a cada hora no banco de dados do Adobe Workfront. Atualizar o relatório não atualiza necessariamente as informações de hora contidas. Você pode visualizar o tempo decorrido desde a última atualização no canto superior direito de cada relatório de Horas orçadas. Atualizar o relatório atualiza as informações nele apenas quando houver mais de uma hora desde a última atualização.
>
>![](assets/budgeted-hour-report-time-sync-warning-350x74.png)>

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis, calendários</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Criar um relatório de horas orçadas

1. Clique em **Menu principal** ![](assets/main-menu-icon.png) no canto superior direito e clique em **Relatórios**.

1. Clique em **Novo relatório > Hora orçada**.

   A visualização padrão é aplicada ao relatório.

1. (Opcional) Para facilitar a leitura do relatório, clique no link **Horas orçadas** coluna, depois **Alternar para modo de texto** e, em seguida, altere o

   ```
   valuefield
   ```

   linha para

   ```
   valueexpreesion
   ```

   e insira a expressão de arredondamento.

   Isso arredonda o número de Horas orçadas para um número de decimais que você especificar.

   Para obter informações sobre como arredondar um número no Workfront, consulte o artigo [Visão geral das expressões de dados calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. (Opcional) Clique em **Adicionar coluna** para adicionar mais colunas.
1. (Opcional) Para facilitar a leitura do relatório, recomendamos adicionar um agrupamento a ele. Sugerimos o seguinte agrupamento:

   Clique em **Agrupamentos** e execute um ou vários dos procedimentos a seguir:

   1. Clique em **Adicionar Agrupamento** e comece digitando &quot;Nome do projeto&quot;, em seguida, selecione-o quando ele aparecer na lista.
   1. Clique em **Adicionar Agrupamento** e comece digitando &quot;Nome da função de trabalho&quot;, em seguida, selecione-o quando ele aparecer na lista.
   1. Clique em **Adicionar Agrupamento** e comece a digitar **Data de Alocação**, selecione-o quando ele aparecer na lista e selecione o período pelo qual deseja agrupar na **Datas de Grupo por** campo.

1. (Opcional) Clique em **Filtros** para adicionar filtros ao relatório.
1. (Opcional) Clique em **Gráfico** para adicionar um gráfico ao relatório.
1. Clique em **Salvar + Fechar**.

## Revise o relatório Hora orçada

As seguintes informações estão disponíveis no relatório de Horas orçadas por padrão:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Projeto </td> 
   <td>Esse é o nome do projeto associado à Hora Orçada.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Função de trabalho</p> </td> 
   <td>Esse é o nome da função de trabalho associada à Hora orçada. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Usuário</td> 
   <td>Esse é o nome do usuário associado à Hora orçada.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Dt Aloc</td> 
   <td> <p>Esta é a Data de Alocação. É o primeiro dia (um domingo) da semana para o qual você orçou as horas.</p> <p>Dica:  <p>Se uma semana se estende por dois meses, isso gera duas linhas no relatório: uma correspondente ao primeiro dia da semana (o domingo da semana que está durante o primeiro mês) e uma segunda correspondente ao primeiro dia do segundo mês (e que pode ser qualquer dia da semana).</p> <p>Por exemplo, se você fizer um orçamento de 8 horas para um usuário para a semana de 30 de junho (domingo) a 6 de julho (sábado), as duas linhas mostrarão uma Data de alocação de 30 de junho e 1º de julho.</p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Hrs Orç</td> 
   <td>Estas são as horas orçadas alocadas para o usuário no planejador de recursos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pln Hrs Orç</td> 
   <td>Estas são as Horas Orçadas alocadas para a Função de Trabalho ou para o Projeto no Planejador de Recursos.</td> 
  </tr> 
 </tbody> 
</table>
