---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos AWS S3
description: O [!DNL Adobe Workfront Fusion AWS] Os módulos S3 permitem executar operações em seus buckets do S3.
author: Becky
feature: Workfront Fusion
exl-id: 33623b5d-d9ff-4d41-b938-33378f50539e
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1381'
ht-degree: 0%

---

# Módulos AWS S3

O [!DNL Adobe Workfront Fusion AWS] Os módulos S3 permitem executar operações em seus buckets do S3.

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

## Pré-requisitos

Para usar [!UICONTROL AWS S3] , você deve ter um [!DNL Amazon Web Service] conta.

## Connect [!DNL AWS] para [!DNL Workfront Fusion] {#connect-aws-to-workfront-fusion}

Para ligar [!DNL AWS S3] para [!DNL Workfront Fusion] você deve conectar seu [!DNL AWS] para [!DNL Workfront Fusion]. Para fazer isso, primeiro será necessário criar um usuário da API em [!DNL AWS] [!UICONTROL IAM].

1. Faça logon em seu [!DNL AWS] [!UICONTROL IAM] conta.
1. Navegar para **[!UICONTROL Gerenciamento de identidade e acesso]** > **[!UICONTROL Gerenciamento de acesso]** > **[!UICONTROL Usuários]**.

1. Clique em **[!UICONTROL Adicionar usuário]**.
1. Insira o nome do novo usuário e selecione o **[!UICONTROL Acesso programático]** na [!UICONTROL Tipo de acesso] seção.
1. Clique em **[!UICONTROL Anexar as políticas existentes diretamente]**, em seguida, pesquise por **[!UICONTROL AmazonS3FullAccess]** na barra de pesquisa. Clique nele quando ele for exibido e, em seguida, clique em **[!UICONTROL Próximo]**.

1. Prossiga pelas outras telas de diálogo e clique em **[!UICONTROL Criar usuário]**.
1. Copie o **[!UICONTROL ID da chave de acesso]** e **[!UICONTROL Chave de acesso secreta]**.

1. Ir para [!DNL Workfront Fusion] e abra o [!DNL AWS S3] do módulo **[!UICONTROL Criar uma conexão]** caixa de diálogo.
1. Insira o [!UICONTROL ID da chave de acesso] e [!UICONTROL Chave de acesso secreta] da etapa 7 para os respectivos campos e clique em **[!UICONTROL Continuar]** para estabelecer a conexão.

A conexão foi estabelecida. Você pode continuar com a configuração do módulo.

## [!DNL AWS S3] módulos e seus campos

Ao configurar [!DNL AWS S3] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL AWS S3] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Ações](#actions)
* [Pesquisas](#searches)

### Ações

* [[!UICONTROL Criar bucket]](#create-bucket)
* [[!UICONTROL Obter arquivo]](#get-file)
* [[!UICONTROL Carregar arquivo]](#upload-file)
* [[!UICONTROL Faça uma chamada de API]](#make-an-api-call)

#### [!UICONTROL Criar bucket]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL AWS] para [!DNL Workfront Fusion], consulte <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Insira o nome do novo bucket.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Região] </td> 
   <td> <p>Selecione o terminal regional. Para obter mais informações, consulte a discussão do <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">endpoints regionais</a> na documentação do AWS.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter arquivo]

Faz o download de um arquivo de um bucket.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL AWS] para [!DNL Workfront Fusion], consulte <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Região] </td> 
   <td> <p>Selecione o terminal regional. Para obter mais informações, consulte a discussão do <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">endpoints regionais</a> no [!DNL AWS] documentação.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>Selecione o bucket do qual deseja baixar o arquivo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Caminho]</p> </td> 
   <td> <p>Insira o caminho para o arquivo. Exemplo: <code>/photos/2019/February/image023.jpg</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Carregar arquivo]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL AWS] para [!DNL Workfront Fusion], consulte <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Região] </td> 
   <td> <p>Selecione o terminal regional. Para obter mais informações, consulte a discussão do <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">endpoints regionais</a> no [!DNL AWS] documentação.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Pasta] (opcional) </p> </td> 
   <td> <p>Especifique a pasta de destino para a qual deseja fazer upload de um arquivo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Cabeçalhos] (opcional)</p> </td> 
   <td> <p> Insira cabeçalhos de solicitação. Os cabeçalhos disponíveis podem ser encontrados no <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutObject.html">[!DNL AWS S3] documentação - objeto [!UICONTROL PUT]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Faça uma chamada de API]

