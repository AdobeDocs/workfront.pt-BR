---
title: Visão geral
description: Visão geral
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
role: Developer
exl-id: 882b657a-1bde-4efd-93e8-1de80c065b2d
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 1%

---

# Visão geral

**Bem-vindo à API do Workfront Proof**

A API do Workfront Proof é um serviço HTTP simples que é protegido usando SSL. A API tem como objetivo fornecer toda a funcionalidade usada em nosso próprio aplicativo.

## Formatos compatíveis

A interface pública é compatível com SOAP 1.1 e WSDL. Todas as solicitações são executadas usando XML sobre HTTPS.

## Controle de versão da API

Para preservar a compatibilidade com as integrações de clientes existentes, introduzimos o controle de versão da API a partir da versão 12.1. Consulte a  Página [Atualizações de API](https://api.proofhq.com/new-updates.html) para obter mais informações. Se um método ou parâmetro não tiver informações de versão, significa que você as encontrará como parte de nossa API padrão. Consulte a seção &quot;Introdução à API&quot; abaixo.

## Introdução à API

O ponto de entrada da API:

`https://soap.proofhq.com/soap` (observe o uso de HTTPS)

O WSDL pode ser encontrado aqui:

`https://soap.proofhq.com/soap?wsdl`

>[!NOTE]
>
>**Este WSDL contém todas as alterações até a versão 12.1, após a qual introduzimos o controle de versão da API. Consulte a página Atualizações de API para obter mais informações sobre as várias versões WSDL e alterações futuras**

Cada solicitação de API exige uma chave de sessão. Essa chave de sessão identifica o usuário do Workfront Proof que executa a(s) ação(ões) e é obtida ao chamar o método doLogin() e transmitir o endereço de email e a senha do usuário. O método doLogin() só precisa ser chamado uma vez antes de uma sequência de solicitações de API. A chave de sessão permanece ativa por um curto período e é renovada em cada chamada de método. *O suporte para autenticação baseada em token será adicionado em breve.*

Todas as solicitações usam o seguinte formato de envelope, cabeçalho e corpo:

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:urn="urn:proofhqapi">`
   <soapenv:Header/>
   <soapenv:Body>
       ... API function and data inserted here ...
    </soapenv:Body>
    </soapenv:Envelope>
```

