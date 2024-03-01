---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Adobe Photoshop
description: Com os módulos do Adobe Photoshop, você pode iniciar um cenário do Adobe Workfront Fusion com base em eventos em sua conta do Adobe Photoshop, criar, ler ou atualizar contratos e outros registros, pesquisar registros usando critérios definidos e fazer upload de documentos.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
source-git-commit: 0ea4ac4c4579d09dafeed47946ae9c7caf906cfe
workflow-type: tm+mt
source-wordcount: '1582'
ht-degree: 0%

---

# [!DNL Adobe Photoshop] módulos

Em um [!DNL Adobe Workfront Fusion] cenário, é possível automatizar workflows que usam [!DNL Adobe Photoshop], bem como conectá-lo a vários aplicativos e serviços de terceiros. [!DNL Adobe Photoshop] Os módulos do permitem criar, ler, atualizar ou excluir registros, listar todos os registros de um determinado tipo, pesquisar registros com base nos critérios especificados ou executar uma chamada de API personalizada para o [!DNL Adobe Photoshop] API.


Se precisar de instruções sobre como criar um cenário, consulte [Criar um cenário](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obter informações sobre módulos, consulte [Módulos no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plano*</td>
      <td>
        <p>[!UICONTROL Pro] ou superior</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] licença*</td>
      <td>
        <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] licença**</td>
      <td >
        <p>[!UICONTROL Workfront Fusion para Automação e Integração do Trabalho]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Produto</td>
      <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td>
    </tr>
    </tr>
  </tbody>
</table>


&#42;Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

&#42;&#42;Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [!DNL [Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Pré-requisitos

Antes de poder usar o [!DNL Adobe Photoshop] deve garantir que os seguintes pré-requisitos sejam atendidos:

* Você deve ter um ativo [!DNL Adobe Photoshop] conta.

## Criar uma conexão com o [!DNL Adobe Photoshop]

Para criar uma conexão para o seu [!DNL Adobe Photoshop] módulos:

1. Clique em **[!UICONTROL Adicionar]** ao lado da caixa Conexão.

1. Preencha os seguintes campos:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
        <td role="rowheader">[!UICONTROL Nome da Conexão]</td>
        <td>
          <p>Insira um nome para esta conexão.</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL ID do Cliente]</td>
        <td>Insira sua [!UICONTROL Adobe] [!UICONTROL ID do cliente]. Isso pode ser encontrado na seção de detalhes [!UICONTROL Credentials] do [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Segredo do Cliente]</td>
        <td>Insira seu [!DNL Adobe] [!UICONTROL Segredo do Cliente]. Isso pode ser encontrado na seção de detalhes [!UICONTROL Credentials] do [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL ID da conta técnica]</td>
        <td>Insira seu [!DNL Adobe] [!UICONTROL ID da conta técnica]. Isso pode ser encontrado na seção de detalhes [!UICONTROL Credentials] do [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL ID da Organização]</td>
        <td>Insira seu [!DNL Adobe] [!UICONTROL ID da Organização]. Isso pode ser encontrado na seção de detalhes [!UICONTROL Credentials] do [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Chave privada]</td>
        <td>
          <p>Insira a chave privada que foi gerada quando suas credenciais foram criadas na [!DNL Adobe Developer Console]. </p>
          <p>Para extrair sua chave privada ou certificado:</p>
          <ol>
            <li value="1">
              <p>Clique em <b>[!UICONTROL Extract]</b>.</p>
            </li>
            <li value="2">
              <p>Selecione o tipo de arquivo que você está extraindo.</p>
            </li>
            <li value="3">
              <p>Selecione o arquivo que contém a chave privada ou o certificado.</p>
            </li>
            <li value="4">
              <p>Digite a senha do arquivo.</p>
            </li>
            <li value="5">
              <p>Clique em <b>Salvar</b> para extrair o arquivo e retornar à configuração da conexão [!UICONTROL ] e.</p>
            </li>
          </ol>
        </td>
        </tr>
      </tbody>
    </table>

1. Clique em **[!UICONTROL Continuar]** para salvar a conexão e retornar ao módulo.

## [!DNL Adobe Photoshop] módulos e seus campos

Ao configurar [!DNL Adobe Photoshop] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Adobe Photoshop] Os campos podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)


### Ações

