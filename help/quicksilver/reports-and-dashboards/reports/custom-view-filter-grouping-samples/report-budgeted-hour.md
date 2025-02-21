---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Relatório: Hora orçada'
description: 'Relatório: Hora orçada'
author: Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 1%

---

# Relatório: Hora orçada

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resource Management and it is super important.) </p>
-->

Quando você deseja compartilhar informações de Hora orçada com outros usuários que não têm acesso ao Planejador de recursos, é possível fazê-lo criando um relatório de Hora orçada. Você pode compartilhar o relatório com eles.

>[!IMPORTANT]
>
>As horas orçadas são normalmente atualizadas a cada hora (raramente, pode levar no máximo três horas) no banco de dados do Adobe Workfront. Atualizar o relatório não atualiza necessariamente as informações de hora contidas. Você pode visualizar o tempo decorrido desde a última atualização no canto superior direito de cada relatório de Horas orçadas. Atualizar o relatório atualiza as informações nele apenas quando houver mais de uma hora desde a última atualização.
>
>![Aviso de sincronização de tempo do relatório de horas orçado](assets/budgeted-hour-report-time-sync-warning-350x74.png)

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> 
    <p>Novo:</p>
   <ul><li><p>Colaborador para modificar um filtro </p></li>
   <li><p>Padrão para modificar um relatório</p></li> </ul>

<p>Atual:</p>
   <ul><li><p>Solicitação para modificar um filtro </p></li>
   <li><p>Planejar a modificação de um relatório</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar um filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar um relatório de horas orçadas

1. Clique no ícone **Menu Principal** ![Ícone do Menu Principal](assets/main-menu-icon.png) no canto superior direito ou no ícone **Menu Principal** ![Linhas do Menu Principal](assets/lines-main-menu.png) no canto superior esquerdo, se disponível, em seguida em **Relatórios**.

1. Clique em **Novo Relatório** > **Mais** > **Hora Orçada**.

   A visualização padrão é aplicada ao relatório.

1. (Opcional) Para facilitar a leitura do relatório, clique no botão **. Horas** coluna, depois **Alternar para Modo de Texto** e clicar em **Editar Modo de Texto**.
1. Altere a linha `valuefield` para `valueexpreesion` e insira a expressão de arredondamento.

   Isso arredonda o número de Horas orçadas para um número de decimais que você especificar.

   Para obter informações sobre como arredondar um número no Workfront, consulte o artigo [Visão geral das expressões de dados calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. Clique em **Concluído**.
1. (Opcional) Clique em **Adicionar coluna** para adicionar outras colunas.
1. (Opcional) Para facilitar a leitura do relatório, recomendamos adicionar um agrupamento a ele. Sugerimos o seguinte agrupamento:

   Clique na guia **Agrupamentos** e siga um ou vários destes procedimentos:

   * Clique em **Adicionar agrupamento**, comece a digitar &quot;Nome do projeto&quot; e depois selecione-o quando ele aparecer na lista.
   * Clique em **Adicionar agrupamento**, comece a digitar &quot;Nome da Função&quot; e depois selecione-o quando ele aparecer na lista.
   * Clique em **Adicionar agrupamento** e comece a digitar &quot;Data de Alocação&quot;, selecione-a quando ela aparecer na lista e, em seguida, selecione o período pelo qual deseja agrupar a partir do campo **Agrupar Datas por**.

1. (Opcional) Clique em **Filtros** para adicionar filtros ao relatório.
1. (Opcional) Clique em **Gráfico** para adicionar um gráfico ao relatório.
1. Clique em **Salvar + Fechar**.

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
