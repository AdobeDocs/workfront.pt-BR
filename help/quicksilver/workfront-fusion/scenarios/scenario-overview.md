---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Visão geral do cenário do Adobe Workfront Fusion
description: O Adobe Workfront Fusion exige uma licença do Adobe Workfront Fusion, além de uma licença do Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: 13d6230d-51f6-4f68-8697-30f8ce6c8599
source-git-commit: 27158301e491d4ff45ce7987a81f841fb4525b2a
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Visão geral do cenário [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] requer uma licença [!DNL Adobe Workfront Fusion] além de [!DNL Adobe Workfront license].

>[!IMPORTANT]
>
>[!DNL Workfront Fusion] cenários não devem ser confundidos com [!DNL Workfront Scenario Planner] cenários. Para obter informações sobre [!DNL Workfront Scenario Planner] cenários, consulte [A [!DNL Scenario Planner] visão geral](../../scenario-planner/scenario-planner-overview.md).

O papel de [!DNL Adobe Workfront Fusion] é automatizar seus processos para que você possa se concentrar em novas tarefas em vez de repetir as mesmas tarefas repetidamente. Ele funciona vinculando ações em e entre aplicativos e serviços para criar um cenário que transfere e transforma seus dados automaticamente. O cenário que você cria observa dados em um aplicativo ou serviço e processa esses dados para fornecer o resultado desejado.

Um cenário é composto de uma série de módulos que indicam como os dados devem ser transformados em um aplicativo ou transferidos entre aplicativos e serviços da Web.

## Exemplo: automatizando processos em [!DNL Adobe Workfront]

>[!NOTE]
>
>Essa funcionalidade está disponível para as seguintes licenças:
>
>* [!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho]
>* [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho]

O [!DNL Workfront Fusion] permite que você automatize fluxos de trabalho simples ou complexos no [!DNL Workfront], economizando tempo e garantindo que o processo seja executado de forma consistente.

Neste exemplo, o cenário é acionado quando um campo especificado é alterado em uma Tarefa ou Problema em [!DNL Workfront]. Quando acionado, o cenário obtém informações no projeto relacionado e cria uma atualização personalizada para uma pessoa atribuída a uma função específica no projeto.

![](assets/fusion-template-example-350x102.png)

## Exemplo: Conectando [!DNL Workfront] a outro aplicativo ou serviço Web

>[!NOTE]
>
>Essa funcionalidade está disponível para a seguinte licença:
>
>* [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho]
>

O [!DNL Workfront Fusion] também pode se conectar a outros aplicativos e serviços Web. É possível acessar, importar, manipular ou exportar dados de outros aplicativos, integrando-os ao Workfront ou entre si. Muitos aplicativos têm [!DNL Workfront Fusion] conectores dedicados. Se não houver um conector dedicado para o aplicativo que deseja acessar, você pode usar os módulos [!UICONTROL HTTP] ou [!UICONTROL SOAP] do [!DNL Workfront Fusion] para se conectar ao aplicativo por meio da API.

Neste exemplo, o cenário é acionado quando um usuário é adicionado a uma planilha do [!DNL Excel]. O cenário verifica se o usuário está em [!DNL Workfront]. Caso contrário, o cenário cria o usuário em [!DNL Workfront] e adiciona sua ID de usuário do Workfront de volta à planilha.

![](assets/fusion-integration-example--350x171.png)

Para obter uma lista de conectores dedicados, consulte [Aplicativos e seus módulos](../../workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

>[!IMPORTANT]
>
>O [!DNL Adobe Workfront Fusion] pode se conectar a quase qualquer serviço Web. Se o aplicativo com o qual você deseja trabalhar não tiver um conector [!DNL Workfront Fusion] dedicado, você poderá usar os seguintes módulos para se conectar diretamente ao serviço Web:
>
>* [[!UICONTROL HTTP] módulos](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)
>* [[!UICONTROL SOAP] módulo](../../workfront-fusion/apps-and-their-modules/soap-module.md)
>* [[!UICONTROL JSON] módulos](../../workfront-fusion/apps-and-their-modules/json-modules.md)
>
