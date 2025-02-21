---
product-area: reporting
navigation-topic: report-usage
title: Visualizar uso do relatório
description: Visualizar uso do relatório
author: Nolan
feature: Reports and Dashboards
exl-id: 51d9067c-8c55-433e-b560-7da241ef33ae
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1011'
ht-degree: 1%

---

# Visualizar uso do relatório

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : *** DO NOT CHANGE, REMOVE, CHANGE LINK, RENAME THIS ARTICLE- IT IS LINKED TO THE PENDO GUIDE FOR THE MAIN REPORTS AREA***)</p>
-->

Para entender quão extensivamente os relatórios são usados em seu sistema, você pode exibir as seguintes informações em uma lista de relatórios:

* Últimos 10 usuários que visualizaram o relatório
* Exibir contagem em um intervalo de tempo especificado

  >[!NOTE]
  >
  >O Adobe Workfront conta uma visualização por usuário por dia. Se você acessar o mesmo relatório várias vezes por dia, o Workfront o contará como uma visualização desse relatório para você. Se o mesmo relatório for acessado por outro usuário no mesmo dia, o Workfront o contará como uma nova visualização para o segundo usuário.

* Última data da visualização
* Última Visualização realizada pelo Usuário
* Uma lista de painéis que contém o relatório\
  Para obter mais informações sobre como exibir o nome dos painéis nos quais os relatórios podem ser adicionados em uma lista de relatórios, consulte o artigo [Entender como organizar relatórios em um painel](../../../reports-and-dashboards/reports/report-usage/understand-how-organize-reports-dashboard.md).

É possível criar uma visualização para uma lista de relatórios onde você pode exibir essas informações.\
Você pode filtrar uma lista de relatórios por alguns desses campos.\
Para obter mais informações sobre quais campos você pode filtrar um relatório, consulte o artigo [Filtrar uma lista de relatórios por informações de uso](#filter-a-report-list-by-usage-information).

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

## Exibir informações de uso do relatório na Exibição de uma lista de relatórios

1. Clique no ícone **Menu Principal** ![Ícone do Menu Principal](assets/main-menu-icon.png) no canto superior direito do Workfront e em **Relatórios**.

1. Na lista de relatórios, clique no menu suspenso **Exibir**.
1. (Opcional) Selecione a exibição **Uso de relatórios** para exibir as informações mais comuns sobre o uso de relatórios.\
   Ou

1. Clique em **Nova Exibição** para criar uma exibição personalizada.
1. Clique em **Adicionar coluna**.
1. Comece a digitar qualquer um dos campos a seguir e selecione-os quando eles aparecerem na lista sob o objeto **Relatório** para adicioná-los a uma nova coluna:

   * **Últimos 10 usuários**: exibe os nomes dos últimos 10 usuários que visualizaram o relatório.
   * **Exibições**: exibe o número de exibições em qualquer um dos seguintes períodos:

      * **Este Mês, Trimestre, Ano**
      * **Último mês, trimestre, ano**
      * **Todas as Exibições**: Exibe uma contagem geral de todas as exibições no relatório

   * **Última Visualização realizada por**: exibe informações sobre o usuário que visualizou o relatório por último
   * **Última Data de Visualização**: Exibe a data em que o relatório foi visualizado pela última vez

1. Clique em **Salvar visualização**.\
   As informações de uso sobre o relatório são exibidas nas colunas adicionadas à visualização.\
   Você também pode criar um relatório para o objeto de relatório e usar essa visualização no relatório.\
   Para obter mais informações sobre a criação de um relatório, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
   Você deve ter acesso para Editar aos Relatórios em seu nível de acesso para criar um relatório.\
   Para obter mais informações sobre o acesso a relatórios, consulte o artigo [Conceder acesso a relatórios, painéis e calendários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Filtrar uma lista de relatórios por informações de uso {#filter-a-report-list-by-usage-information}

1. Clique no ícone **Menu Principal** ![Ícone do Menu Principal](assets/main-menu-icon.png) no canto superior direito do Workfront e em **Relatórios**.
1. Na lista de relatórios, clique no menu suspenso **Filtro**.
1. Clique em **Novo filtro** e em **Adicionar uma regra de filtro**.
1. Comece a digitar qualquer um dos campos a seguir e selecione-os quando eles aparecerem na lista sob o objeto **Relatório** para adicioná-los como uma nova regra de filtro:

   * **Exibições**: exibe o número de exibições em qualquer um dos seguintes períodos:

      * **Este Mês, Trimestre, Ano**
      * **Último mês, trimestre, ano**
      * **Todas as Exibições**

   * **Última Visualização realizada por**: exibe informações sobre o usuário que visualizou o relatório por último
   * **Última Data de Visualização**: Exibe a data em que o relatório foi visualizado pela última vez

1. Selecione um modificador para o campo e especifique um valor quando solicitado.\
   ![Relatar estatísticas de filtro de uso](assets/qs-report-usage-filter-statistics-350x150.png)

1. Clique em **Salvar filtro**.\
   Exibe uma lista de relatórios que atendem às informações de uso definidas.\
   Você também pode criar um relatório para o objeto de relatório e usar esse filtro no relatório.\
   Para obter mais informações sobre a criação de um relatório, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). Você deve ter acesso para Editar aos Relatórios em seu nível de acesso para criar um relatório.\
   Para obter mais informações sobre o acesso a relatórios, consulte o artigo [Conceder acesso a relatórios, painéis e calendários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Exceções ao exibir informações de uso do relatório

>[!IMPORTANT]
>
>As informações de uso do relatório foram coletadas desde março de 2018. Nenhuma informação anterior a esta data está disponível.

A seguir estão algumas exceções que devem ser observadas ao trabalhar com informações de uso de relatório:

* Toda vez que um relatório é exibido em um painel ou em uma guia personalizada, ele é contado como uma exibição. O usuário que está exibindo esse relatório no painel é exibido como o usuário Última visualização por: Nome, e a data em que o painel foi exibido é exibida como a data Última visualização em.
* A Workfront não coleta informações de uso para relatórios integrados.\
  Para obter mais informações sobre relatórios internos do Workfront, consulte o artigo [Usar relatórios internos do Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

* A Workfront não coleta informações de uso sobre relatórios entregues. Um relatório entregue não conta como uma visualização.\
  Para obter mais informações sobre relatórios entregues, consulte o artigo [Visão geral da entrega de relatórios](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

* Quando um administrador de sistema ou de grupo faz logon como outro usuário, as exibições são contadas e associadas ao administrador de sistema ou de grupo.
* A Workfront não coleta informações de uso para relatórios por trimestres personalizados. Somente os trimestres padrão incorporados são referenciados nos campos de uso do relatório.
* A Workfront não coleta informações de uso para relatórios compartilhados e visualizados publicamente. Quando um relatório público é visualizado por alguém sem fazer logon no Workfront, as visualizações de relatório não são contadas.\
  Para obter mais informações sobre como compartilhar relatórios, consulte o artigo [Compartilhar um relatório no Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
