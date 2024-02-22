---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: cenário,desempenho
navigation-topic: get-started-with-workfront-fusion-2-0
title: Medidas de proteção de desempenho do Adobe Workfront Fusion
description: O Adobe Workfront Fusion exige uma licença do Adobe Workfront Fusion, além de uma licença do Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: cdf46eb1-46ba-4707-9063-b76899195a2c
source-git-commit: a866fec950343c73712f22a08e2e045e8b80dbd9
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] medidas de proteção de desempenho

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] exige um [!DNL Adobe Workfront Fusion] além de uma licença [!DNL Adobe Workfront license].

A automação do trabalho exige processamento rápido, de modo que [!DNL Adobe Workfront Fusion] O foi projetado para alto desempenho. Como cenários de longa duração podem retardar o ritmo de seu trabalho, projetamos [!DNL Workfront Fusion] com medidas de proteção que preservam o desempenho e limitam o tempo de execução, o tamanho dos dados e outros parâmetros do cenário. [!DNL Workfront Fusion] os designers devem estar cientes dessas medidas de proteção e incorporá-las às suas práticas de design.

## Navegadores

O Workfront Fusion só é compatível com navegadores baseados no Chrome.

## Cenários

* O tempo limite de execução do cenário padrão é **40 minutos**. Quando a execução atinge esse tempo limite, [!DNL Workfront Fusion] interrompe a execução do cenário após o próximo ciclo ou operação, dependendo do cenário. Isso força o cenário a parar logo após o limite de 40 minutos ser atingido
* O tamanho máximo de um blueprint de cenário é **5 MB**, mas recomendamos manter o tamanho do cenário em **3 MB**.

  Os módulos do aplicativo que criam ou atualizam dados com um grande número de campos podem causar blueprints muito grandes.

   * Ao usar o [!DNL Workfront] selecione apenas os campos necessários para seus casos de uso de criação ou atualização.
   * Ao usar outros aplicativos, use módulos de API personalizados para interagir com qualquer tipo de registro que tenha um grande número de campos.

* Embora não haja limite para o número de módulos em um cenário, cenários com mais de 150 módulos afetam negativamente o desempenho do [!DNL Workfront Fusion] sistema. Por esse motivo, não recomendamos criar cenários com mais de 150 módulos.

## Operações

* Normalmente, o tempo limite da operação padrão é **40 segundos**.

<!--
* The operation timeout for calls to Adobe Workfront is **120 seconds**.
-->

## Arquivos

* A capacidade total de processamento do Fusion para arquivos é **1 GB**. O limite se baseia em um custo total de memória. Cada operação contribui para esse custo. Se um único arquivo de 400 MB for baixado e carregado, o custo total da capacidade do arquivo será de 800 MB.

## Uso de Memória do Servidor

* O uso da memória do servidor para uma única execução é limitado a **1 GB**.

  Muitos fatores, como arquivos grandes ou módulos complexos, podem afetar o uso da memória do servidor de maneiras difíceis de prever ou controlar. Por esse motivo, a execução do cenário pode exceder o limite de memória de 1 GB, mesmo que o cenário siga todas as outras medidas de proteção de desempenho. Exceder o limite de memória causa falha na execução.

## Webhooks

* O tamanho máximo padrão de uma carga é **5 MB**.
* Os webhooks são limitados a **100 solicitações por segundo**. Quando esse limite é atingido, o Workfront Fusion envia um erro 429 ([!UICONTROL Muitas solicitações]).
* [!DNL Workfront Fusion] O armazena cargas do webhook por 30 dias. Acessar uma carga de webhook mais de 30 dias após seu recebimento resulta no erro &quot;[!UICONTROL Falha ao ler o arquivo do armazenamento.]&quot;
* Os webhooks são desativados automaticamente se qualquer uma das seguintes situações se aplicar:

   * O webhook não foi conectado a nenhum cenário por mais de 5 dias
   * O webhook é usado somente em cenários inativos, que ficaram inativos por mais de 30 dias.

* Os webhooks desativados são excluídos e não registrados automaticamente se não estiverem conectados a nenhum cenário e estiverem com o status desativado por mais de 30 dias.

## Histórico de execução

* Os logs do histórico de execução são limitados a um tamanho de **100 MB**. Se o histórico de execução exceder esse tamanho, somente os primeiros 100 MB serão exibidos.

