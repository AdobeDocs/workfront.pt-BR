---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Acesso [!DNL Adobe Workfront] from [!DNL Slack]
description: Integração [!DNL Adobe Workfront] com [!DNL Slack] permite acessar [!DNL Workfront] do Slack ou execute determinadas ações em [!DNL Workfront] usando um comando de barra. A integração pode ser usada de qualquer [!DNL Slack] , incluindo o [!DNL Slack] aplicativo móvel.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5f531217-3bd6-4156-8b9f-eabc95d4df10
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '1075'
ht-degree: 1%

---

# Acesso [!DNL Adobe Workfront] from [!DNL Slack]

Integração [!DNL Adobe Workfront] com [!DNL Slack] permite acessar [!DNL Workfront] from [!DNL Slack]ou executar determinadas ações em [!DNL Workfront] usando um comando de barra. A integração pode ser usada de qualquer [!DNL Slack] , incluindo o [!DNL Slack] aplicativo móvel.

Você ou seu [!DNL Slack] o administrador deve instalar o [!DNL Workfront] no seu aplicativo [!DNL Slack] antes de usar [!DNL Workfront] from [!DNL Slack]. Para obter mais informações, consulte [Configurar o Adobe Workfront para Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Sobre comandos de barra {#about-slash-commands}

Ao usar [!DNL Slack], você digita mensagens dentro de um campo de mensagem. Ao iniciar sua mensagem com uma barra, ela se torna um comando e se comporta de forma diferente de uma mensagem simples. O comando informa [!DNL Slack] para executar uma ação.

Você pode acessar seu [!DNL Workfront] instância de [!DNL Slack] digitando um comando de barra em qualquer [!DNL Slack] canal.

Lembre-se do seguinte ao usar um comando de barra em [!DNL Slack] para acessar [!DNL Workfront]:

* Os comandos de barra fazem distinção entre maiúsculas e minúsculas.
* Os comandos para [!DNL Workfront] são visíveis somente para você, independentemente do canal no qual você está digitando.
* O comando deve sempre começar com `/workfront` ou `/wf`, seguido por um espaço e o nome de uma ação que você deseja executar em [!DNL Workfront].

   Isso indica que seu comando se destina à função [!DNL Workfront] aplicativo. Os comandos para [!DNL Workfront] funcionam somente quando você já tiver configurado a variável [!DNL Workfront] com seu aplicativo [!DNL Slack] instância.

Para obter uma lista de todos os comandos que você pode executar a partir do Slack para [!DNL Workfront], consulte [Acesso [!DNL Workfront] de um comando de barra em [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack).

## Faça logon em [!DNL Workfront] from [!DNL Slack] {#log-in-to-workfront-from-slack}

Ao digitar qualquer comando no campo de mensagem no Slack, você será solicitado a fazer logon no [!DNL Workfront] primeiro.\
Para obter uma lista completa de [!DNL Workfront] comandos de [!DNL Slack], consulte o [Acesso [!DNL Workfront] de um comando de barra em [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack) neste artigo.

Para fazer logon no [!DNL Workfront] from [!DNL Slack]:

1. Faça logon no [!DNL Slack] instância.
1. Em qualquer canal, digite um dos seguintes comandos:\
   `/workfront log in`

   Ou

   `/wf log in`

1. Clique no botão [!DNL Workfront] **[!UICONTROL Fazer logon]** exibido na resposta.\
   Uma nova guia é aberta com campos para [!DNL Workfront] credenciais.

1. Siga as instruções para fazer logon no [!DNL Workfront] usando Autenticação aprimorada, OAuth 2.0 ou o URL de SAML (Security Assertion Markup Language).

   >[!NOTE]
   >
   >* Quando for solicitado a entrar no host do seu [!DNL Workfront] digite-a usando este formato: *sua empresa&#39;sDomain.my.workfront.com*. O domínio de sua empresa geralmente é o nome de sua empresa.
   >* A Autenticação aprimorada não está disponível até que um [!DNL Workfront] O administrador o habilita para essa integração.



   A página de configuração para [!DNL Workfront] notificações em [!DNL Slack] é aberto.

1. (Opcional) Desative qualquer [!DNL Workfront] notificações que você não deseja receber em [!DNL Slack].

   Para obter informações sobre como configurar [!DNL Workfront] configurações para [!DNL Slack], consulte o [Definir configurações](#configure-settings-configure-settings) seção neste artigo

1. Navegue de volta para sua [!DNL Slack] canal.

   Você está conectado a [!DNL Workfront] do [!DNL Slack] instância.

## Acesso [!DNL Workfront] from [!DNL Slack]

* [Sobre comandos de barra](#about-slash-commands-about-slash-commands)
* [Acesso [!DNL Workfront] de um link compartilhado em [!DNL Slack]](#access-workfront-from-a-shared-link-in-slack-access-workfront-from-a-shared-link-in-slack)

## Acesso [!DNL Workfront] de um comando de barra em [!DNL Slack] {#access-workfront-from-a-slash-command-in-slack}

1. Faça logon no [!DNL Slack] instância e faça logon no [!DNL Workfront] from [!DNL Slack].\
   Para obter mais informações sobre como fazer logon no [!DNL Workfront] from [!DNL Slack], consulte [Faça logon em [!DNL Workfront] from [!DNL Slack]](#log-in-to-workfront-from-slack-log-in-to-workfront-from-slack)

1. Em qualquer canal, comece a digitar o seguinte comando no campo de mensagem:

   `/workfront help`

   Ou

   `/wf help`

1. Selecione um dos seguintes comandos:

   * `/wf home`

      Exibe botões dos quais você pode acessar listas de suas tarefas, emissões e aprovações. Clicar em um dos botões exibe os 20 primeiros itens de cada lista em [!DNL Slack].

      ![](assets/slack-home-buttons-350x80.png)

      Para obter mais informações sobre o gerenciamento [!DNL Workfront] itens de trabalho de [!DNL Slack], consulte [Gerencie seu trabalho e suas aprovações no [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf add task <TaskName>`

      Inclua o nome da tarefa da forma que ela aparecerá no [!DNL Workfront] interface.

      Adiciona uma tarefa a [!DNL Workfront].

      Para obter mais informações sobre como adicionar tarefas a [!DNL Workfront] no Slack, consulte &quot;Criando Tarefas de [!DNL Slack]&quot; na seção [Criar tarefas e problemas a partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf add issue <Issue Name>`

      Inclua o nome do problema como ele aparecerá no [!DNL Workfront] interface.

      Adiciona um problema ao [!DNL Workfront]

      Para obter mais informações sobre como adicionar problemas ao [!DNL Workfront] from [!DNL Slack], consulte a seção &quot;Criação de problemas a partir de [!DNL Slack]&quot; na seção [Criar tarefas e problemas a partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf favorites`

      Exibe a lista de [!DNL Workfront] Favoritos.

      Para obter mais informações sobre como acessar seus Favoritos no [!DNL Slack], consulte o [Acessar seu [!UICONTROL Favoritos] Listar de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-favorites) na seção [Acessar seus favoritos e itens recentes de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) artigo 10. o

   * `/wf recent`

      Exibe a lista dos itens acessados mais recentemente em [!DNL Workfront].

      Para obter mais informações sobre como acessar os Itens recentes de [!DNL Slack], consulte o [Acessar seu [!UICONTROL Itens recentes] Listar de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-recent-items) section in the [[!UICONTROL Access your favorites] e [!UICONTROL itens recentes de [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) artigo 10. o

   * `wf tasks`

      Exibe uma lista de suas tarefas.

      Para obter mais informações sobre como gerenciar suas tarefas no [!DNL Slack]consulte &quot;Gerenciando suas Tarefas de [!DNL Slack]&quot; na seção [Gerenciar seu trabalho e aprovações de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf issues`

      Exibe uma lista de seus problemas.

      Para obter mais informações sobre como gerenciar seus problemas no [!DNL Slack], consulte &quot;Gerenciando seus problemas do [!DNL Slack]&quot; na seção [Gerenciar seu trabalho e aprovações de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf approvals` Exibe a [!DNL Workfront] aprovações.\

      Para obter mais informações sobre como gerenciar suas aprovações no [!DNL Slack], consulte &quot;Gerenciando suas aprovações de [!DNL Slack]&quot; na seção [Gerencie seu trabalho e suas aprovações no [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf search <keyword>`

      Incluir palavra-chave.

      Procure por uma palavra-chave específica. Você pode pesquisar os seguintes tipos de objetos:

      * Projeto
      * Tarefa
      * Problema
      * Relatório
      * Pessoas
      * Modelo
      * Documento
      * Portfólio
      * Programa
      * Painel de Controle
      * Empresa
      * Nota  \

         Para obter mais informações sobre como pesquisar em [!DNL Slack], consulte [Procurar por [!DNL Adobe Workfront] itens do Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/search-for-wf-items-from-slack.md).
   * `/wf log in`

      Faça logon no [!DNL Workfront] from [!DNL Slack].

   * `/wf log out `

      Faz logout de [!DNL Workfront] from [!DNL Slack]. Você permanece conectado no [!DNL Workfront] se você tiver um [!DNL Workfront] abra a instância em outra guia do navegador em outro aplicativo.
   * `/wf settings`

      Fornece acesso à configuração do [!DNL Workfront] configurações em [!DNL Slack].

      Para obter informações sobre como configurar [!DNL Workfront] no Slack, consulte [Definir configurações](#configure-settings-configure-settings).

   * `/wf help`
Exibe uma lista completa de comandos para [!DNL Workfront].


   * `Visit Workfront Help`: Abre a variável [!UICONTROL Slack] seção sobre [!DNL Workfront] Site da Ajuda em uma nova guia do navegador.


1. (Opcional) Para excluir a mensagem de qualquer comando, passe o mouse sobre o canto superior direito da mensagem do Slack que contém o comando e clique em &#x200B;**[!UICONTROL Mostrar ações da mensagem]**, depois clique em **[!UICONTROL Excluir mensagem]**.

1. (Opcional e condicional) Clique em **[!UICONTROL Excluir]** para confirmar que deseja excluir esta mensagem.

### Acesso [!DNL Workfront] de um link compartilhado em [!DNL Slack] {#access-workfront-from-a-shared-link-in-slack}

Você pode acessar [!DNL Workfront] objetos de um link para os objetos compartilhados com você em [!DNL Slack].

Para obter mais informações sobre como acessar [!DNL Workfront] em um link compartilhado, consulte [Acesso [!DNL Adobe Workfront] objetos de um link compartilhado em [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-wf-objects-from-shared-linked-in-slack.md).

## Definir configurações {#configure-settings}

1. Dentro de um [!DNL Slack] campo de mensagem, digite o seguinte comando:

   `/workfront settings`

   Ou

   `/wf settings`

   ![](assets/slack-configuring-settings-350x302.png)

   Todas as configurações são ativadas por padrão.

1. Desmarque as seguintes opções para desativar as configurações do Workfront:

   * No **[!UICONTROL Configurações gerais]** , desative a **[!UICONTROL Ao colar um [!DNL Workfront] URL em um [!DNL Slack] canal, mostrar descrição adicional, data de vencimento ou nome do solicitante]**&#x200B; se você não quiser [!DNL Slack] para adicionar mais informações sobre o [!DNL Workfront] objetos ao compartilhar um URL para o objeto em [!UICONTROL Slack].

   * No **[!UICONTROL Configurações de notificações]** , desative as notificações que deseja parar de receber do Workfront.\

      Para obter informações sobre como receber [!DNL Workfront] notificações em [!DNL Slack], consulte [Receber [!DNL Adobe Workfront] notificações em [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Fazer logoff de [!DNL Workfront] from [!DNL Slack]

1. Dentro de um [!DNL Slack] campo de mensagem, digite o seguinte comando:\
   `/workfront log out` Ou\
   `/wf log out`\
   Você recebe uma confirmação de que foi desconectado de [!DNL Workfront].\
   Você permanece conectado no [!DNL Workfront] se você tiver um [!DNL Workfront] abra a instância em outra guia do navegador em outro aplicativo.
