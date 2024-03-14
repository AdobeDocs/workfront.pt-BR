---
content-type: api
navigation-topic: api-navigation-topic
title: Fluxo de código de autorização para aplicativos OAuth 2 personalizados
description: Fluxo de código de autorização para aplicativos OAuth 2 personalizados
author: Becky
feature: Workfront API
role: Developer
exl-id: a1ab60c4-4255-4d80-87f1-f36d325254c2
source-git-commit: 293b7354e4549e51d78ad1aa75927a21d9044c43
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 0%

---


# Configure e use os aplicativos OAuth 2 personalizados de sua organização usando o fluxo de código de autorização

Para integrar ao Workfront e permitir que seu aplicativo cliente se comunique com o Workfront em nome do usuário, é necessário:

* Criar um aplicativo OAuth2
* Configurar o aplicativo de terceiros
* Link para a página Autorizar para seus usuários
* Configurar o fluxo do código de autorização: os usuários fazem logon na instância do Workfront e consentem que permitem que o aplicativo cliente se conecte ao Workfront em seu nome. Como resultado, você recebe um código de autorização que será trocado com tokens de acesso e atualização.
* Configurar Fluxo do Token de Atualização: neste fluxo, você usa o token de atualização para obter um novo token de acesso quando o antigo expira.

## Criar um aplicativo OAuth2

