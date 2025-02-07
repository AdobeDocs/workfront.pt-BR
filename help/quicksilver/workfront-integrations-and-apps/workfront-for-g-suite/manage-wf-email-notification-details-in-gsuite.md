---
product-area: workfront-integrations
keywords: google,doc,documento,planilha,slide
navigation-topic: workfront-for-g-suite
title: Gerenciar [!DNL Adobe Workfront] detalhes de notificação do Google Workspace
description: No Google Workspace, ao abrir um email de notificação que o Adobe [!DNL Workfront] tenha enviado, você poderá exibir os detalhes do item de trabalho associado e responder sem sair da Caixa de entrada. Se as ações estiverem disponíveis, como a aprovação de uma solicitação, você poderá executar essas ações diretamente do Workfront para o Google Workspace.
author: Becky
feature: Workfront Integrations and Apps
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 1%

---

# Gerenciar detalhes de notificação de [!DNL Adobe Workfront] de [!DNL Google Workspace]

>[!NOTE]
>
>A versão mais recente do plug-in do Adobe Workfront para Google foi lançada em 26 de junho de 2023.

Em [!DNL Google Workspace], quando você abre um email de notificação enviado por [!DNL Adobe Workfront], é possível exibir os detalhes do item de trabalho associado e responder sem sair da [!UICONTROL Caixa de entrada]. Se ações estiverem disponíveis, como a aprovação de uma solicitação, você poderá executar essas ações diretamente de [!DNL Workfront for Google Workspace].

>[!NOTE]
>
> O [!DNL Workfront for Google Workspace] oferece suporte a quase todos os tipos de notificações por email que você pode receber do [!DNL Workfront] (cerca de 120 tipos diferentes). Os emails [!UICONTROL Resumo diário] enviados de [!DNL Workfront] não aparecem em [!DNL Workfront for Google Workspace]. Para obter informações sobre os tipos de notificação por email do [!DNL Workfront], consulte [Modificar suas próprias notificações por email](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Trabalho], [!UICONTROL Plano]</p> </td> 
  </tr> 
  </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

## Pré-requisitos

Antes de gerenciar os detalhes de notificação de [!DNL Google Workspace], você deve

* Instalar [!DNL Workfront for Google Workspace]\
   Para obter instruções, consulte [Instalar [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Gerenciar detalhes de notificação de [!DNL Adobe Workfront] de [!DNL Google Workspace]

1. Se o painel [!DNL Workfront for Google Workspace] não for exibido, clique no ícone [!DNL Workfront] ![ícone do Workfront](assets/wf-lion-icon.png) na barra lateral de complementos [!DNL Google Workspace] na extremidade direita da página.
1. Em [!DNL Google Workspace], abra um email de notificação [!DNL Workfront].
1. Clique em **[!UICONTROL Exibir todas as atualizações]** se ele for exibido próximo à parte superior do painel.
1. Clique em **[!UICONTROL Detalhes]**.
1. Clique em qualquer opção disponível.

   As opções exibidas estão relacionadas ao tipo de notificação por email que você abriu. Por exemplo, se for uma notificação por email solicitando a aprovação de uma tarefa, você verá **[!UICONTROL Aprovar]** e **[!UICONTROL Rejeitar]** em vez de opções como **[!UICONTROL Trabalhar nela]** ou **[!UICONTROL Concluído]**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Tipo de notificação por email</th> 
      <th>Ação</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>Tarefa ou problema</td> 
      <td><strong>[!UICONTROL Aprovar]</strong> ele, <strong>[!UICONTROL Rejeitar]</strong> ele, <strong>[!UICONTROL Conceder]</strong> acesso a ele, <strong>[!UICONTROL Ignorar]</strong> uma solicitação de acesso a ele, <strong>[!UICONTROL Trabalhar nele]</strong>, ou clique em uma opção para indicar que você está <strong>[!UICONTROL Concluído]</strong> com ele</td> 
     </tr> 
     <tr> 
      <td>Projeto</td> 
      <td><strong>[!UICONTROL Aprovar]</strong>, <strong>[!UICONTROL Rejeitar]</strong>, <strong>[!UICONTROL Conceder]</strong> acesso a ele ou <strong>[!UICONTROL Ignorar]</strong> uma solicitação de acesso a ele</td> 
     </tr> 
     <tr> 
      <td>Documento</td> 
      <td><strong>[!UICONTROL Aprovar]</strong>, <strong>[!UICONTROL Rejeitar]</strong>, <strong>[!UICONTROL Conceder]</strong> acesso a ele ou <strong>[!UICONTROL Ignorar]</strong> uma solicitação de acesso a ele</td> 
     </tr> 
     <tr> 
      <td>Atualizar </td> 
      <td> <p>Exiba qualquer parte da lista inteira de atualizações do item para que você tenha o contexto necessário para <strong>[!UICONTROL Postagem]</strong> uma nova atualização ou uma <strong>[!UICONTROL Resposta]</strong>. Você pode clicar em <strong>[!UICONTROL Notify]</strong> para alertar usuários específicos sobre sua resposta. </p> <p>Para obter mais informações, consulte <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref">Responder a uma notificação de atualização de [!DNL Adobe Workfront] de [!DNL Google Workspace]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Solicitação de aprovação</td> 
      <td><strong>[!UICONTROL Aprovar]</strong> ou <strong>[!UICONTROL Rejeitar]</strong> ele (você pode mudar de ideia clicando na outra opção), baixá-lo, exibir seu proprietário ou exibir seu número de referência</td> 
     </tr> 
     <tr> 
      <td>Uma alteração no status de um projeto</td> 
      <td> Visualize todas as informações atuais sobre o projeto, incluindo formulários personalizados. </td> 
     </tr> 
    </tbody> 
   </table>
