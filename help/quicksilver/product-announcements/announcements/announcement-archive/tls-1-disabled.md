---
content-type: reference
navigation-topic: announcements
title: TLS 1.2 necessário no Adobe Workfront
description: Para fornecer segurança ideal, o Adobe Workfront exige que todas as conexões de navegador e integrações de API que dependem do TLS 1.0 ou anterior sejam atualizadas para usar o TLS 1.2. No ambiente de Pré-visualização, o TLS 1.0 já está desativado.
author: Luke
feature: Product Announcements
exl-id: 153668ae-0647-47fd-9153-ce45cd8c54ee
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# TLS 1.2 necessário no Adobe Workfront

Para fornecer segurança ideal, o Adobe Workfront exige que todas as conexões de navegador e integrações de API que dependem do TLS 1.0 ou anterior sejam atualizadas para usar o TLS 1.2. No ambiente de Pré-visualização, o TLS 1.0 já está desativado.

A Workfront encerrou oficialmente o suporte ao TLS 1.0 em março de 2018. Todas as integrações que usam o TLS 1.0 deixaram de funcionar a partir de 9 de janeiro de 2019.  O TLS 1.1 será desativado no quarto trimestre de 2019.

As seções a seguir fornecem mais detalhes sobre esses marcos importantes, bem como sobre como você pode se preparar para essa atualização em sua organização:

## O Workfront encerra o suporte oficial ao TLS 1.0 (5 de março de 2018)

O Workfront encerrou o suporte oficial ao TLS 1.0 em março de 2018.

As conexões do navegador e as integrações de API que usam o TLS 1.0 ainda estão operacionais, mas o Workfront não resolverá problemas no aplicativo do Workfront relacionados ao TLS 1.0.

## Integrações do Workfront usando TLS 1.0 desabilitadas (9 de janeiro de 2019)

Em 9 de janeiro de 2019, todas as conexões do navegador Workfront e integrações de API que usam TLS 1.0 devem ser atualizadas para usar o TLS 1.1 ou posterior. As conexões do navegador e as integrações de API que continuam usando o TLS 1.0 (conexões de entrada ou de saída) não poderão mais se comunicar com o aplicativo do Workfront após esse tempo. 

## O TLS 1.1 será desativado no quarto trimestre de 2019

No ambiente de Produção, o TLS 1.1 foi desativado em 21 de outubro de 2019. Após esse tempo, todas as integrações que usam TLS 1.1 não funcionarão.

Essa alteração entrará em vigor nos ambientes Pré-visualização e Sandbox em 7 de agosto para ajudar as organizações a se prepararem para o encerramento.

## Preparação para a atualização do TLS

* [Ao acessar o Workfront pelo navegador](#when-accessing-workfront-via-the-browser)
* [Ao se conectar ao Workfront por meio da API](#when-connecting-to-workfront-via-the-api)

### Ao acessar o Workfront pelo navegador {#when-accessing-workfront-via-the-browser}

Verifique se os usuários em sua organização estão acessando o Workfront por meio de um navegador compatível. (Para obter informações sobre navegadores compatíveis, consulte [requisitos do navegador Adobe Workfront](../../../workfront-basics/workfront-browser-requirements.md).)

Todos os navegadores suportados pelo Workfront são compatíveis com TLS 1.2.

### Ao se conectar ao Workfront por meio da API {#when-connecting-to-workfront-via-the-api}

Se estiver integrando aplicativos de terceiros ao Workfront por meio da API (de entrada ou de saída), verifique se o TLS 1.2 (e os protocolos de criptografia TLS 1.2) estão habilitados em suas integrações.
