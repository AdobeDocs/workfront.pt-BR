---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Acionadores instantâneos (webhooks) no [!DNL Adobe Workfront Fusion]
description: Muitos serviços fornecem webhooks para fornecer notificações instantâneas sempre que uma determinada alteração ocorrer no serviço. Para processar essas notificações, recomendamos que você use acionadores instantâneos. Este artigo descreve o uso e a funcionalidade de acionadores instantâneos no Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 13b3a1bf-9856-4d2c-b1a5-13b044a7c2e5
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '933'
ht-degree: 0%

---

# Acionadores instantâneos (webhooks) no [!DNL Adobe Workfront Fusion]

Muitos serviços fornecem webhooks para fornecer notificações instantâneas sempre que uma determinada alteração ocorrer no serviço. Para processar essas notificações, recomendamos que você use acionadores instantâneos. Você pode reconhecê-los facilmente no [!DNL Adobe Workfront Fusion] devido à tag:

![](assets/instant-350x256.png)

Se o serviço não fornecer webhooks, você precisará usar acionadores de polling para pesquisar o serviço periodicamente.

Para obter uma introdução em vídeo a webhooks no Workfront Fusion, consulte:

* [Introdução aos Webhooks](https://video.tv.adobe.com/v/3427025/){target=_blank}
* [Webhooks intermediários](https://video.tv.adobe.com/v/3427030/){target=_blank}

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!DNL Pro] ou superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Requisito de licença atual: Não [!DNL Workfront Fusion] requisito de licença.</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para automação de trabalho]</p>
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

## Exibir a fila de um webhook

Todas as mensagens de webhooks recebidos são armazenadas na fila do webhook.

1. Clique em **[!UICONTROL Webhooks]** no menu à esquerda.
1. Localize o Webhook para o qual deseja exibir a fila.
1. Clique no botão com um ícone de caminhão e o número de webhooks recebidos.

   ![](assets/webhooks-truck-icon.png)

   >[!NOTE]
   >
   >Os dados de entrada do webhook são sempre armazenados na fila, independentemente de como você definiu a opção [!UICONTROL Dados] é confidencial (descrito na seção [O painel de configurações do cenário no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)). Assim que os dados forem processados em um cenário, eles serão excluídos permanentemente do sistema.

## Agendar acionadores instantâneos

Se o cenário contiver um acionador instantâneo, você poderá agendar sua execução imediatamente:

![](assets/schedule-setting-350x185.png)

Nesse caso, o cenário será executado imediatamente quando [!DNL Workfront Fusion] O recebe novos dados do serviço. Depois que o cenário é executado, a quantidade total de webhooks pendentes em espera na fila é contada e o cenário executa quantos ciclos houver webhooks pendentes, processando um webhook por ciclo. Para obter mais informações, consulte [Execução de cenário, ciclos e fases em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

>[!NOTE]
>
>* Um ciclo não é o mesmo que uma execução de cenário. Pode haver vários ciclos em uma execução de cenário.
>* Quando você executa um cenário com um acionador instantâneo agendado para ser imediato, as seguintes exceções se aplicam:
>
>     * O intervalo entre duas execuções não está sujeito ao intervalo Mínimo de acordo com o plano de precificação.
>
>       Por exemplo, uma vez concluída a execução do cenário, a fila do webhook será verificada novamente. Se houver webhooks pendentes, o cenário será executado imediatamente novamente e todos os webhooks pendentes serão processados novamente.
>   
>     * A configuração de cenário Número máximo de ciclos é ignorada e definida como 100, o que significa que não mais de 100 webhooks pendentes serão processados durante uma única execução de cenário (na taxa de 1 evento por ciclo).
>


Se você usar qualquer configuração de programação diferente de [!UICONTROL Imediatamente], o cenário é executado nos intervalos especificados. Como vários webhooks podem ser coletados na fila durante o intervalo, é recomendável definir a variável [[!UICONTROL Número máximo de ciclos]](../../workfront-fusion/scenarios/scenario-settings-panel.md#maximum) para um valor maior que o padrão 1 para processar mais webhooks em uma execução de cenário:

1. Clique em [!UICONTROL Configurações de cenário] ícone ![](assets/gear-icon-settings.png) na parte inferior do seu cenário.
1. No **[!UICONTROL Configurações de cenário]** que for exibida, digite um número na caixa **[!UICONTROL Número máximo de ciclos]** para indicar o número de webhooks da fila que deseja executar sempre que o cenário for executado.

## Limites de taxa

O limite de taxa atual é de 5 webhooks por segundo. Se o limite for excedido, um código de status 429 será retornado.

## Expiração de webhooks inativos

Um webhook que não foi atribuído a nenhum cenário por mais de 120 horas é removido.

## Cargas do Webhook

[!DNL Workfront Fusion] O armazena cargas do webhook por 30 dias. Acessar uma carga de webhook mais de 30 dias após sua criação resulta no erro &quot;[!UICONTROL Falha ao ler o arquivo do armazenamento.]&quot;

## Tratamento de erros

Quando há um erro no seu cenário com um acionador instantâneo, o cenário:

* Para imediatamente - quando o cenário está definido para execução [!UICONTROL Imediatamente].
* Interrupções após 3 tentativas malsucedidas (3 erros) - quando o cenário está definido para ser executado como programado.

Se ocorrer um erro durante a execução do cenário, o webhook será colocado de volta na fila durante a fase de reversão do acionador instantâneo. Em tal situação, você tem a possibilidade de corrigir o cenário e executá-lo novamente. Para obter mais informações, consulte [Reversão](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) no artigo [Execução de cenário, ciclos e fases em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Se houver um módulo de resposta do Webhook em seu cenário, o erro será enviado para a resposta do Webhook. O módulo de resposta do Webhook é sempre executado por último (no caso em que a variável [!UICONTROL Confirmar automaticamente] nas configurações de Cenário não está habilitada). Para obter mais informações, consulte [Resposta a webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md#respondi) no artigo [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Webhooks personalizados

Você pode criar seus próprios webhooks. Para obter mais informações, consulte [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Desativação do Webhook

Os webhooks são desativados automaticamente se qualquer uma das seguintes situações se aplicar:

* O webhook não foi conectado a nenhum cenário por mais de 5 dias
* O webhook é usado somente em cenários inativos, que ficaram inativos por mais de 30 dias.

Os webhooks desativados são excluídos e não registrados automaticamente se não estiverem conectados a nenhum cenário e estiverem com o status desativado por mais de 30 dias.


