---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Executar um relatório
description: Você pode executar qualquer relatório ao qual tenha acesso para Exibir.
author: Courtney
feature: Reports and Dashboards
exl-id: bd2202a7-040c-4291-ad02-ba8929a37e2b
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 10%

---


# Executar um relatório

Você pode executar qualquer relatório ao qual tenha acesso para Exibir.

<!-- Audited: 11/2024 -->

<!--
NOTE: ***Linked to Getting Started with Reporting.***This information is obsolete, because asynchronous timeline is not enabled for all customers (used to be included in the "Viewing a Cached Report" section): Some reports in Workfront can take a significant time to load. If your report takes longer than 30 seconds to load, your report is cached after it is finished loading, and a message is displayed in the upper-right corner of the page indicating that the report being viewed is a saved report from a specific time.

After a report is cached, it is available for the next 12 hours. Any user who runs the report (as described in "Running a Report") sees the cached report.)
-->

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
      <p>Padrão</p>
      <p>Plano</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Exibir acesso a relatórios, painéis e calendários</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
     <td> <p>Exibir permissões para um relatório</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Executar um relatório

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **[!UICONTROL Relatórios]**.

1. Selecione uma das seguintes opções:

   * **Meus Relatórios:** Relatórios que você criou.
   * **Compartilhado comigo:** relata que outros usuários compartilharam com você.
   * **Todos os relatórios:** todos os relatórios no sistema aos quais você tem acesso.

1. Clique no nome do relatório que deseja executar.\
   Ou\
   Se o relatório foi criado usando prompts, selecione as informações apropriadas nos menus suspensos e clique em **Executar Relatório**.\
   Para obter mais informações sobre prompts, consulte [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).\
   O conteúdo do relatório é exibido com um carimbo de data/hora no canto superior direito do relatório, que inclui a data, a hora e o fuso horário em que o relatório foi executado no contexto do usuário que executou o relatório.

1. (Opcional) Clique no **ícone Recarregar** ![ícone Recarregar](assets/unshimmed-report-refresh-icon.png) para atualizar os resultados em um relatório se o relatório tiver sido exibido no navegador por algum tempo.

1. (Condicional) Se o relatório usar filtros ou prompts, clique em **Mostrar Filtros e Prompts** para exibir uma lista de filtros e prompts que estão sendo usados no relatório que você está exibindo. Se o relatório contiver apenas filtros ou apenas prompts, **Mostrar Filtros** ou **Mostrar Prompts** serão exibidos.

   ![Mostrar filtros e prompts](assets/unshimmed-show-filters-and-prompts.png)

   As informações são exibidas abaixo do nome do relatório no lado esquerdo da página. Para prompts, essas são informações sobre as seleções de prompts feitas no momento em que o relatório foi executado, conforme descrito na Etapa 3.

1. Se você estiver usando Prompts Personalizados, eles não serão exibidos. Somente os prompts do sistema serão exibidos. Os filtros personalizados sempre são exibidos.

## Exibir um relatório armazenado em cache

Seu relatório pode ser armazenado em cache se tiver sido exibido no navegador por algum tempo. Você pode forçar o recarregamento de um relatório armazenado em cache ao executar qualquer uma das seguintes ações:

* Edite as configurações de relatório e salve o relatório.
* Altere o Modo de Exibição, Grupo ou Filtro.
* Clique no **ícone Recarregar** ![ícone Recarregar](assets/unshimmed-report-refresh-icon.png)
Essa opção está disponível no canto superior direito da página na caixa de mensagem que indica a hora em que o relatório foi salvo ou está disponível no canto superior direito do painel no qual o relatório é colocado. Para obter mais informações sobre como recarregar painéis, consulte a seção “Exibir painéis” no artigo [Introdução aos painéis](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

* Acesse qualquer página do relatório além da primeira página navegando até as guias Resumo, Matriz ou Gráfico.
