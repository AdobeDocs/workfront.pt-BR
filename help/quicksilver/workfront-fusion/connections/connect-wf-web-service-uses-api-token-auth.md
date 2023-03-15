---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Connect [!DNL Adobe Workfront Fusion] para um serviço da Web que usa autorização de token de API
description: Alguns serviços não permitem soluções de integração como [!DNL Adobe Workfront Fusion] para criar um aplicativo que possa ser facilmente usado no seu cenário.
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 0%

---

# Connect [!DNL Adobe Workfront Fusion] para um serviço da Web que usa autorização de token de API

Alguns serviços não permitem soluções de integração como [!DNL Adobe Workfront Fusion] para criar um aplicativo que possa ser facilmente usado no seu cenário.

Há uma solução alternativa para essa situação. Você pode conectar o serviço desejado (aplicativo) ao [!DNL Workfront Fusion] usar [!DNL Workfront Fusion]&#39;s [!UICONTROL HTTP] módulo.

Este artigo explica como conectar quase qualquer serviço da Web ao [!DNL Workfront Fusion] usando um token de API/Chave de API.

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!UICONTROL Pro] ou superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licença**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conectar-se a um serviço da Web que usa um token de API

O procedimento de conexão do serviço por meio de um token de API é semelhante para a maioria dos serviços da Web.

1. Crie um aplicativo no site do serviço da Web, conforme explicado na seção [Crie um novo aplicativo e obtenha o token da API](#create-a-new-application-and-obtain-the-api-token) neste artigo.
1. Obtenha a chave da API ou o token da API.
1. Adicionar [!DNL Workfront Fusion]&#39;s [!UICONTROL HTTP] > [!UICONTROL Fazer uma solicitação] para o seu cenário.
1. Configure o módulo de acordo com a documentação da API do serviço da Web e execute o cenário, conforme explicado na seção [Configure o [!UICONTROL HTTP] módulo](#set-up-the-http-module) neste artigo.

>[!NOTE]
>
>Usaremos o [!DNL Pushover] serviço de notificação como exemplo em todo este artigo.

## Crie um novo aplicativo e obtenha o token da API

>[!NOTE]
>
>Há muitas maneiras diferentes de os serviços da Web criar e distribuir chaves de API ou tokens de API. Para obter instruções sobre como obter uma chave de API e um token para o serviço da Web desejado, acesse o site do serviço e pesquise por &quot;chave de API&quot; ou &quot;token de API&quot;.
>
>Estamos incluindo instruções para obter uma chave de API de Pushover somente como um exemplo do que você pode encontrar.

1. Faça logon no [!DNL Pushover] conta.
1. Clique em **[!UICONTROL Criar um token de aplicativo/API]** na parte inferior da página.
1. Preencha as Informações do aplicativo e clique em **[!UICONTROL Criar um aplicativo]**.
1. Armazene o token de API fornecido em um local seguro. Você precisará dele para a [!DNL Workfront Fusion] [!UICONTROL HTTP] >[!UICONTROL Fazer uma solicitação] para se conectar ao serviço da Web desejado ([!DNL Pushover], neste caso).

## Configure o [!UICONTROL HTTP] módulo

Para conectar um serviço da Web a seu [!DNL Workfront Fusion] , é necessário usar o [!UICONTROL HTTP] >[!UICONTROL Fazer uma solicitação] no cenário e configure o módulo de acordo com a documentação da API do serviço da Web.

1. Adicione o [!UICONTROL HTTP] >[!UICONTROL Fazer uma solicitação] para o seu cenário.
1. Para enviar uma mensagem por push usando [!DNL Workfront Fusion], configure o módulo HTTP da seguinte maneira.

   >[!NOTE]
   >
   >Essas configurações de módulo correspondem à [!DNL Pushover] documentação da API do serviço da Web. As configurações podem ser diferentes para outros serviços da Web. Por exemplo, o token de API pode ser inserido no [!UICONTROL Cabeçalho] e não à [!UICONTROL Corpo] campo.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL]</td> 
      <td> <p><code>https://api.pushover.net/1/messages.json</code> </p> <p>O campo URL contém o ponto de extremidade que pode ser encontrado na documentação da API do serviço da Web.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Método]</td> 
      <td> <p><code>[!DNL POST]</code> </p> <p>O método usado depende do endpoint correspondente. O endpoint de push para enviar mensagens usa o método POST.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Cabeçalhos]</p> </td> 
      <td> <p>Alguns serviços da Web podem usar Cabeçalhos para especificar a autenticação de token da API ou outros parâmetros. Esse não é o caso no nosso exemplo, pois o terminal de Push para enviar mensagens usa o Corpo (veja abaixo) para todos os tipos de solicitação.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Sequência de consulta]</p> </td> 
      <td> <p>Alguns serviços da Web podem usar uma String de consulta para especificar outros parâmetros. Não é o que acontece no nosso exemplo, já que [!DNL Pushover] o serviço da web usa o [!UICONTROL Body] (veja abaixo) para todos os tipos de solicitação.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Tipo de corpo]</p> </td> 
      <td> <p><code>Raw</code> </p> <p>Essa configuração permite selecionar o tipo de conteúdo JSON no campo [!UICONTROL Tipo de conteúdo] abaixo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Tipo de conteúdo]</p> </td> 
      <td> <p><code>JSON (application/json)</code> </p> <p>JSON é o tipo de conteúdo necessário pelo aplicativo [!UICONTROL Push]. Isso pode diferir de outros serviços da Web.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Solicitar conteúdo]</p> </td> 
      <td> <p>Insira o conteúdo da solicitação do [!UICONTROL Body] no formato JSON. Você pode usar o módulo [!UICONTROL JSON] &gt; [!UICONTROL Criar JSON] , conforme explicado em <a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref">Corpo JSON mapeado usando o módulo [!UICONTROL JSON] &gt; [!UICONTROL Criar JSON]</a> neste artigo. Ou você pode inserir o conteúdo JSON manualmente, como explicado em <a href="#json-body-entered-manually" class="MCXref xref">Corpo JSON inserido manualmente</a> neste artigo.</p> <p>Consulte a documentação da API do serviço da Web para obter os parâmetros necessários para esse serviço da Web.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Corpo JSON inserido manualmente

