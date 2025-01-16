---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Split.io
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: 4576a2e4-b495-430e-a9de-4e1ec7379ab8
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1872'
ht-degree: 0%

---

# [!DNL Split.io] módulos

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Módulos Split.io](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/split-io-modules.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

Em um cenário [!DNL Adobe Workfront Fusion], você pode automatizar fluxos de trabalho que usam [!DNL Split.io], bem como conectá-los a vários aplicativos e serviços de terceiros.

Se você precisar de instruções sobre como criar um cenário, consulte [Criar um cenário [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

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

Para usar módulos [!DNL Split.io], você deve ter uma conta [!DNL Split.io].

## Informações da API Split.io

O conector Split.io usa o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL base</td> 
   <td> https://api.split.io/internal/api</td>
   </tr> 
  <tr> 
   <td role="rowheader">Versão da API</td> 
   <td> v2 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tag da API</td> 
   <td>v1.34.1</td> 
  </tr>
 </tbody> 
 </table>

## Conectar [!DNL Split.io] a [!DNL Workfront Fusion] {#connect-split-io-to-workfront-fusion}

Você pode criar uma conexão com sua conta do [!DNL Split.io] diretamente de dentro de um módulo do [!DNL Split.io].

1. Em qualquer módulo [!DNL Split.io], clique em **[!UICONTROL Adicionar]** ao lado do campo [!UICONTROL Conexão].
1. Insira um nome para a conexão.
1. Insira sua chave de API [!DNL Split.io].

   Para obter mais informações sobre [!DNL Split.io] chaves de API, consulte [chaves de API](https://help.split.io/hc/en-us/articles/360019916211-API-keys) na documentação [!DNL Split.io].

1. Clique em **[!UICONTROL Continuar]** para criar a conexão e voltar para o módulo.

## [!DNL Split.io] módulos e seus campos

Ao configurar módulos do [!DNL split.io], o [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos [!DNL split.io] adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Ações](#actions)
* [Pesquisas](#searches)

### Ações

* [[!UICONTROL Chamada de API personalizada]](#custom-api-call)
* [[!UICONTROL Obter Divisão]](#get-split)
* [[!UICONTROL Obter Definição de Divisão no Ambiente]](#get-split-definition-in-environment)
* [[!UICONTROL Criar Divisão]](#create-split)
* [[!UICONTROL Excluir Divisão]](#delete-split)
* [[!UICONTROL Criar Definição de Divisão no Ambiente]](#create-split-definition-in-environment)
* [[!UICONTROL Remover definição dividida do ambiente]](#remove-split-definition-from-environment)
* [[!UICONTROL Definição de Divisão de Atualização Parcial no Ambiente]](#partial-update-split-definition-in-environment)
* [[!UICONTROL Marcas Associadas]](#associate-tags)

#### [!UICONTROL Chamada de API personalizada]

Este módulo de ação permite fazer uma chamada autenticada personalizada para a API [!DNL split.io]. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pelos outros módulos do [!DNL split.io].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Split.io] ao [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Split.io] ao [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Insira um caminho relativo para <code>https://api.split.io/internal/api/v2/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formulário de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> <p>O Workfront Fusion adiciona os cabeçalhos de autorização para você.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadeia de Consulta]</td> 
   <td> <p>Adicione a consulta da chamada à API na forma de um objeto JSON padrão.</p> <p>Por exemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada à API na forma de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar instruções condicionais como <code>if</code> em seu JSON, coloque as aspas fora da instrução condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Insira ou mapeie o número máximo de registros com os quais você deseja que o módulo funcione durante cada ciclo de execução de cenário.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter Divisão]

Este módulo de ação recupera a divisão.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Split.io] ao [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Split.io] ao [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selecione ou mapeie o espaço de trabalho que contém a divisão que você deseja recuperar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dividir Nome]</td> 
   <td> <p>Insira ou mapeie o nome da divisão que deseja recuperar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter Definição de Divisão no Ambiente]

Esse módulo de ação recupera uma definição de divisão específica do ambiente designado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Split.io] ao [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Split.io] ao [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selecione ou mapeie o espaço de trabalho que contém a definição de divisão que deseja recuperar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome ou ID de Ambiente]</td> 
   <td>Selecione ou mapeie o ambiente que contém a definição de divisão que deseja recuperar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dividir Nome]</td> 
   <td> <p>Insira ou mapeie o nome da divisão para a qual deseja recuperar a definição de divisão.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar Divisão]

Esse módulo de ação cria uma nova divisão em sua organização, considerando um tipo de tráfego.

>[!NOTE]
>
>A API não configura a divisão em nenhum ambiente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Split.io] ao [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Split.io] ao [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selecione ou mapeie o espaço de trabalho em que deseja criar a divisão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificação ou Nome de Tipo de Tráfego]</td> 
   <td>Selecione ou mapeie o tipo de tráfego que deseja usar para criar a divisão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dividir Nome]</td> 
   <td> <p>Insira ou mapeie um nome para a divisão que deseja criar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dividir Descrição]</td> 
   <td>Insira ou mapeie uma descrição de [!UICONTROL divisão] para a divisão que você deseja criar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir Divisão]

Esse módulo de ação exclui uma divisão da sua organização. Essa ação desconfigura automaticamente a definição de divisão de todos os ambientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Split.io] ao [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Split.io] ao [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selecione ou mapeie o espaço de trabalho no qual deseja excluir a divisão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dividir Nome]</td> 
   <td> <p>Insira ou mapeie o nome da divisão que deseja excluir.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar Definição de Divisão no Ambiente]

Este módulo de ação configura uma definição de divisão para um ambiente específico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Split.io] ao [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Split.io] ao [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selecione ou mapeie o espaço de trabalho em que deseja criar uma definição de divisão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome ou ID de Ambiente]</td> 
   <td>Selecione ou mapeie o ambiente em que deseja criar uma definição de divisão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dividir Nome]</td> 
   <td> <p>Insira ou mapeie o nome da divisão para a qual deseja criar uma definição.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comentários]</td> 
   <td>Insira ou mapeie comentários que deseja adicionar à definição de divisão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Regras]</td> 
   <td> <p>Para cada regra de direcionamento que você deseja adicionar à definição, clique em <b>[!UICONTROL Adicionar item]</b> e, em seguida, insira ou mapeie a regra.</p> <p>Para obter mais informações sobre regras de direcionamento, consulte <a href="https://docs.split.io/reference#create-split-definition-in-environment">Criar definição de divisão em um ambiente</a> na documentação [!DNL Split.io].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Regra padrão]</td> 
   <td> <p>Insira ou mapeie a regra que você deseja que a divisão use para o tráfego que não atende às especificações das outras regras.</p> <p>Para obter mais informações sobre regras de direcionamento, consulte <a href="https://docs.split.io/reference#create-split-definition-in-environment">Criar definição de divisão em um ambiente</a> na documentação [!DNL Split.io].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tratamento padrão]</td> 
   <td> <p>Insira ou mapeie o tratamento que deseja que a divisão use se a divisão for eliminada ou se o cliente não for incluído na alocação de tráfego.</p> <p>Para obter mais informações sobre tratamentos, consulte <a href="https://docs.split.io/reference#create-split-definition-in-environment">Criar definição de divisão em um ambiente</a> na documentação [!DNL Split.io].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tratamentos]</td> 
   <td> <p>Para cada tratamento que você deseja adicionar à definição, clique em <b>[!UICONTROL Adicionar item]</b> e, em seguida, insira ou mapeie o tratamento.</p> <p>Para obter mais informações sobre tratamentos, consulte <a href="https://docs.split.io/reference#create-split-definition-in-environment">Criar definição de divisão em um ambiente</a> na documentação [!DNL Split.io].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remover definição dividida do ambiente]

