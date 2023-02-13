---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Filtrar relatórios por intervalos de tempo
description: Você pode filtrar um relatório pelo período de uma data existente em um objeto. Por exemplo, você pode filtrar um relatório de hora para um período específico de quando as horas foram inseridas.
author: Nolan
feature: Reports and Dashboards
exl-id: 7dea484c-d38e-4786-85d0-f4c106cfa46f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1046'
ht-degree: 4%

---

# Filtrar relatórios por intervalos de tempo

Você pode filtrar um relatório pelo período de uma data existente em um objeto. Por exemplo, você pode filtrar um relatório de hora para um período específico de quando as horas foram inseridas.

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

## Pré-requisitos

O relatório deve ser criado antes que você filtre seus resultados.

Para obter mais informações sobre como criar relatórios, consulte [Criar um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Filtrar um relatório por período de uma data {#filter-a-report-by-the-time-frame-of-a-date}

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png), depois clique em **Relatório**.

1. Clique em **Novo relatório** e selecione o tipo de relatório desejado.\
   Por exemplo, selecione **Relatório de hora**.

1. Selecione o **Filtros** guia .
1. Clique em **Adicionar uma regra de filtro**, em seguida selecione **Data de entrada de hora**.\
   ![](assets/qs-filtering-hour-report-by-timeframe-350x357.png)

1. No menu suspenso a seguir, selecione qualquer uma das seguintes opções:

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
      <td>Após selecionar esse modificador, especifique a data em que as horas foram inseridas, para excluir essa data do relatório. O relatório mostra as horas registradas em todas as datas, as esperadas para a data especificada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Null</td> 
      <td>Selecione este modificador para exibir apenas horas em que a Data de Entrada está ausente.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Not Null</td> 
      <td>Selecione esse modificador para exibir somente horas em que a Data de entrada tenha um valor.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entre</td> 
      <td>Após selecionar esse modificador, especifique um intervalo de datas quando as horas foram inseridas. O relatório mostra horas inseridas entre as datas especificadas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Menor Que</td> 
      <td>Após selecionar esse modificador, especifique uma data antes da qual as horas foram inseridas. O relatório mostra horas inseridas antes da data especificada, sem incluir a data especificada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Menor Que ou Igual</td> 
      <td>Após selecionar esse modificador, especifique uma data antes da qual as horas foram inseridas. O relatório mostra as horas inseridas antes da data especificada, incluindo a data especificada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Maior Que</td> 
      <td>Após selecionar esse modificador, especifique uma data após a qual as horas foram inseridas. O relatório mostra horas inseridas após a data especificada, sem incluir a data especificada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Maior Que ou Igual</td> 
      <td> <p>Após selecionar esse modificador, especifique uma data após a qual as horas foram inseridas. O relatório mostra as horas inseridas após a data especificada, incluindo a data especificada.</p> <p>Selecione qualquer um dos modificadores de período de tempo incorporados, conforme descrito em <a href="#built-in-time-frame-modifiers" class="MCXref xref">Modificadores de período de tempo incorporados</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Esses modificadores estão disponíveis para qualquer campo de data em um filtro ou prompt em qualquer relatório.
1. Clique em **Salvar + Fechar**.

## Modificadores de período de tempo incorporados {#built-in-time-frame-modifiers}

A Adobe Workfront tem modificadores de período de tempo integrados que podem ser usados sem definir uma data específica. 

Esses modificadores estão disponíveis para qualquer campo de data em um filtro ou prompt em qualquer relatório. 

Para obter mais informações sobre como filtrar um relatório por período associado a uma data, consulte  [Filtrar um relatório por período de uma data](#filter-a-report-by-the-time-frame-of-a-date).

Por exemplo, se você estiver criando um relatório de hora e quiser exibir horas inseridas em um intervalo de tempo específico, é possível escolher entre as seguintes opções de filtro de intervalo de tempo integradas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Hoje</td> 
   <td>Exibe horas, onde a Data de entrada é hoje.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Esta Semana</td> 
   <td>Exibe horas, onde a Data de entrada é uma data na semana atual, onde a semana começa em um domingo e termina em um sábado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Próxima Semana</td> 
   <td>Exibe horas, onde a Data de entrada é uma data na semana seguinte à semana atual, onde a semana começa em um domingo e termina em um sábado. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Semana passada</td> 
   <td>Exibe horas em que a Data de entrada é uma data na semana anterior à semana atual, em que a semana começa em um domingo e termina em um sábado. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Este Mês</td> 
   <td>Exibe horas em que a Data de entrada é uma data no mês atual.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Próximo Mês</td> 
   <td>Exibe horas em que a Data de entrada é uma data no mês seguinte ao mês atual.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Último mês</td> 
   <td>Exibe horas em que a Data de entrada é uma data no mês anterior ao mês atual</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Esta Quinzena</td> 
   <td> <p>Exibe horas em que a Data de Entrada é uma data no trimestre atual, em que os trimestres são definidos como:</p> 
    <ul> 
     <li>Primeiro trimestre: 1 de janeiro a 30 de março</li> 
     <li>Segundo trimestre: 1 de abril a 30 de junho</li> 
     <li>Terceiro trimestre: 1° de julho a 30 de setembro</li> 
     <li>Quarto trimestre: 1° de outubro a 31 de dezembro</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Próxima Quinzena</td> 
   <td>Exibe horas em que a Data de entrada é uma data no trimestre seguinte ao trimestre atual, em que os trimestres são definidos acima.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Última Quinzena</td> 
   <td> <p>Exibe horas em que a Data de entrada é uma data no trimestre anterior ao trimestre atual, em que os trimestres são definidos acima.</p> <p>Observação: Se o administrador do Workfront ativou e definiu trimestres personalizados para seu sistema, os filtros incorporados para trimestres serão substituídos pelas informações personalizadas do trimestre. Para obter mais informações sobre como ativar trimestres personalizados, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref">Habilitar trimestres personalizados para projetos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Este ano</td> 
   <td>Exibe horas em que a Data de entrada é uma data no ano atual, em que o ano atual começa em 1º de janeiro e termina em 31 de dezembro.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">No último ano</td> 
   <td>Exibe horas em que a Data de entrada é uma data no ano passado, em que o ano passado começa 12 meses antes da data atual.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ano passado</td> 
   <td> <p>Exibe horas em que a Data de entrada é uma data no último ano, em que o último ano começa em 1º de janeiro e termina em 31 de dezembro do ano anterior ao ano atual.</p> <p>Observação: Não há período de tempo integrado para o ano fiscal. Você pode criar um relatório e filtrar as informações por data usando um modificador personalizado para o intervalo de datas do ano fiscal, conforme definido em sua organização. Se você quiser escolher um período para um ano fiscal no local, use um prompt em vez de um filtro. </p> </td> 
  </tr> 
 </tbody> 
</table>
