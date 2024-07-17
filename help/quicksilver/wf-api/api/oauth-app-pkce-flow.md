---
content-type: api
navigation-topic: api-navigation-topic
title: Uso do fluxo PKCE para aplicativos OAuth 2
description: Uso do fluxo PKCE para aplicativos OAuth 2
author: Becky
feature: Workfront API
role: Developer
exl-id: 61fe77b6-c6d7-4f23-bfb6-617bccaa1989
source-git-commit: 6f041459caf040846ffdec5bc75e9d74c99e318b
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 0%

---

# Configure e use os aplicativos OAuth 2 personalizados de sua organização usando o fluxo PKCE

O PKCE é um fluxo de autorização seguro que funciona bem com a atualização dinâmica de aplicativos, como aplicativos móveis, mas é valioso em todos os clientes OAuth2. Em vez de um segredo de cliente estático, o PKCE usa uma string gerada dinamicamente, eliminando o risco de um segredo de cliente vazado.

## Visão geral do PKCE

Um fluxo PKCE tem as etapas a seguir. As etapas desta seção são apresentadas apenas para fins informativos. Para executar esses procedimentos, consulte outras seções neste artigo.

1. O cliente cria o `code_challenge` transformando o `code_verifier` usando a criptografia `S256`.

1. O cliente direciona o navegador para a página de entrada OAuth2, junto com o `code_challenge` gerado. Você deve registrar seu aplicativo (Cliente) para que OAuth2 possa aceitar a solicitação de autorização. Após o registro, seu aplicativo pode redirecionar o navegador para OAuth2.

1. O servidor de autorização OAuth2 redireciona o prompt de autenticação para o usuário.

1. O usuário é autenticado usando uma das opções de logon configuradas e pode ver uma página de consentimento listando as permissões que o OAuth2 dará ao aplicativo.

1. O OAuth2 redireciona de volta para seu aplicativo com um `authorization code`.

1. Seu aplicativo envia esse código, juntamente com o `code_verifier`, para o OAuth2.

1. O Servidor de Autorização OAuth2 transforma o `code_verifier` usando o `code_challenge_method` da solicitação de autorização inicial e verifica o resultado em relação ao `code_challenge`. Se o valor de ambas as cadeias de caracteres for correspondente, o servidor verificou que as solicitações vieram do mesmo cliente e emitirá um `access token`.

1. OAuth2 retorna o `access token` e, opcionalmente, um `refresh token`.

1. Seu aplicativo agora pode usar esses tokens para chamar o servidor de recursos, como uma API, em nome do usuário.

1. O servidor de recursos valida o token antes de responder à solicitação.


## Configurar o aplicativo

Antes de implementar a autorização, é necessário registrar seu aplicativo no OAuth2 criando uma integração de aplicativo do Workfront.

Para obter instruções sobre como criar o aplicativo OAuth2, consulte [Criar um aplicativo Web de página única OAuth2 usando PKCE](../../administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-single-page-web-application-using-pkce) em [Criar aplicativos OAuth2 para integrações do Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md)

>[!NOTE]
>
>Você pode ter até dez aplicativos OAuth2 ao mesmo tempo.


## Criar a chave da prova para troca de código

Semelhante ao fluxo de Código de autorização padrão, seu aplicativo inicia redirecionando o navegador do usuário para o ponto de extremidade `/authorize` do servidor de autorização. No entanto, nesse caso, também é necessário transmitir um desafio de código.

Sua primeira etapa é gerar um verificador de código e um desafio.

<table>
  <col/>
  <col/>
    <tbody>
      <tr>
        <td role="rowheader">Verificador de código</td>
        <td>
          <p>String aleatória segura para URL com um comprimento mínimo de 43 caracteres</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">Desafio do código</td>
        <td>
          <p>Hash SHA-256 codificado em URL Base64 do verificador de código</p>
        </td>
      </tr>
    </tbody>
</table>


Você deve adicionar código no aplicativo cliente para criar o verificador de código e o desafio de código.

O código do gerador PKCE cria uma saída semelhante à seguinte:

>[!INFO]
>
>**Exemplo:**
>
>```
>{
>  "code\_verifier":"N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat",
>  "code\_challenge":"wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>}
>```

