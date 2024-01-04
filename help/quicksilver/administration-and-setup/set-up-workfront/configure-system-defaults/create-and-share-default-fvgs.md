---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Criar, editar e compartilhar filtros, visualizações e agrupamentos padrão
description: Você pode criar filtros, visualizações e agrupamentos padrão e, em seguida, disponibilizá-los aos usuários em sua organização.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '820'
ht-degree: 0%

---

# Criar, editar e compartilhar filtros, visualizações e agrupamentos padrão

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Você pode criar filtros, visualizações e agrupamentos padrão e, em seguida, disponibilizá-los aos usuários em sua organização.

Ao criar filtros, visualizações e agrupamentos padrão conforme descrito neste artigo, os usuários com os quais você os compartilha podem aproveitá-los ao visualizar suas listas. Os usuários podem criar seus próprios filtros, visualizações e agrupamentos com base naqueles que você cria, mas não podem alterar diretamente aqueles que você cria.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Plano]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador.</p> <p><b>NOTA</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais no seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Criar filtros, visualizações ou agrupamentos padrão

{{step-1-to-setup}}

1. Desempenhe uma das ações a seguir, dependendo se você está criando ou editando um filtro, uma visualização ou um agrupamento:

   * Clique em **[!UICONTROL Interface]** > **[!UICONTROL Filtros]**.

   * Clique em **[!UICONTROL Interface] >** **[!UICONTROL Visualizações]**.

   * Clique em **[!UICONTROL Interface]** > **[!UICONTROL Agrupamentos]**.

1. Se estiver criando um filtro, exibição ou agrupamento, clique em **[!UICONTROL Adicionar filtro]**, **[!UICONTROL Adicionar visualização]** ou **[!UICONTROL Adicionar Agrupamento]**, em seguida, selecione o tipo de objeto ao qual deseja associar o novo filtro, exibição ou agrupamento.

   Ou

   Se você estiver editando um filtro, exibição ou agrupamento existente, selecione-o e clique no link **[!UICONTROL Editar]** ícone ![Ícone Editar](assets/edit-icon.png).

1. Configure o filtro, a visualização ou o agrupamento.

   Para obter informações sobre opções disponíveis, consulte um dos seguintes artigos:

   * [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Visão geral das exibições em [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Visão geral de agrupamentos em [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

1. Clique em **[!UICONTROL Salvar]** próximo ao canto inferior esquerdo.

Você pode disponibilizar o filtro, a visualização ou o agrupamento para os usuários do seu sistema. Para obter mais informações sobre o compartilhamento de filtros, visualizações ou agrupamentos com outros usuários, consulte a seção [Disponibilizar filtros, visualizações ou agrupamentos aos usuários](#make-filters-views-or-groupings-available-to-users) neste artigo.


## Mostrar ou ocultar filtros, exibições ou agrupamentos disponíveis no Modelo de layout

Você pode optar por mostrar ou ocultar filtros, exibições ou agrupamentos do Modelo de layout. Filtros visíveis estão disponíveis para todos os usuários em todo o sistema. Você pode usar um Modelo de layout para ocultar filtros visíveis para usuários ou grupos específicos.

>[!NOTE]
>
>Se um usuário estiver usando ativamente um filtro, uma visualização ou um agrupamento e um administrador desativá-lo, o usuário ainda terá acesso até que escolha um novo filtro, exibição ou agrupamento. Depois de escolher um novo filtro, visualização ou agrupamento, eles não poderão mais reverter para o filtro, visualização ou agrupamento ocultos.

Para mostrar ou ocultar filtros, exibições ou agrupamentos disponíveis no Modelo de layout:

1. Clique em **[!UICONTROL Interface]**, em seguida, clique em uma das opções a seguir: **[!UICONTROL Filtros]**, **[!UICONTROL Visualizações]** ou **[!UICONTROL Agrupamentos]**.

1. (Condicional) Selecione o filtro, a exibição ou o agrupamento que deseja disponibilizar aos usuários e clique em **[!UICONTROL Ativar todo o sistema]**.

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >Se você deseja manter o filtro, a visualização ou o agrupamento disponível para a maioria dos usuários, mas ocultá-lo de outros, é possível usar o Modelo de layout. Para obter mais informações, consulte [Personalizar filtros, visualizações e agrupamentos usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Condicional) Selecione o filtro, a exibição ou o agrupamento que deseja ocultar dos usuários e clique em **[!UICONTROL Desativar todo o sistema]**. Depois de desativado, o filtro, a visualização ou o agrupamento serão ocultados do modelo de layout, bem como dos usuários em todo o sistema.


## Disponibilizar filtros, visualizações ou agrupamentos a todos os usuários {#make-filters-views-or-groupings-available-to-users}

Essas etapas explicam como disponibilizar filtros, visualizações e agrupamentos na [!UICONTROL Compartilhar] no [!UICONTROL Interface] área em [!UICONTROL Configuração]. Esta configuração funciona como uma chave liga/desliga para todo o sistema, incluindo o Modelo de layout.

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Interface]**, em seguida, clique em uma das opções a seguir: **[!UICONTROL Filtros]**, **[!UICONTROL Visualizações]** ou **[!UICONTROL Agrupamentos]**.

1. Selecione o filtro, a exibição ou o agrupamento que deseja disponibilizar para os usuários e clique no link **[!UICONTROL Compartilhar]** ícone ![Ícone Compartilhar](assets/share-icon.png) para abrir o [!UICONTROL Filtrar acesso], [!UICONTROL Acesso de visualização]ou [!UICONTROL Acesso de agrupamento] formulário.
1. (Condicional) Para disponibilizar o filtro, a exibição ou o agrupamento a todos os usuários do sistema, clique no link **[!UICONTROL Engrenagem]** menu suspenso ![](assets/gear-menu-for-sharing-items.png)e, em seguida, clique em **[!UICONTROL Tornar isto visível em todo o sistema]**. Todos os usuários no sistema agora podem ver o filtro, a visualização ou o agrupamento.

   Ou

   Comece digitando o nome de usuários, equipes, funções, grupos ou empresas específicos com os quais compartilhar o filtro, a visualização ou o agrupamento e clique no nome quando ele aparecer na lista suspensa.

   Para obter mais informações sobre compartilhamento, consulte [Visão geral das permissões de compartilhamento em objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Clique em **[!UICONTROL Salvar]**.

   Os usuários especificados agora podem ver o filtro, a visualização ou o agrupamento padrão ao visualizar o tipo de objeto ao qual você o associou.

## Excluir filtros, visualizações e agrupamentos

{{step-1-to-setup}}

1. Desempenhe uma das ações a seguir, dependendo se você está excluindo um filtro, uma exibição ou um agrupamento:

   * Clique em **[!UICONTROL Interface]** > **[!UICONTROL Filtros]**

   * Clique em **[!UICONTROL Interface]** > **[!UICONTROL Visualizações]**

   * Clique em **[!UICONTROL Interface]** > **[!UICONTROL Agrupamentos]**

1. Selecione um ou mais itens na lista e clique no botão **[!UICONTROL Excluir]** ícone ![Ícone Excluir](assets/delete.png).
1. Consulte um dos seguintes artigos para obter informações detalhadas sobre como configurar um filtro, uma visualização ou um agrupamento.

   * [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Visão geral das exibições em [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Visão geral de agrupamentos em [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)
