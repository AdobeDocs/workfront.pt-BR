---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos Split.io
description: Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL Split.io], bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: 4576a2e4-b495-430e-a9de-4e1ec7379ab8
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1773'
ht-degree: 0%

---

# [!DNL Split.io] módulos

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL Split.io], bem como conectá-lo a vários aplicativos e serviços de terceiros.

Se precisar de instruções para criar um cenário, consulte [Crie um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obter informações sobre módulos, consulte [Módulos em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Para usar [!DNL Split.io] módulos, você deve ter um [!DNL Split.io] conta.

## Connect [!DNL Split.io] para [!DNL Workfront Fusion] {#connect-split-io-to-workfront-fusion}

Você pode criar uma conexão com o [!DNL Split.io] conta diretamente de dentro de uma [!DNL Split.io] módulo.

1. Em qualquer [!DNL Split.io] módulo, clique em **[!UICONTROL Adicionar]** ao lado do [!UICONTROL Conexão] campo.
1. Digite um nome para a conexão.
1. Insira seu [!DNL Split.io] Chave da API.

   Para obter mais informações sobre [!DNL Split.io] Chaves de API, consulte [Chaves da API](https://help.split.io/hc/en-us/articles/360019916211-API-keys) no [!DNL Split.io] documentação.

1. Clique em **[!UICONTROL Continuar]** para criar a conexão e retornar ao módulo .

## [!DNL Split.io] módulos e seus campos

Ao configurar [!DNL split.io] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL split.io] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Ações](#actions)
* [Pesquisas](#searches)

### Ações

* [[!UICONTROL Chamada da API personalizada]](#custom-api-call)
* [[!UICONTROL Obter Split]](#get-split)
* [[!UICONTROL Obter definição de divisão no ambiente]](#get-split-definition-in-environment)
* [[!UICONTROL Criar divisão]](#create-split)
* [[!UICONTROL Excluir divisão]](#delete-split)
* [[!UICONTROL Criar definição de divisão no ambiente]](#create-split-definition-in-environment)
* [[!UICONTROL Remover definição de divisão do ambiente]](#remove-split-definition-from-environment)
* [[!UICONTROL Atualização parcial Definição dividida no ambiente]](#partial-update-split-definition-in-environment)
* [[!UICONTROL Associar tags]](#associate-tags)

#### [!UICONTROL Chamada da API personalizada]

Esse módulo de ação permite que você faça uma chamada autenticada personalizada para o [!DNL split.io] API. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pela outra [!DNL split.io] módulos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Split.io] para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] para [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Insira um caminho relativo a <code>https://api.split.io/internal/api/v2/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Selecione o método de solicitação HTTP que você precisa configurar a chamada da API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> <p>O Workfront Fusion adiciona os cabeçalhos de autorização para você.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sequência de consulta]</td> 
   <td> <p>Adicione a query para a chamada de API no formato de um objeto JSON padrão.</p> <p>Por exemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada da API no formato de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Insira ou mapeie o número máximo de registros com os quais deseja que o módulo funcione durante cada ciclo de execução de cenário.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter Split]

Esse módulo de ação recupera a divisão.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Split.io] para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] para [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Workspace]</td> 
   <td>Selecione ou mapeie o espaço de trabalho que contém a divisão que deseja recuperar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome dividido]</td> 
   <td> <p>Insira ou mapeie o nome da divisão que deseja recuperar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter definição de divisão no ambiente]

Esse módulo de ação recupera uma definição de divisão específica do ambiente designado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Split.io] para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] para [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Workspace]</td> 
   <td>Selecione ou mapeie o espaço de trabalho que contém a definição de divisão que deseja recuperar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome ou ID do ambiente]</td> 
   <td>Selecione ou mapeie o ambiente que contém a definição de divisão que deseja recuperar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome dividido]</td> 
   <td> <p>Insira ou mapeie o nome da divisão para a qual você deseja recuperar a definição de divisão.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar divisão]

Esse módulo de ação cria uma nova divisão na organização, considerando um tipo de tráfego.

>[!NOTE]
>
>A API não configura a divisão em nenhum ambiente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Split.io] para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] para [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Workspace]</td> 
   <td>Selecione ou mapeie o espaço de trabalho onde deseja criar a divisão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID ou nome do tipo de tráfego]</td> 
   <td>Selecione ou mapeie o tipo de tráfego que deseja usar para criar a divisão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome dividido]</td> 
   <td> <p>Insira ou mapeie um nome para a divisão que deseja criar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dividir descrição]</td> 
   <td>Insira ou mapeie uma descrição da [!UICONTROL dividido] para a divisão que deseja criar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir divisão]

