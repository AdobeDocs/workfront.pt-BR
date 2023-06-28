---
product-area: workfront-integrations
keywords: google,doc,documento,planilha,slide
navigation-topic: workfront-for-g-suite
title: Gerenciar [!DNL Adobe Workfront] detalhes da notificação do G Suite
description: No G Suite, ao abrir um Adobe de email de notificação [!DNL Workfront] tiver enviado, você poderá visualizar os detalhes do item de trabalho associado e responder sem sair da sua Caixa de entrada. Se as ações estiverem disponíveis, como a aprovação de uma solicitação, você poderá executar essas ações diretamente do Workfront para G Suite.
author: Becky
feature: Workfront Integrations and Apps
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
source-git-commit: 4b95828dc3e6a67c4dbefb46f173303c519643a9
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 1%

---

# Gerenciar [!DNL Adobe Workfront] detalhes da notificação de [!DNL G Suite]

>[!NOTE]
>
>A versão mais recente do plug-in do Adobe Workfront para Google foi lançada em 26 de junho de 2023.

Entrada [!DNL G Suite], quando você abre um email de notificação [!DNL Adobe Workfront] tiver enviado, você poderá exibir os detalhes do item de trabalho associado e responder sem sair da sua [!UICONTROL Caixa de entrada]. Se as ações estiverem disponíveis, como a aprovação de uma solicitação, você poderá executar essas ações diretamente de [!DNL Workfront for G Suite].

>[!NOTE]
>
> [!DNL Workfront for G Suite] O suporta quase todos os tipos de notificação por email que você pode receber do [!DNL Workfront] (cerca de 120 tipos diferentes). [!UICONTROL Resumo diário] emails enviados de [!DNL Workfront] não aparecem em [!DNL Workfront for G Suite]. Para obter informações sobre o [!DNL Workfront] tipos de notificação por email, consulte [Ativar ou desativar suas próprias notificações de eventos](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Trabalho], [!UICONTROL Plano]</p> </td> 
  </tr> 
  </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

## Pré-requisitos

Antes de gerenciar os detalhes da notificação no [!DNL G Suite], você deve

* Instalar [!DNL Workfront for G suite]\
   Para obter instruções, consulte [Instalar [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Gerenciar [!DNL Adobe Workfront] detalhes da notificação de [!DNL G Suite]

1. Se a variável [!DNL Workfront for G Suite] não for exibido, clique na guia [!DNL Workfront] ícone ![](assets/wf-lion-icon.png) no [!DNL G Suite] barra lateral de complementos na extremidade direita da página.
1. Entrada [!DNL G Suite], abra uma [!DNL Workfront] email de notificação.
1. Clique em **[!UICONTROL Exibir todas as atualizações]** se for exibido próximo à parte superior do painel.
1. Clique em **[!UICONTROL Detalhes]**.
1. Clique em qualquer opção disponível.

   As opções exibidas estão relacionadas ao tipo de notificação por email que você abriu. Por exemplo, se for uma notificação por email solicitando a aprovação de uma tarefa, você verá **[!UICONTROL Aprovar]** e **[!UICONTROL Rejeitar]** em vez de opções como **[!UICONTROL Trabalhar na tarefa]** ou **[!UICONTROL Concluído]**:

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
      <td><strong>[!UICONTROL Aprovar]</strong> ele, <strong>[!UICONTROL Rejeitar]</strong> ele, <strong>[!UICONTROL Conceder]</strong> acesso a ele, <strong>[!UICONTROL Ignorar]</strong> um pedido de acesso ao mesmo, <strong>[!UICONTROL Trabalhar nisso]</strong>ou clique em uma opção para indicar que você está <strong>[!UICONTROL Concluído]</strong> com ele</td> 
     </tr> 
     <tr> 
      <td>Projeto</td> 
      <td><strong>[!UICONTROL Aprovar]</strong> ele, <strong>[!UICONTROL Rejeitar]</strong> ele, <strong>[!UICONTROL Conceder]</strong> acesso a ele, ou <strong>[!UICONTROL Ignorar]</strong> um pedido de acesso ao mesmo</td> 
     </tr> 
     <tr> 
      <td>Documento</td> 
      <td><strong>[!UICONTROL Aprovar]</strong> ele, <strong>[!UICONTROL Rejeitar]</strong> ele, <strong>[!UICONTROL Conceder]</strong> acesso a ele, ou <strong>[!UICONTROL Ignorar]</strong> um pedido de acesso ao mesmo</td> 
     </tr> 
     <tr> 
      <td>Atualizar </td> 
      <td> <p>Exibir qualquer parte da lista inteira de atualizações do item para que você tenha o contexto necessário <strong>[!UICONTROL Publicação]</strong> uma nova atualização ou uma nova <strong>[!UICONTROL Responder]</strong>. Você pode clicar em <strong>[!UICONTROL Notificar]</strong> para alertar usuários específicos sobre sua resposta. </p> <p>Para obter mais informações, consulte <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref">Responder a um [!DNL Adobe Workfront] atualizar notificação de [!DNL G Suite]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Solicitação de aprovação</td> 
      <td><strong>[!UICONTROL Aprovar]</strong> ou <strong>[!UICONTROL Rejeitar]</strong> (você pode mudar de ideia clicando na outra opção), baixá-lo, exibir seu proprietário ou exibir seu número de referência</td> 
     </tr> 
     <tr> 
      <td>Uma alteração no status de um projeto</td> 
      <td> Visualize todas as informações atuais sobre o projeto, incluindo formulários personalizados. </td> 
     </tr> 
    </tbody> 
   </table>
