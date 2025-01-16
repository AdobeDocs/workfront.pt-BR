---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Gerar um segmento de cenário usando IA
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 899641a0-a104-4be9-b423-34a32e985b53
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# Gerar um segmento de cenário usando IA

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Gerar um segmento de cenário usando a IA](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/add-a-module-with-ai.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

<!--DO NOT DELETE - linked through CSH-->

>[!IMPORTANT]
>
>Como esse recurso está no Beta, ele está disponível somente para alguns usuários do Workfront.

Você pode usar a IA para inserir um prompt de texto descrevendo o que você precisa que uma seção do seu cenário faça. O Fusion gerará módulos que executarão essas ações, que podem ser usadas no seu cenário.

Assim como em qualquer coisa gerada pela IA, recomendamos que você verifique e teste os módulos gerados para garantir que eles estejam funcionando conforme o esperado.

## Aplicativos do módulo de IA compatíveis no momento

A Fusion AI pode atualmente gerar módulos que se conectam aos seguintes aplicativos:

* Adobe Firefly
* Azure OpenAI
* Gráfico do Microsoft
* Planejamento do Adobe Workfront
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

## Gerar módulos

1. Comece a adicionar um módulo e selecione **Gerar com IA** na lista de aplicativos.

   Ou

   Clique no ícone Gerar com IA ![Gerar com IA](assets/generate-with-ai-icon-beta.png) próximo à parte inferior da página do editor de cenários.

   O painel Assistente de IA é aberto.
1. Digite um prompt de texto na caixa.

   Para obter dicas sobre prompts, consulte [Dicas para criar prompts de texto](#tips-for-creating-text-prompts) neste artigo.

   O Assistente de IA gera o módulo ou conjunto de módulos.
1. (Condicional) Se necessário, adicione seu token de API do aplicativo nos módulos.
1. Verifique os módulos para garantir que eles estejam configurados para o aplicativo e a ação apropriados.
1. (Condicional) Se a seção de cenário gerada não estiver anexada ao seu cenário, arraste-a para o lugar.

Recomendamos testar os módulos para garantir que eles estejam funcionando como esperado.

## Dicas para criar prompts de texto

Os prompts de texto devem incluir as seguintes informações no mínimo:

* O aplicativo ao qual você está se conectando
* A ação ou ações que você deseja executar

>[!IMPORTANT]
>
>Você pode gerar mais de um módulo por vez, mas só pode gerar módulos para um aplicativo por vez.

>[!INFO]
>
>**Exemplos**:
>
>* `Delete the records 'xyz-123', 'xyz-456', 'xyz-789' from Adobe Workfront Planning`
>Isso inclui o aplicativo `Workfront Planning` e a ação `delete records`. Esse prompt cria três módulos, um para cada registro que será excluído.
>* `Change campaign summary of the record 'xyz-123' from Adobe Workfront Planning`
>Isso inclui o aplicativo `Workfront Planning` e a ação `change campaign summary`.
>* `Get all field details in the record type with ID 'test-record' from Adobe Workfront Planning`
>Isso inclui o aplicativo `Workfront Planning` e a ação `get field details`.
>
>O exemplo a seguir NÃO está correto:
>
>* `Generate an image in Adobe Firefly and upload it to Dropbox`
>
>    Este exemplo está incorreto porque inclui mais de um aplicativo

Considere o seguinte ao criar prompts de texto:

* Use linguagem simples e direta.
* Verifique e teste seus módulos. Se o desempenho não for o esperado, refine o prompt e tente novamente.
