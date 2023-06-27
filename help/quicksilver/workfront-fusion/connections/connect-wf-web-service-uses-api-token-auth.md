---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Conectar [!DNL Adobe Workfront Fusion] para um serviço Web que usa a autorização do token de API
description: Alguns serviços não permitem soluções de integração, como [!DNL Adobe Workfront Fusion] para criar um aplicativo que possa ser usado facilmente em seu cenário.
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 0%

---

# Conectar [!DNL Adobe Workfront Fusion] para um serviço Web que usa a autorização do token de API

Alguns serviços não permitem soluções de integração, como [!DNL Adobe Workfront Fusion] para criar um aplicativo que possa ser usado facilmente em seu cenário.

Há uma solução alternativa para essa situação. Você pode conectar o serviço (aplicativo) desejado a [!DNL Workfront Fusion] usar [!DNL Workfront Fusion]do [!UICONTROL HTTP] módulo.

Este artigo explica como conectar quase qualquer serviço Web ao [!DNL Workfront Fusion] usando uma Chave de API/token de API.

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
   <td>
   <p>Requisito de licença atual: Não [!DNL Workfront Fusion] requisito de licença.</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e integração do trabalho] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o [!UICONTROL Select] ou o [!UICONTROL Prime] [!DNL Adobe Workfront] Planejar, sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no [!UICONTROL Ultimate] [!DNL Workfront] plano.</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conexão com um serviço Web que usa um token de API

O procedimento de conexão do serviço por meio de um token de API é semelhante para a maioria dos serviços da Web.

