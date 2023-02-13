---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Visão geral do cenário do Adobe Workfront Fusion
description: O Adobe Workfront Fusion exige uma licença do Adobe Workfront Fusion além de uma licença da Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: 13d6230d-51f6-4f68-8697-30f8ce6c8599
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] visão geral do cenário

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] exige um [!DNL Adobe Workfront Fusion] além de um [!DNL Adobe Workfront license].

>[!IMPORTANT]
>
>[!DNL Workfront Fusion] os cenários não devem ser confundidos com [!DNL Workfront Scenario Planner] cenários. Para obter informações sobre [!DNL Workfront Scenario Planner] cenários, consulte [O [!DNL Scenario Planner] visão geral](../../scenario-planner/scenario-planner-overview.md).

O papel do [!DNL Adobe Workfront Fusion] O é automatizar seus processos para que você possa se concentrar em novas tarefas em vez de repetir as mesmas tarefas várias vezes. Funciona vinculando ações dentro e entre aplicativos e serviços para criar um cenário que transfere e transforma seus dados automaticamente. O cenário criado busca dados em um aplicativo ou serviço e processa esses dados para fornecer o resultado desejado.

Um cenário é composto por uma série de módulos que indicam como os dados devem ser transformados em um aplicativo ou transferidos entre aplicativos e serviços da Web.

## Exemplo: Automatização de processos no [!DNL Adobe Workfront]

>[!NOTE]
>
>Essa funcionalidade está disponível para as seguintes licenças:
>
>* [!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho]
>* [!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho]
>


[!DNL Workfront Fusion] permite automatizar workflows simples ou complexos no [!DNL Workfront], economizando tempo e garantindo que o processo seja executado de forma consistente.

Neste exemplo, o cenário é acionado quando um campo especificado é alterado em uma Tarefa ou Ocorrência em [!DNL Workfront]. Quando acionado, o cenário obtém informações no projeto relacionado e cria uma atualização personalizada para uma pessoa atribuída a uma função específica no projeto.

![](assets/fusion-template-example-350x102.png)

## Exemplo: Conexão [!DNL Workfront] para outro aplicativo ou serviço da Web

>[!NOTE]
>
>Essa funcionalidade está disponível para a seguinte licença:
>
>* [!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho]
>


[!DNL Workfront Fusion] também pode se conectar a outros aplicativos e serviços da Web. Você pode acessar, importar, manipular ou exportar dados de outros aplicativos, integrando-os com o Workfront ou entre si. Muitos aplicativos dedicados [!DNL Workfront Fusion] conectores. Se não houver um conector dedicado para o aplicativo que você deseja acessar, você poderá usar [!DNL Workfront Fusion]&#39;s [!UICONTROL HTTP] ou [!UICONTROL SOAP] módulos para se conectar ao aplicativo por meio de sua API.

Neste exemplo, o cenário é acionado quando um usuário é adicionado a um [!DNL Excel] planilha. O cenário verifica se o usuário está em [!DNL Workfront]. Caso contrário, o cenário criará o usuário em [!DNL Workfront] e adiciona a ID de usuário do Workfront de volta à planilha.

![](assets/fusion-integration-example--350x171.png)

Para obter uma lista de conectores dedicados, consulte [Aplicativos e seus módulos](../../workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

>[!IMPORTANT]
>
>[!DNL Adobe Workfront Fusion] pode se conectar a quase qualquer serviço da Web. Se o aplicativo com o qual você deseja trabalhar não tiver um [!DNL Workfront Fusion] , você pode usar os seguintes módulos para se conectar diretamente ao serviço da Web:
>
>* [[!UICONTROL HTTP] módulos](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)
>* [[!UICONTROL SOAP] módulo](../../workfront-fusion/apps-and-their-modules/soap-module.md)
>* [[!UICONTROL JSON] módulos](../../workfront-fusion/apps-and-their-modules/json-modules.md)
>

