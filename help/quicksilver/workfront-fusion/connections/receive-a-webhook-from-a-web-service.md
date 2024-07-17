---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Receber um webhook de um serviço da Web
description: Se um serviço Web não estiver implementado no momento como um aplicativo no  [!DNL Adobe Workfront Fusion], mas oferecer suporte ao envio de webhooks, você poderá adicionar o serviço a um cenário usando o módulo Webhook personalizado como um acionador instantâneo.
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Receber um webhook de um serviço da Web

Se um serviço Web não estiver implementado no momento como um aplicativo no [!DNL Adobe Workfront Fusion], mas oferecer suporte ao envio de webhooks, você poderá adicionar o serviço a um cenário usando o módulo Webhook personalizado como um acionador instantâneo.

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
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Receber um webhook

1. Adicione o módulo **[!UICONTROL Webhooks] >[!UICONTROL Webhook personalizado]** ao seu cenário.
1. Clique em **[!UICONTROL Adicionar]**, digite um **[!UICONTROL nome do Webhook]** na caixa exibida e clique em **[!UICONTROL Salvar]**.

1. Clique em **[!UICONTROL Copiar endereço para a área de transferência]** e em **[!UICONTROL OK]**.

1. Faça logon no serviço da Web e faça o seguinte:

   1. Na área [!UICONTROL Configurações] do serviço Web, crie um webhook.
   1. Cole o endereço que você copiou para a área de transferência na etapa 3 .
   1. Selecione o evento que acionará o webhook.

1. No cenário [!DNL Workfront Fusion], especifique o(s) evento(s) que deseja acionar o módulo [!UICONTROL Webhook personalizado].
1. Execute o cenário.

   Quando um ou mais eventos ocorrem, o módulo [!UICONTROL Webhook personalizado] é acionado e o cenário é executado.