1. Crie um aplicativo no site do serviço Web, conforme explicado na seção [Crie um novo aplicativo e obtenha o token da API](#create-a-new-application-and-obtain-the-api-token) neste artigo.
1. Obtenha a chave de API ou o token de API.
1. Adicionar [!DNL Workfront Fusion]do [!UICONTROL HTTP] > [!UICONTROL Fazer uma solicitação] para o seu cenário.
1. Configure o módulo de acordo com a documentação da API do serviço Web e execute o cenário, conforme explicado na seção [Configurar o [!UICONTROL HTTP] módulo](#set-up-the-http-module) neste artigo.

>[!NOTE]
>
>Usaremos o [!DNL Pushover] serviço de notificação como exemplo neste artigo.

## Crie um novo aplicativo e obtenha o token da API

>[!NOTE]
>
>Há várias maneiras diferentes pelas quais os serviços da Web criam e distribuem chaves de API ou tokens de API. Para obter instruções sobre como obter uma chave de API e um token para o serviço da Web desejado, vá para o site do serviço e pesquise por &quot;Chave de API&quot; ou &quot;Token de API&quot;.
>
>Estamos incluindo instruções para obter uma chave de API Pushover somente como exemplo do que você pode encontrar.

1. Faça logon no [!DNL Pushover] conta.
1. Clique em **[!UICONTROL Criar um token de aplicativo/API]** na parte inferior da página.
1. Preencha as Informações do aplicativo e clique em **[!UICONTROL Criar um aplicativo]**.
1. Armazene o token de API fornecido em um local seguro. Você precisará dele para o [!DNL Workfront Fusion] [!UICONTROL HTTP] >[!UICONTROL Fazer uma solicitação] módulo para conectar-se ao serviço Web desejado ([!DNL Pushover], neste caso).

## Configurar o [!UICONTROL HTTP] módulo

Para conectar um serviço Web ao [!DNL Workfront Fusion] cenário, é necessário usar a variável [!UICONTROL HTTP] >[!UICONTROL Fazer uma solicitação] no cenário e configure o módulo de acordo com a documentação da API do serviço Web.

1. Adicione o [!UICONTROL HTTP] >[!UICONTROL Fazer uma solicitação] para o seu cenário.
1. Para enviar uma mensagem por push usando [!DNL Workfront Fusion], configure o módulo HTTP da seguinte maneira.

   >[!NOTE]
   >
   >Essas configurações de módulo correspondem à variável [!DNL Pushover] Documentação da API do serviço Web. As configurações podem ser diferentes para outros serviços da Web. Por exemplo, o token da API pode ser inserido no [!UICONTROL Cabeçalho] e não à [!UICONTROL Corpo] campo.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL]</td> 
      <td> <p><code>https://api.pushover.net/1/messages.json</code> </p> <p>O campo URL contém o endpoint que pode ser encontrado na documentação da API do serviço Web.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Método]</td> 
      <td> <p><code>[!DNL POST]</code> </p> <p>O método usado depende do endpoint correspondente. O endpoint Pushover para enviar mensagens usa o método POST.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Cabeçalhos]</p> </td> 
      <td> <p>Alguns serviços da Web podem usar Cabeçalhos para especificar a autenticação do token de API ou outros parâmetros. Esse não é o caso em nosso exemplo, pois o endpoint do Pushover para enviar mensagens usa Corpo (veja abaixo) para todos os tipos de solicitação.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Cadeia de Consulta]</p> </td> 
      <td> <p>Alguns serviços da Web podem usar uma sequência de consulta para especificar outros parâmetros. Esse não é o caso em nosso exemplo como a variável [!DNL Pushover] o serviço da web usa o [!UICONTROL Corpo] (veja abaixo) para todos os tipos de solicitação.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Tipo de Corpo]</p> </td> 
      <td> <p><code>Raw</code> </p> <p>Essa configuração permite selecionar o tipo de conteúdo JSON no campo [!UICONTROL Tipo de Conteúdo] abaixo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Tipo de Conteúdo]</p> </td> 
      <td> <p><code>JSON (application/json)</code> </p> <p>JSON é o tipo de conteúdo necessário para o aplicativo [!UICONTROL Pushover]. Isso pode diferir de outros serviços da Web.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Solicitar Conteúdo]</p> </td> 
      <td> <p>Insira o conteúdo da solicitação [!UICONTROL Body] no formato JSON. Você pode usar o módulo [!UICONTROL JSON] &gt; [!UICONTROL Criar JSON] conforme explicado em <a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref">Corpo JSON mapeado usando o módulo [!UICONTROL JSON] &gt; [!UICONTROL Criar JSON]</a> neste artigo. Ou você pode inserir o conteúdo JSON manualmente, conforme explicado em <a href="#json-body-entered-manually" class="MCXref xref">Corpo JSON inserido manualmente</a> neste artigo.</p> <p>Consulte a documentação da API do serviço Web para obter os parâmetros necessários para esse serviço Web.</p> </td> 
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
   <td> <p>Sua USER_KEY. Isso pode ser encontrado no seu [!DNL Pushover] painel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL token] </td> 
   <td> <p>O token de API/Chave de API gerado para você [!DNL Pushover] aplicativo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL mensagem] </td> 
   <td> <p>O conteúdo de texto da notificação por push enviada para o(s) dispositivo(s).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL título] </td> 
   <td> <p>(Opcional) O título da sua mensagem. Se nenhum valor for inserido, o nome do aplicativo será usado. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Corpo JSON mapeado usando o [!UICONTROL JSON] >[!UICONTROL Criar JSON] módulo

A variável [!UICONTROL Criar JSON] facilita a especificação do JSON. Ela também oferece a possibilidade de definir valores dinamicamente.

Para obter mais informações sobre os módulos JSON, consulte [Módulos JSON](../../workfront-fusion/apps-and-their-modules/json-modules.md).

1. Insira ou mapeie os valores a partir dos quais deseja criar JSON.

   ![](assets/json-values-350x288.png)

1. Conecte o [!UICONTROL JSON] > [!UICONTROL Criar JSON] para o módulo HTTP > Fazer uma solicitação.
1. Mapeie a cadeia de caracteres JSON do [!UICONTROL Criar JSON] módulo para o [!UICONTROL Solicitar conteúdo] no campo [!UICONTROL HTTP] >[!UICONTROL Fazer uma solicitação] módulo.

   Agora, quando você executa o cenário, a notificação por push é enviada para o dispositivo que foi registrado no [!DNL Pushover] conta.
