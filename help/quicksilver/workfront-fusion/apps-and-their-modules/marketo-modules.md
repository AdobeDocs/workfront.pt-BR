---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos Marketo
description: Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL Marketo], bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: 7f6dace5-ab50-45da-a926-1a8919057f7b
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2014'
ht-degree: 0%

---

# [!DNL Marketo] módulos

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL Marketo], bem como conectá-lo a vários aplicativos e serviços de terceiros.

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

Para usar [!DNL Marketo] módulos, você deve ter um [!DNL Marketo] conta.

## Connect [!DNL Marketo] para o Workfront Fusion {#connect-marketo-to-workfront-fusion}

Você pode criar uma conexão com o [!DNL Marketo] conta diretamente de dentro [!DNL Marketo] módulo.

1. Em qualquer [!DNL Marketo] módulo, clique em **[!UICONTROL Adicionar]** ao lado do [!UICONTROL Conexão] campo.
1. Insira seu [!DNL Marketo] ou [!DNL Marketo] [!UICONTROL Munchkin] ID. Essa é a parte exclusiva do URL básico ou do Endpoint atribuído à sua conta, que você usa para acessar [!DNL Marketo] através da [!UICONTROL REST] API. Para obter instruções sobre como localizar isso, consulte [URL básica](https://developers.marketo.com/rest-api/base-url/) no [!DNL Marketo] documentação.
1. Insira seu [!UICONTROL ID do cliente] e [!UICONTROL Segredo do cliente]. Para obter instruções sobre como localizá-los, consulte [Autenticação](https://developers.marketo.com/rest-api/authentication/) no [!DNL Marketo] documentação.
1. Clique em **[!UICONTROL Continuar]** para criar a conexão e retornar ao módulo .

## [!DNL Marketo] Módulos e seus campos

Ao configurar [!DNL Marketo] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Marketo] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Ações](#actions)
* [Pesquisas](#searches)

### Triggers

* [[!UICONTROL Registros de monitoramento]](#watch-records)
* [[!UICONTROL Assista aos eventos (Instant)]](#watch-events-instant)

#### [!UICONTROL Registros de monitoramento]

Esse módulo de acionador inicia um cenário quando um registro é criado ou atualizado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Marketo] para [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione o tipo de registro que deseja criar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Atividade]</strong> </p> <p>Selecione o tipo de atividade que deseja assistir. </p> <p>O módulo assiste somente para novas atividades.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Lead]</strong> </p> <p>Selecione se deseja procurar novos registros, registros atualizados, registros novos e atualizados ou atualizações de campo específicas. Se você optar por assistir a atualizações de campo específicas, selecione o campo que deseja que o módulo assista.</p> </li> 
     <li> <p><strong>[!UICONTROL Program]</strong> </p> <p>Selecione se deseja procurar novos registros, registros atualizados ou registros novos e atualizados.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td> <p>Selecione as informações que deseja incluir no pacote de saída deste módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Assista aos eventos (Instant)]

Esse módulo de acionador inicia um cenário quando um registro é criado ou atualizado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Webhook]</p> </td> 
   <td> <p>Insira o webhook que você deseja que o módulo use.</p> <p>Para obter mais informações sobre webhooks, consulte <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Acionadores instantâneos (webhooks) em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [[!UICONTROL Chamada de API personalizada]](#custom-api-call)
* [[!UICONTROL Criar um registro]](#create-a-record)
* [[!UICONTROL Atualizar um registro]](#update-a-record)
* [[!UICONTROL Baixar um arquivo]](#download-a-file)
* [[!UICONTROL Fazer upload de um arquivo]](#upload-a-file)
* [[!UICONTROL Ler um registro]](#read-a-record)
* [[!UICONTROL Adicionar leads a uma lista]](#add-leads-to-a-list)
* [[!UICONTROL Remover leads de uma lista]](#remove-leads-from-a-list)
* [[!UICONTROL Agendar uma campanha]](#schedule-a-campaign)
* [[!UICONTROL Copiar um programa]](#copy-a-program)

#### [!UICONTROL Chamada de API personalizada]

Esse módulo de ação permite que você faça uma chamada autenticada personalizada para o [!DNL Marketo] API. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pela outra [!DNL Marketo] módulos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Marketo] para [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Insira um caminho relativo a <code>https://{your-base-url}.mktorest.com/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Selecione o método de solicitação HTTP que você precisa configurar a chamada da API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> <p>O [!UICONTROL Workfront Fusion] adiciona os cabeçalhos de autorização para você.</p> </td> 
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
   <td> <p>Insira ou mapeie o número máximo de registros com os quais deseja que o módulo funcione durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar um registro]

Esse módulo de ação cria um novo registro em [!DNL Marketo]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Marketo] para [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione o tipo de registro que deseja criar.</p> 
    <ul> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL Pasta]</p> </li> 
     <li> <p>[!UICONTROL Lead]</p> </li> 
     <li> <p>[!UICONTROL Program]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Selecionar campos a serem mapeados]</td> 
   <td>Se estiver criando uma Empresa ou um Lead, selecione os campos para os quais deseja definir valores quando o novo registro for criado e insira valores para esses campos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de programa]</td> 
   <td>Se você estiver criando um Programa, selecione o tipo de programa que deseja criar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Canal do programa] </td> 
   <td>Se você estiver criando um Programa, selecione o canal de programa no qual deseja criar o programa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta] / [!UICONTROL Nome do programa]</td> 
   <td>Se você estiver criando uma Pasta ou Programa, insira ou mapeie um nome para o novo registro.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descrição]</td> 
   <td> <p>Se você estiver criando uma Pasta ou Programa, insira ou mapeie uma descrição para o novo registro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da pasta pai]</td> 
   <td>Se você estiver criando uma Pasta ou Programa, insira ou mapeie a ID da pasta pai onde deseja criar o novo registro.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custos]</td> 
   <td>Se você estiver criando um Programa, adicione quaisquer custos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tags]</td> 
   <td>Se você estiver criando um Programa, adicione quaisquer tags</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar um registro]

