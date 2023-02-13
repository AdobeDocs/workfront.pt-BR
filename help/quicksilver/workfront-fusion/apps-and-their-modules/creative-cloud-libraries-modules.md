---
filename: creative-cloud-libraries-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos de bibliotecas Adobe Creative Cloud
description: Com o [!DNL Adobe Workfront Fusion Adobe Creative Cloud] Módulos de bibliotecas, é possível iniciar um cenário quando um elemento ou biblioteca é criada ou atualizada. Você também pode fazer upload, recuperar, arquivar ou listar elementos, ou fazer uma chamada para o [!DNL Adobe Creative Cloud Libraries] API.
author: Becky
exl-id: 8affa34b-803d-48a5-a986-9fbe0cb8c8f5
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1193'
ht-degree: 0%

---

# Módulos de bibliotecas Adobe Creative Cloud

Com o [!DNL Adobe Workfront Fusion] [!DNL Adobe Creative Cloud Libraries] , você pode iniciar um cenário quando um elemento ou biblioteca é criada ou atualizada. Você também pode fazer upload, recuperar, arquivar ou listar elementos, ou fazer uma chamada para o [!DNL Adobe Creative Cloud Libraries] API.

Se precisar de instruções para criar um cenário, consulte [Criar um cenário](../../workfront-fusion/scenarios/create-a-scenario.md).

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
      <td >
        <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho]</p>
      </td>
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

Para usar [!DNL Adobe Creative Cloud Libraries] , você deve ter um [!UICONTROL Adobe Creative Cloud] conta.

## [!UICONTROL Bibliotecas de Adobe Creative Cloud] módulos e seus campos

Ao configurar [!UICONTROL Bibliotecas de Adobe Creative Cloud] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Adobe Creative Cloud Libraries] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)


* [Elementos](#elements)

* [Bibliotecas](#libraries)

* [Outro](#other)


### Elementos

* [[!UICONTROL Arquivar um elemento]](#archive-an-element)

* [[!UICONTROL Obter um elemento]](#get-an-element)

* [[!UICONTROL Elementos da lista]](#list-elements)

* [[!UICONTROL Fazer upload de um elemento]](#upload-an-element)

* [!UICONTROL [Assista ao novo elemento na biblioteca]](#watch-new-element-in-library)

* [[!UICONTROL Assista a elementos atualizados]](#watch-updated-elements)


#### [!UICONTROL Arquivar um elemento]

Este módulo de ação arquiva um elemento de uma biblioteca.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Para obter instruções sobre como conectar seu [!DNL Adobe Creative Cloud] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID da biblioteca]</td>
      <td >Selecione a biblioteca que contém o elemento que deseja arquivar.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[!UICONTROL ID do elemento]</td>
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
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Para obter instruções sobre como conectar seu [!DNL Adobe Creative Cloud] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID da biblioteca]</td>
      <td >Selecione a biblioteca que contém o elemento que deseja recuperar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do elemento]</td>
      <td>Insira ou mapeie a ID do elemento que deseja recuperar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Seletor]</td>
      <td>
        <p>Selecione o tipo de informação que o módulo retorna. </p>
        <ul>
          <li>
            <p><b>[!UICONTROL Padrão]</b>
            </p>
            <p>Dados de base</p>
          </li>
          <li>
            <p><b>[!UICONTROL Detalhes]</b>
            </p>
            <p>Todos os dados disponíveis</p>
          </li>
          <li>
            <p><b>[!UICONTROL Representações]</b>
            </p>
            <p>Uma lista nivelada de ativos associados ao elemento da biblioteca</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Elementos da lista]

Esse módulo de ação recupera uma lista de elementos em uma biblioteca.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Para obter instruções sobre como conectar seu [!DNL Adobe Creative Cloud] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID da biblioteca]</td>
      <td >Selecione a biblioteca da qual deseja listar elementos.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Pedido por]</td>
      <td>Selecione se deseja ordenar os resultados por nome ou pela última data em que o elemento foi modificado.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo]</td>
      <td >Insira um tipo MIME para limitar os resultados a elementos identificados com o tipo MIME especificado. Exemplo: <code>string</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Seletor]</td>
      <td>
        <p>Selecione o tipo de informação que o módulo retorna. </p>
        <ul>
          <li>
            <p><b>[!UICONTROL Padrão]</b>
            </p>
            <p>Dados de base</p>
          </li>
          <li>
            <p><b>[!UICONTROL Detalhes]</b>
            </p>
            <p>Todos os dados disponíveis</p>
          </li>
          <li>
            <p><b>[!UICONTROL Representações]</b>
            </p>
            <p>Uma lista nivelada de ativos associados ao elemento da biblioteca</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]</td>
      <td>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Fazer upload de um elemento]

