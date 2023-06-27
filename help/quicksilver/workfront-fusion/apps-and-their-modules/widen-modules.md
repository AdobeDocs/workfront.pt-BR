---
title: Ampliar módulos
description: Em um [!DNL Adobe Workfront Fusion] cenário, é possível automatizar workflows que usam [!UICONTROL Ampliar], bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: d46935bc-4f6c-4502-bd2f-3927f33241e1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1586'
ht-degree: 1%

---

# [!DNL Widen] módulos

Em um [!DNL Adobe Workfront Fusion] cenário, é possível automatizar workflows que usam [!UICONTROL Ampliar], bem como conectá-lo a vários aplicativos e serviços de terceiros.

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

Para usar [!UICONTROL Ampliar] módulos, você deve ter uma [!UICONTROL Ampliar] conta.

## Conectar [!DNL Widen] para [!DNL Workfront Fusion] {#connect-widen-to-workfront-fusion}

Você pode criar uma conexão com o seu [!DNL Widen] conta diretamente de dentro de um [!DNL Widen] módulo.

1. Em qualquer [!DNL Widen] , clique em **[!UICONTROL Adicionar]** ao lado da [!UICONTROL Conexão] campo.
1. Selecione o [!DNL Widen] domínio ao qual você deseja se conectar.
1. Insira o token do [!DNL Widen] conta. Para obter instruções sobre como localizar esse token, consulte [[!DNL Widen] Perguntas frequentes sobre API](https://community.widen.com/collective/s/article/API-FAQs).
1. Clique em **[!UICONTROL Continuar]** para criar a conexão e voltar ao módulo.

## [!DNL Widen] módulos e seus campos

Ao configurar [!DNL Widen] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Widen] Os campos podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Módulos de acionamento](#trigger-modules)
* [Módulos de ação](#action-modules)
* [Pesquisar módulos](#search-modules)

### Módulos de acionamento

#### [!UICONTROL Observar ativos]

Esse módulo de acionamento inicia um cenário quando um ativo é criado ou atualizado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
  <td> <p>Para obter instruções sobre como conectar seu [!DNL Widen] conta para [!DNL Workfront Fusion], consulte <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Widen] para [!DNL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de evento]</td> 
   <td> <p>Selecione se você deseja observar novos ativos ou ativos atualizados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expandir]</td> 
   <td> <p>Selecione as propriedades que deseja incluir na saída do módulo, além dos campos de ativo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td>Selecione os campos que deseja incluir na saída do módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de ativos com os quais você deseja que o módulo funcione durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Módulos de ação

* [[!UICONTROL Chamada de API personalizada]](#custom-api-call)
* [[!UICONTROL Ler informações do ativo]](#read-asset-info)
* [[!UICONTROL Adicionar ativos a coleções]](#add-assets-to-collections)
* [[!UICONTROL Remover ativos da coleção]](#remove-assets-from-collection)
* [[!UICONTROL Atualizar metadados de ativos]](#update-asset-metadata)
* [[!UICONTROL Baixar arquivo]](#download-file)
* [[!UICONTROL Carregar] um arquivo](#upload-a-file)

#### [!UICONTROL Chamada de API personalizada]

Esse módulo de ação permite fazer uma chamada autenticada personalizada para o [!DNL Widen] API. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pelo outro [!DNL Widen] módulos.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Widen] conta para [!DNL Workfront Fusion], consulte <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Widen] para [!DNL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Versão da API]</td> 
   <td>Selecione se deseja usar a versão mais recente do [!DNL Widen] API ou versão 1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Insira ou mapeie o URL da sua chamada de API.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formulário de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> <p>O [!UICONTROL Workfront Fusion] adiciona os cabeçalhos de autorização para você.</p> </td> 
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

#### [!UICONTROL Ler informações do ativo]

Este módulo de ação recupera um ativo individual por sua ID exclusiva.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
  <td> <p>Para obter instruções sobre como conectar seu [!DNL Widen] conta para [!DNL Workfront Fusion], consulte <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Widen] para [!DNL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Ativo]</td> 
   <td> <p>Insira ou mapeie a ID do ativo cujas informações você deseja ler.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expandir]</td> 
   <td> <p>Selecione as propriedades que deseja incluir na saída do módulo, além dos campos de ativo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td>Selecione os campos que deseja incluir na saída do módulo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Adicionar ativos a coleções]

Este módulo de ação adiciona um ou mais ativos às coleções.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
  <td> <p>Para obter instruções sobre como conectar seu [!DNL Widen] conta para [!DNL Workfront Fusion], consulte <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Widen] para [!DNL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Coleções]</td> 
   <td> <p>Para cada coleção à qual você deseja adicionar os ativos:</p> 
    <ol> 
     <li value="1"> <p> Clique em <strong>[!UICONTROL Adicionar]</strong>.</p> </li> 
     <li value="2"> <p>Insira ou mapeie a [!UICONTROL Collection ID].</p> </li> 
     <li value="3"> <p>Clique em <strong>[!UICONTROL Adicionar item]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Ativos]</td> 
   <td> <p>Para cada ativo que você deseja adicionar a uma coleção:</p> 
    <ol> 
     <li value="1"> <p> Clique em <strong>[!UICONTROL Adicionar]</strong>.</p> </li> 
     <li value="2"> <p>Insira ou mapeie a ID do ativo.</p> </li> 
     <li value="3"> <p>Clique em <strong>[!UICONTROL Adicionar item]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de ativos com os quais você deseja que o módulo funcione durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remover ativos da coleção]

