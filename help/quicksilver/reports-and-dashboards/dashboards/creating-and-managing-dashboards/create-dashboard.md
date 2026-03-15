---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Criar um painel
description: Você pode criar painéis para acessar rapidamente informações no Adobe Workfront. Relatórios, calendários e páginas externas podem ser adicionados a painéis que podem ser compartilhados com outras pessoas para colaboração ideal.
author: Courtney
feature: Reports and Dashboards
exl-id: 6a284df4-f011-4b4c-b44c-2e20918f643f
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 11%

---

# Criar um painel

<!--Audited: 01/2025-->

Você pode criar painéis para acessar rapidamente informações no Adobe Workfront. Até 25 relatórios, calendários e páginas externas podem ser adicionados a painéis que podem ser compartilhados com outras pessoas para colaboração ideal.

Para saber mais sobre painéis, consulte [Introdução aos painéis](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

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
   <td> <p>Editar acesso a relatórios, painéis e calendários</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Você obterá permissões de Gerenciamento para os painéis que criar</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Você deve criar qualquer um dos seguintes objetos antes de adicioná-los a um painel de controle:

* **Relatórios**: para obter informações sobre como criar relatórios, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* **Calendários**: para obter informações sobre como criar calendários, consulte [Visão geral de relatórios de calendário](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

Você pode adicionar páginas externas existentes a um painel de controle ou criar uma a partir do novo painel de controle. Para obter informações sobre como criar páginas externas, consulte [Incorporar uma página da Web externa em um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## Criar um painel

{{step1-to-dashboards}}

1. Clique em **Novo Painel**.\
   A caixa de diálogo Novo Painel é exibida.

1. Especifique o seguinte:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Nome</strong></td>
      <td><p>Este é o nome do seu painel. Recomendamos usar apenas caracteres UTF-8 para evitar problemas de compatibilidade.</p><p>Se você não especificar um nome, o nome do primeiro relatório no painel se tornará o nome do painel, por padrão.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Descrição (opcional)</strong></td>
      <td>Esta é uma descrição do seu painel.</td>
     </tr>
    </tbody>
   </table>

1. Selecione um layout clicando no botão de opção correspondente na parte superior da seção **Selecionar layout/Adicionar relatórios/Adicionar calendários**. Este é o layout no qual os relatórios, calendários ou páginas externas serão exibidos no painel.

   O layout de coluna única é o padrão.

   Para obter informações sobre o layout de relatórios em painéis, consulte [Entender como os relatórios são exibidos em um painel](../../../reports-and-dashboards/dashboards/understanding-dashboards/understand-how-reports-display-dashboard.md).

   <!--
   Consider adding the information from this article above here, at some point, instead of linking to it.)
   -->

1. Na seção **Relatórios e Calendários Disponíveis**, comece digitando o nome de um relatório, calendário ou página externa na barra de pesquisa e, em seguida, arraste e solte o relatório, o calendário ou a página externa no painel de layout à direita.

   >[!NOTE]
   >
   >Ao procurar um item, a pesquisa retorna qualquer um dos 2.000 relatórios criados mais recentemente. Nomes de relatório que incluem caracteres unicode não são retornados nos resultados da pesquisa. Como prática recomendada, evite incluir caracteres unicode ao nomear objetos no Workfront digitando nomes em vez de copiar e colar nomes de outra origem.

   ![Pesquisar relatórios](assets/unshimmed-dashboard-ui.png)

1. (Opcional) Clique em **Adicionar Página Externa** para adicionar uma nova Página Externa ao painel.

   Para obter mais informações sobre como criar páginas externas e incorporá-las aos painéis, consulte [Incorporar uma página da Web externa a um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

1. Clique em **Salvar + Fechar**.

   Um carimbo de data/hora é exibido no canto superior direito do painel. O carimbo de data/hora inclui a data, a hora e o fuso horário em que o painel foi atualizado pela última vez.
