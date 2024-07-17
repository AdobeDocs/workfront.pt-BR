---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Executar um relatório
description: Você pode executar qualquer relatório que tenha acesso à Exibição.
author: Nolan
feature: Reports and Dashboards
exl-id: bd2202a7-040c-4291-ad02-ba8929a37e2b
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---


# Executar um relatório

Você pode executar qualquer relatório que tenha acesso à Exibição.

<!--
NOTE: ***Linked to Getting Started with Reporting.***This information is obsolete, because asynchronous timeline is not enabled for all customers (used to be included in the "Viewing a Cached Report" section): Some reports in Workfront can take a significant time to load. If your report takes longer than 30 seconds to load, your report is cached after it is finished loading, and a message is displayed in the upper-right corner of the page indicating that the report being viewed is a saved report from a specific time.

After a report is cached, it is available for the next 12 hours. Any user who runs the report (as described in "Running a Report") sees the cached report.)
-->

## Requisitos de acesso

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
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Visualizar acesso a relatórios, painéis, calendários</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Executar um relatório

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu principal** no canto superior direito do Adobe Workfront e em **Relatórios**.

1. Selecione entre as seguintes opções:

   * **Meus Relatórios:** Relatórios que você criou.
   * **Compartilhado Comigo:** Relatórios que outros usuários compartilharam com você.
   * **Todos os relatórios**: todos os relatórios no sistema aos quais você tem acesso.

1. Clique no nome do relatório que deseja executar.\
   Ou\
   Se o relatório foi criado usando prompts, selecione as informações apropriadas nos menus suspensos e clique em **Executar Relatório**.\
   Para obter mais informações sobre prompts, consulte [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).\
   O conteúdo do relatório é exibido com um carimbo de data e hora no canto superior direito do relatório, que inclui a data, a hora e o fuso horário em que o relatório foi executado no contexto do usuário que o executou.

1. (Opcional) Clique no **ícone Recarregar** ![](assets/qs-report-refresh-icon.png) para atualizar os resultados em um relatório se ele tiver sido exibido no seu navegador por algum tempo.

1. (Condicional) Se o relatório usar filtros ou prompts, clique em **Mostrar Filtros e Prompts** para exibir uma lista de filtros e prompts que estão sendo usados no relatório que você está visualizando. Se o relatório contiver apenas filtros ou somente prompts, **Mostrar Filtros** ou **Mostrar Prompts** será exibido.

   ![Mostrar filtros e prompts](assets/qs-reports-showfiltersandprompts-2022-350x136.png)

   As informações são exibidas abaixo do nome do relatório no lado esquerdo da página. Para prompts, essas são informações sobre as seleções de prompt feitas no momento em que o relatório foi executado, conforme descrito na Etapa 4.

1. Se estiver usando Prompts personalizados, eles não serão exibidos. Somente os prompts do sistema são exibidos. Os Filtros personalizados sempre são exibidos.

## Exibir um relatório em cache

O relatório poderá ser armazenado em cache se for exibido no navegador por algum tempo. É possível forçar o recarregamento de um relatório em cache ao executar uma das seguintes ações:

* Edite as configurações do relatório e salve o relatório.
* Altere a Exibição, Grupo ou Filtro.
* Clique no **ícone Recarregar**
Essa opção está disponível no canto superior direito da página na caixa de mensagem que indica a hora em que o relatório foi salvo ou está disponível no canto superior direito do painel no qual o relatório é colocado. Para obter mais informações sobre como recarregar painéis, consulte a seção &quot;Exibir Painéis&quot; no artigo [Introdução aos painéis](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

* Acesse qualquer página do relatório além da primeira página navegando até as guias Resumo, Matriz ou Gráfico.