* [Criar um novo PSD](#create-a-new-psd)
* [Editar camadas de texto](#edit-text-layers)
* [Executar desfoque de profundidade](#execute-depth-blur)
* [Executar ações do Photoshop](#execute-photoshop-actions)
* [Executar corte do produto](#execute-product-crop)
* [Obter informações da camada](#get-layer-info)
* [Fazer uma chamada de API personalizada](#make-a-custom-api-call)

#### Criar um novo PSD

Esse módulo de ação cria um novo PSD com camadas opcionais e gera representações ou salva como um PSD.

Para campos relacionados a este módulo, consulte [Criar um novo PSD](https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/documentCreate) na documentação do Adobe Photoshop.

#### Editar camadas de texto

Esse módulo de ação edita camadas de texto em um arquivo do Photoshop.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Photoshop], consulte <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Photoshop]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Armazenamento de arquivo de entrada]</td>
      <td>
        <p>Selecione o serviço de arquivos no qual o arquivo que você deseja editar está armazenado.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL do arquivo de entrada]</p>
      </td>
   <td> Insira ou mapeie o URL ou o caminho do arquivo que deseja editar. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gerenciar fontes ausentes]</td>
      <td>
        <p>Selecione a ação a ser tomada se houver uma ou mais fontes ausentes no documento. Se a fonte não for fornecida, o módulo usará a fonte padrão.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Fonte padrão]  </td>
      <td>
        <p>Digite o nome completo do postscript da fonte a ser usada como padrão global para o documento. Essa fonte será usada para qualquer camada de texto que tenha uma fonte ausente e nenhuma outra fonte tenha sido especificamente fornecida para essa camada. Se esta fonte estiver ausente, a opção especificada em Gerenciar fontes ausentes entrará em vigor.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Camadas]</td>
   <td> <p>Para obter detalhes sobre as opções de camada, consulte <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/text">Editar camada de texto</a> na documentação do Adobe Photoshop.</p>  </td>     </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Armazenamento de arquivo de saída]</td>
      <td>
        <p>Selecione o serviço de arquivos no qual você deseja que o arquivo editado seja armazenado.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL do arquivo de saída]</p>
      </td>
   <td> Insira ou mapeie o URL ou o caminho de onde o arquivo editado será armazenado. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Tipo de arquivo de saída]</p>
      </td>
   <td> Selecione o tipo de arquivo para o arquivo editado. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Substituir]</td>
      <td>
        <p>Selecione se o arquivo recém-editado substituirá qualquer arquivo de saída existente.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compactação]</p>
      </td>
   <td> Selecione o nível de compactação para o arquivo de saída. </td> 
    </tr>
  </tbody>
</table>

#### Executar desfoque de profundidade

Esse módulo de ação executa o Desfoque de Profundidade no arquivo selecionado.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Photoshop], consulte <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Photoshop]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Armazenamento de arquivo de entrada]</td>
      <td>
        <p>Selecione o serviço de arquivos no qual o arquivo que você deseja editar está armazenado.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL do arquivo de entrada]</p>
      </td>
   <td> Insira ou mapeie o URL ou o caminho do arquivo que deseja editar. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Armazenamento de arquivo de saída]</td>
      <td>
        <p>Selecione o serviço de arquivos no qual você deseja que o arquivo editado seja armazenado.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL do arquivo de saída]</p>
      </td>
   <td> Insira ou mapeie o URL ou o caminho de onde o arquivo editado será armazenado. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Tipo de arquivo de saída]</p>
      </td>
   <td> Selecione o tipo de arquivo para o arquivo editado. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Outros campos]</td>
      <td>
        <p>Para obter detalhes sobre outras opções de Desfoque de Profundidade, consulte <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/depthBlur">Executar desfoque de profundidade </a>na documentação da API do Adobe Photoshop.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Substituir]</td>
      <td>
        <p>Selecione se o arquivo recém-editado substituirá qualquer arquivo de saída existente.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compactação]</p>
      </td>
   <td> Selecione o nível de compactação para o arquivo de saída. </td> 
    </tr>
  </tbody>
</table>

#### Executar ações do Photoshop

