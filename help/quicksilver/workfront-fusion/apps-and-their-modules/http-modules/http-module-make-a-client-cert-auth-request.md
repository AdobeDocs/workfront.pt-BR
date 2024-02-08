---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: http-modules
title: HTTP &gt; Criar um módulo de solicitação de Autorização de Certificado de Cliente
description: Este [!DNL Adobe Workfront Fusion] O módulo permite configurar uma solicitação HTTP com autorização de certificado de cliente HTTP e enviá-la a um servidor. A resposta HTTP recebida é então contida no pacote de saída.
author: Becky
feature: Workfront Fusion
exl-id: c0b0057f-3db0-4c10-a274-ebaec1a5b87b
source-git-commit: 45540ccc3b9fca98f8aaae86ac4d6574a067a6e4
workflow-type: tm+mt
source-wordcount: '959'
ht-degree: 0%

---

# HTTP >[!UICONTROL Fazer uma solicitação de autorização de certificado de cliente] módulo

>[!NOTE]
>
>O Adobe Workfront Fusion exige uma [!DNL Adobe Workfront Fusion] além de uma licença do Adobe Workfront.

Este [!DNL Adobe Workfront Fusion] O módulo permite configurar uma solicitação HTTP com autorização de certificado de cliente HTTP e enviá-la a um servidor. A resposta HTTP recebida é então contida no pacote de saída.

>[!NOTE]
>
>Se você estiver se conectando a um produto Adobe que não tem um conector dedicado no momento, recomendamos o uso do módulo Adobe Authenticator.
>
>Para obter mais informações, consulte [Módulo Adobe Authenticator](/help/quicksilver/workfront-fusion/apps-and-their-modules/adobe-authenticator-modules.md).

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

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!UICONTROL HTTP] >[!UICONTROL Fazer uma solicitação de autorização de certificado de cliente] configuração do módulo

Ao configurar o [!UICONTROL HTTP] >[!UICONTROL Fazer uma solicitação de autorização de certificado de cliente] módulo, [!DNL Adobe Workfront Fusion] exibe os campos listados abaixo. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

