---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Criar um painel
description: Você pode criar painéis para acessar informações rapidamente no Adobe Workfront. Relatórios, calendários e páginas externas podem ser adicionados a painéis que podem ser compartilhados com outras pessoas para colaboração ideal.
author: Nolan
feature: Reports and Dashboards
exl-id: 6a284df4-f011-4b4c-b44c-2e20918f643f
source-git-commit: c264c0c96b818934a7c25ed54c7666d2d6c95e54
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---

# Criar um painel

<!--Audited: 01/2024-->

Você pode criar painéis para acessar informações rapidamente no Adobe Workfront. Relatórios, calendários e páginas externas podem ser adicionados a painéis que podem ser compartilhados com outras pessoas para colaboração ideal.

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
   <td> <p><strong>plano do Adobe Workfront</strong></p> </td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Licença da Adobe Workfront*</strong></p> </td> 
   <td> <p>Atual: Plano </p>
   Ou
   <p>Novo: Padrão </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Configurações de nível de acesso</strong> </td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Permissões de objeto</strong> </p> </td> 
   <td> <p>Você obterá permissões de gerenciamento para os painéis que criar</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront. Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Pré-requisitos

Você deve criar qualquer um dos seguintes objetos antes de adicioná-los a um painel:

* **Relatórios**: para obter informações sobre como criar relatórios, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* **Calendários**: Para obter informações sobre como criar calendários, consulte [Visão geral dos relatórios de calendário](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

Você pode adicionar páginas externas existentes a um painel ou criar uma a partir do novo painel. Para obter informações sobre como criar páginas externas, consulte [Incorporar uma página externa da Web em um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## Criar um painel

{{step1-to-dashboards}}

1. Clique em **Novo painel**.\
   A caixa de diálogo Novo Painel é exibida.

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
      <td role="rowheader"><strong>Descrição (opcional)</strong></td>
      <td>Esta é uma descrição do seu painel.</td>
     </tr>
    </tbody>
   </table>

1. Selecione um layout clicando no botão de opção correspondente a ele na parte superior do **Selecionar layout/adicionar relatórios/adicionar calendários** seção. Esse é o layout no qual os relatórios, calendários ou páginas externas serão exibidos no painel.

   O layout de coluna única é o padrão.

   Para obter informações sobre o layout de relatórios em painéis, consulte [Entender como os relatórios são exibidos em um painel](../../../reports-and-dashboards/dashboards/understanding-dashboards/understand-how-reports-display-dashboard.md).

   <!--
   Consider adding the information from this article above here, at some point, instead of linking to it.)
   -->

1. Pesquisar relatórios, calendários ou páginas externas no **Pesquisar por nome ou tipo...** e arraste-os para o painel de layout, quando eles aparecerem na lista.

   >[!NOTE]
   >
   >Ao pesquisar por um item, a pesquisa retorna qualquer um dos 2.000 relatórios criados mais recentemente. Os nomes de relatório que incluem caracteres unicode não são retornados nos resultados da pesquisa. Como prática recomendada, evite incluir caracteres unicode ao nomear objetos no Workfront digitando nomes em vez de copiar e colar nomes de outra fonte.

   ![Pesquisar relatórios](assets/qs-new-dashboard-ui-0722.png)

1. (Opcional) Clique em **Adicionar página externa** para adicionar uma nova Página Externa ao painel.

   Para obter mais informações sobre como criar páginas externas e incorporá-las aos painéis, consulte [Incorporar uma página externa da Web em um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

1. Clique em **Salvar + Fechar**.

   Um carimbo de data e hora é exibido no canto superior direito do painel. O carimbo de data e hora inclui a data, a hora e o fuso horário quando o painel foi atualizado pela última vez.
