---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do ServiceNow
description: Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL ServiceNow], bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: b362cd8b-06b3-4f4c-b405-a2afc24abddb
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1565'
ht-degree: 0%

---

# [!DNL ServiceNow] módulos

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL ServiceNow], bem como conectá-lo a vários aplicativos e serviços de terceiros.

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

Para usar [!DNL ServiceNow] módulos, você deve ter um [!DNL ServiceNow] conta.

## Connect [!DNL ServiceNow] para [!DNL Workfront Fusion]

Para criar uma conexão para [!DNL ServiceNow] módulos:

1. Clique em **[!UICONTROL Adicionar]** ao lado do [!UICONTROL Conexão] ao começar a configurar o primeiro [!DNL ServiceNow] módulo.
1. Insira o seguinte:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nome da conexão]</p> </td> 
      <td>Insira um nome para o novo [!DNL ServiceNow] conexão</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nome de usuário]</p> </td> 
      <td>Insira seu [!DNL ServiceNow] nome de usuário.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Senha]</p> </td> 
      <td>Insira a senha do ServiceNow.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Instância]</p> </td> 
      <td> <p>Insira o endereço do [!DNL ServiceNow] sem <code>https://</code> (normalmente <code>&lt;company>.service-now.com</code>).</p> </td> 
     </tr> 
    </tbody> 
   </table>

## [!UICONTROL ServiceNow] módulos e seus campos

Ao configurar [!DNL ServiceNow] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL ServiceNow] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>Se um registro personalizado for selecionado em um &quot;[!UICONTROL Tipo de registro]&quot;, pode levar algum tempo para carregar os campos personalizados.
>
>Se não houver registros personalizados, a lista suspensa ficará vazia.

* [[!UICONTROL Registros de monitoramento]](#watch-records)
* [[!UICONTROL Chamada da API personalizada]](#custom-api-call)
* [[!UICONTROL Ler um registro]](#read-a-record)
* [[!UICONTROL Desativar um usuário]](#deactivate-a-user)
* [[!UICONTROL Baixar um anexo]](#download-an-attachment)
* [[!UICONTROL Fazer upload de um anexo]](#upload-an-attachment)
* [[!UICONTROL Criar um registro]](#create-a-record)
* [[!UICONTROL Atualizar um registro]](#update-a-record)
* [[!UICONTROL Excluir um registro]](#delete-a-record)
* [[!UICONTROL Procurar registros]](#search-for-records)

### [!UICONTROL Registros de monitoramento]

Esse módulo de acionador ativa um cenário quando um registro é criado ou atualizado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] para [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de tabela]</td> 
   <td>Selecione se a tabela que deseja visualizar é uma tabela personalizada ou uma tabela padrão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Selecione o tipo de registro que deseja assistir.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Exibição]</td> 
   <td>Selecione o tipo de valor que deseja exibir.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td>Selecione os campos que o módulo deve exibir.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td>Selecione se deseja assistir a novos registros ou registros atualizados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Chamada da API personalizada]

Esse módulo de ação permite que você faça uma chamada autenticada personalizada para o [!DNL ServiceNow] API. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pela outra [!DNL ServiceNow] módulos.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] para [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL relativo]</td> 
   <td> <p>Digite o endereço no servidor da Web com o qual você deseja que o módulo interaja.</p> <p>Você pode digitar um URL relativo, o que significa que não é necessário incluir o protocolo (como <code>http://</code>no início. Isso sugere ao servidor da Web que a interação está ocorrendo no servidor.</p> <p>Por exemplo: <code>[!DNL /api/conversations].create</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   td&gt; <p>Selecione o método de solicitação HTTP que você precisa configurar a chamada da API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> </td> 
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

### [!UICONTROL Ler um registro]

Esse módulo de ação lê um [!DNL ServiceNow] registre usando a ID do sistema.

O módulo retorna quaisquer campos padrão associados ao registro, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] para [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Registrar ID do sistema]</td> 
   <td>Insira ou mapeie a [!DNL ServiceNow] ID do registro que você deseja que o módulo leia.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de tabela]</td> 
   <td>Selecione se o registro que deseja ler está em uma tabela personalizada ou padrão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Selecione o tipo de [!DNL ServiceNow] registre que deseja que o módulo leia.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Exibição]</td> 
   <td>Selecione o tipo de valor que deseja exibir.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td>Selecione os campos que o módulo deve exibir.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Desativar um usuário]

Esse módulo de ação desativa um usuário em [!DNL ServiceNow] usando a ID do sistema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] para [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do sistema do usuário]</td> 
   <td> Insira ou mapeie a [!DNL ServiceNow] ID do usuário que você deseja que o módulo seja desativado.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Baixar um anexo]

Este módulo de ação baixa um anexo em um [!DNL ServiceNow] gravar.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] para [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Attachment System ID]</td> 
   <td> Insira ou mapeie a [!DNL ServiceNow] ID do anexo que você deseja que o módulo baixe.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Fazer upload de um anexo]

