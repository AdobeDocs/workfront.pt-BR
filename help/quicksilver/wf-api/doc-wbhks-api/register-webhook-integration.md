---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Registrar uma integração do Webhook
description: Registrar uma integração do Webhook
author: John
feature: Workfront API
exl-id: 9a4f8dbe-967f-4a41-a42c-8e3acb604972
source-git-commit: 5cb65c3a0c3ffd374c4002867c9c48985378e03c
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 11%

---


# Registrar uma integração do Webhook

Os administradores do Adobe Workfront podem adicionar uma integração personalizada do webhook para sua empresa navegando até Configuração > Documentos > Integrações personalizadas no Workfront. Na página Integração personalizada em Configurar, os administradores podem exibir uma lista de documentos existentes que fazem parte das integrações do Webhook. Nessa página, as integrações podem ser adicionadas, editadas, habilitadas e desativadas.

Para adicionar uma integração, clique em **Adicionar integração personalizada**.

![](assets/webhooks-integration-350x230.png)

![](assets/webhooks-integration-2-350x220.png)

## Campos disponíveis

Ao adicionar uma integração, o administrador inserirá valores para os seguintes campos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome do Campo</th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Nome</td> 
   <td>O nome dessa integração.</td> 
  </tr> 
  <tr> 
   <td>URL base da API</td> 
   <td> <p>A localização da API de retorno de chamada. Ao fazer chamadas para o sistema externo, a Workfront simplesmente anexará o nome do ponto de extremidade a esse endereço. Por exemplo, se o administrador inserisse o URL da API base, "https://www.mycompany.com/api/v1", o Workfront usaria o seguinte URL para obter os metadados de um documento: https://www.mycompany.com/api/v1/metadata?id=1234.</p> </td> 
  </tr> 
  <tr> 
   <td>Parâmetros da solicitação</td> 
   <td> <p>Valores opcionais a serem acrescentados à querystring de todas as chamadas para a API. Por exemplo, access_type </p> </td> 
  </tr> 
  <tr> 
   <td>Tipo de autenticação</td> 
   <td>OAuth2 ou ApiKey</td> 
  </tr> 
  <tr> 
   <td>URL de autenticação</td> 
   <td> <p>(Somente OAuth2) O URL completo usado para autenticação de usuário. A Workfront navegará pelos usuários para esse endereço como parte do processo de provisionamento do OAuth. Observação: A Workfront anexará um parâmetro de "estado" à string de consulta. O provedor deve reenviar isso para o Workfront, anexando-o ao URI de redirecionamento do Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>URL token da extremidade final</td> 
   <td> <p>(Somente OAuth2) O URL completo da API usado para recuperar tokens OAuth2. Isso é hospedado pelo provedor do webhook ou provedor de documento externo</p> </td> 
  </tr> 
  <tr> 
   <td>ID do cliente</td> 
   <td>(Somente OAuth2) A ID do cliente OAuth2 para essa integração</td> 
  </tr> 
  <tr> 
   <td>Segredo do cliente</td> 
   <td> <p>(Somente OAuth2) O Segredo do Cliente OAuth2 para essa integração</p> </td> 
  </tr> 
  <tr> 
   <td>URL de redirecionamento do Workfront</td> 
   <td>(Somente OAuth2) Este é um campo somente leitura e é gerado pelo Workfront. Esse valor é usado para registrar essa integração no provedor de documentos externos. Observação: Conforme descrito acima para URL de autenticação, o provedor deve anexar o parâmetro "state" e seu valor à sequência de consulta ao executar o redirecionamento.</td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td> <p>(Somente ApiKey) Usado para fazer chamadas de API autorizadas para o provedor webhook. A chave da API emitida pelo provedor do webhook.</p> </td> 
  </tr> 
 </tbody> 
</table>
