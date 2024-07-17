---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Conectar  [!DNL Adobe Workfront Fusion]  a um serviço Web que usa autorização de token de API
description: Alguns serviços não permitem soluções de integração, como o [!DNL Adobe Workfront Fusion] para criar um aplicativo que possa ser usado facilmente em seu cenário.
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: e61dc6646e221cffb30aad055663dcf8fd3299e2
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 0%

---

# Conectar [!DNL Adobe Workfront Fusion] a um serviço Web que usa autorização de token de API

Alguns serviços não permitem que soluções de integração, como o [!DNL Adobe Workfront Fusion], criem um aplicativo que possa ser usado facilmente em seu cenário.

Há uma solução alternativa para essa situação. Você pode conectar o serviço (aplicativo) desejado a [!DNL Workfront Fusion] usando o módulo [!UICONTROL HTTP] de [!DNL Workfront Fusion].

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
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conexão com um serviço Web que usa um token de API

O procedimento de conexão do serviço por meio de um token de API é semelhante para a maioria dos serviços da Web.

1. Crie um aplicativo no site do serviço Web, conforme explicado na seção [Crie um novo aplicativo e obtenha o token de API](#create-a-new-application-and-obtain-the-api-token) neste artigo.
1. Obtenha a chave de API ou o token de API.
1. Adicione o módulo [!UICONTROL HTTP] > [!UICONTROL Fazer uma solicitação] de [!DNL Workfront Fusion] ao seu cenário.
1. Configure o módulo de acordo com a documentação da API do serviço Web e execute o cenário, conforme explicado na seção [Configurar o módulo [!UICONTROL HTTP]](#set-up-the-http-module) deste artigo.

>[!NOTE]
>
>Usaremos o serviço de notificação [!DNL Pushover] como exemplo neste artigo.

## Crie um novo aplicativo e obtenha o token da API

>[!NOTE]
>
>Há várias maneiras diferentes pelas quais os serviços da Web criam e distribuem chaves de API ou tokens de API. Para obter instruções sobre como obter uma chave de API e um token para o serviço da Web desejado, vá para o site do serviço e pesquise por &quot;Chave de API&quot; ou &quot;Token de API&quot;.
>
>Estamos incluindo instruções para obter uma chave de API Pushover somente como exemplo do que você pode encontrar.

1. Faça logon em sua conta do [!DNL Pushover].
1. Clique em **[!UICONTROL Criar um token de aplicativo/API]** na parte inferior da página.
1. Preencha as Informações do Aplicativo e clique em **[!UICONTROL Criar um Aplicativo]**.
1. Armazene o token de API fornecido em um local seguro. Você precisará dele para o módulo [!DNL Workfront Fusion] [!UICONTROL HTTP] >[!UICONTROL Fazer uma Solicitação] para se conectar ao serviço Web desejado ([!DNL Pushover], neste caso).

## Configurar o módulo [!UICONTROL HTTP]

Para conectar um serviço Web ao seu cenário [!DNL Workfront Fusion], você precisa usar o módulo [!UICONTROL HTTP] >[!UICONTROL Fazer uma solicitação] no cenário e configurar o módulo de acordo com a documentação da API do serviço Web.

1. Adicione o módulo [!UICONTROL HTTP] >[!UICONTROL Fazer uma Solicitação] ao seu cenário.
1. Para enviar uma mensagem usando [!DNL Workfront Fusion], configure o módulo HTTP da seguinte maneira.

   >[!NOTE]
   >
   >Essas configurações de módulo correspondem à documentação da API do serviço Web [!DNL Pushover]. As configurações podem ser diferentes para outros serviços da Web. Por exemplo, o token de API pode ser inserido no [!UICONTROL Cabeçalho] e não no campo [!UICONTROL Corpo].

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
      <td> <p>Alguns serviços da Web podem usar uma sequência de consulta para especificar outros parâmetros. Este não é o caso em nosso exemplo, pois o serviço Web [!DNL Pushover] usa [!UICONTROL Corpo] (veja abaixo) para todos os tipos de solicitação.</p> </td> 
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
      <td> <p>Insira o conteúdo da solicitação [!UICONTROL Body] no formato JSON. Você pode usar o módulo [!UICONTROL JSON] &gt; [!UICONTROL Criar JSON] como explicado no <a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref">Corpo JSON mapeado usando o módulo [!UICONTROL JSON] &gt; [!UICONTROL Criar JSON]</a> neste artigo. Ou você pode inserir o conteúdo JSON manualmente, como explicado em <a href="#json-body-entered-manually" class="MCXref xref">Corpo JSON inserido manualmente</a> neste artigo.</p> <p>Consulte a documentação da API do serviço Web para obter os parâmetros necessários para esse serviço Web.</p> </td> 
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
>"token":"123459evz8aepwtxydndydgyumbfx",
>"message":"Hello World!",
>"title":"The Push Notification"}
>```

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL usuário]</p> </td> 
   <td> <p>Sua USER_KEY. Isto pode ser encontrado no seu painel [!DNL Pushover].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL token] </td> 
   <td> <p>O token de API/Chave de API gerado criou o aplicativo [!DNL Pushover].</p> </td> 
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

## Corpo JSON mapeado usando o módulo [!UICONTROL JSON] >[!UICONTROL Criar JSON]

O módulo [!UICONTROL Criar JSON] facilita a especificação do JSON. Ela também oferece a possibilidade de definir valores dinamicamente.

Para obter mais informações sobre os módulos JSON, consulte [módulos JSON](../../workfront-fusion/apps-and-their-modules/json-modules.md).

1. Insira ou mapeie os valores a partir dos quais deseja criar JSON.

   ![](assets/json-values-350x288.png)

1. Conecte o módulo [!UICONTROL JSON] > [!UICONTROL Criar JSON] ao módulo HTTP > Fazer uma Solicitação.
1. Mapeie a cadeia de caracteres JSON do módulo [!UICONTROL Criar JSON] para o campo [!UICONTROL Solicitar conteúdo] no módulo [!UICONTROL HTTP] >[!UICONTROL Fazer uma Solicitação].

   Agora, quando você executa o cenário, a notificação por push é enviada para o dispositivo que foi registrado na sua conta [!DNL Pushover].