Seu aplicativo salva o `code_verifier` para depois e envia o `code_challenge` junto com a solicitação de autorização para a URL `/authorize` do seu Servidor de Autorização.

## Solicitar um código de autorização

Se você estiver usando o Servidor de autorização personalizado padrão, seu URL de solicitação será semelhante ao seguinte:

>[!INFO]
>
>**Exemplo:**
>
>
>```
>/authorize?client\_id=<clientID>&response\_type=code&redirect\_uri=<redirectURL>
>&code\_challenge\_method=S256&code\_challenge=wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>```

Observe os parâmetros que estão sendo transmitidos:

* `client_id` corresponde à ID do cliente do aplicativo OAuth2 que você criou no ao configurar o aplicativo.

  Para obter instruções, consulte Criar um aplicativo web de página única OAuth2 usando PKCE em Criar aplicativos OAuth2 para integrações do Workfront.

* `response_type` é `code`, porque o aplicativo usa o tipo de concessão Código de Autorização.

* `redirect_uri` é o local de retorno de chamada para o qual o agente do usuário é direcionado junto com o `code`. Deve corresponder a um dos URLs de redirecionamento especificados ao criar o aplicativo OAuth2.

* `code_challenge_method` é o método de hash usado para gerar o desafio, que é sempre `S256` para aplicativos Workfront Oauth2 que usam PKCE.

* `code_challenge` é o desafio de código usado para PKCE.


## Trocar o código por tokens

Para trocar o código de autorização por um token de acesso, passe-o para o ponto de extremidade `/token` do Servidor de Autorização junto com o `code_verifier`.

>[!INFO]
>
>**Exemplo:**
>
>```
>/token \\
>  --header 'accept: application/json' \\
>  --header 'cache-control: no-cache' \\
>  --header 'content-type: application/x-www-form-urlencoded' \\
>  --data 'grant\_type=authorization\_code&client\_id=<clientID>&redirect\_uri=<redirectURL>&code=<code>&code\_verifier=N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat
>```

>[!IMPORTANT]
>
> Ao contrário do fluxo normal do Código de autorização, essa chamada não exige o cabeçalho de autorização com a ID do cliente e o segredo. É por isso que essa versão do fluxo do Código de autorização é adequada para aplicativos nativos, como aplicativos móveis ou aplicativos de página única que não têm um back-end.

Observe os parâmetros que estão sendo transmitidos:

* `grant_type` é `authorization_code`, porque o aplicativo usa o tipo de concessão Código de Autorização.

* `redirect_uri` deve corresponder ao URI que foi usado para obter o código de autorização.

* `code` é o código de autorização recebido do ponto de extremidade /authorize.

* `code_verifier` é o verificador de código PKCE gerado pelo seu aplicativo em [Criar a Chave de Prova para Troca de Código](#Create).

* `client_id` identifica seu cliente e deve corresponder ao valor pré-registrado em OAuth2.


Se o código ainda for válido e o verificador de código corresponder, seu aplicativo receberá um token de acesso.

>[!INFO]
>
>**Exemplo:**
>
>```
>{
>    "access\_token": "eyJhd\[...\]Yozv",
>    "expires\_in": 3600,
>    "token\_type": "Bearer"
>}
>```

## Validar o token de acesso

Quando o aplicativo transmite uma solicitação com um token de acesso, o servidor de recursos precisa validá-lo.

Você pode validar seu token de acesso com uma chamada de API semelhante ao seguinte:

>[!INFO]
>
>**Exemplo:**
>
>```
>/attask/api/<api version>/proj/search \\
>  --header 'sessionID: <access\_token>' \\
>```

## Solicitar um token de atualização

Para solicitar um token de atualização, você pode fazer uma chamada de POST para a API, semelhante ao seguinte:

>[!INFO]
>
>**Exemplo:**
>
>```
>/token \\
>  --header 'accept: application/json' \\
>  --header 'cache-control: no-cache' \\
>  --header 'content-type: application/x-www-form-urlencoded' \\
>  --data 'grant\_type=refresh\_token&client\_id=<clientID>&redirect\_uri=<redirectURL>&refresh\_token=<refresh\_token>
>```
