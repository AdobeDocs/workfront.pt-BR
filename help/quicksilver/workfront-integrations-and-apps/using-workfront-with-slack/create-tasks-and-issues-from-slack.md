---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Criar tarefas e problemas do Slack
description: Depois de instalar e configurar o  [!DNL Adobe Workfront] para Slack, você pode criar tarefas e problemas com o Slack e associá-los a projetos no Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cf4a514a-fe69-4c2f-8e35-5738dfaab24e
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# Criar tarefas e problemas de [!DNL Slack]

Após instalar e configurar o [!DNL Adobe Workfront for Slack], você pode criar tarefas e problemas a partir do [!DNL Slack] e associá-los a projetos no [!DNL Workfront].

Para obter mais informações sobre a configuração de [!DNL Workfront] com [!DNL Slack], consulte [Configurar [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Você deve ter acesso para criar tarefas e problemas no seu Nível de Acesso e deve ter permissões do [!UICONTROL Contribute] no projeto ao qual você está associando-os.

Para obter mais informações sobre Níveis de Acesso, consulte [Visão geral sobre Níveis de Acesso](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md). Para obter mais informações sobre permissões para objetos, consulte [Visão geral das permissões de compartilhamento em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/br/products/workfront/pricing.html" target="_blank">[!DNL [!DNL Adobe Workfront] plano]</a>*</td> 
   <td> <p>[!UICONTROL Pro] ou superior</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].\

## Pré-requisitos

Antes de criar tarefas e problemas a partir de [!DNL Slack], você deve

* Configurar o [!DNL Workfront] para o Slack\
   Para obter instruções sobre como configurar o [!DNL Workfront for Slack], consulte [Configurar [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Criar tarefas de [!DNL Slack]

1. Faça logon em sua instância do [!DNL Slack] e em [!DNL Workfront] a partir de [!DNL Slack].\
   Para obter mais informações sobre como fazer logon no Workfront a partir de [!DNL Slack], consulte a seção &quot;Fazendo Logon no [!DNL Workfront] a partir de [!DNL Slack]&quot; no [Acesso [!DNL Adobe Workfront] a partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. De qualquer canal, comece digitando o seguinte comando no campo de mensagem:

   `/workfront add task <Task Name>`

   >[!NOTE]
   >
   >Os comandos diferenciam maiúsculas de minúsculas. Você pode iniciar seu comando com `/wf` em vez de `/workfront`.
   >  
   >O Nome da Tarefa deve ser inserido como aparecerá na interface [!DNL Workfront], sem colchetes ou aspas.

1. (Opcional) Comece digitando o nome de um projeto ao qual deseja associar a nova tarefa e selecione-o quando ele aparecer na lista.\
   Você recebe uma confirmação indicando que a tarefa foi adicionada ao projeto selecionado.
1. (Opcional) Clique no nome da tarefa na mensagem de confirmação para abri-la no [!DNL Workfront], em uma nova guia do navegador.

## Criar problemas a partir de [!DNL Slack]

1. Faça logon em sua instância do [!DNL Slack] e em [!DNL Workfront] a partir de [!DNL Slack].\
   Para obter mais informações sobre como fazer logon no [!DNL Workfront] a partir de [!DNL Slack], consulte a seção &quot;Logon no [!DNL Workfront] a partir de [!DNL Slack]&quot; no [Acesso [!DNL Adobe Workfront] a partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. De qualquer canal, comece digitando o seguinte comando no campo de mensagem:

   `/workfront add issue <Issue Name>`

   >[!NOTE]
   >
   >Os comandos diferenciam maiúsculas de minúsculas. Você pode iniciar seu comando com &#39;/wf&#39; em vez de &#39;/workfront.&#39; \
   >O Nome do Problema deve ser inserido como aparecerá na interface [!DNL Workfront], sem colchetes ou aspas.

1. (Opcional) Comece digitando o nome de um projeto com o qual deseja associar a nova ocorrência e selecione-o quando ele aparecer na lista.\
   Você recebe uma confirmação indicando que o problema foi adicionado ao projeto selecionado.
1. (Opcional) Clique no nome do problema na mensagem de confirmação para abri-lo no [!DNL Workfront], em uma nova guia do navegador.
