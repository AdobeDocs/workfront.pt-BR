---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Executar um relatório
description: Você pode executar qualquer relatório que tenha acesso à Exibição.
author: Nolan
feature: Reports and Dashboards
exl-id: bd2202a7-040c-4291-ad02-ba8929a37e2b
source-git-commit: 12e8bc389c42510b5adbb0190eb71c9f6a9f52a7
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 0%

---


# Executar um relatório

Você pode executar qualquer relatório que tenha acesso à Exibição.

<!-- Audited: 11/2024 -->

<!--
NOTE: ***Linked to Getting Started with Reporting.***This information is obsolete, because asynchronous timeline is not enabled for all customers (used to be included in the "Viewing a Cached Report" section): Some reports in Workfront can take a significant time to load. If your report takes longer than 30 seconds to load, your report is cached after it is finished loading, and a message is displayed in the upper-right corner of the page indicating that the report being viewed is a saved report from a specific time.

After a report is cached, it is available for the next 12 hours. Any user who runs the report (as described in "Running a Report") sees the cached report.)
-->

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
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
      <td> 
      <p>Novo:</p>
         <ul>
         <li><p>Padrão</p></li>
         </ul>
      <p>Atual:</p>
         <ul>
         <li><p>Plano</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Visualizar acesso a relatórios, painéis, calendários</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões para um relatório</p></td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Executar um relatório

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **[!UICONTROL Relatórios]**.

1. Selecione entre as seguintes opções:

   * **Meus Relatórios:** Relatórios que você criou.
   * **Compartilhado Comigo:** Relatórios que outros usuários compartilharam com você.
   * **Todos os relatórios**: todos os relatórios no sistema aos quais você tem acesso.

1. Clique no nome do relatório que deseja executar.\
   Ou\
   Se o relatório foi criado usando prompts, selecione as informações apropriadas nos menus suspensos e clique em **Executar Relatório**.\
   Para obter mais informações sobre prompts, consulte [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).\
   O conteúdo do relatório é exibido com um carimbo de data e hora no canto superior direito do relatório, que inclui a data, a hora e o fuso horário em que o relatório foi executado no contexto do usuário que o executou.

1. (Opcional) Clique no **ícone Recarregar** ![ícone Recarregar](assets/unshimmed-report-refresh-icon.png) para atualizar os resultados em um relatório se ele tiver sido exibido no seu navegador por algum tempo.

1. (Condicional) Se o relatório usar filtros ou prompts, clique em **Mostrar Filtros e Prompts** para exibir uma lista de filtros e prompts que estão sendo usados no relatório que você está visualizando. Se o relatório contiver apenas filtros ou somente prompts, **Mostrar Filtros** ou **Mostrar Prompts** será exibido.

   ![Mostrar filtros e prompts](assets/unshimmed-show-filters-and-prompts.png)

   As informações são exibidas abaixo do nome do relatório no lado esquerdo da página. Para prompts, essas são informações sobre as seleções de prompt feitas no momento em que o relatório foi executado, conforme descrito na Etapa 3.

1. Se estiver usando Prompts personalizados, eles não serão exibidos. Somente os prompts do sistema são exibidos. Os Filtros personalizados sempre são exibidos.

## Exibir um relatório em cache

O relatório poderá ser armazenado em cache se for exibido no navegador por algum tempo. É possível forçar o recarregamento de um relatório em cache ao executar uma das seguintes ações:

* Edite as configurações do relatório e salve o relatório.
* Altere a Exibição, Grupo ou Filtro.
* Clique no **ícone Recarregar** ![ícone Recarregar](assets/unshimmed-report-refresh-icon.png)
Essa opção está disponível no canto superior direito da página na caixa de mensagem que indica a hora em que o relatório foi salvo ou está disponível no canto superior direito do painel no qual o relatório é colocado. Para obter mais informações sobre como recarregar painéis, consulte a seção &quot;Exibir Painéis&quot; no artigo [Introdução aos painéis](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

* Acesse qualquer página do relatório além da primeira página navegando até as guias Resumo, Matriz ou Gráfico.
