---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do AWS S3
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: 33623b5d-d9ff-4d41-b938-33378f50539e
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1455'
ht-degree: 0%

---

# Módulos do AWS S3

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Módulos do AWS S3](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/aws-s3-modules.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

Os módulos S3 [!DNL Adobe Workfront Fusion AWS] permitem executar operações em seus buckets S3.

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
   <p>Requisito atual do produto: se você tiver o plano [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], sua organização deve comprar [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] da [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Para usar os módulos do [!UICONTROL AWS S3], você deve ter uma conta [!DNL Amazon Web Service].

## Informações da API do AWS S3

O conector AWS S3 usa o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL base</td> 
   <td>https://s3.&lbrace;&lbrace;parameters.region&rbrace;&rbrace;.amazonaws.com</td> 
  </tr>
  <tr> 
   <td role="rowheader">Tag da API</td> 
   <td>v1.5.21</td> 
  </tr>
 </tbody> 
 </table>

## Conectar [!DNL AWS] a [!DNL Workfront Fusion] {#connect-aws-to-workfront-fusion}

Para conectar [!DNL AWS S3] a [!DNL Workfront Fusion], você deve conectar sua conta do [!DNL AWS] ao [!DNL Workfront Fusion]. Para fazer isso, primeiro será necessário criar um usuário de API no [!DNL AWS] [!UICONTROL IAM].

1. Entre na sua conta do [!DNL AWS] [!UICONTROL IAM].
1. Navegue até **[!UICONTROL Gerenciamento de Identidade e Acesso]** > **[!UICONTROL Gerenciamento de Acesso]** > **[!UICONTROL Usuários]**.

1. Clique em **[!UICONTROL Adicionar usuário]**.
1. Insira o nome do novo usuário e selecione a opção **[!UICONTROL Acesso programático]** na seção [!UICONTROL Tipo de acesso].
1. Clique em **[!UICONTROL Anexar diretivas existentes diretamente]** e procure por **[!UICONTROL AmazonS3FullAccess]** na barra de pesquisa. Clique nela quando ela aparecer, em seguida, clique em **[!UICONTROL Avançar]**.

1. Prossiga pelas outras telas de diálogo e clique em **[!UICONTROL Criar Usuário]**.
1. Copie a **[!UICONTROL ID da chave de acesso]** e a **[!UICONTROL chave de acesso secreta]** fornecidas.

1. Vá para [!DNL Workfront Fusion] e abra a caixa de diálogo **[!UICONTROL Criar uma conexão]** do módulo [!DNL AWS S3].
1. Insira a [!UICONTROL ID da chave de acesso] e a [!UICONTROL chave de acesso secreta] da etapa 7 para os respectivos campos e clique em **[!UICONTROL Continuar]** para estabelecer a conexão.

A conexão foi estabelecida. Você pode prosseguir com a configuração do módulo.

## [!DNL AWS S3] módulos e seus campos

Ao configurar módulos do [!DNL AWS S3], o [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos [!DNL AWS S3] adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Ações](#actions)
* [Pesquisas](#searches)

### Ações

* [[!UICONTROL Criar bloco]](#create-bucket)
* [[!UICONTROL Obter arquivo]](#get-file)
* [[!UICONTROL Carregar arquivo]](#upload-file)
* [[!UICONTROL Fazer uma chamada de API]](#make-an-api-call)

#### [!UICONTROL Criar bloco]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL AWS] ao [!DNL Workfront Fusion], consulte <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Conectar [!DNL AWS] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome] </td> 
   <td> <p>Informe o nome do novo período.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Região] </td> 
   <td> <p>Selecione seu ponto de extremidade regional. Para obter mais informações, consulte a discussão de <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">pontos de extremidade regionais</a> na documentação do AWS.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter arquivo]

Baixa um arquivo de um bucket.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL AWS] ao [!DNL Workfront Fusion], consulte <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Conectar [!DNL AWS] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Região] </td> 
   <td> <p>Selecione seu ponto de extremidade regional. Para obter mais informações, consulte a discussão de <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">pontos de extremidade regionais</a> na documentação [!DNL AWS].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Compartimento] </td> 
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
    <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL AWS] ao [!DNL Workfront Fusion], consulte <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Conectar [!DNL AWS] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Região] </td> 
   <td> <p>Selecione seu ponto de extremidade regional. Para obter mais informações, consulte a discussão de <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">pontos de extremidade regionais</a> na documentação [!DNL AWS].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Pasta] (opcional) </p> </td> 
   <td> <p>Especifique a pasta de destino para a qual você deseja fazer upload de um arquivo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL arquivo Source]</td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Cabeçalhos] (opcional)</p> </td> 
   <td> <p> Inserir cabeçalhos de solicitação. Cabeçalhos disponíveis podem ser encontrados na documentação <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutObject.html">[!DNL AWS S3] - [!UICONTROL PUT] object</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Fazer uma chamada de API]

Para obter uma discussão detalhada da API [!DNL Amazon S3], consulte a [[!DNL Amazon S3] [!UICONTROL Introdução à API REST]](https://docs.aws.amazon.com/AmazonS3/latest/API/Welcome.html).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL AWS] ao [!DNL Workfront Fusion], consulte <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Conectar [!DNL AWS] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Região] </td> 
   <td> <p>Selecione seu ponto de extremidade regional. Para obter mais informações, consulte a discussão de <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">pontos de extremidade regionais</a> na documentação [!DNL AWS].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>URL Insira um URL de host. O caminho deve ser relativo a <code> https://s3.&lt;selected-region>.amazonaws.com/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Método]</td> 
   <td> <p>Selecione o método de solicitação [!UICONTROL HTTP] necessário para configurar a chamada à API. Para obter mais informações, consulte os métodos de solicitação <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">[!UICONTROL HTTP] em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione um cabeçalho de solicitação. Você pode usar os seguintes cabeçalhos de solicitação comuns. Para obter mais cabeçalhos de solicitação consulte a <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTCommonRequestHeaders.html">[!DNL AWS S3] Documentação da API</a>.</p> <p>[!DNL Workfront Fusion] O adiciona cabeçalhos de autorização automaticamente.</p> 
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
       <td role="rowheader"> <p>[!UICONTROL Tamanho do Conteúdo]</p> </td> 
       <td> <p>Comprimento da mensagem (sem os cabeçalhos) de acordo com RFC 2616. Esse cabeçalho é necessário para [!UICONTROL PUT]s e operações que carregam XML, como log e ACLs.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Tipo de Conteúdo]</p> </td> 
       <td> <p>O tipo de conteúdo do recurso, caso o conteúdo da solicitação esteja no corpo. Exemplo: <code>text/plain</code>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-MD5]</p> </td> 
       <td> <p>O digest MD5 de 128 bits codificado em base64 da mensagem (sem os cabeçalhos) de acordo com a RFC 1864. Esse cabeçalho pode ser usado como uma verificação de integridade da mensagem para verificar se os dados são os mesmos que foram enviados originalmente. Embora seja opcional, recomendamos usar o mecanismo [!UICONTROL Content-MD5] como uma verificação de integridade completa. Para obter mais informações sobre a autenticação de solicitação do [!UICONTROL REST], vá para a Autenticação do <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/RESTAuthentication.html?r=1821">[!UICONTROL REST]</a> no <i>[!DNL Amazon] Guia do Desenvolvedor do Serviço de Armazenamento Simples</i>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Data]</p> </td> 
       <td> <p>A data e a hora atuais de acordo com o solicitante. Exemplo: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. Ao especificar o cabeçalho <code>Authorization </code>, você deve especificar o cabeçalho <code>x-amz-date</code> ou <code>Date </code>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Esperar]</p> </td> 
       <td> <p>Quando seu aplicativo usa [!UICONTROL 100-continue], ele não envia o corpo da solicitação até que receba uma confirmação. Se a mensagem for rejeitada com base nos cabeçalhos, o corpo da mensagem não será enviado. Esse cabeçalho só poderá ser usado se você estiver enviando um corpo.</p> <p>Valores Válidos: [!UICONTROL 100-continue]</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Host]</p> </td> 
       <td> <p>Para solicitações de estilo de caminho, o valor é <code>s3.amazonaws.com</code>. Para solicitações de estilo virtual, o valor é <code>BucketName.s3.amazonaws.com</code>. Para obter mais informações, consulte <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/VirtualHosting.html">Hospedagem Virtual</a> no <i>[!DNL Amazon] Guia do Desenvolvedor do Serviço de Armazenamento Simples</i>.</p> <p>Esse cabeçalho é necessário para HTTP 1.1 (a maioria dos kits de ferramentas adiciona esse cabeçalho automaticamente); opcional para solicitações HTTP/1.0.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-content-sha256]</p> </td> 
       <td> <p>Ao usar a assinatura versão 4 para autenticar a solicitação, este cabeçalho fornece um hash da carga da solicitação. Ao carregar um objeto em partes, defina o valor como <code>STREAMING-AWS4-HMAC-SHA256-PAYLOAD</code> para indicar que a assinatura cobre apenas cabeçalhos e que não há carga útil. Para obter mais informações, consulte <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/sigv4-streaming.html">Cálculos de assinatura para o Cabeçalho de autorização: Transferindo carga em várias partes (Carregamento fragmentado) ([!DNL AWS] Versão de assinatura 4)</a>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL data-x-amz]</p> </td> 
       <td> <p>A data e a hora atuais de acordo com o solicitante. Exemplo: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. Ao especificar o cabeçalho <code>Authorization </code>, você deve especificar o cabeçalho <code>x-amz-date</code> ou <code>Date </code>. Se você especificar ambos, o valor especificado para o cabeçalho <code>x-amz-date</code> terá prioridade.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-security-token]</p> </td> 
       <td> <p>Esse cabeçalho pode ser usado nos seguintes cenários:</p> 
        <ul> 
         <li>Forneça tokens de segurança para [!DNL Amazon DevPay] operações. Cada solicitação que usa [!DNL Amazon DevPay] requer dois cabeçalhos <code>x-amz-security-token</code>: um para o token do produto e um para o token do usuário. Quando [!DNL Amazon S3] recebe uma solicitação autenticada, ele compara a assinatura computada com a assinatura fornecida. Cabeçalhos multivalores formatados incorretamente usados para calcular uma assinatura podem causar problemas de autenticação.</li> 
         <li>Forneça um token de segurança ao usar credenciais de segurança temporárias. Ao fazer solicitações usando credenciais de segurança temporárias obtidas do IAM, você deve fornecer um token de segurança usando esse cabeçalho. Para saber mais sobre credenciais de segurança temporárias, acesse Fazer solicitações.</li> 
        </ul> <p>Este cabeçalho é necessário para solicitações que usam [!DNL Amazon DevPay] e solicitações que são assinadas usando credenciais de segurança temporárias.</p> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cadeia de Consulta]</td> 
   <td> <p>Adicione as cadeias de caracteres de consulta desejadas, como parâmetros ou campos de formulário.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada à API na forma de um objeto JSON padrão.</p> <p>Nota:   <p>Ao usar instruções condicionais como <code>if</code> em seu JSON, coloque as aspas fora da instrução condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### Pesquisas