Especifique parâmetros e valores no formato JSON.

>[!INFO]
>
>**Exemplo:**
>
>```
>{"user":"12345c2ecu1hq42ypqzhswbyam34",
>
>
"token":"123459evz8aepwtxydndydgyumbfx",
>
>
"message":"Hello World!",
>
>
"title":"The Push Notification"}
>```

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL usuário]</p> </td> 
   <td> <p>Sua USER_KEY. Isso pode ser encontrado no [!DNL Pushover] painel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL token] </td> 
   <td> <p>Seu token de API/chave de API que foi gerada por você criou a [!DNL Pushover] aplicativo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL message] </td> 
   <td> <p>O conteúdo do texto da notificação por push que é enviada para os dispositivos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL title] </td> 
   <td> <p>(Opcional) O título da mensagem. Se nenhum valor for inserido, o nome do aplicativo será usado. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Corpo JSON mapeado usando o [!UICONTROL JSON] >[!UICONTROL Criar JSON] módulo

O [!UICONTROL Criar JSON] facilita a especificação do JSON. Também oferece a possibilidade de definir valores dinamicamente.

Para obter mais informações sobre os módulos JSON, consulte [Módulos JSON](../../workfront-fusion/apps-and-their-modules/json-modules.md).

1. Insira ou mapeie os valores a partir dos quais deseja criar o JSON.

   ![](assets/json-values-350x288.png)

1. Conecte o [!UICONTROL JSON] > [!UICONTROL Criar JSON] para o módulo HTTP > Fazer uma solicitação .
1. Mapeie a sequência de caracteres JSON do [!UICONTROL Criar JSON] para [!UICONTROL Solicitar conteúdo] no campo [!UICONTROL HTTP] >[!UICONTROL Fazer uma solicitação] módulo.

   Agora, quando você executa o cenário, a notificação por push é enviada para o dispositivo que foi registrado no [!DNL Pushover] conta.
