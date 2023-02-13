---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: HTTP &gt; Outros módulos
description: O [!DNL Adobe Workfront Fusion] O aplicativo HTTP fornece vários módulos para comunicação com base no protocolo HTTP (Hypertext Transfer Protocol). HTTP é a base da comunicação de dados para a World Wide Web. Você pode usar os módulos para baixar páginas da Web e arquivos, chamar webhooks e pontos de extremidade da API e assim por diante.
author: Becky
feature: Workfront Fusion
exl-id: ff2cd098-d1d7-43a3-9f00-15e0f6e92332
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# HTTP > Outros módulos

>[!NOTE]
>
>[!UICONTROL Adobe Workfront Fusion] exige um [!UICONTROL Adobe Workfront Fusion] além de um [!UICONTROL Adobe Workfront] licença.

O [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] o app fornece vários módulos para comunicação com base no protocolo HTTP (Hypertext Transfer Protocol). HTTP é a base da comunicação de dados para a World Wide Web. Você pode usar os módulos para baixar páginas da Web e arquivos, chamar webhooks e pontos de extremidade da API e assim por diante.

A escolha correta do módulo depende do mecanismo de autenticação/autorização que o recurso que você deseja acessar emprega. Veja a seguir exemplos de módulos

* Solicitar:módulo universal destinado principalmente a recursos que não utilizam qualquer tipo de autenticação/autorização
* Faça uma solicitação básica de autenticação:para recursos que empregam [!DNL HTTP] Autenticação básica (BA)
* Faça uma solicitação do OAuth 2.0: para recursos que utilizam o protocolo de autorização OAuth 2.0
* Faça uma solicitação de Autenticação de certificado do cliente: para recursos que utilizam o protocolo de autorização que requer um certificado do lado do cliente.
* Faça uma solicitação de autorização da Chave de API: para recursos que empregam chaves de API para autorização.

## Módulos de solicitação

Consulte os seguintes artigos para obter instruções específicas do módulo de solicitação:

* [[!UICONTROL HTTP] >[!UICONTROL Fazer uma solicitação] módulo](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Faça uma solicitação de Autorização básica] módulo](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-basic-auth-request.md)
* [[!UICONTROL HTTP] > [!UICONTROL Fazer uma solicitação do OAuth 2.0] módulo](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Fazer uma solicitação de Autorização de Certificado de Cliente] módulo](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-client-cert-auth-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Faça uma solicitação de Autorização de chave de API]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-api-key-auth-request.md)

## Outros módulos de ação

* [[!UICONTROL Obter um arquivo]](#get-a-file)
* [[!UICONTROL Resolver um URL de destino]](#resolve-a-target-url)

### [!UICONTROL Obter um arquivo]

Este módulo de ação baixa um arquivo do URL especificado. Após o download do arquivo, você poderá processar o arquivo (mapear os dados do arquivo) usando outros módulos no cenário.

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

Esse módulo de ação resolve uma cadeia de redirecionamentos HTTP e retorna um URL de destino.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Insira ou mapeie o URL que deseja resolver, como um [!DNL bit.ly] URL.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método] </td> 
   <td> <p>Selecione se deseja usar o método [!UICONTROL HEAD] ou o método [!UICONTROL GET].</p> </td> 
  </tr> 
 </tbody> 
</table>

## Módulos de iterador

### [!UICONTROL Recuperar cabeçalhos]

Esse módulo retorna cada cabeçalho (nome e valor) do módulo HTTP especificado em um pacote separado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Módulo de origem]</td> 
   <td> <p> Selecione o módulo do qual deseja recuperar cabeçalhos.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Geração de tokens da Web JSON (JWT)

É possível gerar um token JWT com a ajuda de funções integradas:

Cabeçalho:

![](assets/jwt-header-350x19.png)

Código para copiar&amp;colar:

```
{{replace(replace(replace(base64("{""alg"":""HS256"",""typ"":""JWT""}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

Carga:

![](assets/jwt-payload-350x17.png)

Código para copiar&amp;colar:

```
{{replace(replace(replace(base64("{""iss"":""key"",""exp"":" + (timestamp + 60) + "}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

Token:

![](assets/jwt-token-350x15.png)

Código para copiar&amp;colar:

```
{{1.value}}.{{2.value}}.{{replace(replace(replace(sha256(1.value + "." + 2.value; "base64"; "secret"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```
