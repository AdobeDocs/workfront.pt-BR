---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Gerenciar seu trabalho e suas aprovações do Slack
description: Você pode acessar sua Lista de trabalho inicial, revisar e concordar em trabalhar em tarefas e problemas e revisar ou tomar decisões sobre aprovações diretamente do Slack.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 802a2f16-d827-455e-9e49-f58f4c5fc482
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 1%

---

# Gerencie seu trabalho e suas aprovações no [!DNL Slack]

Depois de instalar o [!DNL Adobe Workfront for Slack], você pode fazer o seguinte:

* Listas de acesso da sua [!UICONTROL Início] itens de [!DNL Slack]
* Revisar e aceitar o trabalho em tarefas e problemas do [!DNL Slack]
* Revisar e tomar decisões sobre aprovações a partir de [!DNL Slack]

Para obter mais informações sobre como configurar [!DNL Workfront] com [!DNL Slack], consulte [Configurar [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] plano</a>*</td> 
   <td> <p>[!UICONTROL Pro] ou superior</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Antes de gerenciar seu trabalho e aprovações da [!DNL Slack], você deve

* Configurar [!DNL Workfront for Slack]\
   Para obter instruções sobre como configurar [!DNL Workfront for Slack], consulte [Configurar [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Gerenciar seu trabalho do [!DNL Slack]

1. Faça logon no [!DNL Slack] instância e faça logon no [!DNL Workfront] from [!DNL Slack].\
   Para obter mais informações sobre como fazer logon no [!DNL Workfront] from [!DNL Slack], consulte o tópico &quot;Fazer logon no [!DNL Workfront] from [!DNL Slack]&quot; na seção [Acesso [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Em qualquer canal, comece a digitar o seguinte comando no campo de mensagem:

   `/workfront home`

   >[!NOTE]
   >
   >* Os comandos fazem distinção entre maiúsculas e minúsculas.
   >* Você pode iniciar seu comando com `/wf` em vez de `/workfront`.


   Os botões dos quais você pode acessar listas de suas tarefas, emissões e aprovações são exibidos. Clicar em um dos botões exibe os 20 primeiros itens de cada lista em [!DNL Slack].\
   ![](assets/slack-home-buttons-350x80.png)

1. (Opcional) Clique em **[!UICONTROL Tarefas]** para exibir todas as suas tarefas.

   Para obter mais informações sobre o gerenciamento de tarefas no [!DNL Slack], consulte [Gerenciando suas Tarefas de [!DNL Slack]](#manage-your-tasks-from-slack-manage-your-tasks-from-slack).

1. (Opcional) Clique em **[!UICONTROL Problemas]** para exibir todos os seus problemas.

   Para obter mais informações sobre o gerenciamento de problemas no [!DNL Slack], consulte [Gerencie seus problemas com o [!DNL Slack]](#manage-your-issues-from-slack-manage-your-issues-from-slack).

1. (Opcional) Clique em **[!UICONTROL Aprovações]** para exibir todas as aprovações aguardando sua decisão.\
   Para obter mais informações sobre como gerenciar suas aprovações no [!DNL Slack], consulte [Gerencie suas aprovações em [!DNL Slack]](#manage-your-approvals-from-slack-manage-your-approvals-from-slack).

## Gerencie suas tarefas de [!DNL Slack] {#manage-your-tasks-from-slack}

1. Faça logon no [!DNL Slack] instância e faça logon no [!DNL Workfront] from [!DNL Slack].\
   Para obter informações sobre como fazer logon no [!DNL Workfront] from [!DNL Slack], consulte o tópico &quot;Fazer logon no [!DNL Workfront] from [!DNL Slack]&quot; na seção [Acesso [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Em qualquer canal, comece a digitar um dos seguintes comandos no campo de mensagem:

   `/workfront home`, depois clique em **[!UICONTROL Tarefas]**

   Ou

   `/workfront tasks`

   >[!NOTE]
   >
   >* Os comandos fazem distinção entre maiúsculas e minúsculas.
   >* Você pode iniciar seu comando com `/wf` em vez de `/workfront`.


   As primeiras 20 tarefas na lista são exibidas.\
   ![](assets/slack-two-tasks-350x286.png)

1. Clique em **[!UICONTROL +`<remaining number>` more]** para exibir tarefas adicionais.
1. Considere revisar as seguintes informações sobre seus itens de trabalho:

   * **[!UICONTROL Nome]**
   * **[!UICONTROL Nome do projeto]** ou **[!DNL Parent Object Name]**

   * **[!DNL Planned Completion Date]** do item de trabalho.
   * **[!DNL Assigned By Name]**: esse é o nome do usuário que atribuiu a tarefa a você.
   * **[!UICONTROL Status]**

1. (Opcional) Clique no nome de um item para abri-lo no Workfront em uma guia separada do navegador.
1. (Opcional) Na seção **[!UICONTROL Status]** selecione um novo Status .
1. (Opcional) Clique em **[!UICONTROL Hora de registro]** e, em seguida, selecione um **[!UICONTROL Tipo de hora]** e uma quantidade de hora para registrar o tempo no item.

   >[!NOTE]
   >
   >* Você só pode registrar horas em incrementos de uma hora completa ou meia, até 12 horas e 30 minutos.
   >* As horas que você registra têm uma Data de entrada de hoje. Não é possível registrar o tempo para uma data passada ou futura a partir de [!DNL Slack].


   Você recebe uma confirmação de que a hora foi registrada.

1. (Opcional) Clique em **[!UICONTROL Trabalhe nele]** para aceitar trabalhar em uma tarefa. O [!UICONTROL Trabalhe nele] desaparece.

## Gerencie seus problemas no [!DNL Slack] {#manage-your-issues-from-slack}

1. Faça logon no [!DNL Slack] instância e faça logon no [!DNL Workfront] from [!DNL Slack].\
   Para obter mais informações sobre como fazer logon no [!DNL Workfront] from [!DNL Slack], consulte o [Logon em [!DNL Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#logging-in-to-workfront) section in [Access [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Em qualquer canal, comece a digitar um dos seguintes comandos no campo de mensagem:

   `/workfront home`, depois clique em **[!UICONTROL Problemas]**

   Ou

   `/workfront issues`

   >[!NOTE]
   >
   >* Os comandos fazem distinção entre maiúsculas e minúsculas.
   >* Você pode iniciar seu comando com `/wf` em vez de `/workfront`.


   Os primeiros 20 problemas na lista são exibidos.\
   ![](assets/slack-two-issues-350x323.png)

1. Clique em **[!UICONTROL + restante `<number>` more]** para exibir itens adicionais.
1. Considere revisar as seguintes informações sobre seus itens de trabalho:

   * **[!UICONTROL Nome]**
   * **[!UICONTROL Projeto]** Nome ou nome do objeto pai
   * **[!UICONTROL Devido a]** Data: Esta é a Data de Conclusão Planejada do item de trabalho.
   * **[!DNL Requested by]** Nome: Este é o Contato Principal (para problemas) ou o usuário que fez a atribuição (para tarefas).

1. (Opcional) Clique no nome do problema para abri-lo no Workfront em uma guia separada do navegador.
1. (Opcional) Clique em **[!DNL Work on it]** para começar a trabalhar em problemas que você ainda não aceitou.

   O [!UICONTROL Trabalhe nele] desaparece.

## Gerencie suas aprovações em [!DNL Slack] {#manage-your-approvals-from-slack}

1. Faça logon no [!DNL Slack] instância e faça logon no [!DNL Workfront] from [!DNL Slack].\
   Para obter mais informações sobre como fazer logon no [!DNL Workfront] from [!DNL Slack], consulte o tópico &quot;Fazer logon no [!DNL Workfront] from [!DNL Slack]&quot; na seção [Acesso [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Em qualquer canal, comece a digitar um dos seguintes comandos no campo de mensagem:

   `/workfront home`, depois clique em **[!UICONTROL Aprovações]**

   Ou

   `/workfront approvals`

   >[!NOTE]
   >
   >* Os comandos fazem distinção entre maiúsculas e minúsculas.
   >* Você pode iniciar seu comando com `/wf` em vez de `/workfront`.


   Os primeiros 20 itens em seu **[!UICONTROL Aprovações]** exibição de lista. Informações adicionais sobre os itens também são exibidas, como o nome do usuário que o solicitou ou o nome do projeto ao qual o item pertence.

1. Clique em **[!UICONTROL + restante `<number>` more]** para exibir itens adicionais.

   ![slack_access_approvals_list.png](assets/slack-access-approvals-list-350x213.png)

   ![](assets/slack-approve-a-document-350x362.png)

   ![](assets/slack-approve-task-notification-350x105.png)

1. Considere o gerenciamento de aprovações para os seguintes objetos:

   * **Projetos**

      Clique em **[!UICONTROL Aprovar]** ou **[!UICONTROL Rejeitar]** para aceitar ou rejeitar a alteração de status de um projeto.

   * **Tarefas**

      Clique em **[!UICONTROL Aprovar]** ou **[!UICONTROL Rejeitar]** para aceitar ou rejeitar a alteração de status de uma tarefa.

   * **Problemas**

      Clique em **[!UICONTROL Aprovar]** ou **[!DNL Reject]** para aceitar ou rejeitar a alteração de status de um problema.

   * **Documentos**

      Clique em **[!UICONTROL Aprovar]** para aprovar um documento, **[!UICONTROL Rejeitar]** para rejeitá-lo, ou **[!UICONTROL Alterações]** para indicar que você o aprova, mas que o documento precisa de alterações adicionais.\
      (Opcional) Passe o mouse sobre a miniatura do documento para clicar na lupa e visualizar o documento.

   * **Provas**&#x200B; Clique no nome da prova para abri-la em [!DNL Workfront] em uma guia separada e gerencie a aprovação.
   * **Solicitações de Acesso**

      Clique em **[!UICONTROL Conceder acesso]** para conceder permissões aprimoradas ao objeto solicitado, ou **[!UICONTROL Ignorar]** para ignorar a solicitação de mais acesso.

1. (Opcional) Clique no nome do objeto enviado para aprovação para abri-lo em [!DNL Workfront] em uma nova guia do navegador.
