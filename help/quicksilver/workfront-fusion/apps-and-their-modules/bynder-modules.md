---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Bynder
description: Em um [!DNL Adobe Workfront Fusion] cenário, é possível automatizar workflows que usam [!DNL Bynder], bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: e4dc9588-334a-41a3-85d1-996cb819c3fa
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1664'
ht-degree: 0%

---

# [!DNL Bynder] módulos

Em um [!DNL Adobe Workfront Fusion] cenário, é possível automatizar workflows que usam [!DNL Bynder], bem como conectá-lo a vários aplicativos e serviços de terceiros.

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

Para usar [!DNL Bynder] módulos, você deve ter uma [!DNL Bynder] conta.

## Conectar [!DNL Bynder] para o Workfront Fusion  {#connect-bynder-to-workfront-fusion}

* [Criar uma conexão com o [!DNL Bynder] de [!DNL Workfront Fusion]](#create-a-connection-to-bynder-from-workfront-fusion)
* [Gerar um [!UICONTROL ID do cliente] e [!UICONTROL Segredo do cliente] in [!DNL Bynder] (Opcional)](#generate-a-client-id-and-client-secret-in-bynder-optional)

### Criar uma conexão com o [!DNL Bynder] de [!DNL Workfront Fusion]

Você pode criar uma conexão de [!DNL Workfront Fusion] ao seu [!DNL Bynder] conta diretamente de dentro de um [!DNL Bynder] módulo.

1. Em qualquer [!DNL Bynder] , clique em **[!UICONTROL Adicionar]** ao lado da [!UICONTROL Conexão] campo.
1. Selecione o [!DNL Bynder] domínio ao qual você deseja se conectar.
1. (Opcional) Clique em **[!UICONTROL Configurações avançadas]**, em seguida, insira seu [!UICONTROL ID do cliente] e [!UICONTROL Segredo do cliente].

   Para obter instruções sobre como gerar a ID do cliente e o Segredo do cliente, consulte [Gerar uma ID do cliente e um segredo do cliente no [!DNL Bynder] (Opcional)](#generate-a-client-id-and-client-secret-in-bynder-optional) neste artigo.

1. No [!UICONTROL fazer logon] digite seu nome de usuário (endereço de email) e senha.
1. Clique em **[!UICONTROL Continuar]** para criar a conexão e voltar ao módulo.

### Gerar um [!UICONTROL ID do cliente] e [!UICONTROL Segredo do cliente] in [!DNL Bynder] (Opcional)

Se quiser criar uma conexão usando a ID do cliente e o Segredo do cliente, você pode gerá-los a partir da [!DNL Bynder] conta. A ID do cliente e o Segredo do cliente são gerados quando você cria um aplicativo no [!DNL Bynder].

Para obter instruções sobre como criar um aplicativo no [!DNL Bynder], consulte [Aplicativos Oauth 2.0](https://developer-docs.bynder.com/api/authentication-oauth2-oauth-apps/) no [!DNL Bynder] documentação.

>[!NOTE]
>
>Ao criar o aplicativo no [!DNL Bynder], insira o seguinte como o `redirect uri`:
>
>`https://app.workfrontfusion.com/oauth/cb/workfront-bynder`

## [!DNL Bynder] módulos e seus campos

Ao configurar [!DNL Bynder] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Bynder] Os campos podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Ações](#actions)
* [Pesquisas](#searches)
* [Triggers](#triggers)

### Ações

* [[!UICONTROL Chamada de API personalizada]](#custom-api-call)
* [[!UICONTROL Ler metadados de ativos]](#read-asset-metadata)
* [[!UICONTROL Atualizar metadados de ativos]](#update-asset-metadata)
* [[!UICONTROL Adicionar ativos a uma coleção]](#add-assets-to-a-collection)
* [[!UICONTROL Remover ativos da coleção]](#remove-assets-from-collection)
* [[!UICONTROL Adicionar uma tag aos ativos]](#add-a-tag-to-assets)
* [[!UICONTROL Remover uma tag] dos ativos](#remove-a-tag-from-assets)
* [[!UICONTROL Baixar ativo]](#download-asset)
* [[!UICONTROL Fazer upload de ativo]](#upload-asset)

#### [!UICONTROL Chamada de API personalizada]

Esse módulo de ação permite fazer uma chamada autenticada personalizada para o [!DNL Bynder] API. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pelo outro [!DNL Bynder] módulos.

Ao configurar esse módulo, os campos a seguir são exibidos.

O módulo retorna um código de status, juntamente com os cabeçalhos e o corpo da chamada de API.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Bynder] conta para [!DNL Workfront Fusion], consulte <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Bynder] para [!DNL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>Insira um caminho relativo a <code>https://{your-bynder-domain}/api/{api-version}/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   td&gt; <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formulário de um objeto JSON padrão.</p> <p>Por exemplo: <code>{"Content-type":"application/json"}</code></p> <p>O Workfront Fusion adiciona os cabeçalhos de autorização para você.</p> </td> 
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

#### [!UICONTROL Ler metadados de ativos]

Esse módulo de ação lê os metadados de um ativo.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Bynder] conta para [!DNL Workfront Fusion], consulte <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Bynder] para [!DNL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Ativo]</td> 
   <td>Insira ou mapeie a ID do ativo para o qual deseja recuperar metadados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td> <p>Selecione as informações que deseja incluir no pacote de saída deste módulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar metadados de ativos]

Esse módulo de ação atualiza os metadados de um ativo existente.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Bynder] conta para [!DNL Workfront Fusion], consulte <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Bynder] para [!DNL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Ativo]</td> 
   <td>Insira ou mapeie a ID do ativo para o qual deseja atualizar os metadados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos]</td> 
   <td> <p>Selecione os campos para os quais deseja inserir informações e, em seguida, insira ou mapeie as informações com as quais deseja atualizar os metadados nesses campos. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Metapropriedades]</p> </td> 
   <td>Selecione as opções que deseja atualizar e, em seguida, insira ou mapeie as informações nessas propriedades. As metapropriedades são informações sobre o ativo que não representam campos específicos no ativo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Adicionar ativos a uma coleção]

Este módulo de ação adiciona um ou mais ativos a uma coleção.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Bynder] conta para [!DNL Workfront Fusion], consulte <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Bynder] para [!DNL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Coleção]</td> 
   <td> <p>Insira ou mapeie a ID da coleção onde deseja adicionar ativos.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL IDs de Ativo]</td> 
   <td> <p>Para cada ativo que deseja adicionar à coleção, clique em <strong>[!UICONTROL Adicionar item]</strong>e, em seguida, insira ou mapeie a ID do ativo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remover ativos da coleção]

Este módulo de ação remove um ou mais ativos de uma coleção.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Bynder] conta para [!DNL Workfront Fusion], consulte <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Bynder] para [!DNL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Coleção]</td> 
   <td> <p>Insira ou mapeie a ID da coleção onde deseja remover os ativos.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL IDs de Ativo]</td> 
   <td> <p>Para cada ativo que deseja remover da coleção, clique em <strong>[!UICONTROL Adicionar item]</strong>e, em seguida, insira ou mapeie a ID do ativo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Adicionar uma tag aos ativos]

