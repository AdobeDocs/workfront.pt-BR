---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Acionadores instantâneos (webhooks) em [!DNL Adobe Workfront Fusion]
description: Muitos serviços fornecem webhooks para fornecer notificações instantâneas sempre que uma determinada alteração ocorre no serviço. Para processar essas notificações, recomendamos que você use acionadores instantâneos. Este artigo descreve o uso e a funcionalidade de acionadores instantâneos no Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 13b3a1bf-9856-4d2c-b1a5-13b044a7c2e5
source-git-commit: 04191419ab6079cc34576b5a7532cd1596e4b91d
workflow-type: tm+mt
source-wordcount: '855'
ht-degree: 0%

---

# Acionadores instantâneos (webhooks) em [!DNL Adobe Workfront Fusion]

Muitos serviços fornecem webhooks para fornecer notificações instantâneas sempre que uma determinada alteração ocorre no serviço. Para processar essas notificações, recomendamos que você use acionadores instantâneos. Você pode reconhecê-los facilmente em [!DNL Adobe Workfront Fusion] por causa da tag :

![](assets/instant-350x256.png)

Se o serviço não fornecer webhooks, será necessário usar os acionadores de pesquisa para pesquisar periodicamente o serviço.

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
   <td role="rowheader">Licença da [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p> <p>[!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Exibir a fila de um webhook

Todas as mensagens de webhooks recebidos são armazenadas na fila do webhook.

1. Clique em **[!UICONTROL Webhooks]** no menu à esquerda.
1. Encontre o Webhook para o qual deseja visualizar a fila.
1. Clique no botão com um ícone de caminhão e o número de webhooks recebidos.

   ![](assets/webhooks-truck-icon.png)

   >[!NOTE]
   >
   >Os dados de entrada do webhook são sempre armazenados na fila, independentemente de como você definiu a opção [!UICONTROL Dados] é confidencial (descrito em [O painel de configurações de cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)). Assim que os dados forem processados em um cenário, eles serão permanentemente excluídos do sistema.

## Agendar acionadores instantâneos

Se o seu cenário contiver um acionador instantâneo, você poderá agendar a execução imediata do cenário:

![](assets/schedule-setting-350x185.png)

Nesse caso, seu cenário será executado imediatamente quando [!DNL Workfront Fusion] O recebe novos dados do serviço. Depois que o cenário é executado, a quantidade total de webhooks pendentes na fila é contada e o cenário executa quantos ciclos houver webhooks pendentes, processando um webhook por ciclo. Para obter mais informações, consulte [Execução do cenário, ciclos e fases em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

>[!NOTE]
>
>* Um ciclo não é o mesmo que uma execução de cenário. Pode haver vários ciclos em uma execução de cenário.
>* Quando você executa um cenário com um acionador instantâneo programado para ser imediato, as seguintes exceções se aplicam:
   >
   >     * O intervalo entre duas execuções não está sujeito ao intervalo Mínimo de acordo com o plano de precificação.

      >
      >       Por exemplo, uma vez que o cenário conclui a execução, a fila do webhook é marcada novamente. Se houver algum webhooks pendente, o cenário será executado imediatamente novamente, processando todos os webhooks pendentes novamente.
   >   
   >     * A configuração de cenário Número máximo de ciclos é ignorada e definida como 100, o que significa que não mais de 100 webhooks pendentes serão processados durante uma única execução de cenário (à taxa de 1 evento por ciclo).
>



Se você usar qualquer outra configuração de programação diferente de [!UICONTROL Imediatamente], o cenário será executado nos intervalos especificados. Como vários webhooks podem ser reunidos na fila durante o intervalo, é recomendável definir a variável [[!UICONTROL Número máximo de ciclos]](../../workfront-fusion/scenarios/scenario-settings-panel.md#maximum) para um valor superior ao padrão 1 para processar mais webhooks em um cenário executado:

1. Clique no botão [!UICONTROL Configurações de cenário] ícone ![](assets/gear-icon-settings.png) na parte inferior do seu cenário.
1. No **[!UICONTROL Configurações de cenário]** for exibida, digite um número na caixa **[!UICONTROL Número máximo de ciclos]** para indicar o número de webhooks da fila que deseja executar sempre que executar o cenário.

## Limites de taxa

O limite de taxa atual é de 5 webhooks por segundo. Se o limite for excedido, um código de status 429 será retornado.

## Expiração de webhooks inativos

Um webhook que não foi atribuído a nenhum cenário por mais de 120 horas é removido.

## Cargas do Webhook

[!DNL Workfront Fusion] armazena cargas do webhook por 30 dias. Acessar uma carga do webhook mais de 30 dias após sua criação resulta no erro &quot;[!UICONTROL Falha ao ler arquivo do armazenamento.]&quot;

## Tratamento de erros

Quando há um erro no seu cenário com um acionador instantâneo, o cenário:

* Interrompe imediatamente - quando o cenário é definido para ser executado [!UICONTROL Imediatamente].
* Interrompe após 3 tentativas malsucedidas (3 erros) - quando o cenário é definido para ser executado como programado.

Se ocorrer um erro durante a execução do cenário, o webhook será colocado novamente na fila durante a fase de reversão do acionador instantâneo. Em tal situação, você tem a possibilidade de corrigir o cenário e executá-lo novamente. Para obter mais informações, consulte [Reversão](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) no artigo [Execução do cenário, ciclos e fases em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Se houver um módulo de resposta do Webhook em seu cenário, o erro será enviado para a resposta do Webhook. O módulo de resposta do Webhook é sempre executado por último (no caso em que a função [!UICONTROL Confirmação automática] nas configurações de Cenário não estiver ativada). Para obter mais informações, consulte [Responder a ganchos da Web](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md#respondi) no artigo [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Webhooks personalizados

Você pode criar seus próprios webhooks. Para obter mais informações, consulte [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Desativação do Webhook

Os Webhooks são desativados automaticamente se uma das seguintes opções se aplicar:

* O webhook não está conectado a nenhum cenário há mais de 5 dias
* O webhook é usado apenas em cenários inativos, que ficaram inativos por mais de 30 dias.

Os webhooks desativados são excluídos e não são registrados automaticamente se não estiverem conectados a nenhum cenário e estiverem com o status desativado por mais de 30 dias.