Esse módulo de ação atualiza um registro existente usando sua ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Marketo] para [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione o tipo de registro que deseja criar.</p> 
    <ul> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL Lead]</p> </li> 
     <li> <p>[!UICONTROL Program]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Company] / [!UICONTROL Lead] / [!UICONTROL ID do programa]</td> 
   <td>Insira ou mapeie a ID do registro que deseja atualizar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Selecionar campos a serem mapeados]</td> 
   <td>Se estiver atualizando uma Empresa ou um Lead, selecione os campos para os quais deseja atualizar valores e insira valores para esses campos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do programa]</td> 
   <td>Se estiver atualizando um Programa, insira ou mapeie um novo nome para o programa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descrição]</td> 
   <td> <p>Se estiver atualizando um Programa, insira ou mapeie uma nova descrição para o programa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data de início]</td> 
   <td>Se você estiver atualizando um Programa, insira ou mapeie uma nova data de início para o programa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data final]</td> 
   <td>Se você estiver atualizando um Programa, insira ou mapeie uma nova data final para o programa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custos]</td> 
   <td>Se você estiver atualizando um Programa, adicione quaisquer custos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tags]</td> 
   <td>Se você estiver atualizando um programa, adicione quaisquer tags</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Baixar um arquivo]

Este módulo de ação baixa um arquivo usando a ID do arquivo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Marketo] para [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do arquivo]</td> 
   <td>Mapeie a ID do arquivo que deseja baixar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Fazer upload de um arquivo]

Este módulo de ação carrega um novo arquivo para o [!UICONTROL Marketo].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Marketo] para [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da pasta]</td> 
   <td>Insira ou mapeie a ID da pasta onde deseja que o novo arquivo fique localizado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descrição]</td> 
   <td>Insira uma descrição para o arquivo carregado.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ler um registro]

Esse módulo de ação lê informações sobre um registro usando sua ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Marketo] para [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione o tipo de registro que deseja criar.</p> 
    <ul> 
     <li> <p>[!UICONTROL Campaign]</p> </li> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL Lead]</p> </li> 
     <li> <p>[!UICONTROL List]</p> </li> 
     <li> <p>[!UICONTROL Program]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td>Selecione as informações que deseja incluir no pacote de saída deste módulo. Os campos estão disponíveis com base no [!UICONTROL Tipo de registro] selecionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL &lt;object&gt; ID]</td> 
   <td>Insira ou mapeie a ID do objeto sobre o qual deseja recuperar informações.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Adicionar leads a uma lista]

