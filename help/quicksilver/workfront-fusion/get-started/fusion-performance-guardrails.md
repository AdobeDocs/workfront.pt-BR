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
source-git-commit: 7c27dc98c4ce59d598be537a1f09c6eddf9bce42
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] medidas de proteção de desempenho

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] requer uma licença [!DNL Adobe Workfront Fusion] além de [!DNL Adobe Workfront license].

A automação de trabalho requer processamento rápido, portanto, o [!DNL Adobe Workfront Fusion] foi desenvolvido para alto desempenho. Como cenários de longa duração podem retardar o ritmo do seu trabalho, criamos o [!DNL Workfront Fusion] com medidas de proteção que preservam o desempenho e limitam o tempo de execução, o tamanho dos dados e outros parâmetros do cenário. Os designers do [!DNL Workfront Fusion] devem estar cientes dessas medidas de proteção e incorporá-las às suas práticas de design.

## Navegadores

* O Workfront Fusion é compatível apenas com navegadores baseados em Chrome.

## Cenários

* O tempo limite de execução de cenário padrão é de **40 minutos**. Quando a execução atinge esse tempo limite, [!DNL Workfront Fusion] interrompe a execução do cenário após o próximo ciclo ou operação, dependendo do cenário. Isso força o cenário a parar logo após o limite de 40 minutos ser atingido
* O tamanho máximo de um blueprint do cenário é **5 MB**, mas recomendamos manter o tamanho do cenário abaixo de **3 MB**.

  Os módulos do aplicativo que criam ou atualizam dados com um grande número de campos podem causar blueprints muito grandes.

   * Ao usar o aplicativo [!DNL Workfront], selecione apenas os campos necessários para seus casos de uso de criação ou atualização.
   * Ao usar outros aplicativos, use módulos de API personalizados para interagir com qualquer tipo de registro que tenha um grande número de campos.

* Embora não haja um limite para o número de módulos em um cenário, os cenários com mais de 150 módulos afetam negativamente o desempenho do seu sistema [!DNL Workfront Fusion]. Por esse motivo, não recomendamos criar cenários com mais de 150 módulos.

## Operações

* O tempo limite da operação padrão geralmente é de **40 segundos**.

<!--
* The operation timeout for calls to Adobe Workfront is **120 seconds**.
-->

## Arquivos

* A capacidade total de processamento do Fusion para arquivos é de **1 GB**. O limite se baseia em um custo total de memória. Cada operação contribui para esse custo. Se um único arquivo de 400 MB for baixado e carregado, o custo total da capacidade do arquivo será de 800 MB.
* As organizações no plano Workfront Ultimate têm acesso a um maior processamento de arquivos além de 1 GB. A plataforma Fusion pode oferecer suporte a arquivos individuais de até 15 GB para uma única ação (por exemplo, carregar arquivo), mas há outros fatores que afetam a transferência de dados. O limite de tamanho de arquivo de uma única ação depende do serviço Web ao qual o Fusion se conecta. A transferência de dados é o processamento total de uma única execução. Isso significa que várias ações em uma única execução contribuem para a transferência total de dados. O Fusion processará arquivos até que o limite de execução de 40 minutos seja atingido.

  Para obter mais informações, consulte [Trabalhando com arquivos grandes no Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/get-started/fusion-large-files.md).


## Uso de Memória do Servidor

* O uso de memória do servidor para uma única execução é limitado a **1 GB**.

  Muitos fatores, como arquivos grandes ou módulos complexos, podem afetar o uso da memória do servidor de maneiras difíceis de prever ou controlar. Por esse motivo, a execução do cenário pode exceder o limite de memória de 1 GB, mesmo que o cenário siga todas as outras medidas de proteção de desempenho. Exceder o limite de memória causa falha na execução.

## Webhooks

* O tamanho máximo padrão de uma carga é **5 MB**.
* Os webhooks estão limitados a **100 solicitações por segundo**. Quando esse limite é atingido, o Workfront Fusion envia um status 429 ([!UICONTROL Muitas solicitações]).
* O [!DNL Workfront Fusion] armazena cargas de webhook por 30 dias. O acesso a uma carga de webhook por mais de 30 dias após seu recebimento resulta no erro &quot;[!UICONTROL Falha ao ler o arquivo do armazenamento.]&quot;
* Os webhooks são desativados automaticamente se qualquer uma das seguintes situações se aplicar:

   * O webhook não foi conectado a nenhum cenário por mais de 5 dias
   * O webhook é usado somente em cenários inativos, que ficaram inativos por mais de 30 dias.

* Os webhooks desativados são excluídos e não registrados automaticamente se não estiverem conectados a nenhum cenário e estiverem com o status desativado por mais de 30 dias.

## Histórico de execução

* Os logs do histórico de execução são limitados ao tamanho de **100 MB**. Se o histórico de execução exceder esse tamanho, somente os primeiros 100 MB serão exibidos.
* Se um cenário tiver várias execuções simultâneas. apenas 5 execuções são exibidas na área Execuções da página de detalhes do cenário. Isso é verdade mesmo quando mais de 5 execuções estão em andamento.

## Execuções incompletas

* As execuções incompletas estão limitadas a um tamanho total de **500 MB**. Se o limite de 500 MB for atingido, não serão armazenadas mais execuções incompletas.

## Tentativas

* Ao usar o módulo Break e especificar a diretiva Retry, se um cenário falhar consecutivamente 10 vezes em um período de 2 minutos, o cenário será desativado automaticamente.

