---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Alocar módulos
description: Em um [!DNL Adobe Workfront Fusion] Nesse cenário, você pode automatizar workflows que usam o Allocadia, bem como conectá-los a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: f1edefd1-9fe0-48fc-bea2-c3f9facf7363
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1401'
ht-degree: 0%

---

# [!DNL Allocadia] módulos

Em um [!DNL Adobe Workfront Fusion] cenário, é possível automatizar workflows que usam [!DNL Allocadia], bem como conectá-lo a vários aplicativos e serviços de terceiros.

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

Para usar [!DNL Allocadia] módulos, você deve ter um [!DNL Allocadia] conta.

## Conectar [!DNL Allocadia] para [!DNL Workfront Fusion]

Você pode criar uma conexão com o seu [!DNL Allocadia] diretamente de dentro de uma conta [!DNL Allocadia] módulo.

1. Em qualquer [!DNL Allocadia] , clique em **[!UICONTROL Adicionar]** ao lado da [!UICONTROL Conexão] campo.
1. Selecione se deseja usar o servidor da América do Norte ou o servidor da Europa.
1. Digite seu nome de usuário e senha.
1. Clique em **[!UICONTROL Continuar]** para criar a conexão e voltar ao módulo.

## [!DNL Allocadia] módulos e seus campos

Ao configurar [!DNL Allocadia] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Allocadia] Os campos podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Ações](#actions)
* [Pesquisas](#searches)

### Triggers

#### [!UICONTROL Assistir ao registro]

Esse módulo de acionamento executa um cenário quando objetos de um tipo específico são adicionados, atualizados ou ambos. O módulo retorna todos os campos padrão associados ao registro ou aos registros, juntamente com quaisquer campos e valores personalizados que a conexão acesse. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> <table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do Allocadia ao [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!UICONTROL Conectar alocações] ao Workfront Fusion</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filtro</td> 
   <td> <p>Selecione se deseja que o cenário observe Somente Novos Registros, [!UICONTROL Somente Registros Atualizados] ou Registros Novos e Atualizados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo de entidade</td> 
   <td>Selecione o tipo de registro Alocadia que você deseja que o módulo veja.</td> 
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

* [Chamada de API personalizada](#custom-api-call)
* [Ler registro](#read-record)
* [Criar registro](#create-record)
* [Excluir registro](#delete-record)
* [Atualizar registro](#update-record)

#### [!UICONTROL Chamada de API personalizada]

Esse módulo de ação permite fazer uma chamada autenticada personalizada para o [!DNL Allocadia] API. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pelo outro [!DNL Allocadia] módulos.

A ação é baseada no tipo de entidade (tipo de objeto Alocadia) especificado.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Allocadia] conta para [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Allocadia] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Insira um caminho relativo a <code>https://api-na.allocadia.com/{version}</code> ou <code>https://api-eu.allocadia.com/{version}</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formulário de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] O adiciona os cabeçalhos de autorização para você.</p> </td> 
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

#### [!UICONTROL Ler registro]

Este módulo de ação lê os dados de um único registro no [!DNL Allocadia].

Especifique a ID do registro.

O módulo retorna quaisquer campos padrão associados ao registro, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Allocadia] conta para [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Allocadia] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Entidade]</td> 
   <td>Selecione o tipo de [!DNL Allocadia] registre que deseja que o módulo leia.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td> <p>Selecione os campos que deseja incluir na saída do módulo. Os campos disponíveis dependem do [!UICONTROL Entity Type] selecionado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Insira ou mapeie o único [!DNL Allocadia] ID do registro que você deseja que o módulo leia.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar registro]

Este módulo de ação cria um registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Allocadia] conta para [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Allocadia] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Entidade]</td> 
   <td>Selecione se deseja criar um novo registro com base no item da linha ou na escolha da coluna.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Orçamentos]</td> 
   <td> <p>Selecione o orçamento no qual deseja criar um registro.</p> </td> 
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

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Allocadia] conta para [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Allocadia] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Entidade]</td> 
   <td> <p>Selecione o tipo de entidade que deseja excluir.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Item de linha]</strong> </p> <p>Informe a ID do Item da Linha</p> </li> 
     <li> <p><strong>[!UICONTROL Opção de Coluna]</strong> </p> <p>Selecione o orçamento do qual deseja excluir um registro e informe a ID da Coluna e a ID da Opção.</p> </li> 
     <li> <p><strong>[!UICONTROL Marcas de Previsão]</strong> </p> <p>Selecione o orçamento do qual deseja excluir um registro e insira a ID da tag.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar registro]

Esse módulo de ação atualiza um registro, como um item de linha, usuário ou opção de coluna,.

Especifique a ID do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Allocadia] a [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Allocadia] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Entidade]</td> 
   <td>Selecione o tipo de [!DNL Allocadia] registro que você deseja que o módulo atualize. Outros campos são exibidos com base no tipo de entidade selecionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Orçamentos]</td> 
   <td> <p>Selecione o orçamento no qual deseja atualizar um registro. </p> </td> 
  </tr> 
 </tbody> 
</table>

### Pesquisas

#### [!UICONTROL Pesquisar registro]

Este módulo de pesquisa procura registros em um objeto no [!DNL Allocadia] que correspondam à consulta de pesquisa especificada.

Você pode mapear essas informações em módulos subsequentes no cenário.

Especifique o tipo dos registros desejados.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Allocadia] conta para [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Allocadia] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Entidade]</td> 
   <td>Selecione o tipo de [!DNL Allocadia] registro que você deseja que o módulo procure. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Orçamentos]</td> 
   <td> <p>Selecione o orçamento que deseja pesquisar. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conjunto de resultados]</td> 
   <td>Selecione se você deseja que o módulo retorne Todos os registros correspondentes ou somente o Primeiro registro correspondente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contagem máxima de registros]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pesquisar critérios]</td> 
   <td>Selecione o campo que deseja pesquisar, selecione a operação e insira ou mapeie o valor que deseja pesquisar. Você pode adicionar [!DNL AND] ou [!DNL OR] regras para filtrar ainda mais sua pesquisa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td> <p>Selecione os campos que deseja incluir na saída do módulo. Os campos disponíveis dependem do Tipo de entidade selecionado.</p> </td> 
  </tr> 
 </tbody> 
</table>
