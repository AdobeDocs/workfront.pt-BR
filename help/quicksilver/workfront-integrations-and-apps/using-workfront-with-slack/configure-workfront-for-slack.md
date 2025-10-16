---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-slack
title: Configurar [!DNL Adobe Workfront] para Slack
description: Integrar o  [!DNL Adobe Workfront] com o Slack permite que você acesse e crie [!DNL Workfront] itens de trabalho, aprovações, favoritos e itens recentes do Slack.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cac75a81-26e8-4713-a6be-453943b431ab
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Configurar [!DNL Adobe Workfront for Slack]

Integrar [!DNL Adobe Workfront] com [!DNL Slack] permite que você faça o seguinte:

* Acesse seus itens de trabalho, aprovações, favoritos e itens recentes do [!DNL Workfront].[!DNL Slack]
* Inscrever-se para, aprovar, atribuir trabalho de [!DNL Slack].
* Criar tarefas e problemas de [!DNL Slack].
* Receba algumas [!DNL Workfront] notificações em [!DNL Slack].

Dependendo de como o ambiente do [!DNL Slack] está configurado, você mesmo pode instalar e configurar o [!DNL Workfront for Slack], ou o administrador do [!DNL Workfront] deve instalá-lo e configurá-lo primeiro para que você possa configurá-lo para si mesmo.

Quando você integra sua instância do [!DNL Slack] com [!DNL Workfront], os usuários podem usar o [!DNL Workfront] enquanto colaboram dentro de seus canais [!DNL Slack]. A integração pode ser usada de qualquer ambiente [!DNL Slack], incluindo o aplicativo móvel [!DNL Slack]. ## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
   <td> <p>Qualquer</p>
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos para usar o [!DNL Workfront] com [!DNL Slack]

* Você deve ter uma instância [!DNL Slack].
* O administrador do sistema [!DNL Slack] deve permitir que todos os usuários [!DNL Slack] instalem o [!DNL Workfront for Slack].
* Você deve ter uma licença do [!DNL Workfront] para poder usar os recursos integrados no [!DNL Workfront].

  >[!NOTE]
  >
  >Usuários com qualquer tipo de licença do [!DNL Workfront] podem acessar o [!DNL Workfront] a partir do [!DNL Slack]. As ações que você pode executar a partir do [!DNL Slack] estão limitadas aos seus níveis de permissão e licença do [!DNL Workfront].

Para obter mais informações sobre como gerenciar aplicativos no [!DNL Slack], consulte [Gerenciar Aplicativos para o seu Workspace.](https://get.slack.help/hc/en-us/articles/222386767-Manage-apps-for-your-workspace)

## Instalar [!DNL Workfront for Slack]

Cada usuário [!DNL Slack] deve instalar o aplicativo [!DNL Workfront] para usar [!DNL Workfront] de [!DNL Slack].

Você pode instalar o aplicativo das seguintes maneiras:

* [Instalar o aplicativo [!DNL Workfront] fora [!DNL Slack]](#install-the-workfront-app-outside-slack-install-the-workfront-app-outside-slack)
* [Instalar o aplicativo [!DNL Workfront] em [!DNL Slack]](#install-the-workfront-app-within-slack-install-the-workfront-app-within-slack)

### Instalar o aplicativo [!DNL Workfront] fora de [!DNL Slack] {#install-the-workfront-app-outside-slack}

Siga as etapas abaixo para executar o processo de instalação e autorizar o [!DNL Workfront for Slack] na sua instância do [!DNL Slack].

>[!IMPORTANT]
>
>Quando uma nova versão do [!DNL Workfront] for lançada para Slack, você deverá autorizar novamente o aplicativo para continuar usando-o.

1. Localize o complemento [!DNL Adobe Workfront] na [[!DNL Slack] loja](https://workfront.slack.com/apps/A7CLAMVNW-adobe-workfront?tab=more_info).

1. Clique em **[!UICONTROL Abrir em[!DNL Slack]]**.

1. Entre no seu espaço de trabalho especificando a URL do [!DNL Slack] e clicando em **[!UICONTROL Continuar]**.\

1. Examine o acesso que [!DNL Slack] está solicitando. Se você concordar com esse acesso, clique em **[!UICONTROL Permitir acesso]** para autorizar o aplicativo [!DNL Workfront].

Agora você pode acessar [!DNL Workfront] de [!DNL Slack], conforme descrito no [Acesso [!DNL Workfront] de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

### Instalar o aplicativo [!DNL Workfront] em [!DNL Slack] {#install-the-workfront-app-within-slack}

Você pode instalar o aplicativo [!DNL Workfront] diretamente do aplicativo [!DNL Slack]:

1. Navegue até a URL do [!DNL Slack].

   Por exemplo: *`<YourTeamName>`.slack.com/apps*.

   Ou

   Clique no ícone **[!UICONTROL Adicionar Aplicativos]** na instância [!DNL Slack].

1. Comece a digitar *[!DNL Workfront]* no campo de pesquisa.
1. Pressione Enter.
1. Selecione o aplicativo **[!DNL Workfront]**.
1. Clique em **[!UICONTROL Configurações]**.

   A página Diretório de Aplicativos é exibida.

1. Clique em **[!UICONTROL Visitar Site do Aplicativo]**.
1. Clique em **[!UICONTROL Adicionar a[!DNL Slack]]**.
1. Siga as etapas para concluir a instalação.
1. Quando a instalação for concluída, você poderá acessar [!DNL Workfront] de [!DNL Slack], conforme descrito no [[!UICONTROL Access [!DNL Workfront] from [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).