Adicionar uma tag a um ou mais ativos

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Bynder] conta para [!DNL Workfront Fusion], consulte <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Bynder] para [!DNL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Marca]</td> 
   <td> <p>Insira ou mapeie a ID da tag que você deseja adicionar aos ativos.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL IDs de Ativo]</td> 
   <td> <p>Para cada ativo que deseja marcar, clique em <strong>[!UICONTROL Adicionar item]</strong>e, em seguida, insira ou mapeie a ID do ativo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remover uma tag dos ativos]

Remover uma tag de um ou mais ativos

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Bynder] conta para [!DNL Workfront Fusion], consulte <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Bynder] para [!DNL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Marca]</td> 
   <td> <p>Insira ou mapeie a ID da tag que você deseja remover dos ativos.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL IDs de Ativo]</td> 
   <td> <p>Para cada ativo do qual você deseja remover uma tag, clique em <strong>[!UICONTROL Adicionar item]</strong>e, em seguida, insira ou mapeie a ID do ativo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Baixar ativo]

Este módulo de ação baixa um único ativo.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Bynder] conta para [!DNL Workfront Fusion], consulte <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Bynder] para [!DNL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Ativo]</td> 
   <td>Insira ou mapeie a ID do ativo que deseja baixar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Versão do ativo]</td> 
   <td> <p>Insira ou mapeie a versão do ativo que deseja baixar. Para baixar a versão mais recente do ativo, deixe o campo vazio.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Fazer upload de ativo]

