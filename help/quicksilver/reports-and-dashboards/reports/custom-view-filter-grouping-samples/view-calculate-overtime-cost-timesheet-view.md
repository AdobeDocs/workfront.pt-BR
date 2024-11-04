---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualização: Calcular custo de horas extras em uma visualização de folha de horas"
description: As horas extras não são calculadas por padrão no Adobe Workfront, mas você pode criar um relatório de Planilha de horas que calcula as horas extras.
author: Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: ecce7484423419823effa2cb41da892ba3fb207c
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 0%

---

# Exibição: calcular o custo de horas extras em uma Exibição de folha de horas

<!--Audited: 11/2024-->

As horas extras não são calculadas por padrão no Adobe Workfront, mas você pode criar um relatório de Planilha de horas que calcula as horas extras.

Se o usuário estiver associado a uma taxa de Custo por hora em seu perfil, você também poderá calcular a quantidade de custo para a hora extra desse usuário.\
Para obter informações sobre como associar usuários com taxas de Custo por hora, consulte o artigo [Definir minhas configurações](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

>[!NOTE]
>
>O campo Horas extras que você pode adicionar a uma visualização de Folha de horas em uma lista ou relatório exibe as informações encontradas no campo Horas extras da folha de horas. Essas informações são atualizadas manualmente por um usuário com acesso para modificar a folha de horas. Para obter mais informações sobre o campo Horas extras em uma folha de horas, consulte o artigo [Visão geral do layout da folha de horas](../../../timesheets/timesheets/timesheet-layout.md).

![calculated_overtime_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)

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

## Calcular custo de horas extras em uma Exibição de folha de horas

Para adicionar uma coluna de horas extras calculadas a uma visualização de folha de horas:

1. Ir para uma lista de planilhas de horas.

1. Clique no menu suspenso **Exibir** e em **Nova Exibição**.

1. Clique em **Adicionar coluna**.
1. Clique em **Alternar para Modo de Texto** e em **Editar Modo de Texto**.
1. Na caixa **Editar Modo de Texto**, remova o texto da caixa e, em seguida, copie e cole o seguinte código de modo de texto:

   ```
   displayname=Calculated Overtime Cost
   linkedname=direct
   namekey=totalHours
   querysort=totalHours 
   textmode=true
   valueexpression=IF({totalHours}>40,({totalHours}-40)*{user}.{costPerHour},{totalHours}*{user}.{costPerHour})
   valueformat=currencyStringCurrencyRounded
   ```

   >[!NOTE]
   >
   >Esse cálculo presume que o usuário geralmente trabalha uma semana de 40 horas.

1. Clique em **Concluído**, nomeie o novo modo de exibição e clique em **Salvar Modo de Exibição** em uma lista de planilhas de horas.

   O custo das horas extras de cada usuário é exibido na coluna **Custo Calculado de Horas Extras**.


