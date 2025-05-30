---
title: Preencher uma solicitação automaticamente usando IA
content-type: reference
description: Você pode usar a IA para preencher automaticamente os campos de solicitação.
author: Becky
feature: Get Started with Workfront
exl-id: d053e604-5a28-4fd3-8f89-4467b6e46f02
source-git-commit: a3e93311277bc5b68063e0ec1cbdcce3a40eb3dd
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 1%

---

# Preencher uma solicitação automaticamente usando IA

>[!NOTE]
>
>No momento, essa funcionalidade faz parte de um beta fechado. Para ativar essa funcionalidade, entre em contato com sargism@adobe.com.
>
>Para se qualificar para o beta fechado, sua organização deve atender aos requisitos para usar o Workfront AI Assistant. Para obter detalhes, consulte [Pré-requisitos do Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).

A IA pode ajudar a preencher automaticamente os campos de solicitação. Ele pode sugerir valores de campo com base em solicitações anteriores ou analisá-los a partir de texto, como se emails fossem documentos carregados.

Você pode aprovar ou rejeitar essas sugestões antes de enviar a solicitação.

O preenchimento automático não substitui nenhum campo já preenchido.

## Obter sugestões ao preencher o formulário

O preenchimento automático pode sugerir valores de campo enquanto você preenche o formulário. À medida que você informa valores nos campos de solicitação, o Workfront compara esses valores com solicitações anteriores. Se o valor inserido estiver estreitamente correlacionado com outros valores de campo em contextos semelhantes em solicitações anteriores, o Workfront sugere esses valores.

Por exemplo, se uma clínica sempre usar o mesmo código de faturamento, a Workfront sugerirá esse código de faturamento no campo apropriado quando o nome da clínica for inserido.

Para usar sugestões com base em solicitações anteriores:

1. Comece a criar uma solicitação.

   Para obter instruções, consulte [Criar e enviar solicitações](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Comece a preencher os campos.

   À medida que você preenche campos, outros campos podem mostrar sugestões.

1. Para cada sugestão de campo, selecione **Aceitar** ou **Rejeitar** abaixo desse campo.

   Ou

   Selecione **Aceitar tudo** ou **Rejeitar tudo** na parte superior da página para aceitar ou rejeitar todas as sugestões.

## Obter sugestões de um prompt de texto

O preenchimento automático pode sugerir valores de campo com base em texto, como emails. Você cola um bloco de texto e o Workfront processa o texto para sugerir valores de campo com base no texto.

Por exemplo, se o email incluir &quot;Isso vence em 1º de junho&quot; e o formulário de solicitação tiver um campo para data de vencimento, a Workfront sugerirá 1º de junho para esse valor de campo.

Esse tipo de sugestão também verifica solicitações anteriores para contextos semelhantes. Por exemplo, se o prompt mencionar que a solicitação é para um determinado cliente, o Workfront poderá localizar e inserir o endereço de faturamento desse cliente automaticamente, com base em solicitações anteriores.

Você pode colar no texto a ser aplicado a todo o formulário ou a uma única seção do formulário.

Para usar sugestões com base em um prompt de texto colado:

1. Comece a criar uma solicitação.

   Para obter instruções, consulte [Criar e enviar solicitações](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Para aplicar o prompt de texto a todo o formulário, clique no ícone de IA ![Ícone de IA](assets/request-prompt-icon.png) sob o nome do formulário.

   Ou

   Para aplicar o prompt de texto para uma única seção, clique no ícone de IA ![Ícone de IA](assets/request-prompt-icon.png) ao lado do nome da seção.

1. Cole o texto na caixa de prompt.
1. Clique em **Preencher o formulário**.

   O Workfront gera sugestões para o formulário.
1. Para cada sugestão de campo, selecione **Aceitar** ou **Rejeitar** abaixo desse campo.

   Ou

   Selecione **Aceitar tudo** ou **Rejeitar tudo** na parte superior da página para aceitar ou rejeitar todas as sugestões.

## Obter sugestões com base em um documento do qual você fez upload

O preenchimento automático pode sugerir valores de campo com base em um documento que você fez upload.

Esse tipo de sugestão também verifica solicitações anteriores para contextos semelhantes. Por exemplo, se o prompt mencionar que a solicitação é para um determinado cliente, o Workfront poderá localizar e inserir o endereço de faturamento desse cliente automaticamente, com base em solicitações anteriores.

### Proteções de upload de documento

#### Tipos de arquivo compatíveis

Os seguintes tipos de arquivos são compatíveis:

* BMP
* CSV
* DOC
* DOCX
* GIF
* JPEG
* JPG
* ODP
* ODS
* ODT
* PDF
* Imagem PNG
* PPT
* PPTX
* RTF
* TIFF
* TXT
* XLS
* XLSX

#### Tamanho de arquivo suportado

Cada arquivo pode ter até 100 MB

#### Número de arquivos

É possível carregar até 50 arquivos (páginas, slides ou folhas).

>[!IMPORTANT]
>
>Os documentos são convertidos em uma série de imagens, cada uma considerada um arquivo separado.
>
>Por exemplo, você pode carregar um PowerPoint com 50 slides ou 5 documentos do Word com 10 páginas cada.

#### Outras práticas recomendadas

Considere o seguinte ao fazer upload de um documento para preenchimento automático da solicitação:

* O preenchimento automático está otimizado para o alfabeto latino.
* Recomendamos usar um tamanho de texto de 8 pontos ou maior.
* O preenchimento automático pode ter dificuldade com imagens no documento, como imagens giradas ou distorcidas, gráficos e contagem ou uso de motivos espaciais em objetos em imagens.
* Como sempre, recomendamos verificar a precisão dos resultados antes de enviar a solicitação.

### Carregar um documento para preencher uma solicitação automaticamente

Você pode carregar um documento para ser aplicado a todo o formulário ou a uma única seção do formulário.

1. Comece a criar uma solicitação.

   Para obter instruções, consulte [Criar e enviar solicitações](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Para aplicar o documento ao formulário inteiro, clique no ícone de IA ![Ícone de IA](assets/request-prompt-icon.png) sob o nome do formulário.

   Ou

   Para aplicar o documento a uma única seção, clique no ícone de IA ![Ícone de IA](assets/request-prompt-icon.png) ao lado do nome da seção.

1. Clique em **Carregar arquivos** e selecione o arquivo no gerenciador de arquivos.

   Ou

   Arraste o documento do gerenciador de arquivos para a caixa **Carregar arquivos para preencher automaticamente o formulário de solicitação**.
1. Clique em **Preencher o formulário** de **Preencher a seção**.

   O Workfront gera sugestões para o formulário.
1. Para cada sugestão de campo, selecione **Aceitar** ou **Rejeitar** abaixo desse campo.

   Ou

   Selecione **Aceitar tudo** ou **Rejeitar tudo** na parte superior da página para aceitar ou rejeitar todas as sugestões.