* [[!UICONTROL Listar Arquivos]](#list-files)
* [[!UICONTROL Listar pastas]](#list-folders)

#### [!UICONTROL Listar Arquivos]

Retorna uma lista de arquivos de um local especificado.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL AWS] ao [!DNL Workfront Fusion], consulte <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Conectar [!DNL AWS] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Região] </td> 
   <td> <p>Selecione seu ponto de extremidade regional. Para obter mais informações, consulte a discussão de <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">pontos de extremidade regionais</a> na documentação [!DNL AWS].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Compartimento] </td> 
   <td> <p>Selecione o bucket [!DNL Amazon S3] que você deseja pesquisar arquivos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prefixo] (opcional)</p> </td> 
   <td> <p> Caminho para uma pasta na qual procurar arquivos, por exemplo, <code>workfrontfusion/work.</code></p> </td> 
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
    <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL AWS] ao [!DNL Workfront Fusion], consulte <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Conectar [!DNL AWS] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Região] </td> 
   <td> <p>Selecione seu ponto de extremidade regional. Para obter mais informações, consulte a discussão de <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">pontos de extremidade regionais</a> na documentação do AWS.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Compartimento] </td> 
   <td> <p>Selecione o bucket [!DNL Amazon S3] que deseja pesquisar pastas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prefixo] (opcional)</p> </td> 
   <td> <p> Caminho para uma pasta na qual pesquisar pastas, por exemplo, <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
