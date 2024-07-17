---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Gerar um módulo usando IA
description: Você pode inserir um prompt de texto para criar um módulo HTTP configurado para o prompt.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 899641a0-a104-4be9-b423-34a32e985b53
source-git-commit: 0a01acd56b3ea10d1cccc31a21e434da55b1ec13
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 1%

---

# Gerar um módulo usando IA

<!--DO NOT DELETE - linked through CSH-->

>[!IMPORTANT]
>
>Como esse recurso ainda está nos estágios iniciais de desenvolvimento, ele está disponível somente para usuários internos do Workfront.

Você pode usar a IA para inserir um prompt de texto descrevendo o que um módulo precisa fazer. O Fusion gerará um módulo HTTP que se conectará ao endpoint correto da API desejada.

Assim como em qualquer coisa gerada pela IA, recomendamos que você verifique e teste o módulo gerado para garantir que ele esteja funcionando conforme o esperado.

## Aplicativos do módulo de IA compatíveis no momento

A Fusion AI pode atualmente gerar módulos que se conectam aos seguintes aplicativos:

* Adobe Firefly
* Azure OpenAI
* Gráfico do Microsoft
* Adobe Maestro
* Adobe Analytics
* Serviços da Adobe PDF
* Adobe Marketo
* Adobe Frame.io
* Dropbox
* NetSuite
* Calendário do Google
* Atlassian Jira
* GitLab
* Spotify
* Bitbucket
* OpenAI
* Slack

## Gerar um módulo

1. Adicione um módulo e selecione **Gerar com IA** na lista de aplicativos.

   Ou

   Clique com o botão direito do mouse em uma área em branco do editor de cenários e selecione **Gerar com IA**.
1. Digite um prompt de texto na caixa.

   Para obter dicas sobre prompts, consulte [Dicas para criar prompts de texto](#tips-for-creating-text-prompts) neste artigo.
1. Adicione o token da API do aplicativo no módulo.
1. Verifique o módulo para garantir que ele pareça estar configurado para o aplicativo e a ação apropriados.
1. (Condicional) Se o módulo não estiver anexado ao seu cenário, arraste-o para o lugar.

Recomendamos testar o módulo para garantir que o módulo gerado esteja funcionando como esperado.

## Dicas para criar prompts de texto

Os prompts de texto devem incluir as seguintes informações no mínimo:

* O aplicativo ao qual você está se conectando
* A ação que você deseja executar

>[!INFO]
>
>**Exemplos**:
>
>* `Retrieve a list of my calendars from Google Calendar`
>
>   Isso inclui o aplicativo `Google Calendar` e a ação `Retrieve a list of my calendars`.
>
>* `Retrieve popular songs from Spotify`
>
>   Isso inclui o aplicativo `Spotify` e a ação `Retrieve popular songs`.

Considere o seguinte ao criar prompts de texto:

* Como cada módulo Fusion executa uma única ação, seu prompt de texto deve descrever uma ação específica.
* Use linguagem simples e direta.
* Verifique e teste seu módulo. Se o desempenho não for o esperado, refine o prompt e tente novamente.
