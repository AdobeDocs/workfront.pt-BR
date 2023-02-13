---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-slack
title: Configurar [!DNL Adobe Workfront] para Slack
description: Integração [!DNL Adobe Workfront] com o Slack permite acessar e criar [!DNL Workfront] itens de trabalho, aprovações, favoritos, itens recentes do Slack.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cac75a81-26e8-4713-a6be-453943b431ab
source-git-commit: 09b4644a63241fa9e0a213bfa6f1a7e4264a1703
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# Configurar [!DNL Adobe Workfront for Slack]

Integração [!DNL Adobe Workfront] com [!DNL Slack] O permite fazer o seguinte:

* Acesse seu [!DNL Workfront] itens de trabalho, aprovações, favoritos, itens recentes de [!DNL Slack].
* Assinar, aprovar, atribuir trabalho de [!DNL Slack].
* Criar tarefas e problemas a partir de [!DNL Slack].
* Receba alguns [!DNL Workfront] notificações em [!DNL Slack].

Dependendo de como o [!DNL Slack] estiver configurado, você poderá instalar e configurar [!DNL Workfront for Slack] você mesmo ou seu [!DNL Workfront] O administrador deve instalá-lo e configurá-lo primeiro antes que você possa configurá-lo sozinho.

Ao integrar o seu [!DNL Slack] instância com [!DNL Workfront] os usuários podem usar [!DNL Workfront] ao colaborar em [!DNL Slack] canais. A integração pode ser usada de qualquer [!DNL Slack] , incluindo o [!DNL Slack] aplicativo móvel.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] plano]</a>*</td> 
   <td> <p>[!UICONTROL Pro] ou superior</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.\

## Pré-requisitos para usar [!DNL Workfront] com [!DNL Slack]

* Você deve ter um [!DNL Slack] instância.
* Seu [!DNL Slack] o administrador do sistema deve permitir tudo [!DNL Slack] usuários para instalar [!DNL Workfront for Slack].
* Você deve ter um [!DNL Workfront] licença para poder usar os recursos integrados no [!DNL Workfront].

   >[!NOTE]
   >
   >Usuários com qualquer [!DNL Workfront] o tipo de licença pode acessar [!DNL Workfront] from [!DNL Slack]. As ações que você pode executar [!DNL Slack] estão limitadas ao seu [!DNL Workfront] níveis de licença e permissão.

Para obter mais informações sobre o gerenciamento de aplicativos no [!DNL Slack], consulte [Gerencie aplicativos no seu espaço de trabalho.](https://get.slack.help/hc/en-us/articles/222386767-Manage-apps-for-your-workspace)

## Instalar [!DNL Workfront for Slack]

Cada [!DNL Slack] O usuário deve instalar o [!DNL Workfront] para usar [!DNL Workfront] from [!DNL Slack].

Você pode instalar o aplicativo das seguintes maneiras:

* [Instale o [!DNL Workfront] aplicativo fora [!DNL Slack]](#install-the-workfront-app-outside-slack-install-the-workfront-app-outside-slack)
* [Instale o [!DNL Workfront] aplicativo dentro [!DNL Slack]](#install-the-workfront-app-within-slack-install-the-workfront-app-within-slack)

### Instale o [!DNL Workfront] aplicativo fora [!DNL Slack] {#install-the-workfront-app-outside-slack}

Siga as etapas abaixo para executar o processo de instalação e autorizar [!DNL Workfront for Slack] em seu [!DNL Slack] instância.

>[!IMPORTANT]
>
>Quando uma nova versão de [!DNL Workfront] para que o Slack seja lançado, é necessário autorizar novamente o aplicativo para continuar a usá-lo.

1. Localize a variável [!DNL Adobe Workfront] no complemento [[!DNL Slack] loja](https://workfront.slack.com/apps/A7CLAMVNW-adobe-workfront?tab=more_info).

1. Clique em **[!UICONTROL Abrir em[!DNL Slack]]**.

1. Faça logon no seu espaço de trabalho especificando [!DNL Slack] URL e clique em **[!UICONTROL Continuar]**.\
   ![Screen_Shot_2017-10-17_at_8.27.38_AM.png](assets/screen-shot-2017-10-17-at-8.27.38-am-350x432.png)

1. Examine o acesso que [!DNL Slack] O está solicitando o . Se você concordar com esse acesso, clique em **[!UICONTROL Permitir acesso]** para autorizar a [!DNL Workfront] aplicativo.

   ![](assets/integrations-access-screen-350x429.png)

Agora você pode acessar [!DNL Workfront] from [!DNL Slack], conforme descrito no [Acesso [!DNL Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

### Instale o [!DNL Workfront] aplicativo dentro [!DNL Slack] {#install-the-workfront-app-within-slack}

Você pode instalar o [!DNL Workfront] aplicativo diretamente do [!DNL Slack] aplicativo:

1. Navegue até seu [!DNL Slack] URL.

   Por exemplo: *`<YourTeamName>`.slack.com/apps*.

   Ou

   Clique no botão **[!UICONTROL Adicionar aplicativos]** ícone em seu [!DNL Slack] instância.

   ![add_apps_in_Slack.png](assets/add-apps-in-slack-350x112.png)

1. Comece a digitar *[!DNL Workfront]* no campo de pesquisa.
1. Pressione Enter.
1. Selecione o **[!DNL Workfront]** aplicativo.
1. Clique em **[!UICONTROL Configurações]**.

   A página Diretório do aplicativo é exibida.

1. Clique em **[!UICONTROL Visitar site do aplicativo]**.
1. Clique em **[!UICONTROL Adicionar a[!DNL Slack]]**.
1. Siga as etapas para concluir a instalação.
1. Quando a instalação for concluída, você poderá acessar [!DNL Workfront] from [!DNL Slack], conforme descrito no [[!UICONTROL Acesso [!DNL Workfront] from [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).
