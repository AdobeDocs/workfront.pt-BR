---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obter tokens do OAuth2
description: Obter tokens do OAuth2
author: Becky
feature: Workfront API
role: Developer
exl-id: f3a2630d-d34e-4d36-b2bb-707ba0d3258e
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 3%

---


# Obter tokens do OAuth2

## Obtenção de tokens do OAuth2

Retorna o token de atualização OAuth2 e o token de acesso para um usuário autenticado. Isso é chamado uma vez quando o usuário provisiona um Provedor de documentos. As chamadas subsequentes são feitas para obter um token de acesso atualizado.

**URL**

POST /any/url

O URL é configurável e corresponde ao valor do URL do endpoint do token na página de configuração da integração personalizada.

### Parâmetros de consulta

<table style="table-layout:auto">
 <col>
 <col>
 <col>
 <thead>
  <tr>
   <th>Nome</th>
   <th>Obrigatório</th>
   <th>Descrição</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>grant_type</td>
   <td>sim</td>
   <td><p>Os valores incluem "authorization_code" ou "refresh_token". O valor especificado indica qual dos dois parâmetros será passado para esta chamada de API: code ou refresh_token.</p></td>
  </tr>
  <tr>
   <td>código</td>
   <td>depende</td>
   <td><p>O código de autorização enviado ao Adobe Workfront logo após o usuário clicar no botão "Conceder". Isso só é necessário quando o tipo de concessão é "authorization_code". O código de autorização deve ter uma vida curta, geralmente expirando em 10 minutos ou menos.</p></td>
  </tr>
  <tr>
   <td>refresh_token</td>
   <td>depende</td>
   <td><p>Isso só é necessário ao fazer chamadas subsequentes para recuperar um novo access_token, visto que o access_token anterior expirou. Ao enviar esse valor, defina o parâmetro grant_type como "refresh_token".</p></td>
  </tr>
  <tr>
   <td>client_id</td>
   <td>sim</td>
   <td>A ID do cliente configurada no Workfront para essa integração personalizada.</td>
  </tr>
  <tr>
   <td>client_secret</td>
   <td>sim</td>
   <td> O Segredo do cliente configurado no Workfront para essa integração personalizada.</td>
  </tr>
 </tbody>
</table>

 

## Resposta

<table style="table-layout:auto">
 <col>
 <col>
 <col>
 <thead>
  <tr>
   <th>Nome</th>
   <th>Tipo </th>
   <th>Descrição</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>access_token </td>
   <td>String</td>
   <td><p>Um token usado para fazer chamadas de API autorizadas em nome do usuário. Isso deve expirar para evitar chamadas de API não autorizadas.</p></td>
  </tr>
  <tr>
   <td>refresh_token </td>
   <td>String</td>
   <td><p>Um token de longa duração usado para recuperar um novo access_token chamando esse método de API.</p></td>
  </tr>
  <tr>
   <td>expires_in </td>
   <td>long</td>
   <td><p>(opcional) O tempo (em segundos) antes que o access_token expire, geralmente 3.600.</p></td>
  </tr>
 </tbody>
</table>

**Exemplo**

```
POST /oauth2/token
grant_type=authorization_code
code=d9ac7asdf6asdf579d7a8
client_id=123456
client_secret=6asdf7a7a9a4af
```

## Resposta

```
{
access_token:"ad8af5ad5ads759",
refresh_token:"9a0h5d87d808ads",
expires_id:3600
}
```
