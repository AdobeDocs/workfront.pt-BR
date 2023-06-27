---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Datadog
description: Em um [!DNL Adobe Workfront Fusion] Nesse cenário, você pode automatizar workflows que usam o Datadog, bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: a0b4352d-a1ce-4459-a58e-71de860b8a90
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 1%

---

# [!DNL Datadog] módulos

Em um [!DNL Adobe Workfront Fusion] cenário, é possível automatizar workflows que usam [!DNL Datadog], bem como conectá-lo a vários aplicativos e serviços de terceiros.

Se precisar de instruções sobre como criar um cenário, consulte [Criar um cenário no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obter informações sobre módulos, consulte [Módulos no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

## Pré-requisitos

Para usar [!DNL Datadog] módulos, você deve ter uma [!DNL Datadog] conta.

## Conectar [!DNL Datadog] para [!DNL Workfront Fusion] {#connect-datadog-to-workfront-fusion}

### Recuperar a chave de API e a chave de aplicativo {#retrieve-your-api-key-and-application-key}

Para conectar seu [!DNL Datadog] conta para [!DNL Workfront Fusion] você precisa recuperar uma Chave de API e uma chave de aplicativo de seu [!DNL Datadog] conta.

1. Faça logon no [!DNL Datadog] conta.
1. No painel de navegação esquerdo, clique em **[!UICONTROL Integrações]** e, em seguida, clique em **[!UICONTROL APIs]**.
1. Na tela principal, clique em **[!UICONTROL Chaves de API]**.
1. Passe o mouse sobre a barra roxa para revelar a chave de API.
1. Copie a chave da API para um local seguro.
1. Na tela principal, clique em **[!UICONTROL Chaves do aplicativo]**.
1. Passe o mouse sobre a barra roxa para revelar a chave do aplicativo.
1. Copie a chave do aplicativo para um local seguro.

### Criar uma conexão com o [!DNL Datadog] in [!DNL Workfront Fusion]

Você pode criar uma conexão com o seu [!DNL Datadog] conta diretamente de dentro de um [!UICONTROL Datadog] módulo.

1. Em qualquer [!UICONTROL Datadog] , clique em **[!UICONTROL Adicionar]** ao lado da [!UICONTROL Conexão] campo.
1. Preencha os campos do módulo da seguinte maneira:

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo de Conexão]</td> 
      <td> <p> Selecione o [!UICONTROL [!DNL Datadog] opção] para obter acesso total ao [!DNL Datadog] API.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome da Conexão]</td> 
      <td> <p> Insira um nome para a conexão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Domínio] </td> 
      <td> <p>Selecione o domínio ao qual deseja se conectar (EUA ou UE).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Chave de API]</td> 
      <td> <p> Insira seu [!DNL Datadog] Chave da API. </p> <p>Para obter instruções sobre como recuperar a chave de API, consulte <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">Recuperar a chave de API e a chave de aplicativo</a> neste artigo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Chave do Aplicativo]</td> 
      <td> <p> Insira seu [!DNL Datadog] chave do aplicativo. </p> <p>Para obter instruções sobre como recuperar a chave do aplicativo, consulte <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">Recuperar a chave de API e a chave de aplicativo</a> neste artigo.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Continuar]** para criar a conexão e voltar ao módulo.

## [!DNL Datadog] módulos e seus campos

Ao configurar [!DNL Datadog] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Datadog] Os campos podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Ações

* [[!UICONTROL Postar pontos da série temporal]](#post-timeseries-points)
* [[!UICONTROL Fazer uma chamada de API]](#make-an-api-call)

#### [!UICONTROL Postar pontos da série temporal]

O módulo permite publicar dados de série temporal que podem ser grafados em [!DNL Datadog]Painéis do.

O limite para payloads compactados é de 3,2 megabytes (3200000) e 62 megabytes (62914560) para payloads descompactados.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Datadog] conta para [!DNL Workfront Fusion], consulte <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Datadog] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Série]</td> 
   <td> <p>Adicionar séries de tempo que você deseja enviar [!DNL Datadog].</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Métrica]</strong> </p> <p>Insira o nome da série temporal.</p> </li> 
     <li> <p><strong>[!UICONTROL Tipo]</strong> </p> <p>Selecione o tipo de métrica.</p> </li> 
     <li> <p><strong>[!UICONTROL Intervalo]</strong> </p> <p> Se o tipo da métrica for taxa ou contagem, defina o intervalo correspondente.</p> </li> 
     <li> <p><strong>[!UICONTROL Pontos]</strong> </p> <p>Adicionar pontos relacionados a uma métrica.</p> <p>Esta é uma matriz de pontos JSON. Cada ponto tem o formato: <code>[[POSIX_timestamp, numeric_value], ...] </code></p> <p>Nota:  <p>O carimbo de data/hora deve estar em segundos.</p> <p>O carimbo de data/hora deve ser atual. O valor atual é definido como não mais de 10 minutos no futuro ou mais de 1 hora no passado.</p> <p> O formato do valor numérico deve ser um valor flutuante.</p> </p> <p>Este campo deve conter pelo menos 1 item.</p> </li> 
     <li> <p><strong>[!UICONTROL Host]</strong> </p> <p>Informe o nome do host que produziu a métrica.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Fazer uma chamada de API]

Esse módulo de ação permite executar uma chamada de API personalizada.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Datadog] conta para [!DNL Workfront Fusion], consulte <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Datadog] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Insira um caminho relativo a <code>https://api.datadoghq.com/api/</code>. Exemplo:<code> /v1/org</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formulário de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> <p>O Workfront Fusion adiciona os cabeçalhos de autorização para você.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadeia de Consulta]</td> 
   <td> <p>Adicione a consulta da chamada à API na forma de um objeto JSON padrão.</p> <p>Por exemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada à API na forma de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Exemplo:** A chamada de API a seguir retorna todos os painéis em seu [!DNL Datadog] conta:

URL: `/v1/dashboard`

Método: `GET`

![](assets/datadog-api-example.png)

O resultado pode ser encontrado na Saída do módulo em Pacote > Corpo > painéis.

No nosso exemplo, 3 painéis foram retornados:

![](assets/datadog-api-response-example.png)
