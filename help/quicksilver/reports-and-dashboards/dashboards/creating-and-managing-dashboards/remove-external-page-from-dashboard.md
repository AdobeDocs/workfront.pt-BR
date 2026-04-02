---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Remover uma página externa de um painel
description: Você pode remover uma Página externa de um painel se ela não for mais necessária.
author: Courtney
feature: Reports and Dashboards
exl-id: 9e400b8a-bbb8-4d1f-b419-d4a4518c0b2e
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 22%

---

# Remover uma página externa de um painel

<!-- Audited: 1/2025 -->

Você pode remover uma Página externa de um painel se ela não for mais necessária.

No entanto, não é possível excluir uma página externa após sua criação no Adobe Workfront. Você pode excluir uma página externa somente usando a API. Para obter informações sobre a API do Workfront, consulte [noções básicas sobre API](../../../wf-api/general/api-basics.md). Para obter informações sobre como criar páginas externas, consulte [Incorporar uma página da Web externa em um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

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
   <td> <p>Gerenciar permissões no painel</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Remover uma página externa de um painel

1. Vá para o painel que contém a página externa que deseja excluir.

1. Clique em **Ações do Painel** e em **Editar**.

   ![Editar painel](assets/unshimmed-edit-dashboard.png)

1. No lado direito da tela, localize a página externa que deseja remover e clique no ícone **Excluir** ![Ícone Excluir](assets/delete.png).

   ![Excluir ícone de página externa dentro do painel](assets/delete-external-page-icon-inside-dashboard-nwe-350x284.png)

1. Clique em **Salvar + Fechar** no canto inferior esquerdo.

   Essa ação remove a página externa do painel selecionado. A página externa permanece no Workfront e pode ser acessada de um relatório. Para obter informações, consulte a seção &quot;Exibir páginas externas em um relatório&quot; no artigo [Incorporar uma página da Web externa em um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).