<img src="assets/map-toggle-350x74.png" style="width: 350;height: 74;" data-mc-conditions="QuicksilverOrClassic.Draft mode">

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Credenciais]</td> 
   <td> <p>Selecione a chave que contém suas credenciais de autenticação de certificado de cliente ou clique em <strong>[!UICONTROL Adicionar]</strong> para adicionar suas credenciais a uma nova chave. </p> <p>Observação: você pode adicionar mais credenciais para alternar facilmente entre cada conexão.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Avaliar todos os estados como erros (exceto para 2xx e 3xx )] </td> 
   <td> <p>Use esta opção para configurar o tratamento de erros.</p> <p>Para obter mais informações, consulte <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">Tratamento de erros no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Insira o URL para o qual você deseja enviar uma solicitação, como um endpoint de API, site etc.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   <td> <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos] </td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formulário de um objeto JSON padrão. Por exemplo, <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadeia de Consulta]</td> 
   <td> <p> Insira os pares de valor-chave da consulta desejados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de corpo]</p> </td> 
   <td> <p>O Corpo HTTP são os bytes de dados transmitidos em uma mensagem de transação HTTP imediatamente após os cabeçalhos, se houver algum a ser usado.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Bruto]</strong> </p> <p>O tipo de corpo bruto geralmente é adequado para a maioria das solicitações de corpo HTTP, mesmo em situações em que a documentação do desenvolvedor não especifica os dados a serem enviados.</p> <p>Especifique uma forma de análise dos dados no campo [!UICONTROL Content type].</p> <p>Apesar do tipo de conteúdo selecionado, o módulo insere dados em qualquer formato estipulado ou exigido pela documentação do desenvolvedor.</p> </li> 
     <li> <p><strong>[!UICONTROL Aplicativo/x-www-form-urlencoded]</strong> </p> <p>Este tipo de corpo é para [!UICONTROL POST] dados usando <code>application/x-www-form-urlencoded</code>.</p> <p>Para <code>[!UICONTROL application/x-www-form-urlencoded]</code>, o corpo da mensagem HTTP enviada ao servidor é essencialmente uma sequência de consulta. As chaves e os valores são codificados em pares de valores chave separados por <code>&amp;</code> e com um <code>=</code> entre a chave e o valor. </p> <p>Para dados binários, use <code>[!UICONTROL multipart/form-data]</code> em vez disso.</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>Exemplo: </b></span></span> 
       <p>Exemplo do formato de solicitação HTTP resultante:</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[!UICONTROL Multipart/dados de formulário]</strong> </p> <p>O [!UICONTROL Multipart/form-data] é uma solicitação HTTP multipart usada para enviar arquivos e dados. Normalmente, é usado para carregar arquivos no servidor.</p> <p>Adicione campos a serem enviados na solicitação. Cada campo deve conter um par de valor-chave.</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Texto]</strong> </p> <p>Informe a chave e o valor a serem enviados dentro do corpo da solicitação.</p> </li> 
       <li> <p><strong>[!UICONTROL Arquivo]</strong> </p> <p>Informe a chave e especifique o arquivo de origem que deseja enviar no corpo da solicitação.</p> <p>Mapeie o arquivo que você deseja carregar do módulo anterior (como [!UICONTROL HTTP] &gt;[!UICONTROL Obter um Arquivo] ou [!UICONTROL Unidade Google] &gt;[!UICONTROL Baixar um Arquivo)] ou insira o nome do arquivo e os dados do arquivo manualmente.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Analisar resposta]</p> </td> 
   <td> <p>Habilite esta opção para analisar respostas automaticamente e converter respostas JSON e XML, de modo que você não precise usar os módulos [!UICONTROL JSON] &gt; [!UICONTROL Parse JSON] ou [!UICONTROL XML] &gt; [!UICONTROL Parse XML].</p> <p>Antes de usar o conteúdo JSON ou XML analisado, execute o módulo uma vez manualmente para que o módulo possa reconhecer o conteúdo da resposta e permitir que você o mapeie em módulos subsequentes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tempo Limite] </td> 
   <td> <p>Especifique o tempo limite da solicitação em segundos (1-300). O padrão é 40 segundos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Compartilhar cookies com outros módulos HTTP]</td> 
   <td> <p> Habilite essa opção para compartilhar cookies do servidor com todos os módulos HTTP em seu cenário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Certificado autoassinado]</td> 
   <td> <p> Faça upload do seu certificado se quiser usar o TLS usando seu certificado autoassinado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rejeitar conexões que estão usando certificados não verificados (autoassinados)] </td> 
   <td> <p>Habilite esta opção para rejeitar conexões que estejam usando certificados TLS não verificados.</p> </td> 
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
   <td role="rowheader"> <p>[!UICONTROL Desabilitar serialização de várias chaves de cadeia de caracteres de consulta como matrizes]</p> </td> 
   <td> <p>Por padrão, [!DNL Workfront Fusion] O processa vários valores para a mesma chave de parâmetro de string de consulta de URL que os arrays. Por exemplo, <code>www.test.com?foo=bar&amp;foo=baz</code> será convertido em <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code>. Ative esta opção para desativar este recurso. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Solicitar conteúdo compactado]</td> 
   <td> <p> Habilite esta opção para solicitar uma versão compactada do site.</p> <p>Adiciona um <code>[!UICONTROL Accept-Encoding]</code> cabeçalho para solicitar conteúdo compactado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Usar TLS Mútuo]</td> 
   <td> <p>Habilite esta opção para usar o TLS mútuo na solicitação HTTP.</p> <p>Para obter mais informações sobre o TLS mútuo, consulte <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">Usar o TLS mútuo em módulos HTTP no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
