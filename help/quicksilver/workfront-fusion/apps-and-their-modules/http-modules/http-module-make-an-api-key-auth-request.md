---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: http-modules
title: HTTP &gt; Faça uma solicitação de Autorização de chave de API
description: Essa [!DNL Adobe Workfront Fusion] o módulo de ação envia uma solicitação HTTPS para um URL especificado que requer uma autorização de Auth da chave de API e processa a resposta.
author: Becky
feature: Workfront Fusion
exl-id: 70bf87c7-6d51-4ef4-9dce-80ad004e613f
source-git-commit: 58db2129dd764d24b0a681735c2405be402d8b43
workflow-type: tm+mt
source-wordcount: '932'
ht-degree: 0%

---

# HTTP >[!UICONTROL Faça uma solicitação de Autorização de chave de API]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] exige um [!DNL Adobe Workfront Fusion] além de uma licença da Adobe Workfront.

Essa [!DNL Adobe Workfront Fusion] o módulo de ação envia uma solicitação HTTPS para um URL especificado que requer uma autorização de Auth da chave de API e processa a resposta.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!UICONTROL Adobe Workfront Fusion] licenças, consulte [Licenças do Adobe Workfront Fusion](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!UICONTROL HTTP] >[!UICONTROL Faça uma solicitação de Autorização de chave de API] configuração do módulo

