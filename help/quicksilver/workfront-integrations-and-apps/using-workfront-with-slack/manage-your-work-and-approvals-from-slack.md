---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Gerencie seu trabalho e suas aprovações no Slack
description: Você pode acessar a Lista de trabalho da página inicial, revisar e concordar em trabalhar em tarefas e problemas e revisar ou tomar decisões sobre aprovações diretamente do Slack.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 802a2f16-d827-455e-9e49-f58f4c5fc482
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '907'
ht-degree: 1%

---

# Gerenciar seu trabalho e suas aprovações de [!DNL Slack]

Depois de instalar o [!DNL Adobe Workfront for Slack], você pode fazer o seguinte:

* Acessar listas de itens da sua [!UICONTROL Página Inicial] de [!DNL Slack]
* Revisar e aceitar para trabalhar em tarefas e problemas de [!DNL Slack]
* Revisar e tomar decisões sobre aprovações de [!DNL Slack]

Para obter mais informações sobre a configuração de [!DNL Workfront] com [!DNL Slack], consulte [Configurar [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Requisitos de acesso

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

## Pré-requisitos

Antes de gerenciar seu trabalho e suas aprovações do [!DNL Slack], você deve

* Configurar [!DNL Workfront for Slack]\
  Para obter instruções sobre como configurar o [!DNL Workfront for Slack], consulte [Configurar [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Gerencie seu trabalho a partir de [!DNL Slack]

1. Faça logon em sua instância do [!DNL Slack] e em [!DNL Workfront] a partir de [!DNL Slack].\
   Para obter mais informações sobre como fazer logon no [!DNL Workfront] a partir de [!DNL Slack], consulte a seção &quot;Logon no [!DNL Workfront] a partir de [!DNL Slack]&quot; no [Acesso [!DNL Adobe Workfront] a partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. De qualquer canal, comece digitando o seguinte comando no campo de mensagem:

   `/workfront home`

   >[!NOTE]
   >
   >* Os comandos diferenciam maiúsculas de minúsculas.
   >* Você pode iniciar seu comando com `/wf` em vez de `/workfront`.

   Os botões dos quais você pode acessar listas de tarefas, problemas e aprovações são exibidos. Clicar em um dos botões exibe os primeiros 20 itens de cada lista em [!DNL Slack].

1. (Opcional) Clique em **[!UICONTROL Tarefas]** para exibir todas as suas tarefas.

   Para obter mais informações sobre como gerenciar tarefas no [!DNL Slack], consulte [Gerenciando suas Tarefas de [!DNL Slack]](#manage-your-tasks-from-slack-manage-your-tasks-from-slack).

1. (Opcional) Clique em **[!UICONTROL Problemas]** para exibir todos os seus problemas.

   Para obter mais informações sobre o gerenciamento de problemas no [!DNL Slack], consulte [Gerenciando seus problemas do [!DNL Slack]](#manage-your-issues-from-slack-manage-your-issues-from-slack).

1. (Opcional) Clique em **[!UICONTROL Aprovações]** para exibir todas as aprovações que estão aguardando sua decisão.\
   Para obter mais informações sobre como gerenciar suas aprovações no [!DNL Slack], consulte [Gerenciar suas aprovações do [!DNL Slack]](#manage-your-approvals-from-slack-manage-your-approvals-from-slack).

## Gerencie suas tarefas em [!DNL Slack] {#manage-your-tasks-from-slack}

1. Faça logon em sua instância do [!DNL Slack] e em [!DNL Workfront] a partir de [!DNL Slack].\
   Para obter informações sobre como fazer logon no [!DNL Workfront] a partir de [!DNL Slack], consulte a seção &quot;Logon no [!DNL Workfront] a partir de [!DNL Slack]&quot; no [Acesso [!DNL Adobe Workfront] a partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Em qualquer canal, comece digitando um dos seguintes comandos no campo de mensagem:

   `/workfront home`, depois clique em **[!UICONTROL Tarefas]**

   Ou

   `/workfront tasks`

   >[!NOTE]
   >
   >* Os comandos diferenciam maiúsculas de minúsculas.
   >* Você pode iniciar seu comando com `/wf` em vez de `/workfront`.

   As primeiras 20 tarefas na lista são exibidas.

1. Clique em **[!UICONTROL +`<remaining number>` mais]** para exibir tarefas adicionais.
1. Considere revisar as seguintes informações sobre os itens de trabalho:

   * **[!UICONTROL Nome]**
   * **[!UICONTROL Nome do Projeto]** ou **[!DNL Parent Object Name]**

   * **[!DNL Planned Completion Date]** do item de trabalho.
   * **[!DNL Assigned By Name]**: este é o nome do usuário que atribuiu a tarefa a você.
   * **[!UICONTROL Status]**

1. (Opcional) Clique no nome de um item para abri-lo no Workfront em uma guia do navegador separada.
1. (Opcional) No campo **[!UICONTROL Status]**, selecione um novo Status.
1. (Opcional) Clique em **[!UICONTROL Registrar Tempo]**, em seguida selecione um **[!UICONTROL Tipo de Hora]** e um valor de hora para registrar o tempo no item.

   >[!NOTE]
   >
   >* Você só pode registrar horas em incrementos de uma hora completa ou de meia hora, até 12 horas e 30 minutos.
   >* As horas registradas têm uma Data de entrada de hoje. Você não pode registrar horas para uma data passada ou futura de [!DNL Slack].

   Você receberá uma confirmação de que a hora foi registrada.

1. (Opcional) Clique em **[!UICONTROL Trabalhar nisto]** para aceitar trabalhar em uma tarefa. O botão [!UICONTROL Trabalhar nisto] desaparece.

## Gerenciar seus problemas a partir do [!DNL Slack] {#manage-your-issues-from-slack}

1. Faça logon em sua instância do [!DNL Slack] e em [!DNL Workfront] a partir de [!DNL Slack].\
   Para obter mais informações sobre como fazer logon no [!DNL Workfront] a partir de [!DNL Slack], consulte o [Logon no [!DNL Workfront] a partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#logging-in-to-workfront) section in [Access [!DNL Adobe Workfront] a partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Em qualquer canal, comece digitando um dos seguintes comandos no campo de mensagem:

   `/workfront home`, depois clique em **[!UICONTROL Problemas]**

   Ou

   `/workfront issues`

   >[!NOTE]
   >
   >* Os comandos diferenciam maiúsculas de minúsculas.
   >* Você pode iniciar seu comando com `/wf` em vez de `/workfront`.

   As primeiras 20 ocorrências na lista são exibidas.

1. Clique em **[!UICONTROL + restante(s) `<number>` mais]** para exibir itens adicionais.
1. Considere revisar as seguintes informações sobre os itens de trabalho:

   * **[!UICONTROL Nome]**
   * Nome do **[!UICONTROL Projeto]** ou Nome do Objeto Pai
   * **[!UICONTROL Data de conclusão]**: esta é a Data de conclusão planejada do item de trabalho.
   * Nome do **[!DNL Requested by]**: este é o Contato Primário (para problemas) ou o usuário que fez a atribuição (para tarefas).

1. (Opcional) Clique no nome do problema para abri-lo no Workfront em uma guia do navegador separada.
1. (Opcional) Clique em **[!DNL Work on it]** para começar a trabalhar em problemas que você ainda não aceitou.

   O botão [!UICONTROL Trabalhar nisto] desaparece.

## Gerenciar suas aprovações de [!DNL Slack] {#manage-your-approvals-from-slack}

1. Faça logon em sua instância do [!DNL Slack] e em [!DNL Workfront] a partir de [!DNL Slack].\
   Para obter mais informações sobre como fazer logon no [!DNL Workfront] a partir de [!DNL Slack], consulte a seção &quot;Logon no [!DNL Workfront] a partir de [!DNL Slack]&quot; no [Acesso [!DNL Adobe Workfront] a partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Em qualquer canal, comece digitando um dos seguintes comandos no campo de mensagem:

   `/workfront home`, depois clique em **[!UICONTROL Aprovações]**

   Ou

   `/workfront approvals`

   >[!NOTE]
   >
   >* Os comandos diferenciam maiúsculas de minúsculas.
   >* Você pode iniciar seu comando com `/wf` em vez de `/workfront`.

   Os primeiros 20 itens na lista de **[!UICONTROL Aprovações]** são exibidos. Informações adicionais sobre os itens também são exibidas, como o nome do usuário que o solicitou ou o nome do projeto ao qual o item pertence.

1. Clique em **[!UICONTROL + restante(s) `<number>` mais]** para exibir itens adicionais.

1. Considere o gerenciamento de aprovações para os seguintes objetos:

   * **Projetos**

     Clique em **[!UICONTROL Aprovar]** ou **[!UICONTROL Rejeitar]** para aceitar ou rejeitar a alteração de status de um projeto.

   * **Tarefas**

     Clique em **[!UICONTROL Aprovar]** ou **[!UICONTROL Rejeitar]** para aceitar ou rejeitar a alteração de status de uma tarefa.

   * **Problemas**

     Clique em **[!UICONTROL Aprovar]** ou **[!DNL Reject]** para aceitar ou rejeitar a alteração de status de um problema.

   * **Documentos**

     Clique em **[!UICONTROL Aprovar]** para aprovar um documento, **[!UICONTROL Rejeitar]** para rejeitá-lo ou **[!UICONTROL Alterações]** para indicar que você o aprova, mas que o documento precisa de alterações adicionais.\
     (Opcional) Passe o mouse sobre a miniatura do documento para clicar na lupa e visualizar o documento.

   * **Provas**&#x200B;Clique no nome da prova para abri-la em [!DNL Workfront], em uma guia separada, e gerenciar a aprovação.
   * **Solicitações de Acesso**

     Clique em **[!UICONTROL Conceder Acesso]** para conceder permissões aprimoradas ao objeto solicitado ou **[!UICONTROL Ignorar]** para ignorar a solicitação de mais acesso.

1. (Opcional) Clique no nome do objeto enviado para aprovação para abri-lo no [!DNL Workfront] em uma nova guia do navegador.
