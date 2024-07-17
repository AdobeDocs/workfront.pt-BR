---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Filtrar relatórios por períodos de tempo
description: Você pode filtrar um relatório pelo intervalo de tempo de uma data que existe em um objeto. Por exemplo, você pode filtrar um relatório de horas para um intervalo de tempo específico de quando as horas foram inseridas.
author: Nolan
feature: Reports and Dashboards
exl-id: 7dea484c-d38e-4786-85d0-f4c106cfa46f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1059'
ht-degree: 4%

---

# Filtrar relatórios por períodos de tempo

Você pode filtrar um relatório pelo intervalo de tempo de uma data que existe em um objeto. Por exemplo, você pode filtrar um relatório de horas para um intervalo de tempo específico de quando as horas foram inseridas.

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
   <td> <p>Editar acesso a relatórios, painéis, calendários</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Pré-requisitos

O relatório deve ser criado antes de você filtrar seus resultados.

Para obter mais informações sobre como criar relatórios, consulte [Criar um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Filtrar um relatório pelo período de uma data {#filter-a-report-by-the-time-frame-of-a-date}

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu principal** e em **Relatórios**.

1. Clique em **Novo relatório** e selecione o tipo de relatório desejado.\
   Por exemplo, selecione **Relatório de Horas**.

1. Selecione a guia **Filtros**.
1. Clique em **Adicionar uma Regra de Filtro** e selecione **Data de Entrada da Hora**.\
   ![](assets/qs-filtering-hour-report-by-timeframe-350x357.png)

1. No menu suspenso a seguir, selecione uma das seguintes opções:

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
      <td>Após selecionar esse modificador, especifique a data em que as horas foram informadas, para excluir essa data do seu relatório. O relatório mostra horas registradas em todas as datas, esperadas para a data especificada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Null</td> 
      <td>Selecione este modificador para exibir apenas as horas em que a Data de Entrada está ausente.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Not Null</td> 
      <td>Selecione esse modificador para exibir apenas as horas em que a Data de Entrada tem um valor.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entre</td> 
      <td>Após selecionar esse modificador, especifique um intervalo de datas em que as horas foram inseridas. O relatório mostra as horas informadas entre as datas especificadas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Menor Que</td> 
      <td>Após selecionar esse modificador, especifique uma data antes da qual as horas foram informadas. O relatório mostra as horas informadas antes da data especificada, sem incluir a data especificada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Menor Que ou Igual</td> 
      <td>Após selecionar esse modificador, especifique uma data antes da qual as horas foram informadas. O relatório mostra as horas informadas antes da data especificada, incluindo a data especificada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Maior Que</td> 
      <td>Após selecionar esse modificador, especifique uma data após a qual as horas foram informadas. O relatório mostra as horas informadas após a data especificada, sem incluir a data especificada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Maior Que ou Igual</td> 
      <td> <p>Após selecionar esse modificador, especifique uma data após a qual as horas foram informadas. O relatório mostra horas informadas após a data especificada, incluindo a data especificada.</p> <p>Selecione qualquer um dos modificadores de período predefinidos, conforme descrito em <a href="#built-in-time-frame-modifiers" class="MCXref xref">Modificadores de período predefinidos</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Esses modificadores estão disponíveis para qualquer campo de data em um filtro ou um prompt em qualquer relatório.
1. Clique em **Salvar + Fechar**.

## Modificadores de intervalo de tempo incorporados {#built-in-time-frame-modifiers}

O Adobe Workfront tem modificadores de intervalo de tempo incorporados que podem ser usados sem definir uma data específica. 

Esses modificadores estão disponíveis para qualquer campo de data em um filtro ou um prompt em qualquer relatório. 

Para obter mais informações sobre como filtrar um relatório por um período associado a uma data, consulte  [Filtrar um relatório pelo período de uma data](#filter-a-report-by-the-time-frame-of-a-date).

Por exemplo, se você estiver criando um relatório de horas e quiser exibir as horas informadas em um intervalo de tempo específico, poderá escolher entre as seguintes opções de filtro de intervalo de tempo interno:

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
   <td role="rowheader">Esta Quinzena</td> 
   <td> <p>Exibe horas em que a Data de Entrada é uma data no trimestre atual, onde os trimestres são definidos como:</p> 
    <ul> 
     <li>Primeiro trimestre: 1 de janeiro a 30 de março</li> 
     <li>Segundo trimestre: 1 de abril - 30 de junho</li> 
     <li>Terceiro trimestre: 1 de julho a 30 de setembro</li> 
     <li>Quarto trimestre: 1 de outubro a 31 de dezembro</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Próxima Quinzena</td> 
   <td>Exibe horas em que a Data de Entrada é uma data no trimestre seguinte ao trimestre atual, em que os trimestres estão definidos acima.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Última Quinzena</td> 
   <td> <p>Exibe horas em que a Data de Entrada é uma data no trimestre anterior ao trimestre atual, em que os trimestres estão definidos acima.</p> <p>Observação: se o administrador do Workfront tiver ativado e definido trimestres personalizados para seu sistema, os filtros integrados para trimestres serão substituídos pelas informações de trimestre personalizadas. Para obter mais informações sobre como habilitar trimestres personalizados, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref">Habilitar trimestres personalizados para projetos</a>.</p> </td> 
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