Este módulo de ação remove um ou mais ativos das coleções.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
  <td> <p>Para obter instruções sobre como conectar seu [!DNL Widen] conta para [!DNL Workfront Fusion], consulte <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Widen] para [!DNL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Coleções]</td> 
   <td> <p>Para cada coleção da qual você deseja remover os ativos:</p> 
    <ol> 
     <li value="1"> <p> Clique em <strong>[!UICONTROL Adicionar]</strong>.</p> </li> 
     <li value="2"> <p>Insira ou mapeie a ID da coleção.</p> </li> 
     <li value="3"> <p>Clique em <strong>[!UICONTROL Adicionar item]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID de ativos</td> 
   <td> <p>Para cada ativo que você deseja remover de uma coleção:</p> 
    <ol> 
     <li value="1"> <p> Clique em <strong>[!UICONTROL Adicionar]</strong>.</p> </li> 
     <li value="2"> <p>Insira ou mapeie a ID do ativo.</p> </li> 
     <li value="3"> <p>Clique em <strong>[!UICONTROL Adicionar item]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de ativos com os quais você deseja que o módulo funcione durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar metadados de ativos]

Esse módulo de ação atualiza os campos de metadados de um ativo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
  <td> <p>Para obter instruções sobre como conectar seu [!DNL Widen] conta para [!DNL Workfront Fusion], consulte <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Widen] para [!DNL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Ativo]</td> 
   <td> <p>Insira ou mapeie a ID do ativo no qual deseja atualizar os metadados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de metadados]</td> 
   <td> <p>Selecione o tipo de metadados para os metadados que deseja atualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadados]</td> 
   <td>Selecione os campos de metadados que deseja atualizar. Para cada campo, insira o novo valor do campo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de ativos com os quais você deseja que o módulo funcione durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Baixar arquivo]

Esse módulo de ação baixa um ativo do [!DNL Widen] conta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
  <td> <p>Para obter instruções sobre como conectar seu [!DNL Widen] conta para [!DNL Workfront Fusion], consulte <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Widen] para [!DNL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Ativo]</td> 
   <td> <p>Insira ou mapeie a ID do ativo que deseja baixar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Carregar um arquivo]

Esse módulo de ação carrega um arquivo no [!DNL Widen] conta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
  <td> <p>Para obter instruções sobre como conectar seu [!DNL Widen] conta para [!DNL Workfront Fusion], consulte <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Widen] para [!DNL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carregar Perfil]</td> 
   <td> <p>Selecione o perfil de upload que deseja que o módulo use.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método de Carregamento]</td> 
   <td> <p>Selecione como deseja fazer upload do arquivo.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Do Arquivo]</strong> </p> <p>Selecione ou mapeie o arquivo de origem de um módulo anterior.</p> </li> 
     <li> <p><strong>[!UICONTROL Por URL]</strong> </p> <p>Insira ou mapeie o URL do arquivo que você deseja fazer upload.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do arquivo]</td> 
   <td>Insira ou mapeie um nome para o arquivo carregado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Metadados]</td> 
   <td>Selecione o tipo de metadados para o arquivo que você deseja fazer upload.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadados]</td> 
   <td>Selecione os campos de metadados que deseja incluir no upload do arquivo. Para cada campo, insira o [!UICONTROL value] para o campo.</td> 
  </tr> 
 </tbody> 
</table>

### Pesquisar módulos

* [[!UICONTROL Ler ativos da coleção]](#read-collection-assets)
* [[!UICONTROL Pesquisar ativos]](#search-assets)

#### [!UICONTROL Ler ativos da coleção]

Este módulo de ação recupera uma lista de ativos em uma coleção.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
  <td> <p>Para obter instruções sobre como conectar seu [!DNL Widen] conta para [!DNL Workfront Fusion], consulte <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Widen] para [!DNL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Coleção]</td> 
   <td> <p>Insira ou mapeie a ID da coleção que contém os ativos que você deseja ler.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Iniciar]</td> 
   <td>Informe ou mapeie o número do primeiro item que deseja listar. Essa é uma maneira de paginar os registros.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Máx.]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Classificar por]</td> 
   <td> <p>Selecione a propriedade pela qual deseja classificar os ativos. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordem]</td> 
   <td>Selecione se deseja classificar ativos em ordem crescente ou decrescente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td>Selecione os campos que deseja incluir na saída do módulo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Pesquisar ativos]

Este módulo de pesquisa recupera uma lista de ativos que correspondem aos critérios de pesquisa específicos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
  <td> <p>Para obter instruções sobre como conectar seu [!DNL Widen] conta para [!DNL Workfront Fusion], consulte <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Widen] para [!DNL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pesquisar consulta]</td> 
   <td> <p>Informe os critérios pelos quais deseja pesquisar ativos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Classificar por]</td> 
   <td> <p>Selecione como deseja classificar os ativos. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordem]</td> 
   <td>Selecione se deseja classificar ativos em ordem crescente ou decrescente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Incluir excluído]</td> 
   <td>Habilite essa opção para incluir ativos excluídos na pesquisa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Incluir arquivado]</p> </td> 
   <td> <p>Ative essa opção para incluir ativos arquivados na pesquisa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pesquisar texto do documento]</td> 
   <td>Habilite esta opção para incluir o texto do documento na pesquisa, ou falso para incluir apenas ativos para os quais o título corresponde aos critérios de pesquisa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Deslocamento]</td> 
   <td>Informe ou mapeie o número do primeiro item para o qual deseja recuperar detalhes. Essa é uma maneira de paginar os registros.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rolagem]</td> 
   <td>Ative essa opção para permitir a rolagem.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expandir]</td> 
   <td> <p>Selecione as propriedades que deseja incluir na saída do módulo, além dos campos de ativo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td>Selecione os campos que deseja incluir na saída do módulo.</td> 
  </tr> 
 </tbody> 
</table>
