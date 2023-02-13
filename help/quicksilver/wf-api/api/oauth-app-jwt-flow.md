---
content-type: api
navigation-topic: api-navigation-topic
title: Uso do fluxo JWT para aplicativos OAuth 2 personalizados
description: Uso do fluxo JWT para aplicativos OAuth 2 personalizados
author: John
feature: Workfront API
exl-id: 4bd56fe6-1f36-4c36-82cd-96de748ad680
source-git-commit: 38e957253775f73cee7fe0c0d31bfeedb58ebf53
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# Configure e use os aplicativos OAuth 2 personalizados de sua organização usando o fluxo JWT

Para se integrar ao Workfront e permitir que seu aplicativo cliente se comunique com o Workfront em nome do usuário, é necessário:

* Criar um aplicativo OAuth2
* Criar um certificado de chave pública
* Criar um JSON Web Token (JWT)

## Criar um aplicativo OAuth2

Para obter instruções sobre como criar o aplicativo OAuth2, consulte [Criar um aplicativo OAuth2 usando autenticação de servidor (fluxo JWT)](../../administration-and-setup/configure-integrations/create-oauth-application.md#create2) em [Criar aplicativos OAuth2 para integrações do Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## Criar um certificado de chave pública

O JWT deve ser assinado e a base 64 deve ser codificada para inclusão na solicitação de acesso. As bibliotecas JWT fornecem funções para executar essas tarefas.

O token deve ser assinado usando a chave privada para um certificado de assinatura digital. Nesse caso, você pode usar a chave privada de qualquer certificado associado para assinar a JWT.

O algoritmo usado é RS256 (Assinatura RSA com SHA-256). Este é um algoritmo assimétrico e usa um par de chaves públicas/privadas. O provedor de identidade tem uma chave privada (secreta) usada para gerar a assinatura, e o consumidor do JWT recebe uma chave pública para validar a assinatura.

Para gerar a chave pública, faça **one** do seguinte.

* Abra o terminal MacOS/Linux e execute o seguinte comando e faça upload `certificate_pub.crt` usando o **Adicionar chave pública** na configuração do aplicativo OAuth2 no Workfront.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>openssl req -x509 -sha256 -nodes -newkey rsa:2048 -keyout private.key -out certificate_pub.crt</code></pre>

* Use o **Gerar um par de chaves público/privado** na configuração do aplicativo OAuth2 no Workfront para gerar o RSA.

## Criar um token da Web JSON

Um token Web JSON para autenticação da conta de serviço requer um conjunto específico de solicitações e deve ser assinado usando um certificado de assinatura digital válido. Recomendamos que você use uma das bibliotecas ou ferramentas disponíveis publicamente para criar seu JWT.

A tabela a seguir contém informações sobre campos que podem ser necessários ao configurar o token JWT.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">exp</td> 
   <td> <p>Obrigatório. O parâmetro de expiração é um parâmetro obrigatório que mede o tempo absoluto desde 01/01/1970 GMT. Você deve garantir que a hora de expiração seja posterior à hora do problema. Após esse tempo, o JWT não é mais válido. </p> <p>Observação: Recomendamos que você tenha um token de duração muito curta (alguns minutos), para que ele expire logo após ter sido trocado por um token de acesso. Toda vez que um novo token de acesso é necessário, um JWT é assinado e trocado. Esta é uma abordagem mais segura. Não recomendamos tokens com vida mais longa que sejam reutilizados para obter tokens de acesso, conforme necessário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">iss</td> 
   <td>Obrigatório. O emissor é sua ID do cliente nos detalhes do aplicativo OAuth2.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">sub</td> 
   <td>Obrigatório. O assunto é a ID de usuário que criou a chave pública na configuração.</td> 
  </tr> 
 </tbody> 
</table>

## Troque o JWT para recuperar um token de acesso

1. Envie uma solicitação POST para:

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>https://yourdomain.my.workfront.com/integrations/oauth2/api/v1/jwt/exchange</code></pre>

1. O corpo da solicitação deve conter parâmetros codificados em URL com sua ID do cliente, o Segredo do cliente e o JWT:

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>client_id={client_id_value}&client_secret={client_secret_value}&jwt_token={base64_encoded_JWT}</code></pre>

 
