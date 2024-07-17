---
filename: creative-cloud-libraries-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos de bibliotecas do Adobe Creative Cloud
description: Com os módulos  [!DNL Adobe Workfront Fusion Adobe Creative Cloud] Bibliotecas, você pode iniciar um cenário quando um elemento ou biblioteca for criado ou atualizado. Você também pode carregar, recuperar, arquivar ou listar elementos ou fazer uma chamada para a API  [!DNL Adobe Creative Cloud Libraries] .
author: Becky
feature: Workfront Fusion
exl-id: 8affa34b-803d-48a5-a986-9fbe0cb8c8f5
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '1241'
ht-degree: 0%

---

# Módulos de bibliotecas da Adobe Creative Cloud

Com os módulos [!DNL Adobe Workfront Fusion] [!DNL Adobe Creative Cloud Libraries], é possível iniciar um cenário quando um elemento ou biblioteca é criado ou atualizado. Você também pode carregar, recuperar, arquivar ou listar elementos, ou fazer uma chamada para a API [!DNL Adobe Creative Cloud Libraries].

Se você precisar de instruções sobre como criar um cenário, consulte [Criar um cenário](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obter informações sobre módulos, consulte [Módulos em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

## Pré-requisitos

Para usar módulos do [!DNL Adobe Creative Cloud Libraries], você deve ter uma conta do [!UICONTROL Adobe Creative Cloud].

## [!UICONTROL Módulos de bibliotecas do Adobe Creative Cloud] e seus campos

Ao configurar os módulos [!UICONTROL Bibliotecas de Adobe Creative Cloud], o [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos [!DNL Adobe Creative Cloud Libraries] adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)


* [Elementos](#elements)

* [Bibliotecas](#libraries)

* [Outro](#other)


### Elementos

* [[!UICONTROL Arquivar um elemento]](#archive-an-element)

* [[!UICONTROL Obter um elemento]](#get-an-element)

* [[!UICONTROL Listar Elementos]](#list-elements)

* [[!UICONTROL Carregar um Elemento]](#upload-an-element)

* [!UICONTROL [Observar novo elemento na biblioteca]](#watch-new-element-in-library)

* [[!UICONTROL Observar elementos atualizados]](#watch-updated-elements)


#### [!UICONTROL Arquivar um elemento]

Este módulo de ação arquiva um elemento de uma biblioteca.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como conectar sua conta do [!DNL Adobe Creative Cloud] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID da Biblioteca]</td>
      <td >Selecione a biblioteca que contém o elemento que você deseja arquivar.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[!UICONTROL ID de Elemento]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Selecione o elemento que deseja arquivar.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obter um elemento]

Esse módulo de ação retorna um único elemento de uma biblioteca.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como conectar sua conta do [!DNL Adobe Creative Cloud] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID da Biblioteca]</td>
      <td >Selecione a biblioteca que contém o elemento que você deseja recuperar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Elemento]</td>
      <td>Insira ou mapeie a ID do elemento que você deseja recuperar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Seletor]</td>
      <td>
        <p>Selecione o tipo de informação que o módulo retorna. </p>
        <ul>
          <li>
            <p><b>[!UICONTROL Padrão]</b>
            </p>
            <p>Dados base</p>
          </li>
          <li>
            <p><b>[!UICONTROL Detalhes]</b>
            </p>
            <p>Todos os dados disponíveis</p>
          </li>
          <li>
            <p><b>[!UICONTROL Representações]</b>
            </p>
            <p>Uma lista nivelada de ativos associados ao elemento de biblioteca</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Listar Elementos]

Este módulo de ação recupera uma lista de elementos em uma biblioteca.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como conectar sua conta do [!DNL Adobe Creative Cloud] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID da Biblioteca]</td>
      <td >Selecione a biblioteca da qual deseja listar elementos.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ordenar por]</td>
      <td>Selecione se deseja ordenar os resultados por nome ou pela última data em que o elemento foi modificado.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo]</td>
      <td >Informe um tipo MIME para limitar os resultados aos elementos identificados com o tipo MIME especificado. Exemplo: <code>string</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Seletor]</td>
      <td>
        <p>Selecione o tipo de informação que o módulo retorna. </p>
        <ul>
          <li>
            <p><b>[!UICONTROL Padrão]</b>
            </p>
            <p>Dados base</p>
          </li>
          <li>
            <p><b>[!UICONTROL Detalhes]</b>
            </p>
            <p>Todos os dados disponíveis</p>
          </li>
          <li>
            <p><b>[!UICONTROL Representações]</b>
            </p>
            <p>Uma lista nivelada de ativos associados ao elemento de biblioteca</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]</td>
      <td>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Carregar um Elemento]