Ao configurar o [!UICONTROL HTTP] >[!UICONTROL Faça uma solicitação de Autorização de chave de API] módulo, [!DNL Adobe Workfront Fusion] exibe os campos listados abaixo. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Credentials]</td> 
   <td> <p>Selecione a chave que contém suas credenciais de autenticação da chave de API. Para adicionar uma nova chave, clique em <strong>[!UICONTROL Adicionar]</strong> e configure as seguintes informações:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome da chave]</strong></p> <p>Insira um nome para esse conjunto de credenciais da API.</p> </li> 
     <li> <p><strong>[!UICONTROL Chave]</strong> </p> <p>Insira a chave da API.</p> </li> 
     <li> <p><strong>[!UICONTROL Inserção de chave da API]</strong> </p> <p>Selecione se deseja colocar a Chave da API no cabeçalho ou na consulta da chamada da API.</p> </li> 
     <li> <p><strong>[!UICONTROL Nome do parâmetro da chave de API]</strong> </p> <p>Insira o nome pelo qual a chamada da API identifica a Chave da API, como "apiKey" ou "X-API-Key". Você pode encontrar essas informações na documentação do serviço da Web ao qual o módulo está se conectando.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Avaliar todos os estados como erros (exceto para 2xx e 3xx)] </td> 
   <td> <p>Use essa opção para configurar o tratamento de erros.</p> <p>Para obter mais informações, consulte <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">Tratamento de erros no Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Insira o URL para o qual você deseja enviar uma solicitação, como um endpoint da API, site da Web, etc.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   <td> <p>Selecione o método de solicitação HTTP que você precisa configurar a chamada da API. Para obter mais informações, consulte <a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos] </td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão. Por exemplo, <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sequência de consulta]</td> 
   <td> <p> Insira os pares de valor-chave da consulta desejados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de corpo]</p> </td> 
   <td> <p>O Corpo HTTP são os bytes de dados transmitidos em uma mensagem de transação HTTP imediatamente após os cabeçalhos, se houver algum para ser usado.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL bruto]</strong> </p> <p>O tipo de corpo bruto geralmente é adequado para a maioria das solicitações de corpo HTTP, mesmo em situações em que a documentação do desenvolvedor não especifica dados para enviar.</p> <p>Especifique um formulário de análise dos dados no campo [!UICONTROL Content type] .</p> <p>Apesar do tipo de conteúdo selecionado, o módulo insere dados em qualquer formato estipulado ou exigido pela documentação do desenvolvedor.</p> </li> 
     <li> <p><strong>[!UICONTROL Aplicativo/x-www-form-urlencoded]</strong> </p> <p>Esse tipo de corpo é para dados do [!UICONTROL POST] usando <code>application/x-www-form-urlencoded</code>.</p> <p>Para <code>[!UICONTROL application/x-www-form-urlencoded]</code>, o corpo da mensagem HTTP enviada para o servidor é essencialmente uma sequência de consulta. As chaves e os valores são codificados em pares de valores chave separados por <code>&amp;</code> e com um <code>=</code> entre a chave e o valor. </p> <p>Para dados binários, use <code>[!UICONTROL multipart/form-data]</code> em vez disso.</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>Exemplo: </b></span></span> 
       <p>Exemplo do formato de solicitação HTTP resultante:</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[!UICONTROL Multipart/form-data]</strong> </p> <p>O [!UICONTROL Multipart/form-data] é uma solicitação HTTP multipart usada para enviar arquivos e dados. Geralmente é usado para fazer upload de arquivos para o servidor.</p> <p>Adicione campos a serem enviados na solicitação. Cada campo deve conter o par Valor-Chave .</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Texto]</strong> </p> <p>Insira a chave e o valor a ser enviado dentro do corpo da solicitação.</p> </li> 
       <li> <p><strong>[!UICONTROL Arquivo]</strong> </p> <p>Insira a chave e especifique o arquivo de origem que deseja enviar no corpo da solicitação.</p> <p>Mapeie o arquivo que deseja fazer upload do módulo anterior (como [!UICONTROL HTTP] &gt;[!UICONTROL Obter um arquivo] ou [!UICONTROL Google Drive] &gt;[!UICONTROL Baixar um arquivo)] ou insira o nome do arquivo e os dados do arquivo manualmente.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Analisar resposta]</p> </td> 
   <td> <p>Ative essa opção para analisar automaticamente as respostas e converter as respostas JSON e XML de forma que não precise usar os módulos [!UICONTROL JSON] &gt; [!UICONTROL Analisar JSON] ou [!UICONTROL XML] &gt; [!UICONTROL Analisar XML] .</p> <p>Antes de usar conteúdo JSON ou XML analisado, execute o módulo uma vez manualmente para que ele possa reconhecer o conteúdo da resposta e mapeá-lo em módulos subsequentes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tempo limite] </td> 
   <td> <p>Especifique o tempo limite da solicitação em segundos (1-300). O padrão é 40 segundos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Compartilhar cookies com outros módulos HTTP]</td> 
   <td> <p> Ative essa opção para compartilhar cookies do servidor com todos os módulos HTTP no seu cenário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Certificado autoassinado]</td> 
   <td> <p> Carregue seu certificado se quiser usar o TLS usando seu certificado autoassinado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rejeitar conexões que estejam usando certificados não verificados (autoassinados)] </td> 
   <td> <p>Ative essa opção para rejeitar conexões que estejam usando certificados TLS não verificados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seguir redirecionamento]</td> 
   <td> <p> Ative essa opção para seguir os redirecionamentos de URL com respostas 3xx.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seguir todos os redirecionamentos] </td> 
   <td> <p>Ative essa opção para seguir os redirecionamentos de URL com todos os códigos de resposta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Desativar a serialização de várias chaves da mesma sequência de consulta como matrizes]</p> </td> 
   <td> <p>Por padrão, [!DNL Workfront Fusion] O lida com vários valores para a mesma chave de parâmetro da string de consulta de URL que os arrays. Por exemplo, <code>www.test.com?foo=bar&amp;foo=baz</code> será convertido em <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code>. Ative essa opção para desativar esse recurso. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Solicitar conteúdo compactado]</td> 
   <td> <p> Ative essa opção para solicitar uma versão compactada do site.</p> <p>Adiciona um <code>[!UICONTROL Accept-Encoding]</code> para solicitar conteúdo compactado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Usar TLS mútuo]</td> 
   <td> <p>Ative essa opção para usar o TLS mútuo na solicitação HTTP.</p> <p>Para obter mais informações sobre TLS Mútuos, consulte <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">Usar TLS mútuo em módulos HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