Este módulo de ação carrega um pequeno ativo de arquivo em uma biblioteca existente. O tamanho máximo do arquivo é de 1 GB.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Para obter instruções sobre como conectar seu [!DNL Adobe Creative Cloud] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID da biblioteca]</td>
      <td >Selecione a biblioteca da qual deseja listar elementos.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Modo de chamada]</td>
      <td>
        <p>Selecione o modo de processamento com o qual invocar este processo de solicitação.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL sincronizar]</b>
            </p>
            <p>A chamada da API é processada de forma síncrona. A resposta é entregue quando o processamento é concluído (a menos que a chamada atinja o tempo limite).</p>
          </li>
          <li>
            <p><b>[!UICONTROL async]</b>
            </p>
            <p>A resposta do monitor assíncrono é retornada imediatamente e o processamento da solicitação ocorre de forma assíncrona. A chamada é responsável pela pesquisa do terminal até a conclusão.</p>
          </li>
          <li>
            <p><b>[!UICONTROL sincronizar,async]</b> (Padrão)</p>
            <p>Tentativa de processamento síncrono da solicitação. Quando o processamento ultrapassa os 5000 ms, a resposta do monitor assíncrono é retornada. O URL do monitor deve ser sondado até que a solicitação seja concluída.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Arquivo de tipo]</td>
      <td >Insira ou mapeie o tipo MIME do arquivo carregado.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Arquivo de origem]</td>
      <td>
        <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Assista ao novo elemento na biblioteca]

Esse módulo de acionador inicia um cenário quando um elemento é adicionado a uma biblioteca.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Para obter instruções sobre como conectar seu [!DNL Adobe Creative Cloud] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID da biblioteca]</td>
      <td >Selecione a biblioteca que deseja visualizar para elementos atualizados.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]</td>
      <td>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL Assista a elementos atualizados]

Esse módulo de acionador inicia um cenário quando um elemento em uma biblioteca é atualizado.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Para obter instruções sobre como conectar seu [!DNL Adobe Creative Cloud] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID da biblioteca]</td>
      <td >Selecione a biblioteca que deseja visualizar para novos elementos.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]</td>
      <td>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</td>
    </tr>
  </tbody>
</table>

### Bibliotecas

* [[!UICONTROL Assista às novas bibliotecas]](#watch-new-libraries)

* [[!UICONTROL Assista às bibliotecas atualizadas]](#watch-updated-libraries)


#### [!UICONTROL Assista às novas bibliotecas]

Esse módulo de acionador inicia um cenário quando uma nova biblioteca é criada.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Para obter instruções sobre como conectar seu [!DNL Adobe Creative Cloud] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]</td>
      <td>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Assista às bibliotecas atualizadas]

Esse módulo de acionador inicia um cenário quando uma biblioteca existente é atualizada.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Para obter instruções sobre como conectar seu [!DNL Adobe Creative Cloud] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]</td>
      <td>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</td>
    </tr>
  </tbody>
</table>

### Outro

#### [!UICONTROL Faça uma chamada de API]

Esse módulo faz uma chamada de API personalizada para o [!DNL Adobe Creative Cloud Libraries] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Para obter instruções sobre como conectar sua conta do Adobe Creative Cloud ao Workfront Fusion, consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crie uma conexão com o Adobe Workfront Fusion - Instruções básicas.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Insira um caminho relativo a <code>https://cc-libraries.adobe.io/api</code>.</p>
    <p>Por exemplo <code>/v1/libraries</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL versão da API]</td>
      <td>
        <p>Selecione a versão do [!DNL Adobe Analytics] API à qual você deseja se conectar.</p>
      </td>
    </tr>    <tr>
      <td role="rowheader">[!UICONTROL Método]</td>
      <td> <p>Selecione o método de solicitação HTTP que você precisa configurar a chamada da API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cabeçalhos]</td>
      <td>
        <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão.</p>
        <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p>
        <p>O Workfront Fusion adiciona os cabeçalhos de autorização para você.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Sequência de consulta]</td>
      <td>
        <p>Adicione a query para a chamada de API no formato de um objeto JSON padrão.</p>
        <p>Por exemplo: <code>{"name":"something-urgent"}</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Corpo]</td>
   <td> <p>Adicione o conteúdo do corpo para a chamada da API no formato de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
       <tr>
      <td role="rowheader">[!UICONTROL Fazer upload de um documento transitório]</td>
      <td>
      <p>Para carregar um documento transitório, insira o arquivo de origem do documento que deseja fazer upload.</p>
      <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p>
    </td>
    </tr>

</tbody>
</table>
