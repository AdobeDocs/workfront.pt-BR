---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: cenário,desempenho
navigation-topic: get-started-with-workfront-fusion-2-0
title: Medidas de proteção de desempenho do Adobe Workfront Fusion
description: O Adobe Workfront Fusion exige uma licença do Adobe Workfront Fusion além de uma licença da Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: cdf46eb1-46ba-4707-9063-b76899195a2c
source-git-commit: 229fd48d604385a1bfcaba2fd34eb6f3bbdde7a7
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] medidas de proteção de desempenho

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] exige um [!DNL Adobe Workfront Fusion] além de um [!DNL Adobe Workfront license].

A automação de trabalho requer processamento rápido, portanto [!DNL Adobe Workfront Fusion] O foi projetado para alto desempenho. Como cenários de longa duração podem retardar o ritmo de seu trabalho, nós criamos [!DNL Workfront Fusion] com medidas de proteção de desempenho que limitam o tempo de execução, o tamanho dos dados e outros parâmetros do cenário. [!DNL Workfront Fusion] os criadores devem estar cientes destas medidas de proteção e incorporá-las nas suas práticas de concepção.

## Cenários

* O tempo limite de execução do cenário padrão é **40 minutos**. Quando a execução atinge esse tempo limite, [!DNL Workfront Fusion] interrompe a execução do cenário após o próximo ciclo ou operação, dependendo do cenário. Isso faz com que o cenário pare logo após o limite de 40 minutos ser atingido
* O tamanho máximo de um blueprint de cenário é **5 MB**, mas recomendamos manter o tamanho do cenário em **3 MB**.

   Os módulos de aplicativo que criam ou atualizam dados com grandes números de campos podem causar blueprints muito grandes.

   * Ao usar a variável [!DNL Workfront] no aplicativo, selecione apenas os campos necessários para criar ou atualizar casos de uso.
   * Ao usar outros aplicativos, use módulos de API personalizados para interagir com qualquer tipo de registro que tenha um grande número de campos.

* Embora não haja limite para o número de módulos em um cenário, os cenários com mais de 150 módulos afetam negativamente o desempenho de seu [!DNL Workfront Fusion] sistema. Por isso, não recomendamos criar cenários com mais de 150 módulos.

## Operações

* Normalmente, o tempo limite da operação padrão é **40 segundos**.

<!--
* The operation timeout for calls to Adobe Workfront is **120 seconds**.
-->

## Arquivos

* A capacidade total de processamento de arquivos da Fusion é **1 GB**. O limite é baseado em um custo total de memória. Cada operação contribui para esse custo. Se um único arquivo de 400 MB for baixado e carregado, o custo total para a capacidade do arquivo será de 800 MB.

## Uso de memória do servidor

* O uso de memória do servidor para uma única execução é limitado a **1 GB**.

   Muitos fatores, como arquivos grandes ou módulos complexos, podem afetar o uso da memória do servidor de maneiras difíceis de prever ou controlar. Por esse motivo, a execução do cenário pode exceder o limite de memória de 1 GB, mesmo que o cenário siga todas as outras medidas de proteção de desempenho. Exceder o limite de memória faz com que a execução falhe.

## Webhooks

* O tamanho máximo padrão de uma carga é **5 MB**.
* Os Webhooks estão limitados a **100 solicitações por segundo**. Quando esse limite é atingido, o Workfront Fusion envia um 429 ([!UICONTROL Demasiadas Solicitações]).
* [!DNL Workfront Fusion] armazena cargas do webhook por 30 dias. Acessar uma carga do webhook mais de 30 dias depois de ela ser recebida resulta no erro &quot;[!UICONTROL Falha ao ler arquivo do armazenamento.]&quot;
* Os Webhooks são desativados automaticamente se uma das seguintes opções se aplicar:

   * O webhook não está conectado a nenhum cenário há mais de 5 dias
   * O webhook é usado apenas em cenários inativos, que ficaram inativos por mais de 30 dias.

* Os webhooks desativados são excluídos e não são registrados automaticamente se não estiverem conectados a nenhum cenário e estiverem com o status desativado por mais de 30 dias.