Para obter instruções sobre como criar o aplicativo OAuth2, consulte [Criar um aplicativo OAuth2 usando credenciais do usuário (Fluxo de código de autorização)](../../administration-and-setup/configure-integrations/create-oauth-application.md#create3) in [Criar aplicativos OAuth2 para integrações do Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## Link para a página Autorizar para seus usuários

Seus usuários precisam fazer logon para autorizar essa integração em sua própria conta. A página que eles devem autorizar tem um formato específico, descrito aqui. Use essas informações para determinar o endereço da página de autorização do aplicativo e forneça aos usuários esse endereço ou um link para ele.

* O URL completo do domínio de sua organização. Exemplo:

  ```
  https://myorganization.my.workfront.com
  ```


* `client_id`: esta é a ID do cliente gerada quando você criou o aplicativo OAuth2 no Workfront.

* `redirect_uri`: este é o URL de redirecionamento que você inseriu ao criar o aplicativo. Seus usuários serão direcionados para esta página depois que autorizarem o aplicativo para sua conta.

* `response_type`: deve ter o valor `code`.

O URL da página de autorização é, portanto:

```
https://<URL of your organization's domain>/integrations/oauth2/authorize?client_id=<Your ClientID>&redirect_uri=<Your redirect URL>&response_type=code
```

>[!NOTE]
>
>Recomendamos a criação de um botão ou outro link que seus usuários possam clicar para ser direcionado a esta página.

## Configurar o aplicativo de terceiros

O aplicativo de terceiros pode exigir configuração. A tabela a seguir contém informações sobre campos que podem ser necessários ao configurar o aplicativo de terceiros.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URI de autorização</td> 
   <td> <p><code>https://&lt;the full URL of your organization's domain&gt;/integrations/oauth2/authorize</code> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code> https://myorganization.my.workfront.com/integrations/oauth2/authorize</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL do token</td> 
   <td> <p><code>https://&lt;the full URL of your organization's domain&gt;/integrations/oauth2/api/v1/token</code> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>https://myorganization.my.workfront.com/integrations/oauth2/api/v1/token</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Escopos</td> 
   <td>Não é necessário especificar escopos. </td> 
  </tr> 
 </tbody> 
</table>

## Configurar Fluxo de Código de Autorização

![](assets/oauth-2-authorization-code-flow.png)

Para fazer logon dos usuários com o OAuth2, use o seguinte processo:

1. Quando o usuário abre a página de autorização, ela redireciona para a página de logon do Workfront, para que o usuário possa fazer logon no Workfront. Se o usuário tiver uma configuração de SSO, a página de logon do provedor de identidade será aberta.

   Se o usuário já estiver conectado ao Workfront no mesmo navegador ou se fizer logon com êxito no Workfront, ele será redirecionado para a tela de consentimento:

   ![](assets/consent-screen-350x227.png)

1. Se o usuário Conceder acesso, a página será redirecionada para a variável `redirect_url`. O redirecionamento deve incluir os seguintes parâmetros de consulta:

* `code`: o código de autorização necessário para obter o token de acesso/atualização.
* `domain`: o domínio de sua organização. Exemplo: em `myorganization.my.workfront.com`, o domínio é `myorganization`.
* `lane`: o itinerário da solicitação. Exemplo: em `myorganization.preview.workfront.com`, a pista é `preview`.

  >[!IMPORTANT]
  >
  >A variável `code` é válido por apenas 2 minutos. Portanto, você deve obter os tokens de atualização e acesso dentro desse período.

1. Quando você tem um código, pode solicitar tokens de atualização e acesso enviando o código junto com as credenciais do aplicativo cliente para o `/integrations/oauth2/api/v1/token` terminal.

   O URL completo da solicitação de token é

   ```
   https://<URL of your organization's domain></span>/integrations/oauth2/api/v1/token
   ```

   **Exemplos:**  Exemplo de chamada CURL para o endpoint do token:

   Exemplo 1

   ```
      curl --location --request POST '**<workfront host>**/integrations/oauth2/api/v1/token' \
      --header 'Authorization: Basic **<base64(client_id:client_secret)>**' \
      --header 'Content-Type: application/json' \
      --data-raw '{
      "code": "**<code>**",
      "grant_type": "**authorization_code**",
      "redirect_uri": "**<redirect_url>**"
      }'
   ```

   Exemplo 2

   ```
      curl --location --request POST '**<workfront host>**/integrations/oauth2/api/v1/token' \
      --header 'Content-Type: application/x-www-form-urlencoded' \
      --data-urlencode 'grant_type=**authorization_code**' \
      --data-urlencode 'redirect_uri=**<redirect_url>**' \
      --data-urlencode 'code=**<code>**' \
      --data-urlencode 'client_id=**<client_id>**' \
      --data-urlencode 'client_secret=**<client_secret>**'  
   ```


   >[!IMPORTANT]
   >
   > O segredo do cliente foi gerado ao registrar o aplicativo no Workfront. Você deve armazená-lo em um local seguro, pois ele não poderá ser recuperado se for perdido.

   Quando todos os parâmetros transmitidos estiverem corretos, o endpoint do token retornará a seguinte carga:

   ```
   {
      "token_type": "sessionID",
      "access_token": "string", // the value of sessionID
      "refresh_token": "string",
      "expires_in": 0,
      "wid": "string"
   }
   ```

   O token de acesso é o mesmo que ```sessionID```e expira da mesma forma que o normal ```sessionID```

   >[!IMPORTANT]
   >
   > Armazene o token de atualização em um local seguro. Você precisará dele para obter um novo token de atualização quando o antigo expirar. A Workfront não armazena o token de atualização.

1. Agora, quando você tem um token de acesso, pode fazer chamadas de API para o Workfront

   ```
   curl --request GET 'https://<workfront host>/attask/api/v14.0/proj/search \
   --header 'sessionID: <access_token>'
   ```

## Configurar o token de acesso para atualização

![](assets/refresh-access-token-flow-350x142.png)

Para atualizar o access_token, precisamos fazer novamente uma chamada &quot;POST&quot; para o endpoint do token. Desta vez, enviamos dados de formulário diferentes da seguinte maneira:

```
curl --location --request POST '<workfront host>/integrations/oauth2/api/v1/token' \
--header 'Authorization: Basic <base64(client_id:client_secret)>' \
--header 'Content-Type: application/json' \
--data-raw '{
   "grant_type": "refresh_token",
   "refresh_token": "<refresh_token>"
}'

###### OR

curl --location --request POST '<workfront host>/integrations/oauth2/api/v1/token' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--data-urlencode 'grant_type=refresh_token' \
--data-urlencode 'redirect_uri=<redirect_url>' \
--data-urlencode 'refresh_token=<refresh_token>' \
--data-urlencode 'client_id=<client_id>' \
--data-urlencode 'client_secret=<client_secret>'
```

Ele retornará o seguinte resultado:

```
{
  "token_type": "sessionID",
  "access_token": "string", // the value of sessionID
  "refresh_token": "string",
  "expires_in": 0,
  "wid": "string"
}
```

E novamente o token de acesso é o `sessionID` que pode ser usado para fazer uma solicitação de API para o Workfront.