Esse módulo de ação adiciona um ou mais leads a uma lista, usando a ID do lead.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Marketo] para [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td>Insira ou mapeie a ID da lista onde deseja adicionar leads.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL IDs de lead]</td> 
   <td> <p>Para cada lead que deseja adicionar à lista, clique em <b>[!UICONTROL Adicionar]</b>, em seguida, insira ou mapeie a ID do lead que deseja adicionar. É possível adicionar até 300 leads ao módulo a ser adicionado à lista.</p> <p>Clique na alternância de mapa para mapear uma coleção existente de leads que você deseja adicionar à lista.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remover leads de uma lista]

Esse módulo de ação remove um ou mais leads de uma lista, usando a ID do lead.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Marketo] para [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td>Insira ou mapeie a ID da lista onde deseja remover leads.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL IDs de lead]</td> 
   <td> <p>Para cada lead que você deseja remover da lista, clique em <b>[!UICONTROL Adicionar]</b>, em seguida, insira ou mapeie a ID do cliente potencial que deseja remover. Você pode adicionar até 300 leads para que o módulo remova da lista. </p> <p>Clique na alternância de mapa para mapear uma coleção existente de leads que você deseja remover da lista.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Agendar uma campanha]

Esse módulo de ação agenda uma campanha existente para uma determinada data.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Marketo] para [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da campanha]</td> 
   <td>Insira ou mapeie a ID da campanha que deseja agendar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Agendamento para data]</p> </td> 
   <td>Selecione a data em que deseja que a campanha seja executada. Se esse campo ficar em branco, a campanha será executada cinco minutos após o início do cenário.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiar um programa]

Este módulo de ação faz uma cópia de um programa usando a ID do programa existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Marketo] para [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do programa existente]</td> 
   <td>Insira ou mapeie a ID do programa que você deseja copiar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Novo nome do programa]</p> </td> 
   <td> <p>Inserir ou mapear um nome para o novo programa</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da pasta]</td> 
   <td>Insira ou mapeie a ID da pasta onde deseja que o novo programa fique localizado.</td> 
  </tr> 
 </tbody> 
</table>

### Pesquisas

* [[!UICONTROL Listar registros]](#list-records)
* [[!UICONTROL Pesquisar registros]](#update-a-record)

#### [!UICONTROL Listar registros]

Esse módulo de ação recupera todos os registros de um tipo específico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Marketo] para [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione o tipo de registro que deseja listar.</p> 
    <ul> 
     <li> <p>[!UICONTROL Ler todas as campanhas]</p> </li> 
     <li> <p>[!UICONTROL Ler todos os programas]</p> </li> 
     <li> <p>[!UICONTROL Ler todos os leads] </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campo]</td> 
   <td>Se você selecionou recuperar leads, selecione se deseja recuperar leads de uma lista ou de um programa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td>Selecione as informações que deseja incluir no pacote de saída deste módulo. Os campos estão disponíveis com base no [!UICONTROL Tipo de registro] selecionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Pesquisar registros]

Esse módulo de pesquisa recupera uma lista de registros que correspondem a critérios de pesquisa específicos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Marketo] para [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione o tipo de registro que deseja pesquisar.</p> 
    <ul> 
     <li> <p>[!UICONTROL Campanhas]</p> </li> 
     <li> <p>[!UICONTROL Leads]</p> </li> 
     <li> <p>[!UICONTROL Programas]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Campo]</p> </td> 
   <td> <p>Selecione se deseja pesquisar por nome, nome do programa ou nome do espaço de trabalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valores]</td> 
   <td>Para cada valor que deseja pesquisar, clique em <b>[!UICONTROL Adicionar item]</b> e insira o valor .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saída]</td> 
   <td> <p>Selecione as informações que deseja incluir no pacote de saída deste módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>
