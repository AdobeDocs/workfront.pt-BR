---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: "Exibição: calcular o custo de horas extras em uma Exibição de folha de horas"
description: As horas extras não são calculadas por padrão no Adobe Workfront, mas você pode criar um relatório de Planilha de horas que calcula as horas extras.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---

# Exibição: calcular o custo de horas extras em uma Exibição de folha de horas

As horas extras não são calculadas por padrão no Adobe Workfront, mas você pode criar um relatório de Planilha de horas que calcula as horas extras.

Se o usuário estiver associado a uma taxa de Custo por hora em seu perfil, você também poderá calcular a quantidade de custo para a hora extra desse usuário.\
Para obter informações sobre como associar usuários com taxas de Custo por hora, consulte o artigo [Definir minhas configurações](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

>[!NOTE]
>
>O campo Horas extras que você pode adicionar a uma visualização de Folha de horas em uma lista ou relatório exibe as informações encontradas no campo Horas extras da folha de horas. Essas informações são atualizadas manualmente por um usuário com acesso para modificar a folha de horas. Para obter mais informações sobre o campo Horas extras em uma folha de horas, consulte o artigo [Entender o layout de Planilha de Horas](../../../timesheets/timesheets/timesheet-layout.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitação para modificar uma exibição </p>
   <p>Planejar a modificação de um relatório</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar uma visualização</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Calcular custo de horas extras em uma Exibição de folha de horas

Para adicionar uma coluna de horas extras calculadas a uma visualização de folha de horas:

1. Ir para uma lista de planilhas de horas ou criar um relatório de planilha de horas.

   Para obter informações sobre como criar relatórios, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Clique em **Personalizar visualização** em uma lista de folhas de horas.

   Ou

   Selecione o **Colunas (Exibir)** em um relatório de Planilha de horas.

1. Clique em **Adicionar coluna**.
1. Clique em **Alternar para modo de texto**.
1. No **Mostrar nesta coluna** clique em **Clique para editar o texto**.
1. Copie e cole o seguinte código de modo de texto no **Modo de texto** caixa de diálogo.
   <pre>displayname=Custo de horas extras calculado<br>linkedname=direct<br>namekey=totalHours<br>querysort=totalHours <br>textmode=true<br>valueexpression=IF({totalHours}&gt;40,({totalHours}-40)*{user}.{costPerHour},{totalHours}*{user}.{costPerHour})<br>valueformat=currencyStringCurrencyRounded</pre>

   >[!NOTE]
   >
   >Esse cálculo presume que o usuário geralmente trabalha uma semana de 40 horas.

1. Clique em **Salvar**, nomeie a nova exibição e clique em **Salvar visualização** em uma lista de folhas de horas.

   Ou

   Clique em **Salvar + Fechar** em um relatório de Planilha de Horas.

1. (Opcional e condicional) se você estiver criando um relatório de Planilha de Horas, especifique um nome para o relatório e, em seguida, clique em **Salvar relatório**.

   O custo das horas extras de cada usuário é exibido na **Custo Calculado de Horas Extras** coluna.

   ![calculated_overtime_cost_in_time_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)