Este módulo de ação desconfigura uma definição de divisão para um ambiente específico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Split.io] ao [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Split.io] ao [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selecione ou mapeie o espaço de trabalho para o qual deseja remover uma definição de divisão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome ou ID de Ambiente]</td> 
   <td>Selecione ou mapeie o ambiente no qual deseja remover uma definição de divisão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dividir Nome]</td> 
   <td> <p>Insira ou mapeie o nome da divisão para a qual deseja remover uma definição.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comentários]</td> 
   <td>Insira ou mapeie comentários que deseja adicionar à definição de divisão.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Definição de Divisão de Atualização Parcial no Ambiente]

Este módulo de ação atualiza uma definição de divisão para um ambiente específico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Split.io] ao [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Split.io] ao [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selecione ou mapeie o espaço de trabalho no qual deseja atualizar uma definição de divisão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome ou ID de Ambiente]</td> 
   <td>Selecione ou mapeie o ambiente em que deseja atualizar uma definição de divisão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dividir Nome]</td> 
   <td> <p>Insira ou mapeie o nome da divisão para a qual deseja atualizar uma definição.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Atualizar conteúdo]</td> 
   <td> <p>Para cada atributo da divisão que você deseja atualizar, clique em <b>[!UICONTROL Adicionar item]</b> e insira ou mapeie as alterações desejadas.</p> <p>Para obter mais informações, consulte <a href="https://docs.split.io/reference#partial-update-split-definition-in-environment">Definição de Divisão de Atualização Parcial em Ambiente</a> na documentação [!DNL Split.io].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comentários]</td> 
   <td>Insira ou mapeie comentários que deseja adicionar à definição de divisão.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Marcas Associadas]

