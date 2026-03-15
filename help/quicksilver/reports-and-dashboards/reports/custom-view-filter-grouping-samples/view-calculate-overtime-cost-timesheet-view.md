---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: Calcular Custo de Horas Extras em uma View de Quadro de Horários'
description: As horas extras não são calculadas por padrão no Adobe Workfront, mas você pode criar um relatório Quadro de horários que calcule as horas extras.
author: Courtney
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 14%

---

# Exibir: calcular o custo das horas extras em uma exibição da folha de horas

<!--Audited: 11/2024-->

As horas extras não são calculadas por padrão no Adobe Workfront, mas você pode criar um relatório Quadro de horários que calcule as horas extras.

Se o usuário estiver associado a uma taxa de Custo por Hora em seu perfil, você também poderá calcular a quantia do custo da hora extra desse usuário.\
Para obter informações sobre como associar usuários às taxas de Custo por Hora, consulte o artigo [Configurar Minhas Configurações](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

>[!NOTE]
>
>O campo Horas Extras que você pode adicionar a um modo de exibição Quadro de Horários em uma lista ou relatório exibe as informações encontradas no campo Horas Extras do quadro de horários. Essas informações são atualizadas manualmente por um usuário com acesso para modificar o quadro de horários. Para obter mais informações sobre o campo Horas Extras em um quadro de horários, consulte o artigo [Visão geral do layout do quadro de horários](../../../timesheets/timesheets/timesheet-layout.md).

![calculated_overtime_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Colaborador ou solicitação para modificar um filtro </p>
   <p>Padrão ou Plano para modificar um relatório</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso de edição a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a filtros, exibições e agrupamentos para modificar um filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Calcular custo de horas extras em uma Exibição de Quadro de Horários

Para adicionar uma coluna de Hora Extra calculada a uma view de quadro de horários:

1. Ir para uma lista de quadros de horários.

1. Clique no menu suspenso **Exibição** e clique em **Nova Exibição**.

1. Clique em **Adicionar coluna**.
1. Clique em **Alternar para o Modo de Texto** e clique em **Editar Modo de Texto**.
1. Na caixa **Editar Modo de Texto**, remova o texto da caixa e copie e cole o seguinte código de modo de texto:

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
   >Esse cálculo pressupõe que o usuário normalmente trabalha 40 horas por semana.

1. Clique em **Concluído**, nomeie o novo modo de exibição e clique em **Salvar Modo de Exibição** em uma lista de quadros de horários.

   O custo das horas extras de cada usuário é exibido na coluna **Custo Calculado de Horas Extras**.


