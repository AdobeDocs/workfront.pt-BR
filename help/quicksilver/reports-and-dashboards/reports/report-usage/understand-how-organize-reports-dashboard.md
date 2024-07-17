---
content-type: overview
product-area: reporting;dashboards
navigation-topic: report-usage
title: Entender como organizar relatórios em um painel
description: Você pode ver se um relatório é adicionado a um painel no Adobe Workfront. Isso pode ser útil ao decidir quais relatórios você pode manter e quais podem ser excluídos do sistema. Se os relatórios estiverem nos painéis, os usuários ainda poderão depender deles. Recomendamos não excluir relatórios listados nos painéis que os usuários estão usando. Para obter mais informações sobre como adicionar relatórios a painéis, consulte o artigo Adicionar um relatório a um painel.
author: Nolan
feature: Reports and Dashboards
exl-id: ce00c307-9e64-49f5-997b-f7fc461c960c
source-git-commit: d738ef3f6642d5b1a646f58896575a2971bbc06a
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 1%

---

# Entender como organizar relatórios em um painel

## Acessar informações do painel em uma lista de relatórios

Você pode ver se um relatório é adicionado a um painel no Adobe Workfront. Isso pode ser útil ao decidir quais relatórios você pode manter e quais podem ser excluídos do sistema. Se os relatórios estiverem nos painéis, os usuários ainda poderão depender deles. Recomendamos não excluir relatórios listados nos painéis que os usuários estão usando.\
Para obter mais informações sobre como adicionar relatórios a painéis, consulte o artigo [Adicionar um relatório a um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

Você pode ver se um relatório é adicionado a um painel seguindo um destes procedimentos:

* Criação de uma exibição para uma lista de relatórios e inclusão de informações do painel nas colunas
* Filtrar uma lista de relatórios por um ou vários painéis específicos que você sabe que estão sendo usados ativamente
* Criar um relatório para o objeto de relatório e usar uma visualização ou um filtro que inclua informações do painel

Qualquer pessoa pode criar uma visualização ou um filtro, mas você deve ter acesso para Editar relatórios no seu nível de acesso para criar um relatório.\
Para obter mais informações sobre o acesso a relatórios, consulte o artigo [Conceder acesso a relatórios, painéis e calendários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).\
Para obter mais informações sobre a criação de um relatório, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

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

## Exibir informações do painel na Exibição de uma lista de relatórios

>[!WARNING]
>
>A inclusão da coluna Painéis em uma lista de relatórios pode aumentar significativamente os tempos de carregamento, especialmente em listas de relatórios longas.

Para criar uma view com informações do painel para uma lista de relatórios:

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu principal** no canto superior direito do Workfront e em **Relatórios**.
1. Na lista de relatórios, clique no menu suspenso **Exibir**.
1. Clique em **Nova Exibição**.
1. Clique em **Adicionar coluna**.
1. Comece a digitar &quot;Painéis&quot; no campo **Comece a digitar o nome do campo**.
1. No objeto **Relatório**, selecione **Painéis**.

1. Clique em **Salvar visualização**.\
   Os painéis nos quais um relatório é exibido são exibidos na coluna Dashboards da lista de relatórios.\
   ![](assets/qs-dashboards-in-report-view.png)

## Filtrar uma lista de relatórios por informações do painel

Para filtrar uma lista de relatórios por informações do painel:

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu principal** no canto superior direito do Workfront e em **Relatórios**.

1. Na lista de relatórios, clique no menu suspenso **Filtro**.
1. Clique em **Novo filtro** e em **Adicionar uma regra de filtro**.

1. Comece a digitar &quot;Painéis&quot; no campo **Comece a digitar o nome do campo**.

1. No objeto **Painéis**, selecione **Nome**.

1. Selecione **Igual** no menu suspenso do modificador e comece a digitar o nome do painel pelo qual você deseja filtrar. Você pode selecionar vários painéis para o filtro.\
   ![](assets/qs-dashboards-in-report-filters-350x143.png)

1. Clique em **Salvar + Fechar**.\
   Isso exibe uma lista de relatórios que estão listados somente nos painéis especificados.\
   Você também pode criar um relatório para o objeto de relatório e usar esse filtro no relatório.