Esse módulo de ação adiciona tags ao objeto especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Split.io] ao [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Split.io] ao [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selecione ou mapeie o espaço de trabalho ao qual deseja adicionar uma tag.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do Objeto]</td> 
   <td>Insira ou mapeie o nome do objeto ao qual você deseja adicionar tags,</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Objeto]</td> 
   <td> <p>Insira ou mapeie o tipo de objeto ao qual você deseja adicionar tags.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Marcas]</td> 
   <td> <p>Para cada marca que você deseja adicionar, clique em <b>[!UICONTROL Adicionar item]</b> e insira ou mapeie a marca.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Pesquisas

* [[!UICONTROL Obter Espaços de Trabalho]](#get-workspaces)
* [[!UICONTROL Obter ambientes]](#get-environments)
* [[!UICONTROL Obter Divisões]](#get-splits)
* [[!UICONTROL Listar definições divididas em um ambiente]](#list-split-definitions-in-an-environment)
* [[!UICONTROL Obter Tipos de Tráfego]](#get-traffic-types)

#### [!UICONTROL Obter Espaços de Trabalho]

Este módulo de pesquisa recupera os espaços de trabalho de uma organização.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Split.io] ao [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Split.io] ao [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Insira ou mapeie o número máximo de espaços de trabalho que você deseja que o módulo recupere durante cada ciclo de execução de cenário.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter ambientes]

Este módulo de pesquisa recupera uma lista de ambientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Split.io] ao [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Split.io] ao [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selecione ou mapeie o espaço de trabalho que contém os ambientes que deseja listar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter Divisões]

Este módulo de pesquisa recupera uma lista de divisões.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Split.io] ao [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Split.io] ao [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selecione ou mapeie o espaço de trabalho que contém as divisões que deseja listar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Insira ou mapeie o número máximo de divisões que você deseja que o módulo recupere durante cada ciclo de execução do cenário.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listar definições divididas em um ambiente]

Este módulo de pesquisa recupera uma lista de definições de divisão em um determinado ambiente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Split.io] ao [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Split.io] ao [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selecione ou mapeie o espaço de trabalho que contém as definições de divisão que deseja listar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome ou ID de Ambiente]</td> 
   <td>Selecione ou mapeie o ambiente que contém as definições de divisão que deseja listar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Insira ou mapeie o número máximo de definições de divisão que você deseja que o módulo recupere durante cada ciclo de execução de cenário.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter Tipos de Tráfego]

Este módulo de pesquisa recupera uma lista de tipos de tráfego.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Split.io] ao [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Split.io] ao [!UICONTROL Workfront Fusion] </a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selecione ou mapeie o espaço de trabalho que contém os tipos de tráfego que deseja listar.</td> 
  </tr> 
 </tbody> 
</table>
