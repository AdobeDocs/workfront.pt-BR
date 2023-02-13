---
title: Visão geral
description: Visão geral
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
exl-id: 882b657a-1bde-4efd-93e8-1de80c065b2d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 1%

---

# Visão geral

**Bem-vindo à API de prova do Workfront**

A Workfront Proof API é um serviço HTTP simples, protegido por SSL. A API tem como objetivo fornecer toda a funcionalidade usada em nosso próprio aplicativo.

## Formatos compatíveis

A interface pública é compatível com SOAP 1.1 com suporte a WSDL. Todas as solicitações são executadas usando XML em HTTPS.

## Controle de versão da API

Para preservar a compatibilidade com a integração do cliente existente, introduzimos o controle de versão da API a partir da versão 12.1. Consulte a  [Atualizações da API](http://api.proofhq.com/new-updates) para obter mais informações. Se um método ou parâmetro não tiver informações de versão, significa que você o encontrará como parte de nossa API padrão, consulte a seção &quot;Introdução à API&quot; abaixo.

## Introdução à API

O ponto de entrada da API:

`https://soap.proofhq.com/soap` (observe o uso de HTTPS)

O WSDL pode ser encontrado aqui:

`https://soap.proofhq.com/soap?wsdl`

>[!NOTE]
>
>**Esse WSDL contém todas as alterações até a versão 12.1, após a qual introduzimos o controle de versão da API. Consulte a página Atualizações da API para obter mais informações sobre as várias versões do WSDL e as alterações futuras**

Cada solicitação de API requer uma chave de sessão. Essa chave de sessão identifica o usuário da Workfront Proof que está executando as ações e é obtida chamando o método doLogin() e transmitindo o endereço de email e a senha do usuário. O método doLogin() só precisa ser chamado uma vez antes de uma sequência de solicitações de API. A chave de sessão permanece ativa por um curto período de tempo e é renovada em cada chamada de método. *Em breve, adicionaremos suporte à autenticação baseada em token.*

Todas as solicitações usam o seguinte envelope, cabeçalho e formato de corpo:

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:urn="urn:proofhqapi">`
   <soapenv:Header/>
   <soapenv:Body>
	   ... API function and data inserted here ...
	</soapenv:Body>
	</soapenv:Envelope>
```

## Perguntas frequentes

Para obter uma coleção de perguntas frequentes, visite [this](http://api.proofhq.com/faqs) página.