Esse módulo de ação exclui uma divisão da organização. Isso desconfigura automaticamente a definição de divisão de todos os ambientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Split.io] para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] para [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Workspace]</td> 
   <td>Selecione ou mapeie o espaço de trabalho onde deseja excluir a divisão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome dividido]</td> 
   <td> <p>Insira ou mapeie o nome da divisão que deseja excluir.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar definição de divisão no ambiente]

Esse módulo de ação configura uma definição de divisão para um ambiente específico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Split.io] para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] para [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Workspace]</td> 
   <td>Selecione ou mapeie o espaço de trabalho onde deseja criar uma definição de divisão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome ou ID do ambiente]</td> 
   <td>Selecione ou mapeie o ambiente em que deseja criar uma definição de divisão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome dividido]</td> 
   <td> <p>Insira ou mapeie o nome da divisão para a qual deseja criar uma definição.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comentários]</td> 
   <td>Insira ou mapeie quaisquer comentários que deseja adicionar à definição de divisão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Regras]</td> 
   <td> <p>Para cada regra de direcionamento que deseja adicionar à definição, clique em <b>[!UICONTROL Adicionar item]</b>, em seguida, insira ou mapeie a regra.</p> <p>Para obter mais informações sobre regras de direcionamento, consulte <a href="https://docs.split.io/reference#create-split-definition-in-environment">Criar definição de divisão em um ambiente</a> no [!DNL Split.io] documentação.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Regra padrão]</td> 
   <td> <p>Insira ou mapeie a regra que você deseja que a divisão use para o tráfego que não atende às especificações das outras regras.</p> <p>Para obter mais informações sobre regras de direcionamento, consulte <a href="https://docs.split.io/reference#create-split-definition-in-environment">Criar definição de divisão em um ambiente</a> no [!DNL Split.io] documentação.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tratamento padrão]</td> 
   <td> <p>Insira ou mapeie o tratamento que você deseja que a divisão use se a divisão for encerrada ou se o cliente não estiver incluído na alocação de tráfego.</p> <p>Para obter mais informações sobre tratamentos, consulte <a href="https://docs.split.io/reference#create-split-definition-in-environment">Criar definição de divisão em um ambiente</a> no [!DNL Split.io] documentação.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tratamentos]</td> 
   <td> <p>Para cada tratamento que deseja adicionar à definição, clique em <b>[!UICONTROL Adicionar item]</b>, em seguida, insira ou mapeie o tratamento.</p> <p>Para obter mais informações sobre tratamentos, consulte <a href="https://docs.split.io/reference#create-split-definition-in-environment">Criar definição de divisão em um ambiente</a> no [!DNL Split.io] documentação.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remover definição de divisão do ambiente]

Esse módulo de ação desconfigura uma definição de divisão para um ambiente específico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Split.io] para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] para [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Workspace]</td> 
   <td>Selecione ou mapeie o espaço de trabalho onde deseja remover uma definição de divisão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome ou ID do ambiente]</td> 
   <td>Selecione ou mapeie o ambiente onde deseja remover uma definição de divisão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome dividido]</td> 
   <td> <p>Insira ou mapeie o nome da divisão para a qual deseja remover uma definição.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comentários]</td> 
   <td>Insira ou mapeie quaisquer comentários que deseja adicionar à definição de divisão.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualização parcial Definição dividida no ambiente]

