---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Receber um webhook de um serviço da Web
description: Se um serviço Web não estiver implementado como um aplicativo no [!DNL Adobe Workfront Fusion], mas com suporte ao envio de webhooks, você pode adicionar o serviço a um cenário usando o módulo Webhook personalizado como um acionador instantâneo.
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# Receber um webhook de um serviço da Web

Se um serviço Web não estiver implementado como um aplicativo no [!DNL Adobe Workfront Fusion], mas com suporte ao envio de webhooks, você pode adicionar o serviço a um cenário usando o módulo Webhook personalizado como um acionador instantâneo.

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
   <td>
   <p>Requisito de licença atual: Não [!DNL Workfront Fusion] requisito de licença.</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e integração do trabalho] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o [!UICONTROL Select] ou o [!UICONTROL Prime] [!DNL Adobe Workfront] Planejar, sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no [!UICONTROL Ultimate] [!DNL Workfront] plano.</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Receber um webhook

1. Adicione o **[!UICONTROL Webhooks] >[!UICONTROL Webhook personalizado]** para o seu cenário.
1. Clique em **[!UICONTROL Adicionar]**, digite um **[!UICONTROL Nome do Webhook]** na caixa exibida, clique em **[!UICONTROL Salvar]**.

1. Clique em **[!UICONTROL Copiar endereço para a área de transferência]** e, em seguida, clique em **[!UICONTROL OK]**.

1. Faça logon no serviço Web e faça o seguinte:

   1. No [!UICONTROL Configurações] para o serviço da web, crie um webhook.
   1. Cole o endereço que você copiou para a área de transferência na etapa 3 .
   1. Selecione o evento que acionará o webhook.

1. No [!DNL Workfront Fusion] cenário, especifique o(s) evento(s) que deseja acionar a [!UICONTROL Webhook personalizado] módulo.
1. Execute o cenário.

   Quando o evento ou eventos ocorrerem, a variável [!UICONTROL Webhook personalizado] O módulo é acionado e o cenário é executado.
