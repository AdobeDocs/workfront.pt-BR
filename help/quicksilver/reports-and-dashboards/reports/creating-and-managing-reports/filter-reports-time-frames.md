---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Filtrar relatórios por períodos
description: Você pode filtrar um relatório pelo período de uma data que existe em um objeto. Por exemplo, você pode filtrar um relatório de horas para um período específico de quando as horas foram inseridas.
author: Courtney
feature: Reports and Dashboards
exl-id: 7dea484c-d38e-4786-85d0-f4c106cfa46f
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 5%

---

# Filtrar relatórios por períodos

<!-- Audited: 4/2025 -->

Você pode filtrar um relatório pelo período de uma data que existe em um objeto. Por exemplo, você pode filtrar um relatório de horas para um período específico de quando as horas foram inseridas.

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
   <td role="rowheader">Licença do Adobe Workfront</td> 
      <td> 
      <p>Novo: Padrão</p>
       <p> Ou</p>
      <p>Atual: Plano</p>
   </td>

</tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a relatórios, painéis, calendários</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

O relatório deve ser criado antes que você possa filtrar seus resultados.

Para obter mais informações sobre como criar relatórios, consulte [Criar um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Filtrar um relatório pelo período de uma data {#filter-a-report-by-the-timeframe-of-a-date}

{{step1-to-reports}}

1. No canto superior esquerdo, clique em **Novo relatório** e selecione o tipo de relatório que deseja criar.

1. Na página **Novo Relatório**, selecione a guia **Filtros**.

1. Clique em **Adicionar uma Regra de Filtro** e em **Selecionar um campo**.

1. Na caixa de diálogo **Selecionar um campo**, selecione **Hora** e depois **Data de Entrada**.
   ![Filtrar relatório de horas por período](assets/qs-filtering-hour-report-by-timeframe-350x357.png)

1. Na lista suspensa exibida, selecione uma das seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Igual</td> 
      <td>Após selecionar esse modificador, especifique a data em que as horas foram inseridas.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Não Igual</td> 
      <td>Após selecionar esse modificador, especifique a data em que as horas foram informadas para excluir essa data do seu relatório. O relatório mostra horas registradas em todas as datas, esperadas para a data especificada.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Menor que</td> 
      <td>Após selecionar esse modificador, especifique uma data antes da qual as horas foram informadas. O relatório mostra as horas informadas antes da data especificada, sem incluir a data especificada.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Menor Que ou Igual</td> 
      <td>Após selecionar esse modificador, especifique uma data antes da qual as horas foram informadas. O relatório mostra as horas informadas antes da data especificada, incluindo a data especificada.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Maior que</td> 
      <td>Após selecionar esse modificador, especifique uma data após a qual as horas foram informadas. O relatório mostra horas informadas após a data especificada, sem incluir a data especificada.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Maior Que ou Igual</td> 
      <td> Após selecionar esse modificador, especifique uma data após a qual as horas foram informadas. O relatório mostra horas informadas após a data especificada, incluindo a data especificada. </td> 
     </tr>

   <tr> 
      <td role="rowheader">Entre</td> 
      <td>Após selecionar esse modificador, especifique um intervalo de datas em que as horas foram inseridas. O relatório mostra as horas informadas entre as datas especificadas.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Nulo</td> 
      <td>Selecione este modificador para exibir apenas as horas em que a Data de Entrada está ausente.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Não nulo</td> 
      <td>Selecione esse modificador para exibir apenas as horas em que a Data de Entrada tem um valor.</td> 
     </tr>

   </tbody> 
   </table>

1. Clique em **Salvar + Fechar**.

## Modificadores de período predefinidos {#built-in-timeframe-modifiers}

O Adobe Workfront tem modificadores de período incorporados que podem ser usados sem definir uma data específica. Esses modificadores estão disponíveis para qualquer campo de data em um filtro ou um prompt em qualquer relatório.

Por exemplo, se você estiver criando um relatório de horas e quiser exibir as horas informadas em um período específico, poderá escolher entre as seguintes opções de filtro de período:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Hoje</td> 
   <td>Exibe horas em que a Data de Entrada é hoje.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Esta Semana</td> 
   <td>Exibe horas em que a Data de Entrada é uma data na semana atual, em que a semana começa em um domingo e termina em um sábado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Próxima Semana</td> 
   <td>Exibe horas em que a Data de Entrada é uma data na semana seguinte à semana atual, em que a semana começa em um domingo e termina em um sábado. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Semana passada</td> 
   <td>Exibe horas em que a Data de Entrada é uma data na semana anterior à semana atual, em que a semana começa em um domingo e termina em um sábado. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Este Mês</td> 
   <td>Exibe horas em que a Data de Entrada é uma data do mês atual.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Próximo Mês</td> 
   <td>Exibe horas em que a Data de Entrada é uma data no mês seguinte ao mês atual.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Último mês</td> 
   <td>Exibe horas em que a Data de Entrada é uma data no mês anterior ao mês atual</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Este trimestre</td> 
   <td> <p>Exibe horas em que a Data de Entrada é uma data no trimestre atual, onde os trimestres são definidos como:</p> 
    <ul> 
     <li>Primeiro trimestre: 1 de janeiro a 30 de março</li> 
     <li>Segundo trimestre: 1 de abril - 30 de junho</li> 
     <li>Terceiro trimestre: 1 de julho a 30 de setembro</li> 
     <li>Quarto trimestre: 1 de outubro a 31 de dezembro</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Próximo trimestre</td> 
   <td>Exibe horas em que a Data de Entrada é uma data no trimestre seguinte ao trimestre atual, em que os trimestres estão definidos acima.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Último trimestre</td> 
   <td> <p>Exibe horas em que a Data de Entrada é uma data no trimestre anterior ao trimestre atual, em que os trimestres estão definidos acima.</p> <p>Observação: se o administrador do Workfront tiver ativado e definido trimestres personalizados para seu sistema, os filtros integrados para trimestres serão substituídos pelas informações de trimestre personalizadas. Para obter mais informações sobre como habilitar trimestres personalizados, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref">Habilitar trimestres personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Este ano</td> 
   <td>Exibe horas em que a Data de Entrada é uma data no ano atual, em que o ano atual começa em 1º de janeiro e termina em 31 de dezembro.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">No último ano</td> 
   <td>Exibe horas em que a Data de Entrada é uma data no ano passado, em que o ano passado começa 12 meses antes da data atual.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ano passado</td> 
   <td> <p>Exibe horas em que a Data de Entrada é uma data no último ano, em que o último ano começa em 1º de janeiro e termina em 31 de dezembro do ano anterior ao ano atual.</p> <p>Nota: Não há período de tempo incorporado para o ano fiscal. Você pode criar um relatório e filtrar as informações por data usando um modificador personalizado para o intervalo de datas do ano fiscal, conforme definido em sua organização. Se você quiser escolher um período para um ano fiscal no local, deverá usar um prompt em vez de um filtro. </p> </td> 
  </tr> 
 </tbody> 
</table>