Esse módulo de ação faz upload de um pequeno ativo de arquivo para uma biblioteca existente. O tamanho máximo do arquivo é 1 GB.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como conectar sua conta do [!DNL Adobe Creative Cloud] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID da Biblioteca]</td>
      <td >Selecione a biblioteca da qual deseja listar elementos.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Modo de Chamada]</td>
      <td>
        <p>Selecione o modo de processamento com o qual chamar este processo de solicitação.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL sincronização]</b>
            </p>
            <p>A chamada à API é processada de forma síncrona. A resposta é entregue quando o processamento é concluído (a menos que a chamada atinja o tempo limite.)</p>
          </li>
          <li>
            <p><b>[!UICONTROL assíncrono]</b>
            </p>
            <p>A resposta do monitor assíncrono é retornada imediatamente e o processamento de solicitações ocorre de forma assíncrona. A chamada é responsável por sondar o endpoint até a conclusão.</p>
          </li>
          <li>
            <p><b>[!UICONTROL sync,async]</b> (Padrão)</p>
            <p>Tentativa de processamento síncrono da solicitação. Quando o processamento se estende além de 5000 ms, a resposta do monitor assíncrono é retornada. O URL do monitor deve ser sondado até que a solicitação seja concluída.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Arquivo de Tipo]</td>
      <td >Insira ou mapeie o tipo MIME do arquivo carregado.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Arquivo Source]</td>
      <td>
        <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Assistir ao Novo Elemento na Biblioteca]

Esse módulo de acionamento inicia um cenário quando um elemento é adicionado a uma biblioteca.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como conectar sua conta do [!DNL Adobe Creative Cloud] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID da Biblioteca]</td>
      <td >Selecione a biblioteca que deseja observar por elementos atualizados.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]</td>
      <td>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL Observar elementos atualizados]

Esse módulo de acionamento inicia um cenário quando um elemento em uma biblioteca é atualizado.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como conectar sua conta do [!DNL Adobe Creative Cloud] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID da Biblioteca]</td>
      <td >Selecione a biblioteca que deseja observar para novos elementos.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]</td>
      <td>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</td>
    </tr>
  </tbody>
</table>

### Bibliotecas

* [[!UICONTROL Assistir a Novas Bibliotecas]](#watch-new-libraries)

* [[!UICONTROL Assistir Bibliotecas Atualizadas]](#watch-updated-libraries)


#### [!UICONTROL Assistir a Novas Bibliotecas]

Esse módulo de acionamento inicia um cenário quando uma nova biblioteca é criada.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como conectar sua conta do [!DNL Adobe Creative Cloud] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]</td>
      <td>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Assistir Bibliotecas Atualizadas]

Esse módulo de acionamento inicia um cenário quando uma biblioteca existente é atualizada.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como conectar sua conta do [!DNL Adobe Creative Cloud] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]</td>
      <td>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</td>
    </tr>
  </tbody>
</table>

### Outro

#### [!UICONTROL Fazer uma chamada de API]

Este módulo faz uma chamada de API personalizada para a API [!DNL Adobe Creative Cloud Libraries].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td> <p>Para obter instruções sobre como conectar sua conta do Adobe Creative Cloud ao Workfront Fusion, consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe Workfront Fusion - Instruções básicas.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Insira um caminho relativo para <code>https://cc-libraries.adobe.io/api</code>.</p>
    <p>Por exemplo <code>/v1/libraries</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL versão da API]</td>
      <td>
        <p>Selecione a versão da API [!DNL Adobe Analytics] à qual você deseja se conectar.</p>
      </td>
    </tr>    <tr>
      <td role="rowheader">[!UICONTROL Método]</td>
      <td> <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cabeçalhos]</td>
      <td>
        <p>Adicione os cabeçalhos da solicitação no formulário de um objeto JSON padrão.</p>
        <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p>
        <p>O Workfront Fusion adiciona os cabeçalhos de autorização para você.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cadeia de Consulta]</td>
      <td>
        <p>Adicione a consulta da chamada à API na forma de um objeto JSON padrão.</p>
        <p>Por exemplo: <code>{"name":"something-urgent"}</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Corpo]</td>
   <td> <p>Adicione o conteúdo do corpo para a chamada à API na forma de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar instruções condicionais como <code>if</code> em seu JSON, coloque as aspas fora da instrução condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
       <tr>
      <td role="rowheader">[!UICONTROL Carregar um documento transitório]</td>
      <td>
      <p>Para fazer upload de um documento transitório, informe o arquivo de origem do documento que deseja fazer upload.</p>
      <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p>
    </td>
    </tr>

</tbody>
</table>
