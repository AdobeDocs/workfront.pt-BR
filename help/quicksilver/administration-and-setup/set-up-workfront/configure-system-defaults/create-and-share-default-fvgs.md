---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Criar, editar e compartilhar filtros, exibições e agrupamentos padrão
description: Você pode criar filtros, exibições e agrupamentos padrão, depois disponibilizá-los aos usuários em sua organização.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: 75c4abfa9aebf1d07a851486391291cddc94f1a9
workflow-type: tm+mt
source-wordcount: '822'
ht-degree: 0%

---

# Criar, editar e compartilhar filtros, exibições e agrupamentos padrão

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Você pode criar filtros, exibições e agrupamentos padrão, depois disponibilizá-los aos usuários em sua organização.

Ao criar filtros padrão, exibições e agrupamentos conforme descrito neste artigo, os usuários com os quais você os compartilha poderão aproveitá-los ao exibir suas listas. Os usuários podem criar seus próprios filtros, visualizações e agrupamentos com base naqueles que você criar, mas não podem alterar diretamente os que você criar.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador.</p> <p><b>OBSERVAÇÃO</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Criar filtros, visualizações ou agrupamentos padrão

{{step-1-to-setup}}

1. Siga qualquer um destes procedimentos, dependendo se você está criando ou editando um filtro, visualização ou agrupamento:

   * Clique em **[!UICONTROL Interface]** > **[!UICONTROL Filtros]**.

   * Clique em **[!UICONTROL Interface] >** **[!UICONTROL Exibições]**.

   * Clique em **[!UICONTROL Interface]** > **[!UICONTROL Agrupamentos]**.

1. Se estiver criando um filtro, visualização ou agrupamento, clique em **[!UICONTROL Adicionar filtro]**, **[!UICONTROL Adicionar Exibição]** ou **[!UICONTROL Adicionar agrupamento]**, selecione o tipo de objeto ao qual deseja associar o novo filtro, visualização ou agrupamento.

   Ou

   Se você estiver editando um filtro, visualização ou agrupamento existente, selecione-o e clique no botão **[!UICONTROL Editar]** ícone ![Ícone Editar](assets/edit-icon.png).

1. Configure o filtro, a visualização ou o agrupamento.

   Para obter informações sobre opções disponíveis, consulte um dos seguintes artigos:

   * [Visão geral dos filtros em [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Visão geral das exibições em [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Visão geral dos agrupamentos em [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

1. Clique em **[!UICONTROL Salvar]** próximo ao canto inferior esquerdo.

Você pode disponibilizar o filtro, a visualização ou o agrupamento para os usuários em seu sistema. Para obter mais informações sobre o compartilhamento de filtros, exibições ou agrupamentos com outros usuários, consulte a seção [Disponibilizar filtros, visualizações ou agrupamentos para os usuários](#make-filters-views-or-groupings-available-to-users) neste artigo.


## Mostrar ou ocultar filtros, visualizações ou agrupamentos disponíveis no Modelo de layout

Você pode optar por mostrar ou ocultar filtros, exibições ou agrupamentos do Modelo de layout. Filtros visíveis estão disponíveis para todos os usuários em todo o sistema. Você pode usar um Modelo de layout para ocultar filtros visíveis para usuários ou grupos específicos.

>[!NOTE]
>
>Se um usuário estiver usando ativamente um filtro, visualização ou agrupamento e, em seguida, um administrador desativar o, ele ainda terá acesso até que escolha um novo filtro, visualização ou agrupamento. Depois de escolher um novo filtro, visualização ou agrupamento, eles não poderão mais reverter para o filtro, visualização ou agrupamento oculto.

Para mostrar ou ocultar filtros, exibições ou agrupamentos disponíveis no Modelo de layout:

1. Clique em **[!UICONTROL Interface]** e, em seguida, clique em uma das seguintes opções: **[!UICONTROL Filtros]**, **[!UICONTROL Exibições]** ou **[!UICONTROL Agrupamentos]**.

1. (Condicional) Selecione o filtro, a visualização ou o agrupamento que deseja disponibilizar para os usuários e clique em **[!UICONTROL Ativar todo o sistema]**.

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >Se desejar manter o filtro, a visualização ou o agrupamento disponível para a maioria dos usuários, mas ocultá-lo de outros, é possível usar o Modelo de layout. Para obter mais informações, consulte [Personalizar filtros, exibições e agrupamentos usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Condicional) Selecione o filtro, a visualização ou o agrupamento que deseja fazer ocultar dos usuários e clique em **[!UICONTROL Desativar todo o sistema]**. Depois de desativado, o filtro, a visualização ou o agrupamento ficará oculto do modelo de layout, bem como dos usuários do sistema inteiro.


## Disponibilizar filtros, visualizações ou agrupamentos para todos os usuários {#make-filters-views-or-groupings-available-to-users}

Essas etapas explicam como disponibilizar filtros, visualizações e agrupamentos da variável [!UICONTROL Compartilhar] na caixa de diálogo do [!UICONTROL Interface] área em [!UICONTROL Configuração]. Essa configuração funciona como um interruptor de ativação/desativação para todo o sistema, incluindo o Modelo de layout.

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Interface]** e, em seguida, clique em uma das seguintes opções: **[!UICONTROL Filtros]**, **[!UICONTROL Exibições]** ou **[!UICONTROL Agrupamentos]**.

1. Selecione o filtro, a visualização ou o agrupamento que deseja disponibilizar para os usuários e clique no botão **[!UICONTROL Compartilhar]** ícone ![Ícone Compartilhar](assets/share-icon.png) para abrir o [!UICONTROL Filtrar acesso], [!UICONTROL Ver Acesso]ou [!UICONTROL Agrupar acesso] formulário.
1. (Condicional) Para disponibilizar o filtro, a visualização ou o agrupamento para todos os usuários no sistema, clique no botão **[!UICONTROL Engrenagem]** menu suspenso ![](assets/gear-menu-for-sharing-items.png), depois clique em **[!UICONTROL Tornar esse sistema visível]**. Todos os usuários no sistema agora podem ver o filtro, a visualização ou o agrupamento.

   Ou

   Comece digitando o nome de usuários, equipes, funções, grupos ou empresas específicos com os quais deseja compartilhar o filtro, a visualização ou o agrupamento e clique no nome quando ele for exibido na lista suspensa.

   Para obter mais informações sobre compartilhamento, consulte [Visão geral do compartilhamento de permissões em objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Clique em **[!UICONTROL Salvar]**.

   Os usuários especificados agora podem ver o filtro padrão, a visualização ou o agrupamento ao visualizar o tipo de objeto ao qual você o associou.

## Excluir filtros, visualizações e agrupamentos

{{step-1-to-setup}}

1. Siga qualquer um destes procedimentos, dependendo se você está excluindo um filtro, visualização ou agrupamento:

   * Clique em **[!UICONTROL Interface]** > **[!UICONTROL Filtros]**

   * Clique em **[!UICONTROL Interface]** > **[!UICONTROL Exibições]**

   * Clique em **[!UICONTROL Interface]** > **[!UICONTROL Agrupamentos]**

1. Selecione um ou mais itens na lista e clique no botão **[!UICONTROL Excluir]** ícone ![Ícone Excluir](assets/delete.png).
1. Consulte um dos artigos a seguir para obter informações detalhadas sobre como configurar um filtro, visualização ou agrupamento.

   * [Visão geral dos filtros em [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Visão geral das exibições em [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Visão geral dos agrupamentos em [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)
