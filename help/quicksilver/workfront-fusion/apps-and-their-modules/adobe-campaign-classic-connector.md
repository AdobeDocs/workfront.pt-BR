---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Adobe Campaign Classic
description: Com o [!DNL Adobe Campaign Classic] módulos, você pode iniciar um [!DNL Adobe Workfront Fusion] cenário com base em eventos no seu [!DNL Adobe Campaign Classic] conta, criar, ler ou atualizar contratos e outros registros, pesquisar registros usando os critérios que você definiu e fazer upload de documentos.
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: 482725764ede6b2700985fa67dc2cb9f92d3bb12
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 1%

---

# [!DNL Adobe Campaign Classic] módulos

Com o [!DNL Adobe Campaign Classic] módulos, você pode iniciar um [!DNL Adobe Workfront Fusion] cenário com base em eventos no seu [!DNL Adobe Campaign Classic] criar, ler ou atualizar registros, pesquisar registros usando os critérios definidos e executar chamadas de API personalizadas.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para Automação e integração do trabalho] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conectar [!DNL Adobe Campaign Classic] para [!DNL Adobe Workfront Fusion]

1. Em qualquer [!DNL Adobe Campaign Classic] , clique em **[!UICONTROL Adicionar]** ao lado da [!UICONTROL Conexão] campo.
1. Insira o URL base que você usa para se conectar ao seu [!DNL Adobe Campaign Classic] instância.
1. Digite seu nome de usuário e senha.
1. Clique em **[!UICONTROL Continuar]** para criar a conexão e voltar ao módulo.

## [!DNL Adobe Campaign Classic] módulos e seus campos

Ao configurar [!DNL Adobe Campaign Classic] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Adobe Campaign Classic] Os campos podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Ações](#actions)
* [Pesquisas](#searches)

### Triggers

#### [!UICONTROL Observar registros]

Esse módulo de acionador agendado inicia um cenário quando um registro é alterado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Campaign Classic]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td>Selecione se deseja observar novos registros, registros atualizados ou ambos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Selecione o recurso que deseja observar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos a serem incluídos na saída]</td> 
   <td>Selecione os campos que deseja incluir na saída do módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos personalizados a serem incluídos na saída]</td> 
   <td>Para cada campo personalizado que deseja incluir na saída, clique em <b>[!UICONTROL Adicionar]</b> e insira o nome do campo personalizado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de resultados retornados]</td> 
   <td>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</td> 
  </tr> 
 </tbody> 
</table>


### Ações

* [[!UICONTROL Criar um registro]](#create-a-record)
* [[!UICONTROL Fazer uma chamada de API personalizada]](#make-a-custom-api-call)
* [[!UICONTROL Excluir um registro]](#delete-record)
* [[!UICONTROL Executar uma ação]](#perform-an-action)
* [[!UICONTROL Ler um registro]](#-read-a-record)
* [[!UICONTROL Assinar ou cancelar inscrição]](#subscribe-or-unsubscribe)
* [[!UICONTROL Atualizar um registro]](#update-record)

#### [!UICONTROL Criar um registro]

Este módulo de ação cria um novo registro no [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td>
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Campaign Classic]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Selecione o tipo de [!DNL Adobe Campaign Classic] registro que deseja criar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos] </td> 
   <td>Selecione os campos para os quais deseja definir valores quando o registro for criado e preencha os valores desses campos. Os campos variam de acordo com o tipo de registro selecionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos personalizados]</td> 
   <td> Para cada campo personalizado que deseja adicionar ao novo registro, clique em <b>[!UICONTROL Adicionar item]</b> e insira ou mapeie o nome e o valor do campo. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Fazer uma chamada de API personalizada]

Esse módulo faz uma chamada de API personalizada para o [!DNL Adobe Campaign Classic] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Campaign Classic]</a> neste artigo.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ação]</td>
      <td><p>Selecione a ação que você deseja que a chamada de API execute.</p>
      <p>[!UICONTROL Executar consulta]</p>
      <p>[!UICONTROL Gravar]</p>
      <p>[!UICONTROL Obter entidade se mais recente]</p>
      <p>[!UICONTROL Selecionar tudo]</p>
      <p>[!UICONTROL Evento Push]</p>
    </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cabeçalhos]</td>
      <td>
        <p>Adicione os cabeçalhos da solicitação no formulário de um objeto JSON padrão.</p>
        <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] adiciona automaticamente o cabeçalho do token [!UICONTROL x-security].</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Corpo XML]</td>
   <td> <p>Adicione o conteúdo do corpo para a chamada da API em XML, sem o elemento de sessão. </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Excluir registro]

