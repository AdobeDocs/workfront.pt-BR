---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Criar um painel
description: Você pode criar painéis para acessar informações rapidamente em relatórios, calendários e páginas externas.
author: Nolan
feature: Reports and Dashboards
exl-id: 6a284df4-f011-4b4c-b44c-2e20918f643f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Criar um painel

Você pode criar painéis para acessar informações rapidamente em relatórios, calendários e páginas externas.

Para saber mais sobre painéis, consulte [Introdução aos painéis](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Plano Adobe Workfront*</strong></p> </td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Licença da Adobe Workfront*</strong></p> </td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Configurações de nível de acesso*</strong> </td> 
   <td> <p>Editar acesso a Relatórios, Painéis e Calendários</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Permissões de objeto</strong> </p> </td> 
   <td> <p>Você obterá permissões de gerenciamento para o novo painel</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.<br>Para obter mais informações sobre permissões para painéis, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md" class="MCXref xref">Compartilhar relatórios, painéis e calendários </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Você deve criar qualquer um dos seguintes objetos antes de adicioná-los a um painel:

* **Relatórios**: Para obter informações sobre como criar relatórios, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* **Calendários**: Para obter informações sobre como criar calendários, consulte [Visão geral dos relatórios de calendário](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

* **Páginas externas**: Para obter informações sobre a criação de páginas externas, consulte [Incorporar uma página da Web externa em um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## Criar um painel

1. Clique no ícone do Menu principal ![](assets/main-menu-icon.png), depois clique em **Painéis.**
1. Clique em **Novo painel**.\
   A caixa de diálogo Novo painel é exibida.

1. Especifique o seguinte:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Nome</strong></td>
      <td><p>Este é o nome do seu painel.</p><p>Se você não especificar um nome, o nome do primeiro relatório no painel se tornará o nome do painel, por padrão.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Descrição (Opcional)</strong></td>
      <td>Esta é uma descrição do seu painel.</td>
     </tr>
    </tbody>
   </table>

1. Selecione um layout clicando no botão de opção correspondente a ele.

   O layout de coluna única é o padrão.

   Para obter informações sobre o layout do relatório em painéis, consulte [Entender como os relatórios são exibidos em um painel](../../../reports-and-dashboards/dashboards/understanding-dashboards/understand-how-reports-display-dashboard.md).

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Consider adding the information from this article here, at some point, instead of linking to it.)
   </MadCap:conditionalText>
   -->

1. Adicione relatórios, calendários ou páginas externas existentes pesquisando-os na **Pesquisar por nome ou tipo ...** , depois arrastando-os para o painel de layout, quando aparecerem na lista.

   >[!NOTE]
   >
   >Ao pesquisar por um item, a pesquisa retorna qualquer um dos 2.000 relatórios criados mais recentemente. Nomes de relatórios que incluem caracteres unicode não são retornados nos resultados da pesquisa. Como prática recomendada, evite incluir caracteres unicode ao nomear objetos no Workfront digitando nomes em vez de copiar e colar nomes de outra fonte.

   ![Pesquisar relatórios](assets/qs-new-dashboard-ui-0722.png)

1. (Opcional) Clique em **Adicionar página externa** para adicionar uma Página externa ao painel.\
   Para obter mais informações sobre como criar páginas externas e incorporá-las a painéis, consulte [Incorporar uma página da Web externa em um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

1. Clique em **Salvar + Fechar**.\
   Um carimbo de data e hora é exibido no canto superior direito do painel. O carimbo de data e hora inclui a data, a hora e o fuso horário em que o painel foi atualizado pela última vez.
