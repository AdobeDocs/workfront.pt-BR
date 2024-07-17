---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Autenticação para webhooks de documentos
description: Autenticação para webhooks de documentos
author: Becky
feature: Workfront API
role: Developer
exl-id: 2303c202-27c7-4922-a613-e9824910504c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Autenticação para webhooks de documentos

## Autenticação

Os webhooks de documento do Adobe Workfront são compatíveis com duas formas diferentes de autenticação: OAuth2 e ApiKey. Em ambos os casos, o Workfront transmite tokens de autenticação no cabeçalho ao fazer uma chamada de API.

### OAuth2

O OAuth2 permite que o Workfront faça chamadas de API autorizadas para um provedor de webhook em nome de um usuário. Antes de fazer isso, o usuário deve conectar a conta do provedor de documentos externo ao Workfront e conceder o Workfront

acesso para agirem em seu nome. Esse processo de handshaking só ocorre uma vez para cada usuário. Veja como isso funciona:

1. O usuário começa conectando a integração do webhook à conta. Atualmente, isso é feito clicando na lista suspensa &quot;Adicionar documento&quot; > &quot;Adicionar serviço&quot; > Nome da integração personalizada.
1. O Workfront navega o usuário pelo URL de autenticação, que pode solicitar que o usuário faça logon no provedor de documentos externo. Esta página é hospedada pelo provedor de webhook ou pelo sistema de gerenciamento de documentos externo. Ao fazer isso, o Workfront adiciona um parâmetro de &quot;estado&quot; ao URL de autenticação. Esse valor deve ser passado de volta para o Workfront, anexando o mesmo valor ao URI de retorno do Workfront na etapa abaixo.
1. Depois de fazer logon no sistema externo (ou se o usuário já estiver conectado), o usuário é direcionado para uma página &quot;Autenticação&quot;, que explica que a Workfront está solicitando acesso para executar um conjunto de ações em nome do usuário.
1. Se o usuário clicar no botão &quot;Permitir&quot;, o navegador será redirecionado para o URI de Redirecionamento do Workfront, adicionando &quot;code=`<code>`&quot; à querystring. De acordo com a especificação do OAuth2, esse token tem vida curta. A sequência de consulta também deve ter o seguinte, &quot;state=`<sent_by_workfront>`&quot;.
1. O Workfront processa essa solicitação e faz uma chamada de API para o URL do ponto de extremidade token com o código de autorização.
1. O URL do ponto de extremidade do token retorna um token de atualização e um token de acesso.
1. O Workfront armazena esses tokens e provisiona totalmente a integração de webhook para esse usuário.
1. A partir desse ponto, o Workfront poderá fazer chamadas autorizadas para a API do provedor do webhook. Ao fazer essas chamadas, o Workfront enviará o token de acesso no cabeçalho da solicitação HTTP, conforme mostrado abaixo:

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. Se o token de acesso tiver expirado, a Workfront fará uma chamada para o URL do ponto de extremidade do token para recuperar um novo token de acesso e, em seguida, tentará realizar a chamada de API autorizada novamente com o novo token de acesso.

### ApiKey

Fazer chamadas de API autorizadas para um provedor de webhook usando uma ApiKey é muito mais simples do que o OAuth2. Ao fazer uma chamada de API, o Workfront simplesmente passará o ApiKey e o nome de usuário do Workfront no cabeçalho da solicitação HTTP: 

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

O provedor Webhook pode usar o nome de usuário para aplicar permissões específicas do usuário. Isso funciona melhor quando ambos os sistemas se conectam ao LDAP usando o Logon único (SSO).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Adding Request Headers (optional)</h3>
<p>In addition to using either OAuth2 tokens or an ApiKey for authentication, Workfront can send a predefined set of headers to the webhook provider for every API call. A Workfront admin can setup set this up when&nbsp;registering or editing a Webook Integration, as described in the section above. See Registering a Webhook Integration.</p>
<p>For example, this can be used for Basic Authentication. To do this, the Workfront administrator would add the following Request Header information in the Custom Integration dialog:</p>
<p>&nbsp; &nbsp; &nbsp;Authorization Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==</p>
<p>where QWxhZGRpbjpvcGVuIHNlc2FtZQ== is a base-64 encoded string of "username:password". See Basic Authentication . Provided that this added, Workfront will pass this in the HTTP request header, in addition to other request headers:&nbsp;</p>
<p>-------------------------------</p>
<p>apiKey: 12345</p>
<p>username: johndoe@foo.com</p>
<p>Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­</p>
<p>-------------------------------</p>
</div>
-->