Este módulo de ação exclui um único registro de [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td>
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Campaign Classic]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Selecione o tipo de recurso que deseja excluir.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Insira ou mapeie a ID do recurso que deseja excluir.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Executar uma ação]

Este módulo de ação executa uma ação selecionada em um objeto na [!DNL Adobe Campaign Classic] API.

Para obter informações sobre ações e campos específicos, consulte [[!DNL Adobe Campaign] - Documentação da API](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td>
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Campaign Classic]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ação]</td> 
   <td><p>Selecione a ação a ser executada no objeto.</p>
   <ul>
   <li><p><b>[!DNL List]</b></p><p> Para obter os campos disponíveis, consulte <a href="#search" class="MCXref xref" >[!UICONTROL Pesquisar]</a> neste artigo. </p></li>
     <li><p><b>[!UICONTROL Obter]</b></p><p> Para obter os campos disponíveis, consulte <a href="#search" class="MCXref xref" >[!UICONTROL Pesquisar]</a> neste artigo. </p></li> 
   <li><p><b>[!UICONTROL Criar]</b></p><p> Para obter os campos disponíveis, consulte <a href="#create-a-record" class="MCXref xref" >[!UICONTROL Criar um registro]</a> neste artigo. </p></li>
   <li><p><b>[!UICONTROL Atualizar]</b></p><p> Para obter os campos disponíveis, consulte <a href="#update-record" class="MCXref xref" >[!UICONTROL Atualizar um registro]</a> neste artigo. </p></li>
   <li><p><b>[!UICONTROL Excluir]</b></p><p> Para obter os campos disponíveis, consulte <a href="#delete-record" class="MCXref xref" >[!UICONTROL Excluir um registro]</a> neste artigo. </p></li>
   </ul>
   </td>
</tr> 
 </tbody> 
</table>

#### [!UICONTROL Ler um registro]

Este módulo de ação lê um registro de [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td>
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Campaign Classic]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Selecione o tipo de [!DNL Adobe Campaign Classic] registro que você deseja ler.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Insira do mapa a ID do registro que você deseja ler.</td> 
  </tr> 
 <tr> 
   <td role="rowheader">[!UICONTROL Campos a serem incluídos na saída] </td> 
   <td>Selecione os campos que deseja incluir na saída do módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos personalizados a serem incluídos na saída]</td> 
   <td>Para cada campo personalizado que deseja incluir na saída, clique em <b>[!UICONTROL Adicionar]</b> e insira o nome do campo personalizado.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Assinar ou cancelar inscrição]

Este módulo de ação assina um usuário ou cancela a assinatura de um usuário em um serviço de informação.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td>
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Campaign Classic]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assinar ou cancelar assinatura]</td> 
   <td>Selecione se deseja assinar ou cancelar a assinatura do serviço de informações.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do serviço]</td> 
   <td>Selecione o serviço que deseja assinar ou do qual deseja cancelar a assinatura.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Endereço de email do destinatário] </td> 
   <td>Insira ou mapeie o endereço de email do usuário que deseja assinar ou cancelar a assinatura do serviço de informações.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar registro]

Este módulo de ação atualiza um único registro no [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td>
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Campaign Classic]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Selecione o tipo de [!DNL Adobe Campaign Classic] registro que deseja criar.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Insira do mapa a ID do registro que você deseja atualizar.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Campos] </td> 
   <td>Selecione os campos para os quais deseja atualizar valores e preencha os valores desses campos. Os campos variam de acordo com o tipo de registro selecionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos personalizados]</td> 
   <td> Para cada campo personalizado que deseja atualizar, clique em <b>[!UICONTROL Adicionar item]</b> e insira ou mapeie o nome e o valor do campo. </td> 
  </tr> 
 </tbody> 
</table>

### Pesquisas

#### [!UICONTROL Pesquisa]

Este módulo de pesquisa retorna registros com base nos critérios especificados.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td>
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Campaign Classic]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Selecione o tipo de [!DNL Adobe Campaign Classic] registro que deseja criar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite] </td> 
   <td>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</td> 
  </tr> 
 </tbody> 
</table>
