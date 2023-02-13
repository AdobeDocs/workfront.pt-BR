---
product-area: reporting
navigation-topic: report-usage
title: Visualizar uso de relatório
description: Visualizar uso de relatório
author: Nolan
feature: Reports and Dashboards
exl-id: 51d9067c-8c55-433e-b560-7da241ef33ae
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '997'
ht-degree: 0%

---

# Visualizar uso de relatório

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : *** DO NOT CHANGE, REMOVE, CHANGE LINK, RENAME THIS ARTICLE- IT IS LINKED TO THE PENDO GUIDE FOR THE MAIN REPORTS AREA***)</p>
-->

Para entender como os relatórios são usados em seu sistema, você pode exibir as seguintes informações em uma lista de relatórios:

* Últimos 10 usuários que visualizaram o relatório
* Exibir contagem em um período especificado

   >[!NOTE]
   >
   >O Adobe Workfront conta uma visualização por usuário por dia. Se você acessar o mesmo relatório várias vezes por dia, o Workfront conta isso como uma visualização para esse relatório. Se o mesmo relatório for acessado por outro usuário no mesmo dia, o Workfront o contará como uma nova visualização para o segundo usuário.

* Última data da visualização
* Última visualização por usuário
* Uma lista de painéis que contém o relatório\
   Para obter mais informações sobre como exibir o nome dos painéis nos quais os relatórios podem ser adicionados em uma lista de relatórios, consulte o artigo [Entender como organizar relatórios em um painel](../../../reports-and-dashboards/reports/report-usage/understand-how-organize-reports-dashboard.md).

Você pode criar uma visualização para uma lista de relatórios, onde pode exibir essas informações.\
É possível filtrar uma lista de relatórios por alguns desses campos.\
Para obter mais informações sobre quais campos você pode filtrar um relatório por, consulte o artigo [Filtrar uma lista de relatórios por informações de uso](#filter-a-report-list-by-usage-information).

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

## Exibir informações de uso do relatório na Exibição de uma lista de relatórios

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, em seguida, clique em **Relatórios**.

1. Na lista de relatórios, clique no botão **Exibir** menu suspenso.
1. (Opcional) Selecione o **Uso de relatórios** exibir para exibir as informações mais comuns de uso do relatório.\
   Ou

1. Clique em **Nova exibição** para criar uma exibição personalizada.
1. Clique em **Adicionar coluna**.
1. Comece a digitar qualquer um dos campos a seguir e selecione-os quando aparecerem na lista sob a **Relatório** para adicioná-los a uma nova coluna:

   * **Últimos 10 usuários**: Exibe os nomes dos últimos 10 usuários que visualizaram o relatório.
   * **Exibições**: Exibe o número de visualizações em qualquer um dos seguintes intervalos de tempo:

      * **Este Mês, Trimestre, Ano**
      * **Último Mês, Trimestre, Ano**
      * **Todas as exibições**: Exibe uma contagem geral para todas as exibições no relatório
   * **Última visualização por**: Exibe informações sobre o usuário que visualizou o relatório por último
   * **Data da Última Visualização**: Exibe a data em que o relatório foi visualizado por último


1. Clique em **Salvar exibição**.\
   As informações de uso sobre o relatório são exibidas nas colunas adicionadas à visualização.\
   Você também pode criar um relatório para o objeto do relatório e usar essa visualização no relatório.\
   Para obter mais informações sobre como criar um relatório, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
   É necessário ter o acesso Editar aos Relatórios no nível de acesso para criar um relatório.\
   Para obter mais informações sobre o acesso a relatórios, consulte o artigo [Conceder acesso a relatórios, painéis e calendários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Filtrar uma lista de relatórios por informações de uso {#filter-a-report-list-by-usage-information}

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, em seguida, clique em **Relatórios**.
1. Na lista de relatórios, clique no botão **Filtro** menu suspenso.
1. Clique em **Novo filtro**, depois clique em **Adicionar uma regra de filtro**.
1. Comece a digitar qualquer um dos campos a seguir e selecione-os quando aparecerem na lista sob a **Relatório** para adicioná-los como uma nova regra de filtro:

   * **Exibições**: Exibe o número de visualizações em qualquer um dos seguintes intervalos de tempo:

      * **Este Mês, Trimestre, Ano**
      * **Último Mês, Trimestre, Ano**
      * **Todas as Exibições**
   * **Última visualização por**: Exibe informações sobre o usuário que visualizou o relatório por último
   * **Data da Última Visualização**: Exibe a data em que o relatório foi visualizado por último


1. Selecione um modificador para seu campo e, em seguida, especifique um valor, quando solicitado.\
   ![](assets/qs-report-usage-filter-statistics-350x150.png)

1. Clique em **Salvar filtro**.\
   Isso exibe uma lista de relatórios que atendem às informações de uso que você definiu.\
   Você também pode criar um relatório para o objeto do relatório e usar esse filtro no relatório.\
   Para obter mais informações sobre como criar um relatório, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). É necessário ter o acesso Editar aos Relatórios no nível de acesso para criar um relatório.\
   Para obter mais informações sobre o acesso a relatórios, consulte o artigo [Conceder acesso a relatórios, painéis e calendários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Exceções ao exibir informações de uso do relatório

>[!IMPORTANT]
>
>As informações de uso do relatório são coletadas desde março de 2018. As informações anteriores a esta data não estão disponíveis.

Estas são algumas exceções que devem ser observadas ao trabalhar com informações de uso do relatório:

* Toda vez que um relatório é exibido em um painel ou em uma guia personalizada, ele é contado como uma visualização. O usuário que está exibindo esse relatório em seu painel é exibido como a Última exibição por: Nomeie o usuário e a data em que o painel foi exibido é exibida como a data da Última visualização.
* O Workfront não coleta informações de uso para relatórios incorporados.\
   Para obter mais informações sobre relatórios internos do Workfront, consulte o artigo [Usar relatórios internos do Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

* A Workfront não coleta informações de uso em relatórios entregues. Um relatório entregue não conta como uma visualização.\
   Para obter mais informações sobre relatórios entregues, consulte o artigo [Visão geral da entrega de relatórios](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

* Quando um administrador de sistema ou de grupo faz logon como outro usuário, as exibições são contabilizadas e associadas ao administrador do sistema ou de grupo.
* A Workfront não coleta informações de uso para relatórios por trimestres personalizados. Somente os trimestres internos padrão são referenciados nos campos de uso do relatório.
* O Workfront não coleta informações de uso para relatórios compartilhados e exibidos publicamente. Quando um relatório público é visualizado por alguém sem fazer logon no Workfront, as visualizações do relatório não são contadas.\
   Para obter mais informações sobre compartilhamento de relatórios, consulte o artigo [Compartilhar um relatório no Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