Para uma discussão detalhada do [!DNL Amazon S3] API, consulte [[!DNL Amazon S3] [!UICONTROL REST] Introdução à API](https://docs.aws.amazon.com/AmazonS3/latest/API/Welcome.html).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL AWS] para [!DNL Workfront Fusion], consulte <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Região] </td> 
   <td> <p>Selecione o terminal regional. Para obter mais informações, consulte a discussão do <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">endpoints regionais</a> no [!DNL AWS] documentação.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>URL Insira um URL de host. O caminho deve ser relativo a<code> https://s3.&lt;selected-region>.amazonaws.com/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Método]</td> 
   <td> <p>Selecione o método de solicitação [!UICONTROL HTTP] que você precisa configurar a chamada da API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitação [!UICONTROL HTTP] em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione um cabeçalho de solicitação. Você pode usar os seguintes cabeçalhos de solicitação comuns. Para obter mais cabeçalhos de solicitação, consulte <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTCommonRequestHeaders.html">[!DNL AWS S3] Documentação da API</a>.</p> <p>[!DNL Workfront Fusion] adiciona cabeçalhos de autorização automaticamente.</p> 
    <table style="table-layout:auto">
     <col> 
     <col> 
     <thead> 
      <tr> 
       <th>Nome do cabeçalho</th> 
       <th> <p> Descrição</p> </th> 
      </tr> 
     </thead> 
     <tbody> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-Length]</p> </td> 
       <td> <p>Comprimento da mensagem (sem os cabeçalhos) de acordo com a RFC 2616. Esse cabeçalho é necessário para [!UICONTROL PUT e operações que carregam XML, como registro e ACLs.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-Type]</p> </td> 
       <td> <p>O tipo de conteúdo do recurso, caso o conteúdo da solicitação esteja no corpo. Exemplo: <code>text/plain</code>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-MD5]</p> </td> 
       <td> <p>A base64 codificou o resumo MD5 de 128 bits da mensagem (sem os cabeçalhos) de acordo com a RFC 1864. Esse cabeçalho pode ser usado como uma verificação de integridade de mensagem para verificar se os dados são os mesmos dados enviados originalmente. Embora seja opcional, recomendamos usar o mecanismo [!UICONTROL Content-MD5] como uma verificação de integridade completa. Para obter mais informações sobre a autenticação de solicitação [!UICONTROL REST], acesse <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/RESTAuthentication.html?r=1821">Autenticação [!UICONTROL REST]</a> no <i>[!DNL Amazon] Guia do desenvolvedor do Simple Storage Service</i>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Data]</p> </td> 
       <td> <p>A data e hora atuais de acordo com o solicitante. Exemplo: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. Quando você especifica a variável <code>Authorization </code>você deve especificar a variável <code>x-amz-date</code> ou <code>Date </code>cabeçalho.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Esperado]</p> </td> 
       <td> <p>Quando seu aplicativo usa o [!UICONTROL 100-continue], ele não envia o corpo da solicitação até receber uma confirmação. Se a mensagem for rejeitada com base nos cabeçalhos, o corpo da mensagem não será enviado. Esse cabeçalho só pode ser usado se você estiver enviando um corpo.</p> <p>Valores Válidos: [!UICONTROL 100-continue]</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Host]</p> </td> 
       <td> <p>Para solicitações de estilo de caminho, o valor é <code>s3.amazonaws.com</code>. Para solicitações de estilo virtual, o valor é <code>BucketName.s3.amazonaws.com</code>. Para obter mais informações, consulte <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/VirtualHosting.html">Hospedagem virtual</a> no <i>[!DNL Amazon] Guia do desenvolvedor do Simple Storage Service</i>.</p> <p>Esse cabeçalho é necessário para o HTTP 1.1 (a maioria dos kits adiciona esse cabeçalho automaticamente); opcional para solicitações HTTP/1.0.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-content-sha256]</p> </td> 
       <td> <p>Ao usar a versão de assinatura 4 para autenticar a solicitação, esse cabeçalho fornece um hash da carga da solicitação. Ao fazer upload de um objeto em partes, defina o valor como <code>STREAMING-AWS4-HMAC-SHA256-PAYLOAD</code> para indicar que a assinatura abrange apenas cabeçalhos e que não há carga útil. Para obter mais informações, consulte <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/sigv4-streaming.html">Cálculos de assinatura para o cabeçalho da autorização: Transferindo carga em vários blocos (upload fragmentado) ([!DNL AWS] Assinatura (Versão 4)</a>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-date]</p> </td> 
       <td> <p>A data e hora atuais de acordo com o solicitante. Exemplo: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. Quando você especifica a variável <code>Authorization </code>você deve especificar a variável <code>x-amz-date</code> ou <code>Date </code>cabeçalho. Se você especificar ambos, o valor especificado para a variável <code>x-amz-date</code> tem prioridade.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-security-token]</p> </td> 
       <td> <p>Esse cabeçalho pode ser usado nos seguintes cenários:</p> 
        <ul> 
         <li>Fornecer tokens de segurança para [!DNL Amazon DevPay] operações. Cada solicitação que usa [!DNL Amazon DevPay] exige dois <code>x-amz-security-token</code> cabeçalhos: um para o token de produto e um para o token de usuário. When [!DNL Amazon S3] recebe uma solicitação autenticada, compara a assinatura computada com a assinatura fornecida. Cabeçalhos de vários valores formatados incorretamente usados para calcular uma assinatura podem causar problemas de autenticação.</li> 
         <li>Forneça um token de segurança ao usar credenciais de segurança temporárias. Ao fazer solicitações usando credenciais de segurança temporárias obtidas do IAM, você deve fornecer um token de segurança usando esse cabeçalho. Para saber mais sobre credenciais de segurança temporárias, acesse Fazer solicitações .</li> 
        </ul> <p>Este cabeçalho é necessário para solicitações que usam [!DNL Amazon DevPay] e solicitações que são assinadas usando credenciais de segurança temporárias.</p> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sequência de consulta]</td> 
   <td> <p>Adicione as sequências de consulta desejadas, como parâmetros ou campos de formulário.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada da API no formato de um objeto JSON padrão.</p> <p>Nota:   <p>Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### Pesquisas

* [[!UICONTROL Listar arquivos]](#list-files)
* [[!UICONTROL Listar pastas]](#list-folders)

#### [!UICONTROL Listar arquivos]

Retorna uma lista de arquivos de um local especificado.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL AWS] para [!DNL Workfront Fusion], consulte <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Região] </td> 
   <td> <p>Selecione o terminal regional. Para obter mais informações, consulte a discussão do <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">endpoints regionais</a> no [!DNL AWS] documentação.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>Selecione o [!DNL Amazon S3] bucket que você deseja pesquisar por arquivos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prefixo] (opcional)</p> </td> 
   <td> <p> Caminho para uma pasta na qual procurar arquivos, por exemplo <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listar pastas]

Retorna uma lista de pastas de um local especificado.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL AWS] para [!DNL Workfront Fusion], consulte <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Região] </td> 
   <td> <p>Selecione o terminal regional. Para obter mais informações, consulte a discussão do <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">endpoints regionais</a> na documentação do AWS.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>Selecione o [!DNL Amazon S3] bucket que você deseja pesquisar por pastas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prefixo] (opcional)</p> </td> 
   <td> <p> Caminho para uma pasta na qual procurar pastas, por exemplo <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
