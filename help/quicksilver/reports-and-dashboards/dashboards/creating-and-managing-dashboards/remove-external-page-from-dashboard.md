---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Remover uma Página Externa de um painel
description: Você pode remover uma Página externa de um painel se ela não for mais necessária.
author: Nolan
feature: Reports and Dashboards
exl-id: 9e400b8a-bbb8-4d1f-b419-d4a4518c0b2e
source-git-commit: a9abbeaa9abd0e905c60000a218eddb85d0389b9
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 0%

---

# Remover uma Página Externa de um painel

<!-- Audited: 1/2025 -->

Você pode remover uma Página externa de um painel se ela não for mais necessária.

No entanto, não é possível excluir uma página externa após sua criação no Adobe Workfront. Você pode excluir uma página externa somente usando a API. Para obter informações sobre a API do Workfront, consulte [noções básicas sobre API](../../../wf-api/general/api-basics.md). Para obter informações sobre como criar páginas externas, consulte [Incorporar uma página da Web externa em um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plano do Adobe Workfront</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença do Adobe Workfront</strong></td> 
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
   <td role="rowheader"><strong>Configurações de nível de acesso</strong></td> 
   <td> <p>Editar acesso a relatórios, painéis, calendários</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Gerenciar permissões no painel</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Remover uma página externa de um painel

1. Vá para o painel que contém a página externa que deseja excluir.

1. Clique em **Ações do Painel** e em **Editar**.

   ![](assets/unshimmed-edit-dashboard.png)

1. No lado direito da tela, localize a página externa que deseja remover e clique no ícone **Excluir**: ![](assets/delete.png).

   ![](assets/delete-external-page-icon-inside-dashboard-nwe-350x284.png)

1. Clique em **Salvar + Fechar** no canto inferior esquerdo.

   Essa ação remove a página externa do painel selecionado. A página externa permanece no Workfront e pode ser acessada de um relatório. Para obter informações, consulte a seção &quot;Exibir páginas externas em um relatório&quot; no artigo [Incorporar uma página da Web externa em um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).