Esse módulo de ação executa uma ação Photoshop na imagem selecionada.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Photoshop], consulte <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Photoshop]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Armazenamento de arquivo de entrada]</td>
      <td>
        <p>Selecione o serviço de arquivos no qual o arquivo que você deseja editar está armazenado.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL do arquivo de entrada]</p>
      </td>
   <td> Insira ou mapeie o URL ou o caminho do arquivo que deseja editar. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ações armazenamento de arquivo]</td>
      <td>
        <p>Selecione o serviço de arquivos onde o arquivo de ações está armazenado.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL do arquivo de ações]</p>
      </td>
   <td> Insira ou mapeie o URL ou o caminho do arquivo de ações. </td> 
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Nome da ação]</p>
      </td>
   <td> Se desejar executar apenas uma ação específica, você pode especificar qual ação executar a partir do ActionSet. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Armazenamento de fonte / padrão / pincel]</td>
      <td>
        <p>Selecione o serviço de arquivos no qual o arquivo que deseja usar está armazenado.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Fonte / Padrão / URL do arquivo de Pincel]</p>
      </td>
   <td> Insira ou mapeie o URL ou o caminho do arquivo que deseja usar. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Armazenamento de arquivo de saída]</td>
      <td>
        <p>Selecione o serviço de arquivos no qual você deseja que o arquivo editado seja armazenado.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL do arquivo de saída]</p>
      </td>
   <td> Insira ou mapeie o URL ou o caminho de onde o arquivo editado será armazenado. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Tipo de arquivo de saída]</p>
      </td>
   <td> Selecione o tipo de arquivo para o arquivo editado. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Substituir]</td>
      <td>
        <p>Selecione se o arquivo recém-editado substituirá qualquer arquivo de saída existente.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compactação]</p>
      </td>
   <td> Selecione o nível de compactação para o arquivo de saída. </td> 
    </tr>
  </tbody>
</table>

#### Executar corte do produto

Esse módulo de ação executa o Recorte de produto na imagem selecionada.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Photoshop], consulte <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Photoshop]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Armazenamento de arquivo de entrada]</td>
      <td>
        <p>Selecione o serviço de arquivos onde o arquivo que você deseja cortar está armazenado.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL do arquivo de entrada]</p>
      </td>
   <td> Insira ou mapeie o URL ou o caminho do arquivo que você deseja cortar. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Unidade]</p>
      </td>
   <td> Selecione se deseja descrever o ajuste de altura e largura em pixels ou como uma porcentagem. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Largura]</p>
      </td>
   <td> Insira ou mapeie a quantidade de preenchimento de largura que deseja adicionar. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Altura]</p>
      </td>
   <td> Insira ou mapeie a quantidade de preenchimento de altura que deseja adicionar. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Armazenamento de arquivo de saída]</td>
      <td>
        <p>Selecione o serviço de arquivos no qual você deseja que o arquivo editado seja armazenado.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL do arquivo de saída]</p>
      </td>
   <td> Insira ou mapeie o URL ou o caminho de onde o arquivo editado será armazenado. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Tipo de arquivo de saída]</p>
      </td>
   <td> Selecione o tipo de arquivo para o arquivo editado. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Substituir]</td>
      <td>
        <p>Selecione se o arquivo recém-editado substituirá qualquer arquivo de saída existente.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compactação]</p>
      </td>
   <td> Selecione o nível de compactação para o arquivo de saída. </td> 
    </tr>
  </tbody>
</table>

#### Obter informações da camada

Esse módulo de ação recupera informações de camada do arquivo de PSD especificado.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Photoshop], consulte <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Photoshop]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Armazenamento de arquivo de entrada]</td>
      <td>
        <p>Selecione o serviço de arquivo no qual o arquivo do qual você deseja recuperar as informações de camada é armazenado.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL do arquivo de entrada]</p>
      </td>
   <td> Insira ou mapeie o URL ou o caminho do arquivo do qual deseja recuperar as informações da camada. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Miniaturas]</p>
      </td>
   <td> </td> 
    </tr>
  </tbody>
</table>

#### Fazer uma chamada de API personalizada

Esse módulo de ação faz uma chamada personalizada para a API do Photoshop.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Photoshop], consulte <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Photoshop]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Insira um caminho relativo a <code>https://image.adobe.io/pie/psdService</code>. Exemplo: <code>/photoshopActions</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Método]</p>
      </td>
   <td> <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cabeçalhos]</td>
      <td>
        <p>Adicione os cabeçalhos da solicitação no formulário de um objeto JSON padrão.</p>
        <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] O adiciona cabeçalhos de autorização automaticamente.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cadeia de Consulta]  </td>
      <td>
        <p>Insira a string de consulta da solicitação.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Corpo]</td>
   <td> <p>Adicione o conteúdo do corpo para a chamada à API na forma de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

