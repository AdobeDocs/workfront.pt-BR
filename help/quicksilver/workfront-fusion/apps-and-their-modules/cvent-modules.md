---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de evento
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: c95b9764-29a5-4d8c-8e6d-68a3969129e0
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1111'
ht-degree: 1%

---

# [!DNL Cvent] módulos

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Cvent modules](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/cvent-modules.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

Em um cenário [!DNL Adobe Workfront Fusion], você pode automatizar fluxos de trabalho que usam [!DNL Cvent], bem como conectá-los a vários aplicativos e serviços de terceiros.

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

Para usar módulos [!DNL Cvent], você deve ter uma conta [!DNL Cvent].

## Informações da API de evento

O Conector de evento usa o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Versão da API</td> 
   <td> V200611.ASMX </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tag da API</td> 
   <td>v1.7.14</td> 
  </tr>
 </tbody> 
 </table>

## Conectar [!DNL Cvent] a [!DNL Adobe Workfront Fusion] {#connect-cvent-to-adobe-workfront-fusion}

>[!NOTE]
>
>Os módulos [!DNL Cvent] funcionam por meio de uma API [!UICONTROL SOAP]. Para criar uma conexão com [!DNL Cvent], você deve garantir o seguinte:
>
>* Você tem acesso de [!UICONTROL SOAP] à API [!DNL Cvent].
>* Os [!DNL Workfront Fusion] endereços IP foram adicionados ao incluo na lista de permissões de pesquisa da sua organização.
>
>  Para obter uma lista de [!DNL Workfront Fusion] endereços IP, consulte [Endereços IP para acessar [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)


Você pode criar uma conexão com sua conta do [!DNL Cvent] diretamente de dentro de um módulo do [!DNL Cvent].

1. Em qualquer módulo [!DNL Cvent], clique em **[!UICONTROL Adicionar]** ao lado do campo [!UICONTROL Conexão].
1. Selecione a região à qual deseja se conectar.

   * [!UICONTROL América do Norte]
   * [!UICONTROL Europa]
   * [!UICONTROL Sandbox]

1. Clique em **[!UICONTROL Continuar]** para criar a conexão e voltar para o módulo.

## [!DNL Cvent] módulos e seus campos

Ao configurar módulos do [!DNL Cvent], o [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos [!DNL Cvent] adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Ações](#actions)
* [Pesquisas](#searches)

### Ações

* [[!UICONTROL Chamada de API personalizada]](#create-meeting-request)
* [[!UICONTROL Ler um registro]](#read-a-record)
* [[!UICONTROL Registrar Convite]](#register-invitee)
* [[!UICONTROL Adicionar convite]](#add-invitee)
* [[!UICONTROL Excluir Contato]](#delete-contact)
* [[!UICONTROL Atualizar Contato]](#update-contact)
* [[!UICONTROL Criar solicitação de reunião]](#create-meeting-request)

#### [!UICONTROL Chamada de API personalizada]

Este módulo de ação permite fazer uma chamada autenticada personalizada para a API [!DNL Cvent]. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pelos outros módulos do [!DNL Cvent].

Ao configurar esse módulo, os campos a seguir são exibidos.

O módulo retorna o código de status a, juntamente com os cabeçalhos e o corpo da chamada de API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Cvent] ao [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Cvent] ao [!DNL Adobe Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Operação</td> 
   td&gt; <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Corpo (XML)</td> 
   <td> <p>Insira ou mapeie o corpo da chamada à API. Isso deve incluir somente o XML. O módulo incluirá automaticamente cabeçalhos de autenticação. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ler um registro]

Esse módulo de ação lê informações sobre um registro específico.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Cvent] ao [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Cvent] ao [!DNL Adobe Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de registro]</p> </td> 
   <td>Selecione o tipo de item do registro que deseja ler.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contato] / [!UICONTROL Evento] / [!UICONTROL ID do Convite]</td> 
   <td> <p>Insira ou mapeie a ID do item que você deseja ler.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td> <p>Selecione os campos que deseja incluir na saída do módulo. Os campos estão disponíveis com base no tipo de item selecionado.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Registrar Convite]

Este módulo de ação registra um convidado para um evento.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Cvent] ao [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Cvent] ao [!DNL Adobe Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ID do convite</p> </td> 
   <td> <p>Insira ou mapeie a ID do convidado que você deseja registrar em um evento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID de evento</td> 
   <td> <p>Insira ou mapeie a ID do evento para o qual você deseja registrar o convite.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Adicionar convite]

Este módulo de ação convida um contato para um evento.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Cvent] ao [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Cvent] ao [!DNL Adobe Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de Contato]</p> </td> 
   <td> <p>Insira ou mapeie a ID do contato que deseja adicionar a um evento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Evento]</td> 
   <td> <p>Insira ou mapeie a ID do evento ao qual deseja adicionar o contato.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir Contato]

Este módulo de ação exclui um único contato no Evento.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Cvent] ao [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Cvent] ao [!DNL Adobe Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Contato]</td> 
   <td> <p>Insira ou mapeie a ID do contato que deseja excluir.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar Contato]

Este módulo de ação atualiza um contato existente usando sua ID.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Cvent] ao [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Cvent] ao [!DNL Adobe Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de Contato]</p> </td> 
   <td> <p>Insira ou mapeie a ID do contato que você deseja atualizar.</p> </td> 
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
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Cvent] ao [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Cvent] ao [!DNL Adobe Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de Formulário]</p> </td> 
   <td> <p>Insira ou mapeie a ID do Formulário que deseja usar para criar a nova solicitação de reunião.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos de Solicitação de Reunião]</td> 
   <td> <p>Selecione os campos de solicitação de reunião para os quais deseja inserir informações e preencha os valores desejados para esses campos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos de Solicitação de Evento]</td> 
   <td> <p>Selecione os campos de solicitação de evento para os quais você deseja inserir informações e preencha os valores desejados para esses campos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos de Solicitação de RFP]</td> 
   <td> <p>Selecione os campos de solicitação de proposta para os quais deseja inserir informações e preencha os valores desejados para esses campos.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Pesquisas

#### [!UICONTROL Listar registros]

Este módulo de pesquisa recupera informações sobre todos os registros de um tipo específico.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Cvent] ao [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Cvent] ao [!DNL Adobe Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de registro]</p> </td> 
   <td> <p>Selecione o tipo de registro que deseja listar.</p> 
    <ul> 
     <li> <p>Todos os eventos da sua conta [!DNL Cvent]</p> </li> 
     <li> <p>Todas as sessões de um evento</p> </li> 
     <li> <p>Todos os convidados para um evento</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Evento]</td> 
   <td> <p>Se você estiver listando convidados ou sessões, informe ou mapeie a ID do evento ao qual esses convidados ou sessões estão associados.</p> </td> 
  </tr> 
 </tbody> 
</table>
