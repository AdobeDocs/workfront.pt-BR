---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: HTTP &gt; Outros módulos
description: A variável [!DNL Adobe Workfront Fusion] O aplicativo HTTP fornece vários módulos para comunicação com base no protocolo HTTP (Hypertext Transfer Protocol). HTTP é a base da comunicação de dados para a World Wide Web. Você pode usar os módulos do para baixar páginas e arquivos da Web, chamar webhooks e endpoints de API e assim por diante.
author: Becky
feature: Workfront Fusion
exl-id: ff2cd098-d1d7-43a3-9f00-15e0f6e92332
source-git-commit: 45540ccc3b9fca98f8aaae86ac4d6574a067a6e4
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---

# HTTP > Outros módulos

>[!NOTE]
>
>[!UICONTROL Adobe Workfront Fusion] exige um [!UICONTROL Adobe Workfront Fusion] além de uma licença [!UICONTROL Adobe Workfront] licença.

A variável [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] O aplicativo fornece vários módulos para comunicação com base no protocolo HTTP (Hypertext Transfer Protocol). HTTP é a base da comunicação de dados para a World Wide Web. Você pode usar os módulos do para baixar páginas e arquivos da Web, chamar webhooks e endpoints de API e assim por diante.

A escolha correta do módulo depende do mecanismo de autenticação/ autorização que o recurso que você deseja acessar emprega. Veja a seguir exemplos de módulos

* Fazer uma solicitação:módulo universal destinado principalmente a recursos que não empregam nenhum tipo de autenticação/autorização
* Fazer uma solicitação de Autenticação básica:para recursos que empregam [!DNL HTTP] Autenticação básica (BA)
* Fazer uma solicitação OAuth 2.0: para recursos que empregam o protocolo de autorização OAuth 2.0
* Fazer uma solicitação de Autenticação de certificado de cliente: para recursos que utilizam protocolo de autorização que requer um certificado do lado do cliente.
* Fazer uma solicitação de autorização de Chave de API: para recursos que utilizam Chaves de API para autorização.

>[!NOTE]
>
>Se você estiver se conectando a um produto Adobe que não tem um conector dedicado no momento, recomendamos o uso do módulo Adobe Authenticator.
>
>Para obter mais informações, consulte [Módulo Adobe Authenticator](/help/quicksilver/workfront-fusion/apps-and-their-modules/adobe-authenticator-modules.md).

## Módulos de solicitação

Consulte os seguintes artigos para obter instruções específicas do módulo de solicitação:

* [[!UICONTROL HTTP] >[!UICONTROL Fazer uma solicitação] módulo](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Fazer uma solicitação de autorização básica] módulo](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-basic-auth-request.md)
* [[!UICONTROL HTTP] > [!UICONTROL Fazer uma solicitação do OAuth 2.0] módulo](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Fazer uma solicitação de autorização de certificado de cliente] módulo](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-client-cert-auth-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Fazer uma solicitação de autorização de chave de API]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-api-key-auth-request.md)

## Outros módulos de ação

* [[!UICONTROL Obter um arquivo]](#get-a-file)
* [[!UICONTROL Resolver um URL de destino]](#resolve-a-target-url)

### [!UICONTROL Obter um arquivo]

Este módulo de ação baixa um arquivo do URL especificado. Depois que o arquivo for baixado, você poderá processar ainda mais o arquivo (mapear os dados do arquivo) usando outros módulos no cenário.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Insira ou mapeie o URL do arquivo que deseja baixar. </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Resolver um URL de destino]

Este módulo de ação resolve uma cadeia de redirecionamentos HTTP e retorna um URL de destino.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Insira ou mapeie o URL que você deseja resolver, como um [!DNL bit.ly] URL.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método] </td> 
   <td> <p>Selecione se você deseja usar o método [!UICONTROL HEAD] ou o método [!UICONTROL GET].</p> </td> 
  </tr> 
 </tbody> 
</table>

## Módulos iteradores

### [!UICONTROL Recuperar cabeçalhos]

Esse módulo retorna cada cabeçalho (nome e valor) do módulo HTTP especificado em um pacote separado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Módulo de Origem]</td> 
   <td> <p> Selecione o módulo do qual deseja recuperar cabeçalhos.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Geração de tokens da Web JSON (JWT)

É possível gerar um token JWT com a ajuda de funções integradas:

Cabeçalho

![](assets/jwt-header-350x19.png)

Código para copiar e colar:

```
{{replace(replace(replace(base64("{""alg"":""HS256"",""typ"":""JWT""}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

Carga:

![](assets/jwt-payload-350x17.png)

Código para copiar e colar:

```
{{replace(replace(replace(base64("{""iss"":""key"",""exp"":" + (timestamp + 60) + "}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

Token:

![](assets/jwt-token-350x15.png)

Código para copiar e colar:

```
{{1.value}}.{{2.value}}.{{replace(replace(replace(sha256(1.value + "." + 2.value; "base64"; "secret"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```