Este módulo de ação carrega um anexo em um [!DNL ServiceNow] gravar.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] para [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome da tabela]</td> 
   <td>Insira ou mapeie o nome da tabela onde deseja fazer upload do anexo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do sistema]</td> 
   <td>Insira ou mapeie a [!DNL ServiceNow] ID do Sistema no qual você deseja fazer upload do anexo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do arquivo]</td> 
   <td>Inserir ou mapear um nome para o anexo</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conteúdo do arquivo]</td> 
   <td>Insira ou mapeie o arquivo para o qual você deseja fazer upload [!DNL ServiceNow].</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Criar um registro]

Esse módulo de ação cria um novo [!DNL ServiceNow] gravar.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] para [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de tabela]</td> 
   <td>Selecione se deseja criar um registro em uma tabela personalizada ou padrão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Selecione o tipo de [!DNL ServiceNow] registre que deseja que o módulo crie. Em seguida, é possível preencher os campos disponíveis para esse tipo de registro.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Atualizar um registro]

Esse módulo de ação cria um novo [!DNL ServiceNow] gravar.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] para [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Registrar ID do sistema]</td> 
   <td>Insira ou mapeie a [!DNL ServiceNow] ID do registro que você deseja que o módulo atualize.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de tabela]</td> 
   <td>Selecione se o registro deseja atualizar está em uma tabela personalizada ou padrão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Selecione o tipo de [!DNL ServiceNow] registre que deseja que o módulo seja atualizado. Em seguida, é possível preencher os campos disponíveis para esse tipo de registro.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Excluir um registro]

Esse módulo de ação exclui um incidente ou um usuário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] para [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Selecione se deseja excluir um incidente ou um usuário.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do sistema]</td> 
   <td>Insira ou mapeie a [!DNL ServiceNow] ID do registro que você deseja que o módulo exclua.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Procurar registros]

Esse módulo pesquisa registros usando critérios selecionados.

O módulo retorna quaisquer campos padrão associados ao registro, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] para [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de tabela]</td> 
   <td>Selecione se a tabela que deseja pesquisar é uma tabela personalizada ou padrão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Selecione o tipo de registro que deseja pesquisar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conjunto de resultados]</td> 
   <td>Selecione se deseja que o módulo retorne todos os registros que correspondam aos critérios ou somente o primeiro registro a corresponder a ele. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contagem máxima de registros]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de pesquisa]</td> 
   <td> <p>Selecione o tipo de pesquisa que deseja que o módulo execute</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Advanced query]</strong> </p> 
      <ul> 
       <li> <p>[!UICONTROL Consulta de pesquisa]</p> <p>Insira a consulta de pesquisa personalizada. Para obter informações sobre [!DNL ServiceNow] consultas de pesquisa personalizadas, consulte o <a href="https://docs.servicenow.com/bundle/orlando-platform-user-interface/page/use/common-ui-elements/reference/r_OpAvailableFiltersQueries.html">Documentação de consulta do ServiceNow</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Simples]</strong> </p> 
      <ul> 
       <li> <p>[!UICONTROL Critérios de pesquisa]</p> <p>Insira os critérios pelos quais deseja que o módulo pesquise. Para obter mais informações sobre como configurar filtros de pesquisa, consulte <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Adicionar um filtro a um cenário no Adobe Workfront Fusion</a>.</p> </li> 
       <li> <p>[!UICONTROL Classificar por]</p> <p>Indique em qual campo você deseja que o módulo classifique os resultados e se eles devem ser classificados em ordem crescente ou decrescente.</p> </li> 
      </ul> </li> 
    </ul> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Exibição]</td> 
   <td>Selecione o tipo de valor que deseja exibir.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td>Selecione os campos que o módulo deve exibir.</td> 
  </tr> 
 </tbody> 
</table>