Esse módulo de ação carrega um único ativo.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Bynder] conta para [!DNL Workfront Fusion], consulte <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Bynder] para [!DNL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salvar como]</td> 
   <td> <p>Selecione como deseja salvar o arquivo que você está fazendo upload.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Novo ativo]</strong> </p> <p>Selecione os campos e metapropriedades para os quais você deseja inserir informações e insira as informações nesses campos.</p> <p>Insira ou mapeie a ID da marca que você deseja usar para o ativo carregado.</p> </li> 
     <li> <p><strong>[!UICONTROL Nova versão de ativo]</strong> </p> <p>Insira a ID do ativo para o qual você está fazendo upload de uma nova versão.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</td> 
  </tr> 
 </tbody> 
</table>

### Pesquisas

* [[!UICONTROL Listar registro]](#list-record)
* [[!UICONTROL Pesquisar por ativos]](#search-for-assets)

#### [!UICONTROL Listar registro]

Este módulo de pesquisa recupera todos os itens de um tipo específico.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Bynder] conta para [!DNL Workfront Fusion], consulte <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Bynder] para [!DNL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Registro]</td> 
   <td> <p>Selecione o tipo de registro que deseja listar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Ler todas as coleções]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Ler informações sobre todas as marcas]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Ler todos os ativos de uma coleção]</strong> </p> <p>Insira ou mapeie a ID da coleção da qual você deseja listar ativos.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td> <p>Selecione os campos que deseja incluir na saída do módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de ativos que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Pesquisar por ativos]

Este módulo de pesquisa procura por ativos com base nos critérios que você forneceu.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Bynder] conta para [!DNL Workfront Fusion], consulte <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Bynder] para [!DNL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Critério]</td> 
   <td> <p>Informe os critérios de pesquisa. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Campo]</strong> </p> <p>Selecione o campo que deseja usar na pesquisa</p> </li> 
     <li> <p><strong>[!UICONTROL Operador Lógico]</strong> </p> <p>Selecione o operador que deseja usar na pesquisa.</p> </li> 
     <li> <p><strong>[!UICONTROL Valor]</strong> </p> <p>Insira ou mapeie o valor a ser procurado no campo selecionado. O tipo de valor deve ser igual ao tipo de dados do campo selecionado. </p> <p>Para obter mais informações sobre tipos de dados, consulte <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Tipos de dados de item no [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conjunto de resultados]</td> 
   <td>Selecione se deseja retornar o primeiro ativo correspondente ou todos os ativos correspondentes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Classificar por]</td> 
   <td> <p>Selecione o campo pelo qual deseja classificar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Direção de Classificação]</td> 
   <td> <p>Selecione se deseja classificar em ordem crescente ou decrescente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td> <p>Selecione os campos que deseja incluir na saída do módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de ativos que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Triggers

#### [!UICONTROL Observar ativos]

Esse módulo de acionamento inicia um cenário quando um ativo é criado ou atualizado.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Bynder] conta para [!DNL Workfront Fusion], consulte <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Bynder] para [!DNL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Event type</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select whether you want to start the scenario when a new asset is created or when an existing asset is updated.</td>
   --> 
  </tr> 
  <tr>
     <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Coleções]</td>
   <td> <p>Selecione a coleção que você deseja observar para novos ativos. Para observar todas as coleções, deixe este campo vazio.</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Outputs</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the fields that you want to include in the output.</td>
   --> 
  </tr> 
  <tr> 
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Limite]</td>

<td> <p>Insira o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>
