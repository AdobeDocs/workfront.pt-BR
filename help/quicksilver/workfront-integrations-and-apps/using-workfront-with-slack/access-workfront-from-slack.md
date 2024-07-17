---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Acessar [!DNL Adobe Workfront] de [!DNL Slack]
description: A integração [!DNL Adobe Workfront] com [!DNL Slack] permite acessar [!DNL Workfront] do Slack ou executar determinadas ações [!DNL Workfront] usando um comando de barra. A integração pode ser usada em qualquer ambiente  [!DNL Slack] , incluindo o aplicativo móvel  [!DNL Slack] .
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5f531217-3bd6-4156-8b9f-eabc95d4df10
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '1077'
ht-degree: 1%

---

# Acessar [!DNL Adobe Workfront] de [!DNL Slack]

Integrar [!DNL Adobe Workfront] com [!DNL Slack] permite que você acesse [!DNL Workfront] de [!DNL Slack] ou execute determinadas ações em [!DNL Workfront] usando um comando de barra. A integração pode ser usada de qualquer ambiente [!DNL Slack], incluindo o aplicativo móvel [!DNL Slack].

Você ou o administrador do [!DNL Slack] deve instalar o aplicativo [!DNL Workfront] na instância do [!DNL Slack] antes de usar o [!DNL Workfront] no [!DNL Slack]. Para obter mais informações, consulte [Configurar Adobe Workfront para Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Sobre comandos de barra {#about-slash-commands}

Ao usar [!DNL Slack], você digita mensagens dentro de um campo de mensagem. Quando você inicia a mensagem com uma barra, ela se torna um comando e se comporta de forma diferente de uma mensagem simples. O comando informa [!DNL Slack] para executar uma ação.

Você pode acessar sua instância [!DNL Workfront] de [!DNL Slack] digitando um comando de barra em qualquer canal [!DNL Slack].

Lembre-se do seguinte ao usar um comando de barra em [!DNL Slack] para acessar [!DNL Workfront]:

* Os comandos de barra fazem distinção entre maiúsculas e minúsculas.
* Os comandos para [!DNL Workfront] só são visíveis para você, independentemente do canal em que você os está digitando.
* O comando deve sempre iniciar com `/workfront` ou `/wf`, seguido por um espaço e o nome de uma ação que você deseja executar em [!DNL Workfront].

  Isso indica que seu comando se destina ao aplicativo [!DNL Workfront]. Os comandos para [!DNL Workfront] funcionam somente quando você já configurou o aplicativo [!DNL Workfront] com sua instância [!DNL Slack].

Para obter uma lista de todos os comandos que você pode executar do Slack para [!DNL Workfront], consulte [Acesso [!DNL Workfront] de um comando de barra em [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack).

## Fazer logon em [!DNL Workfront] a partir de [!DNL Slack] {#log-in-to-workfront-from-slack}

Ao digitar qualquer comando no campo de mensagem em Slack, você será solicitado a fazer logon em [!DNL Workfront] primeiro.\
Para obter uma lista completa dos comandos [!DNL Workfront] de [!DNL Slack], consulte o [Acesso [!DNL Workfront] de um comando de barra na seção  [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack) deste artigo.

Para fazer login em [!DNL Workfront] a partir de [!DNL Slack]:

1. Faça logon na instância do [!DNL Slack].
1. Em qualquer canal, digite um dos seguintes comandos:\
   `/workfront log in`

   Ou

   `/wf log in`

1. Clique no link [!DNL Workfront] **[!UICONTROL Fazer Logon]** exibido na resposta.\
   Uma nova guia é aberta com campos para credenciais [!DNL Workfront].

1. Siga as instruções para fazer logon no [!DNL Workfront] usando a Autenticação Aprimorada, o OAuth 2.0 ou a URL da Linguagem de Marcação de Asserção de Segurança (SAML).

   >[!NOTE]
   >
   >* Quando for solicitado que você insira o host da sua conta do [!DNL Workfront], digite-o usando este formato: *yourCompany&#39;sDomain.my.workfront.com*. O domínio da sua empresa geralmente é o nome da sua empresa.
   >* A Autenticação Aprimorada não estará disponível até que um administrador do [!DNL Workfront] a habilite para esta integração.


   A página de configuração para [!DNL Workfront] notificações em [!DNL Slack] é aberta.

1. (Opcional) Desative todas as notificações do [!DNL Workfront] que você não deseja receber em [!DNL Slack].

   Para obter informações sobre como definir as configurações de [!DNL Workfront] para [!DNL Slack], consulte a seção [Definir configurações](#configure-settings-configure-settings) neste artigo

1. Navegue de volta para o canal [!DNL Slack].

   Você está conectado ao [!DNL Workfront] a partir da sua instância [!DNL Slack].

## Acessar [!DNL Workfront] de [!DNL Slack]

* [Sobre comandos de barra](#about-slash-commands-about-slash-commands)
* [Acessar [!DNL Workfront] de um link compartilhado em [!DNL Slack]](#access-workfront-from-a-shared-link-in-slack-access-workfront-from-a-shared-link-in-slack)

## Acessar [!DNL Workfront] de um comando de barra em [!DNL Slack] {#access-workfront-from-a-slash-command-in-slack}

1. Faça logon em sua instância do [!DNL Slack] e em [!DNL Workfront] a partir de [!DNL Slack].\
   Para obter mais informações sobre como fazer logon no [!DNL Workfront] a partir de [!DNL Slack], consulte [Fazer logon no [!DNL Workfront] a partir de [!DNL Slack]](#log-in-to-workfront-from-slack-log-in-to-workfront-from-slack)

1. De qualquer canal, comece digitando o seguinte comando no campo de mensagem:

   `/workfront help`

   Ou

   `/wf help`

1. Selecione um dos seguintes comandos:

   * `/wf home`

     Exibe botões nos quais você pode acessar listas de tarefas, problemas e aprovações. Clicar em um dos botões exibe os primeiros 20 itens de cada lista em [!DNL Slack].

     Para obter mais informações sobre como gerenciar itens de trabalho do [!DNL Workfront] a partir do [!DNL Slack], consulte [Gerenciar seu trabalho e aprovações a partir do [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf add task <TaskName>`

     Inclua o nome da tarefa como ele aparecerá na interface [!DNL Workfront].

     Adiciona uma tarefa a [!DNL Workfront].

     Para obter mais informações sobre como adicionar tarefas a [!DNL Workfront] do Slack, consulte a seção &quot;Criando Tarefas a partir de [!DNL Slack]&quot; em [Criar tarefas e problemas a partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf add issue <Issue Name>`

     Inclua o nome do problema como ele aparecerá na interface [!DNL Workfront].

     Adiciona um problema a [!DNL Workfront]

     Para obter mais informações sobre como adicionar problemas a [!DNL Workfront] a partir de [!DNL Slack], consulte a seção &quot;Criando problemas a partir de [!DNL Slack]&quot; em [Criar tarefas e problemas a partir de  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf favorites`

     Exibe a lista dos Favoritos do [!DNL Workfront].

     Para obter mais informações sobre como acessar seus Favoritos do [!DNL Slack], consulte a seção [Acessando sua Lista de [!UICONTROL Favoritos] do [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-favorites) no artigo [Acessando seus Favoritos e Itens Recentes do [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md).

   * `/wf recent`

     Exibe a lista dos itens acessados mais recentemente em [!DNL Workfront].

     Para obter mais informações sobre como acessar seus Itens Recentes do [!DNL Slack], consulte o artigo [Acessando seus [!UICONTROL Itens Recentes] da Lista do [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-recent-items) section in the [[!UICONTROL Access your favorites] e [!UICONTROL itens recentes do [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md).

   * `wf tasks`

     Exibe uma lista de tarefas.

     Para obter mais informações sobre como gerenciar suas tarefas do [!DNL Slack], consulte a seção &quot;Gerenciando suas Tarefas do [!DNL Slack]&quot; em [Gerenciando seu Trabalho e Aprovações do [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf issues`

     Exibe uma lista de seus problemas.

     Para obter mais informações sobre como gerenciar seus problemas do [!DNL Slack], consulte a seção &quot;Gerenciando seus problemas do [!DNL Slack]&quot; em [Gerenciando seu trabalho e suas aprovações do [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf approvals` Exibe suas [!DNL Workfront] aprovações.\

     Para obter mais informações sobre como gerenciar suas aprovações do [!DNL Slack], consulte a seção &quot;Gerenciando suas Aprovações do [!DNL Slack]&quot; em [Gerenciar seu trabalho e aprovações do [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf search <keyword>`

     Incluir palavra-chave.

     Procure por uma palavra-chave específica. Você pode pesquisar pelos seguintes tipos de objetos:

      * Projeto
      * Tarefa
      * Problema
      * Relatório
      * Pessoas
      * Modelo
      * Documento
      * Portfólio
      * Programa
      * Painel
      * Empresa
      * Nota \

        Para obter mais informações sobre a pesquisa no [!DNL Slack], consulte [Pesquisar [!DNL Adobe Workfront] itens do Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/search-for-wf-items-from-slack.md).
   * `/wf log in`

     Faz logon em [!DNL Workfront] de [!DNL Slack].

   * `/wf log out `

     Faz logoff de [!DNL Workfront] de [!DNL Slack]. Você continuará conectado ao [!DNL Workfront] se tiver uma instância [!DNL Workfront] separada aberta em outra guia do navegador em outro aplicativo.
   * `/wf settings`

     Fornece acesso para definir suas configurações do [!DNL Workfront] no [!DNL Slack].

     Para obter informações sobre como definir as configurações de [!DNL Workfront] no Slack, consulte [Definir configurações](#configure-settings-configure-settings).

   * `/wf help`
Exibe uma lista completa de comandos para [!DNL Workfront].


   * `Visit Workfront Help`: Abre a seção [!UICONTROL Slack] no Site de Ajuda [!DNL Workfront] em uma nova guia do navegador.


1. (Opcional) Para excluir a mensagem de qualquer comando, passe o mouse sobre o canto superior direito da mensagem Slack que contém o comando e clique em&#x200B;**[!UICONTROL Mostrar ações da mensagem]**, depois clique em **[!UICONTROL Excluir mensagem]**.

1. (Opcional e condicional) Clique em **[!UICONTROL Excluir]** para confirmar que deseja excluir esta mensagem.

### Acessar [!DNL Workfront] de um link compartilhado em [!DNL Slack] {#access-workfront-from-a-shared-link-in-slack}

Você pode acessar [!DNL Workfront] objetos de um link para esses objetos que é compartilhado com você no [!DNL Slack].

Para obter mais informações sobre como acessar [!DNL Workfront] de um link compartilhado, consulte [Acessar [!DNL Adobe Workfront] objetos de um link compartilhado em [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-wf-objects-from-shared-linked-in-slack.md).

## Definir configurações {#configure-settings}

1. Dentro de um campo de mensagem [!DNL Slack], digite o seguinte comando:

   `/workfront settings`

   Ou

   `/wf settings`

   Todas as configurações são ativadas por padrão.

1. Desmarque entre as seguintes opções para desativar as configurações do Workfront:

   * Na área **[!UICONTROL Configurações Gerais]**, desabilite a configuração **[!UICONTROL Ao colar a URL [!DNL Workfront] em um canal [!DNL Slack], mostre descrição adicional, data de vencimento ou nome do solicitante]**&#x200B;se você não quiser que [!DNL Slack] adicione mais informações sobre os objetos [!DNL Workfront] quando compartilhar uma URL com o objeto em [!UICONTROL Slack].

   * Na área **[!UICONTROL Configurações de notificações]**, desabilite as notificações que você deseja parar de receber do Workfront.\

     Para obter informações sobre como receber [!DNL Workfront] notificações em [!DNL Slack], consulte [Receber [!DNL Adobe Workfront] notificações em [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Sair de [!DNL Workfront] de [!DNL Slack]

1. Dentro de um campo de mensagem [!DNL Slack], digite o seguinte comando:\
   `/workfront log out` Ou\
   `/wf log out`\
   Você receberá uma confirmação de que foi desconectado do [!DNL Workfront].\
   Você continuará conectado ao [!DNL Workfront] se tiver uma instância [!DNL Workfront] separada aberta em outra guia do navegador em outro aplicativo.
