---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Autenticação para Webhooks de Documento
description: Autenticação para Webhooks de Documento
author: John
feature: Workfront API
exl-id: 2303c202-27c7-4922-a613-e9824910504c
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Autenticação para Webhooks de Documento

## Autenticação

Os webhooks de documentos do Adobe Workfront oferecem suporte a duas formas diferentes de autenticação: OAuth2 e ApiKey. Em ambos os casos, o Workfront transmite tokens de autenticação no cabeçalho ao fazer uma chamada de API.

### OAuth2

O OAuth2 permite que o Workfront faça chamadas de API autorizadas para um provedor de webhook em nome de um usuário. Antes de fazer isso, o usuário deve conectar sua conta externa de provedor de documentos à Workfront e conceder a Workfront

o acesso à ação em seu nome. Esse processo de handshaking só acontece uma vez para cada usuário. Veja como funciona:

1. O usuário começa a conectar a integração do webhook à sua conta. Atualmente, isso é feito clicando na lista suspensa &quot;Adicionar documento&quot; > &quot;Adicionar serviço&quot; > Nome da integração personalizada.
1. O Workfront navega pelo usuário o URL de autenticação, que pode solicitar que o usuário faça logon no provedor de documento externo. Esta página é hospedada pelo provedor do webhook ou pelo sistema externo de gerenciamento de documentos. Ao fazer isso, o Workfront adiciona um parâmetro &quot;state&quot; ao URL de autenticação. Esse valor deve ser retornado ao Workfront, anexando o mesmo valor ao URI de retorno do Workfront na etapa abaixo.
1. Depois de fazer logon no sistema externo (ou se o usuário já estiver conectado), o usuário é levado a uma página de &quot;Autenticação&quot;, o que explica que a Workfront está solicitando acesso para executar um conjunto de ações em nome do usuário.
1. Se o usuário clicar no botão &quot;Permitir&quot;, o navegador redirecionará para o URI de redirecionamento do Workfront , adicionando &quot;code=`<code>`&quot; para a querystring. De acordo com a especificação do OAuth2, esse token tem duração curta. A querystring também deve ter o seguinte, &quot;state=`<sent_by_workfront>`&quot;.
1. A Workfront processa essa solicitação e faz uma chamada de API para o URL do ponto de extremidade do token com o código de autorização.
1. O URL do Ponto de Extremidade do Token retorna um token de atualização e um token de acesso.
1. A Workfront armazena esses tokens e fornece a integração do webhook para esse usuário.
1. A partir desse ponto, o Workfront poderá fazer chamadas de API autorizadas para o provedor do webhook. Ao fazer essas chamadas, o Workfront enviará o token de acesso no cabeçalho da solicitação HTTP, como mostrado abaixo:

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. Se o token de acesso tiver expirado, o Workfront fará uma chamada para o URL do ponto de extremidade do token para recuperar um novo token de acesso e, em seguida, tentará a chamada da API autorizada novamente com o novo token de acesso.

### ApiKey

Fazer chamadas de API autorizadas para um provedor de webhook usando uma ApiKey é muito mais simples do que o OAuth2. Ao fazer uma chamada de API, o Workfront simplesmente passará a ApiKey e o nome de usuário Workfront no cabeçalho de solicitação HTTP: 

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

O provedor Webhook pode usar o nome de usuário para aplicar permissões específicas do usuário. Isso funciona melhor quando ambos os sistemas se conectam ao LDAP usando o Single Sign On (SSO).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Adding Request Headers (optional)</h3>
<p>In addition to using either OAuth2 tokens or an ApiKey for authentication, Workfront can send a predefined set of headers to the webhook provider for every API call. A Workfront admin can setup set this up when&nbsp;registering or editing a Webook Integration, as described in the section above. See Registering a Webhook Integration.</p>
<p>For example, this can be used for Basic Authentication. To do this, the Workfront administrator would add the following Request Header information in the Custom Integration dialog:</p>
<p>&nbsp; &nbsp; &nbsp;Authorization Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==</p>
<p>where QWxhZGRpbjpvcGVuIHNlc2FtZQ== is a base-64 encoded string of “username:password”. See Basic Authentication . Provided that this added, Workfront will pass this in the HTTP request header, in addition to other request headers:&nbsp;</p>
<p>-------------------------------</p>
<p>apiKey: 12345</p>
<p>username: johndoe@foo.com</p>
<p>Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­</p>
<p>-------------------------------</p>
</div>
-->
