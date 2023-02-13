---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Exibir: calcular custo de horas extras em uma Exibição da Folha de Horas'''
description: As horas extras não são calculadas por padrão no Adobe Workfront, mas você pode criar um relatório de Folha de Horas que calcula as horas extras.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Exibir: calcular o custo de horas extras em uma Exibição da Folha de Horas

As horas extras não são calculadas por padrão no Adobe Workfront, mas você pode criar um relatório de Folha de Horas que calcula as horas extras.

Se o usuário estiver associado a uma taxa de Custo por hora em seu perfil, você também poderá calcular a quantidade de custo para as horas extras desse usuário.\
Para obter informações sobre como associar usuários com as taxas de Custo por Hora, consulte o artigo [Definir minhas configurações](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

>[!NOTE]
>
>O campo Hora extra que pode ser adicionado a uma exibição Folha de horas em uma lista ou relatório exibe as informações encontradas no campo Hora extra da folha de horas. Essas informações são atualizadas manualmente por um usuário com acesso para modificar a folha de ponto. Para obter mais informações sobre o campo Hora extra em uma folha de ponto, consulte o artigo [Noções básicas sobre o layout da folha de horas](../../../timesheets/timesheets/timesheet-layout.md).

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

## Calcular o custo de horas extras em uma Exibição de Folha de Horas

Para adicionar uma coluna Hora extra calculada a uma exibição de folha de ponto:

1. Vá para uma lista de folhas de ponto ou crie um Relatório de folha de ponto.

   Para obter informações sobre como criar relatórios, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Clique em **Personalizar exibição** em uma lista de folhas de horas.

   Ou

   Selecione o **Colunas (Exibir)** em um relatório de Folha de Horas.

1. Clique em **Adicionar coluna**.
1. Clique em **Alternar para o modo de texto**.
1. No **Mostrar nesta coluna** , clique em **Clique para editar texto**.
1. Copie e cole o seguinte código do modo de texto no **Modo de texto** caixa de diálogo.
   <pre>displayname=Custo Calculado de Hora excedente<br>linkedname=direct<br>namekey=totalHours<br>querysort=totalHours <br>textmode=true<br>valueexpression=IF({totalHours}&gt;40,({totalHours}-40)*{user}.{costPerHour},{totalHours}*{user}.{costPerHour})<br>valueformat=currencyStringCurrencyRounding</pre>

   >[!NOTE]
   >
   >Esse cálculo assume que o usuário geralmente funciona em uma semana de 40 horas.

1. Clique em **Salvar**, nomeie a nova visualização e clique em **Salvar exibição** em uma lista de folhas de horas.

   Ou

   Clique em **Salvar + Fechar** em um relatório de Folha de Horas.

1. (Opcional e condicional) se você estiver criando um relatório de Folha de Horas, especifique um nome para o relatório e clique em **Salvar relatório**.

   O custo das horas extras de cada usuário é exibido na variável **Custo Calculado de Horas Extraordinárias** coluna.

   ![calculated_overtime_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)