Esse módulo de ação atualiza uma definição de divisão para um ambiente específico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Split.io] para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] para [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Workspace]</td> 
   <td>Selecione ou mapeie o espaço de trabalho onde deseja atualizar uma definição de divisão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome ou ID do ambiente]</td> 
   <td>Selecione ou mapeie o ambiente onde deseja atualizar uma definição de divisão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome dividido]</td> 
   <td> <p>Insira ou mapeie o nome da divisão para a qual deseja atualizar uma definição.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Atualizar conteúdo]</td> 
   <td> <p>Para cada atributo da divisão que deseja atualizar, clique em <b>[!UICONTROL Adicionar item]</b> e insira ou mapeie as alterações desejadas.</p> <p>Para obter mais informações, consulte <a href="https://docs.split.io/reference#partial-update-split-definition-in-environment">Atualização parcial Definição dividida no ambiente</a> no [!DNL Split.io] documentação.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comentários]</td> 
   <td>Insira ou mapeie quaisquer comentários que deseja adicionar à definição de divisão.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Associar tags]

Esse módulo de ação adiciona tags ao objeto especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Split.io] para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] para [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Workspace]</td> 
   <td>Selecione ou mapeie o espaço de trabalho onde deseja adicionar uma tag.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do objeto]</td> 
   <td>Insira ou mapeie o nome do objeto ao qual deseja adicionar tags,</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de objeto]</td> 
   <td> <p>Insira ou mapeie o tipo de objeto ao qual deseja adicionar tags.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tags]</td> 
   <td> <p>Para cada tag que deseja adicionar, clique em <b>[!UICONTROL Adicionar item]</b> e insira ou mapeie a tag .</p> </td> 
  </tr> 
 </tbody> 
</table>

### Pesquisas

* [[!UICONTROL Obter espaços de trabalho]](#get-workspaces)
* [[!UICONTROL Obter ambientes]](#get-environments)
* [[!UICONTROL Obter Divisões]](#get-splits)
* [[!UICONTROL Listar definições divididas em um ambiente]](#list-split-definitions-in-an-environment)
* [[!UICONTROL Obter tipos de tráfego]](#get-traffic-types)

#### [!UICONTROL Obter espaços de trabalho]

Esse módulo de pesquisa recupera os espaços de trabalho de uma organização.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Split.io] para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] para [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Insira ou mapeie o número máximo de espaços de trabalho que você deseja que o módulo recupere durante cada ciclo de execução de cenário.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter ambientes]

Esse módulo de pesquisa recupera uma lista de ambientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Split.io] para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] para [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Workspace]</td> 
   <td>Selecione ou mapeie o espaço de trabalho que contém os ambientes que deseja listar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter Divisões]

Esse módulo de pesquisa recupera uma lista de divisões.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Split.io] para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] para [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Workspace]</td> 
   <td>Selecione ou mapeie o espaço de trabalho que contém as divisões que deseja listar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Insira ou mapeie o número máximo de divisões que você deseja que o módulo recupere durante cada ciclo de execução de cenário.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listar definições divididas em um ambiente]

Esse módulo de pesquisa recupera uma lista de definições divididas em um determinado ambiente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Split.io] para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] para [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Workspace]</td> 
   <td>Selecione ou mapeie o espaço de trabalho que contém as definições de divisão que deseja listar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome ou ID do ambiente]</td> 
   <td>Selecione ou mapeie o ambiente que contém as definições de divisão que deseja listar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Insira ou mapeie o número máximo de definições de divisão que você deseja que o módulo recupere durante cada ciclo de execução de cenário.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter tipos de tráfego]

Este módulo de pesquisa recupera uma lista de tipos de tráfego.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Split.io] para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] para [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Workspace]</td> 
   <td>Selecione ou mapeie o espaço de trabalho que contém os tipos de tráfego que deseja listar.</td> 
  </tr> 
 </tbody> 
</table>
