---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos Adobe Campaign Classic
description: Com o [!DNL Adobe Campaign Classic] módulos, você pode iniciar um [!DNL Adobe Workfront Fusion] com base nos eventos em seu [!DNL Adobe Campaign Classic] contas, criar, ler ou atualizar contratos e outros registros, procurar registros usando critérios definidos e carregar documentos.
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 1%

---

# [!DNL Adobe Campaign Classic] módulos

Com o [!DNL Adobe Campaign Classic] módulos, você pode iniciar um [!DNL Adobe Workfront Fusion] com base nos eventos em seu [!DNL Adobe Campaign Classic] crie, leia ou atualize registros, pesquise registros usando critérios definidos e execute chamadas de API personalizadas.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Connect [!DNL Adobe Campaign Classic] para [!DNL Adobe Workfront Fusion]

1. Em qualquer [!DNL Adobe Campaign Classic] módulo, clique em **[!UICONTROL Adicionar]** ao lado do [!UICONTROL Conexão] campo.
1. Insira o URL básico que você usa para se conectar ao seu [!DNL Adobe Campaign Classic] instância.
1. Insira seu nome de usuário e senha.
1. Clique em **[!UICONTROL Continuar]** para criar a conexão e retornar ao módulo .

## [!DNL Adobe Campaign Classic] módulos e seus campos

Ao configurar [!DNL Adobe Campaign Classic] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Adobe Campaign Classic] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Ações](#actions)
* [Pesquisas](#searches)

### Triggers

#### [!UICONTROL Registros de monitoramento]

Esse módulo de acionador agendado inicia um cenário quando um registro é alterado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Campaign Classic]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td>Selecione se deseja procurar novos registros, registros atualizados ou ambos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Selecione o recurso que deseja observar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos para incluir na saída]</td> 
   <td>Selecione os campos que deseja incluir na saída do módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos personalizados para incluir na saída]</td> 
   <td>Para cada campo personalizado que deseja incluir na saída, clique em <b>[!UICONTROL Adicionar]</b> e insira o nome do campo personalizado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de resultados retornados]</td> 
   <td>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</td> 
  </tr> 
 </tbody> 
</table>


### Ações

* [[!UICONTROL Criar um registro]](#create-a-record)
* [[!UICONTROL Efetuar uma chamada de API personalizada]](#make-a-custom-api-call)
* [[!UICONTROL Excluir um registro]](#delete-record)
* [[!UICONTROL Executar uma ação]](#perform-an-action)
* [[!UICONTROL Ler um registro]](#-read-a-record)
* [[!UICONTROL Assinar ou cancelar a assinatura]](#subscribe-or-unsubscribe)
* [[!UICONTROL Atualizar um registro]](#update-record)

#### [!UICONTROL Criar um registro]

Esse módulo de ação cria um novo registro em [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Campaign Classic]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Selecione o tipo de [!DNL Adobe Campaign Classic] gravar que deseja criar.</td> 
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

#### [!UICONTROL Efetuar uma chamada de API personalizada]

Esse módulo faz uma chamada de API personalizada para o [!DNL Adobe Campaign Classic] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Campaign Classic]</a> neste artigo.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ação]</td>
      <td><p>Selecione a ação que deseja que a chamada da API execute.</p>
      <p>[!UICONTROL Executar consulta]</p>
      <p>[!UICONTROL Gravação]</p>
      <p>[!UICONTROL Obter entidade se mais recente]</p>
      <p>[!UICONTROL Selecionar tudo]</p>
      <p>[!UICONTROL Evento de push]</p>
    </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cabeçalhos]</td>
      <td>
        <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão.</p>
        <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] adiciona o cabeçalho do token [!UICONTROL x-security] automaticamente.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Corpo XML]</td>
   <td> <p>Adicione o conteúdo do corpo para a chamada da API em XML, sem o elemento de sessão. </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Excluir registro]

Esse módulo de ação exclui um único registro do [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Campaign Classic]</a> neste artigo.</td> 
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
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Campaign Classic]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ação]</td> 
   <td><p>Selecione a ação a ser executada no objeto.</p>
   <ul>
   <li><p><b>[!DNL List]</b></p><p> Para campos disponíveis, consulte <a href="#search" class="MCXref xref" >[!UICONTROL Search]</a> neste artigo. </p></li>
     <li><p><b>[!UICONTROL Get]</b></p><p> Para campos disponíveis, consulte <a href="#search" class="MCXref xref" >[!UICONTROL Search]</a> neste artigo. </p></li> 
   <li><p><b>[!UICONTROL Criar]</b></p><p> Para campos disponíveis, consulte <a href="#create-a-record" class="MCXref xref" >[!UICONTROL Criar um registro]</a> neste artigo. </p></li>
   <li><p><b>[!UICONTROL Atualização]</b></p><p> Para campos disponíveis, consulte <a href="#update-record" class="MCXref xref" >[!UICONTROL Atualizar um registro]</a> neste artigo. </p></li>
   <li><p><b>[!UICONTROL Excluir]</b></p><p> Para campos disponíveis, consulte <a href="#delete-record" class="MCXref xref" >[!UICONTROL Excluir um registro]</a> neste artigo. </p></li>
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
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Campaign Classic]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Selecione o tipo de [!DNL Adobe Campaign Classic] gravar que deseja ler.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Digite do mapa a ID do registro que deseja ler.</td> 
  </tr> 
 <tr> 
   <td role="rowheader">[!UICONTROL Campos para incluir na saída] </td> 
   <td>Selecione os campos que deseja incluir na saída do módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos personalizados para incluir na saída]</td> 
   <td>Para cada campo personalizado que deseja incluir na saída, clique em <b>[!UICONTROL Adicionar]</b> e insira o nome do campo personalizado.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Assinar ou cancelar a assinatura]

Este módulo de ação assina um usuário ou cancela a assinatura de um usuário de um serviço de informação.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Campaign Classic]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assinar ou cancelar inscrição]</td> 
   <td>Selecione se deseja assinar ou cancelar a assinatura do serviço de informação.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Service name]</td> 
   <td>Selecione o serviço do qual deseja assinar ou cancelar a assinatura.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Endereço de email do destinatário] </td> 
   <td>Insira ou mapeie o endereço de email do usuário que deseja assinar ou cancelar a assinatura do serviço de informação.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar registro]

Este módulo de ação atualiza um único registro em [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Campaign Classic]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Selecione o tipo de [!DNL Adobe Campaign Classic] gravar que deseja criar.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Digite do mapa a ID do registro que deseja atualizar.</td> 
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

#### [!UICONTROL Pesquisar]

Esse módulo de pesquisa retorna registros com base nos critérios especificados.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Campaign Classic]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Selecione o tipo de [!DNL Adobe Campaign Classic] gravar que deseja criar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite] </td> 
   <td>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</td> 
  </tr> 
 </tbody> 
</table>
