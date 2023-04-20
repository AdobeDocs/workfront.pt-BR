---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos Allocadia
description: Em um [!DNL Adobe Workfront Fusion] você pode automatizar fluxos de trabalho que usam o Allocadia, bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: f1edefd1-9fe0-48fc-bea2-c3f9facf7363
source-git-commit: c88b00a086a9e1c5e44d481dde94f4244c7c959d
workflow-type: tm+mt
source-wordcount: '1353'
ht-degree: 0%

---

# [!DNL Allocadia] módulos

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL Allocadia], bem como conectá-lo a vários aplicativos e serviços de terceiros.

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

Para usar [!DNL Allocadia] , você deve ter um [!DNL Allocadia] conta.

## Connect [!DNL Allocadia] para [!DNL Workfront Fusion]

Você pode criar uma conexão com o [!DNL Allocadia] conta diretamente de dentro de uma [!DNL Allocadia] módulo.

1. Em qualquer [!DNL Allocadia] módulo, clique em **[!UICONTROL Adicionar]** ao lado do [!UICONTROL Conexão] campo.
1. Selecione se deseja usar o servidor da América do Norte ou o servidor da Europa.
1. Insira seu nome de usuário e senha.
1. Clique em **[!UICONTROL Continuar]** para criar a conexão e retornar ao módulo .

## [!DNL Allocadia] módulos e seus campos

Ao configurar [!DNL Allocadia] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Allocadia] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Ações](#actions)
* [Pesquisas](#searches)

### Triggers

#### [!UICONTROL Registro de monitoramento]

Esse módulo de acionador executa um cenário quando objetos de um tipo específico são adicionados, atualizados ou ambos. O módulo retorna todos os campos padrão associados ao registro ou registros, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> <table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowhader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta Allocadia a [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect Allocadia] para Workfront Fusion</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filtro</td> 
   <td> <p>Selecione se deseja que o cenário assista a Novos Registros Somente, [!UICONTROL Registros Atualizados Somente] ou Registros Novos e Atualizados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo de entidade</td> 
   <td>Selecione o tipo de registro Allocadia que você deseja que o módulo assista.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Saídas</td> 
   <td> <p>Selecione os campos que deseja incluir na saída do módulo. Os campos disponíveis dependem do Tipo de entidade selecionado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limite</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo assista durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [Chamada da API personalizada](#custom-api-call)
* [Ler Registro](#read-record)
* [Criar registro](#create-record)
* [Excluir registro](#delete-record)
* [Atualizar registro](#update-record)

#### [!UICONTROL Chamada da API personalizada]

Esse módulo de ação permite que você faça uma chamada autenticada personalizada para o [!DNL Allocadia] API. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pela outra [!DNL Allocadia] módulos.

A ação é baseada no tipo de entidade (tipo de objeto Allocadia) especificado.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Allocadia] para [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Insira um caminho relativo a <code>https://api-na.allocadia.com/{version}</code> ou <code>https://api-eu.allocadia.com/{version}</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Selecione o método de solicitação HTTP que você precisa configurar a chamada da API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] adiciona os cabeçalhos de autorização para você.</p> </td> 
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
 </tbody> 
</table>

#### [!UICONTROL Ler Registro]

Este módulo de ação lê dados de um único registro em [!DNL Allocadia].

Especifique a ID do registro.

O módulo retorna quaisquer campos padrão associados ao registro, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowhader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Allocadia] para [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de entidade]</td> 
   <td>Selecione o tipo de [!DNL Allocadia] registre que deseja que o módulo leia.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td> <p>Selecione os campos que deseja incluir na saída do módulo. Os campos disponíveis dependem do [!UICONTROL Tipo de entidade] selecionado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Insira ou mapeie a [!DNL Allocadia] ID do registro que você deseja que o módulo leia.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar registro]

Esse módulo de ação cria um registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowhader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Allocadia] para [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de entidade]</td> 
   <td>Selecione se deseja criar um novo registro com base no item da linha ou na escolha da coluna.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Orçamentos]</td> 
   <td> <p>Selecione o orçamento onde deseja criar um registro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Column choices]</td> 
   <td>Selecione a coluna que deseja usar para criar um novo registro.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Label]</td> 
   <td>Inserir ou mapear um rótulo para o novo registro</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir registro]

Esse módulo de ação exclui um registro específico.

Especifique a ID do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowhader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Allocadia] para [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de entidade]</td> 
   <td> <p>Selecione o tipo de entidade que deseja excluir.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Item de linha]</strong> </p> <p>Informe a ID do Item de Linha</p> </li> 
     <li> <p><strong>[!UICONTROL Coluna Choice]</strong> </p> <p>Selecione o orçamento do qual deseja excluir um registro e insira a ID da Coluna e a ID de Escolha.</p> </li> 
     <li> <p><strong>[!UICONTROL Tags de previsão]</strong> </p> <p>Selecione o orçamento do qual deseja excluir um registro e insira a ID da tag.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar registro]

Esse módulo de ação atualiza um registro, como um item de linha, usuário ou escolha de coluna.

Especifique a ID do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Allocadia] ao [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de entidade]</td> 
   <td>Selecione o tipo de [!DNL Allocadia] registre que deseja que o módulo seja atualizado. Outros campos são exibidos com base no tipo de entidade selecionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Orçamentos]</td> 
   <td> <p>Selecione o orçamento onde deseja atualizar um registro. </p> </td> 
  </tr> 
 </tbody> 
</table>

### Pesquisas

#### [!UICONTROL Registro de pesquisa]

Este módulo de pesquisa procura registros em um objeto em [!DNL Allocadia] que correspondem à consulta de pesquisa especificada.

Você pode mapear essas informações em módulos subsequentes do cenário.

Especifique o tipo dos registros desejados.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowhader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Allocadia] para [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de entidade]</td> 
   <td>Selecione o tipo de [!DNL Allocadia] registre que deseja que o módulo procure. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Orçamentos]</td> 
   <td> <p>Selecione o orçamento que deseja pesquisar. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conjunto de resultados]</td> 
   <td>Selecione se deseja que o módulo retorne Todos os Registros Correspondentes ou Somente o Primeiro Registro Correspondente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contagem máxima de registros]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Critérios de pesquisa]</td> 
   <td>Selecione o campo que deseja pesquisar, selecione a operação e insira ou mapeie o valor que deseja pesquisar. Você pode adicionar [!DNL AND] ou [!DNL OR] regras para filtrar ainda mais sua pesquisa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td> <p>Selecione os campos que deseja incluir na saída do módulo. Os campos disponíveis dependem do Tipo de entidade selecionado.</p> </td> 
  </tr> 
 </tbody> 
</table>
