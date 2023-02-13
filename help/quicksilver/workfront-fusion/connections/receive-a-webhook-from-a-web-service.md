---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Receber um webhook de um serviço da Web
description: Se um serviço da Web não estiver implementado no momento como um aplicativo em [!DNL Adobe Workfront Fusion], mas suporta o envio de webhooks, você pode adicionar o serviço a um cenário usando o módulo Webhook personalizado como um acionador instantâneo.
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Receber um webhook de um serviço da Web

Se um serviço da Web não estiver implementado no momento como um aplicativo em [!DNL Adobe Workfront Fusion], mas suporta o envio de webhooks, você pode adicionar o serviço a um cenário usando o módulo Webhook personalizado como um acionador instantâneo.

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!UICONTROL Pro] ou superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licença**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Receber um webhook

1. Adicione o **[!UICONTROL Webhooks] >[!UICONTROL Webhook personalizado]** para o seu cenário.
1. Clique em **[!UICONTROL Adicionar]**, digite a **[!UICONTROL Nome do Webhook]** na caixa exibida, em seguida, clique em **[!UICONTROL Salvar]**.

1. Clique em **[!UICONTROL Copiar endereço para a área de transferência]**, depois clique em **[!UICONTROL OK]**.

1. Faça logon no serviço da Web e faça o seguinte aqui:

   1. No [!UICONTROL Configurações] para o serviço da Web, crie um webhook.
   1. Cole o endereço copiado para a área de transferência na etapa 3 .
   1. Selecione o evento que acionará o webhook.

1. No [!DNL Workfront Fusion] , especifique o evento ou eventos que você deseja acionar [!UICONTROL Webhook personalizado] módulo.
1. Execute o cenário.

   Quando o evento ou os eventos ocorrem, a variável [!UICONTROL Webhook personalizado] e o cenário é executado.
