---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Configurar o acesso a blueprints
description: Como administrador do sistema, você pode habilitar o acesso de usuários para solicitar a instalação de blueprints configurando uma fila de solicitações para armazenar as solicitações. Lá, você tem um único local para rastrear e atualizar solicitações.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d85f363f-2ab4-45cb-b851-a7f33e1ca905
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Configurar o acesso a blueprints

Todos [!DNL Adobe Workfront] os usuários do podem navegar pelo catálogo de blueprints.

Como administrador do sistema, você pode:

* Adicionar [!UICONTROL Blueprints] ao menu principal em modelos de layout e atribua o modelo de layout a usuários ou grupos. Para obter mais informações, consulte [Personalize o [!UICONTROL Menu principal] uso de um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md) e [Atribuir usuários a um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   >[!NOTE]
   >
   >* Os usuários que não tiverem um modelo de layout atribuído a eles verão a variável [!UICONTROL Blueprints] no ícone na [!UICONTROL Menu principal].
   >* Ao criar um novo modelo de layout, a variável [!UICONTROL Blueprints] está incluído na variável [!UICONTROL Itens ativos] para a [!UICONTROL Menu principal] por padrão.



* Permita que os usuários solicitem a instalação de blueprints configurando uma fila de solicitações para armazenar as solicitações. Lá, você tem um único local para rastrear e atualizar solicitações. Para obter mais informações, siga o procedimento abaixo.
* Instale blueprints. Para obter mais informações, consulte [Instalar um blueprint](../../administration-and-setup/blueprints/blueprints-install.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano</strong></td> 
   <td> <p> Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] licença</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso</strong></td> 
   <td> <p>[!UICONTROL Administrador do sistema]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Pré-requisitos {#prerequisites}

* Você deve usar uma fila de solicitações existente para armazenar solicitações do blueprint. O projeto deve ser salvo como uma fila de solicitações e deve estar em [!UICONTROL Atual] status.
* A fila de solicitações deve ser pública. Nos detalhes da fila de solicitações, &quot;[!UICONTROL Quem pode adicionar solicitações a esta fila?]&quot; deve ser definido como **[!UICONTROL Qualquer pessoa]**.

>[!TIP]
>
>Se você quiser criar uma nova fila de solicitações para solicitações do blueprint, crie-a antes de configurar o acesso do blueprints. Para obter informações sobre como criar uma fila de solicitações, consulte [Criar uma fila de solicitações](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Selecionar a fila de solicitações para armazenar solicitações do blueprint

Antes que os usuários possam solicitar a instalação de blueprints para eles, você deve selecionar uma fila de solicitações para essas solicitações. Até que a fila de solicitações seja definida, os usuários só poderão navegar pelo catálogo de blueprints.

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Blueprints]**.
1. Clique em **[!UICONTROL Configurar solicitações do blueprint]** na parte superior direita da tela do catálogo.

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>In the <strong>Configure blueprints</strong> dialog, ensure that the <strong>Configure request queues</strong> tab is selected.</p> </li>
   -->

1. No **[!UICONTROL Configurar blueprints]** , comece digitando o nome de uma fila de solicitações ativa e selecione-a quando ela for exibida nos resultados da pesquisa.

   >[!IMPORTANT]
   >
   >Somente as filas de solicitação públicas aparecem nesta lista. Para tornar sua fila de solicitações pública, consulte o [Pré-requisitos](#prerequisites) acima.

   A preferência da fila de solicitações é definida e os usuários agora podem solicitar a instalação do blueprint.

   ![Configurar fila de solicitações](assets/Blueprints_access_setup_request_queue.png)

1. (Opcional) Para fazer alterações na fila de solicitações real, clique em **[!UICONTROL Editar esta fila de solicitações]**.

   O projeto da fila de solicitações é aberto em uma nova guia do navegador e você pode atualizá-lo conforme necessário.

1. (Opcional) Se a fila de solicitações contiver grupos de tópicos ou tópicos da fila, você poderá selecioná-los na lista.
1. Para retornar ao catálogo de blueprints, clique em **[!UICONTROL Fechar]**.

>[!NOTE]
>
>Ao instalar um blueprint solicitado, você deve alterar o status do problema para **[!UICONTROL Fechado]** ou **[!UICONTROL Resolvido]** na fila de solicitações para que o solicitante seja notificado. Para obter informações sobre como instalar um blueprint, consulte [Instalar um blueprint](../../administration-and-setup/blueprints/blueprints-install.md).
