---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de conversão
description: Em um [!DNL Adobe Workfront Fusion] você pode automatizar os fluxos de trabalho que usam o Creative Cloud, bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: c95b9764-29a5-4d8c-8e6d-68a3969129e0
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '996'
ht-degree: 1%

---

# [!DNL Cvent] módulos

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL Cvent], bem como conectá-lo a vários aplicativos e serviços de terceiros.

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

Para usar [!DNL Cvent] módulos, você deve ter um [!DNL Cvent] conta.

## Connect [!DNL Cvent] para [!DNL Adobe Workfront Fusion] {#connect-cvent-to-adobe-workfront-fusion}

>[!NOTE]
>
>O [!DNL Cvent] os módulos funcionam por meio de [!UICONTROL SOAP] API. Para criar uma conexão com o [!DNL Cvent], você deve garantir o seguinte:
>
>* Você tem [!UICONTROL SOAP] acesso ao [!DNL Cvent] API.
>* O [!DNL Workfront Fusion] Os endereços IP foram adicionados à  de lista de permissões da sua organização.
>
>  Para uma lista de [!DNL Workfront Fusion] Endereços IP, consulte [Endereços IP para acessar [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)


Você pode criar uma conexão com o [!DNL Cvent] conta diretamente de dentro de uma [!DNL Cvent] módulo.

1. Em qualquer [!DNL Cvent] módulo, clique em **[!UICONTROL Adicionar]** ao lado do [!UICONTROL Conexão] campo.
1. Selecione a região à qual deseja se conectar.

   * [!UICONTROL América do Norte]
   * [!UICONTROL Europa]
   * [!UICONTROL Sandbox]

1. Clique em **[!UICONTROL Continuar]** para criar a conexão e retornar ao módulo .

## [!DNL Cvent] módulos e seus campos

Ao configurar [!DNL Cvent] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Cvent] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Ações](#actions)
* [Pesquisas](#searches)

### Ações

* [[!UICONTROL Chamada da API personalizada]](#create-meeting-request)
* [[!UICONTROL Ler um registro]](#read-a-record)
* [[!UICONTROL Registrar Convite]](#register-invitee)
* [[!UICONTROL Adicionar Convidado]](#add-invitee)
* [[!UICONTROL Excluir Contato]](#delete-contact)
* [[!UICONTROL Atualizar contato]](#update-contact)
* [[!UICONTROL Criar solicitação de reunião]](#create-meeting-request)

#### [!UICONTROL Chamada da API personalizada]

Esse módulo de ação permite que você faça uma chamada autenticada personalizada para o [!DNL Cvent] API. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pela outra [!DNL Cvent] módulos.

Ao configurar esse módulo, os seguintes campos são exibidos.

O módulo retorna um código de status, juntamente com os cabeçalhos e o corpo da chamada à API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Cvent] para [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] para [!DNL Adobe Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Operação</td> 
   td&gt; <p>Selecione o método de solicitação HTTP que você precisa configurar a chamada da API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Corpo (XML)</td> 
   <td> <p>Insira ou mapeie o corpo da chamada de API. Isso deve incluir somente o XML. O módulo incluirá automaticamente cabeçalhos de autenticação. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ler um registro]

Este módulo de ação lê informações sobre um registro específico.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Cvent] para [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] para [!DNL Adobe Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de registro]</p> </td> 
   <td>Selecione o tipo de item do registro que deseja ler.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contato] / [!UICONTROL Evento] / [!UICONTROL ID do convite]</td> 
   <td> <p>Insira ou mapeie a ID do item que deseja ler.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td> <p>Selecione os campos que deseja incluir na saída do módulo. Os campos estão disponíveis com base no tipo de item selecionado.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Registrar Convite]

Esse módulo de ação registra um convidado para um evento.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Cvent] para [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] para [!DNL Adobe Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ID de Convite</p> </td> 
   <td> <p>Insira ou mapeie a ID do convidado que deseja registrar para um evento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID do evento</td> 
   <td> <p>Insira ou mapeie a ID do evento para o qual deseja registrar o convidado.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Adicionar Convidado]

Este módulo de ação convida um contato para um evento.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Cvent] para [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] para [!DNL Adobe Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID do contato]</p> </td> 
   <td> <p>Insira ou mapeie a ID do contato que deseja adicionar a um evento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do evento]</td> 
   <td> <p>Insira ou mapeie a ID do evento ao qual deseja adicionar o contato.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir Contato]

Este módulo de ação exclui um único contato no Cevent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Cvent] para [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] para [!DNL Adobe Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do contato]</td> 
   <td> <p>Insira ou mapeie a ID do contato que deseja excluir.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar contato]

Esse módulo de ação atualiza um contato existente usando sua ID.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Cvent] para [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] para [!DNL Adobe Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID do contato]</p> </td> 
   <td> <p>Insira ou mapeie a ID do contato que deseja atualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos]</td> 
   <td> <p>Selecione os campos para os quais deseja inserir informações e preencha os valores desejados para esses campos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos personalizados]</td> 
   <td> <p>Selecione os campos para os quais deseja inserir informações e preencha os valores desejados para esses campos.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar solicitação de reunião]

Este módulo de ação adiciona uma solicitação de reunião à sua conta.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Cvent] para [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] para [!DNL Adobe Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID do formulário]</p> </td> 
   <td> <p>Insira ou mapeie a ID do Formulário que deseja usar para criar a nova solicitação de reunião.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos de solicitação de reunião]</td> 
   <td> <p>Selecione os campos de solicitação de reunião para os quais deseja inserir informações e preencha os valores desejados para esses campos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos de solicitação de evento]</td> 
   <td> <p>Selecione os campos de solicitação de evento para os quais deseja inserir informações e preencha os valores desejados para esses campos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL RFP Request Fields]</td> 
   <td> <p>Selecione a solicitação de campos de proposta para os quais deseja inserir informações e preencha os valores desejados para esses campos.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Pesquisas

#### [!UICONTROL Listar registros]

Esse módulo de pesquisa recupera informações sobre todos os registros de um tipo específico.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Cvent] para [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] para [!DNL Adobe Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de registro]</p> </td> 
   <td> <p>Selecione o tipo de registro que deseja listar.</p> 
    <ul> 
     <li> <p>Todos os eventos do [!DNL Cvent] account</p> </li> 
     <li> <p>Todas as sessões para um evento</p> </li> 
     <li> <p>Todos os convidados de um evento</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do evento]</td> 
   <td> <p>Se você estiver listando convidados ou sessões, insira ou mapeie a ID do evento ao qual esses convidados ou sessões estão associados.</p> </td> 
  </tr> 
 </tbody> 
</table>
