---
product-area: documents
navigation-topic: proofing-overview
title: Revisar conteúdo interativo na extensão do visualizador de provas web
description: A ferramenta de revisão do Adobe Workfront é uma extensão de navegador que permite revisar o conteúdo interativo em um arquivo ZIP ou com um URL.
author: Courtney
feature: Digital Content and Documents
exl-id: 4fea13cc-2d56-466e-8851-6134782e7e80
source-git-commit: 7b02d5670ebba1456e37e6fd815e7812ec06def2
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 1%

---

# Revisar conteúdo interativo com a ferramenta de revisão do Adobe Workfront

<span class="preview">A ferramenta Adobe Workfront Review estará disponível em 7 de novembro de 2024. Esta extensão está atualmente na versão beta.</span>

A ferramenta de revisão do Adobe Workfront é uma extensão de navegador baseada na Web que permite revisar o conteúdo interativo em um arquivo ZIP ou com um URL. A ferramenta de revisão do Adobe Workfront está disponível nos seguintes navegadores:

* Firefox
* Chrome
* Edge
* Safari

Recomendamos o uso do Visualizador de provas de desktop se o conteúdo que você precisa revisar estiver em um site que

* Requer autenticação SSO
* Impede a abertura do site em iFrames, como o Figma


## Instalar a extensão

### Pré-requisitos

* Remova a extensão do Web Viewer herdado para usar a ferramenta Adobe Workfront Review.

### Instalar a extensão

<!--This extension is required to review conent in GS and Ex.

You must install the extension to reiew content in GenS and Express.

To review content in GS, Express, or Wou must install the extension if you are using GenStuido or Creative cloud express-->

Revisores e aprovadores devem instalar a ferramenta de revisão do Adobe Workfront. em um dos seguintes navegadores:

* [Extensão do Firefox](https://addons.mozilla.org/en-US/firefox/addon/adobe-workfront-review-tool/)

* [Extensão do Chrome](https://chromewebstore.google.com/detail/adobe-workfront-review-to/lhdepbgeilldghlfnankdnponhljpgml)

* [Edge](https://microsoftedge.microsoft.com/addons/detail/adobe-workfront-review-to/llhapmaiiddmcamgeapaipjpagnoijen)


Para que as provas interativas sejam abertas automaticamente na ferramenta de revisão do Adobe Workfront, um administrador do Workfront deve atualizar as configurações de Prova no Workfront, conforme descrito nas seções abaixo.

## Atualizar padrões de prova do Workfront

### Tornar a ferramenta de revisão do Adobe Workfront o visualizador padrão para provas de URL e ZIP

Para usar a ferramenta de revisão da Web para provas de URL e ZIP, um administrador do Workfront deve ajustar a configuração padrão para provas interativas.

1. No menu principal do Workfront, clique em **Revisão**.
1. Clique em **Configurações da conta** e na guia **Configurações**.
1. Na seção **Padrões de Prova**, localize o **Visualizador de Provas de Desktop para Provas Interativas** e clique em **Configurar**.
1. No menu suspenso, escolha **Desabilitado**. As provas interativas criadas a partir de um URL ou arquivo ZIP agora são abertas automaticamente na ferramenta Adobe Workfront Review, que é um navegador baseado na Web.
1. Clique em **Salvar**.

>[!NOTE]
>
>Essa alteração se aplica a todas as provas interativas na instância do Workfront. Recomendamos testar a nova experiência no ambiente de Pré-visualização antes de habilitá-la na Produção. Você pode voltar facilmente para o Visualizador de Área de Trabalho alterando a configuração da conta **Visualizador de Revisão de Desktop para Prova Interativa** de volta para **Habilitado para todas as provas interativas**.

### Tornar a ferramenta de revisão do Adobe Workfront o visualizador padrão somente para provas de ZIP

Para usar a ferramenta de revisão da Web somente para provas ZIP, um administrador do Workfront deve ajustar a configuração padrão para provas interativas.

1. No menu principal do Workfront, clique em **Revisão**.
1. Clique em **Configurações da conta** e na guia **Configurações**.
1. Na seção **Padrões de Prova**, localize o **Visualizador de Provas de Desktop para Provas Interativas** e clique em **Configurar**.
1. No menu suspenso, escolha **Habilitado apenas para provas interativas criadas a partir de uma URL**. As provas interativas criadas a partir de um arquivo ZIP agora são abertas automaticamente na ferramenta Adobe Workfront Review, que é um navegador baseado na Web. As provas interativas criadas a partir de um URL ainda estão abertas no Visualizador de provas da área de trabalho.
1. Clique em **Salvar**.

>[!NOTE]
>
>Essa alteração se aplica a todas as provas de ZIP na instância do Workfront. Recomendamos testar a nova experiência no ambiente de Pré-visualização antes de habilitá-la na Produção. Você pode voltar facilmente para o Visualizador de Área de Trabalho alterando a configuração da conta **Visualizador de Revisão de Desktop para Prova Interativa** de volta para **Habilitado para todas as provas interativas**.



