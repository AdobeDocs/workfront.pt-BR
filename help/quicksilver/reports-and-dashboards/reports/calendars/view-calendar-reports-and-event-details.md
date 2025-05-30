---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Exibir Relatórios de Calendário e Detalhes do Evento
description: Você pode exibir relatórios de calendário e detalhes de eventos que você criou ou que foram compartilhados com você no Adobe Workfront.
author: Lisa
feature: Reports and Dashboards
exl-id: db016e91-43e4-400c-ac9d-1639c7f94479
source-git-commit: a411c1ddf0c6d19dc7f6e181cceeebba5504530c
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 0%

---

# Exibir relatórios de calendário e detalhes do evento

Você pode exibir relatórios de calendário e detalhes de eventos que você criou ou que foram compartilhados com você no Adobe Workfront.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront plan]</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td><p>Novo: Colaborador</p>
       <p>ou</p>
       <p>Atual: solicitação</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>[!UICONTROL Exibir] ou acesso superior a [!UICONTROL Relatórios], [!UICONTROL Painéis] e [!UICONTROL Calendários]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td>[!UICONTROL Exibir] ou permissões superiores para o relatório de calendário</td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exibir um relatório de calendário

<!--{{step1-to-calendars}}-->

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **[!UICONTROL Calendários]**.

   Dependendo do seu nível de acesso, você poderá ver os seguintes calendários listados:

   * Seu calendário [!DNL Adobe Workfront] padrão

     O Workfront cria um calendário para você com base nos projetos, tarefas e problemas atribuídos a você ou atribuídos a equipes, grupos ou funções atribuídas a você.

   * Calendários criados por você

     Para saber mais sobre como criar calendários, consulte [Visão geral dos relatórios de calendário](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

   * Calendários que outros usuários compartilharam com você

     Para saber mais sobre o compartilhamento de calendários, consulte [[!UICONTROL Compartilhar um calendário] relatório](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

1. (Condicional) Clique no menu suspenso **[!UICONTROL Exibir]** e selecione a duração do calendário que deseja exibir.
   ![Duração do calendário](assets/view-menu-calendar-report-350x189.png)
Você pode escolher entre as seguintes exibições de relatório do calendário:

   * **[!UICONTROL Mês]**: exibe quatro semanas do calendário
   * **[!UICONTROL Semana]**: exibe uma semana do calendário
   * **[!UICONTROL Gantt]**: exibe uma exibição contínua do calendário

     Você pode ver mais eventos em uma visualização de **Gantt** rolando para baixo ou para os lados. Um símbolo de carregamento é exibido à medida que os dados são preenchidos para a exibição.

   >[!NOTE]
   >
   >Nos modos de exibição **Mês** e **Semana**, os eventos atuais ou futuros (incluindo eventos que abrangem vários dias, desde que contenham hoje ou um dia futuro) têm sombreamento que corresponde à cor no agrupamento de projeto ou calendário. Os eventos anteriores têm um sombreamento mais claro para indicar que não são mais atuais, mas ainda é possível selecionar e visualizar esses eventos.

1. (Opcional) Se você estiver exibindo o calendário nos modos de exibição **Mês** ou **Semana**, poderá alterar o modo de exibição do calendário com as seguintes opções:

   <!--   * To include or exclude weekends:
      1. On the **[!UICONTROL Calendar]** toolbar, click **[!UICONTROL Calendar Actions]**, then from the drop-down list select either **[!UICONTROL Show Weekend]** or **[!UICONTROL Hide Weekend]**.-->

   * Para alterar rapidamente as datas exibidas:

      1. Na barra de ferramentas **[!UICONTROL Calendário]**, clique na seta para a esquerda do indicador de data para voltar no calendário ou na seta para a direita para avançar.

         ![Clique na seta para alterar a data](assets/click-arrows-to-change-dates-calendar-report.png)

         As datas exibidas são ajustadas por um intervalo com base na exibição do calendário atual. Por exemplo, se você estiver exibindo o calendário na exibição **Semana**, o calendário será exibido uma semana depois ou uma semana atrás, dependendo da seta selecionada.

      1. (Opcional) Para voltar ao dia atual, clique em [!UICONTROL **Hoje**].

1. (Opcional) Para ocultar os eventos de um projeto ou agrupamento de calendário vinculado ao calendário, desmarque o projeto ou agrupamento de calendário na lista de projetos.
   ![Ocultar eventos](assets/hide-events-for-project-or-cal-grouping.png)
Você pode tornar os eventos visíveis novamente selecionando o [!UICONTROL projeto] ou o agrupamento de calendário na lista de projetos.

## Exibir detalhes do evento de relatório do calendário

Você pode ver os detalhes de um evento em um calendário, para eventos atuais e passados.

1. Vá para o evento cujos detalhes você deseja saber e clique nele. Os detalhes são abertos em um painel no lado direito.
1. (Opcional) Para abrir o projeto, tarefa ou problema associado, clique no título do objeto.
