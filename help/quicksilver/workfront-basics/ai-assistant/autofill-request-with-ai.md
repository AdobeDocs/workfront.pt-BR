---
title: Preencher uma solicitação automaticamente usando IA
content-type: reference
description: Você pode usar a IA para preencher automaticamente os campos de solicitação.
author: Becky
feature: Get Started with Workfront
hide: true
hidefromtoc: true
source-git-commit: 9e1a5718092092bb9ca98cf92ddd2a1a07f32f51
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# Preencher uma solicitação automaticamente usando IA

A IA pode ajudar a preencher automaticamente os campos de solicitação. Ele pode sugerir valores de campo com base em solicitações anteriores ou analisá-los a partir de texto, como emails.

Você pode aprovar ou rejeitar esses envios antes de enviar a solicitação.

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

O preenchimento automático pode sugerir valores de campo com base em texto, como emails. Você cola em um bloco de texto e o Workfront processa o texto para sugerir valores de campo com base no texto.

Por exemplo, se o email incluir &quot;Isso vence em 1º de junho&quot; e o formulário de solicitação tiver um campo para data de vencimento, a Workfront sugerirá 1º de junho para esse valor de campo.

Esse tipo de sugestão também verifica solicitações anteriores para contextos semelhantes. Por exemplo, se o prompt mencionar que a solicitação é para um determinado cliente, o Workfront poderá localizar e inserir o endereço de faturamento desse cliente automaticamente, com base em solicitações anteriores.

Você pode colar no texto a ser aplicado a todo o formulário ou a uma única seção do formulário.

Para usar sugestões com base em um prompt de texto colado:

1. Comece a criar uma solicitação.

   Para obter instruções, consulte [Criar e enviar solicitações](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Para aplicar o prompt de texto a todo o formulário, clique em **Preenchimento automático com IA** no canto superior direito da tela.

   Ou

   Para aplicar o prompt de texto para uma única seção, clique no ícone de IA ![Ícone de IA](assets/request-prompt-icon.png) ao lado do nome da seção.

1. Cole o texto na caixa de prompt.
1. Clique em **Preencher o formulário**.

   O Workfront gera sugestões para o formulário.
1. Para cada sugestão de campo, selecione **Aceitar** ou **Rejeitar** abaixo desse campo.

   Ou

   Selecione **Aceitar tudo** ou **Rejeitar tudo** na parte superior da página para aceitar ou rejeitar todas as sugestões.

