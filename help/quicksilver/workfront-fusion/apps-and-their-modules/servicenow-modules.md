---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do ServiceNow
description: Em um [!DNL Adobe Workfront Fusion] cenário, é possível automatizar workflows que usam [!DNL ServiceNow], bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: b362cd8b-06b3-4f4c-b405-a2afc24abddb
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1613'
ht-degree: 1%

---

# [!DNL ServiceNow] módulos

Em um [!DNL Adobe Workfront Fusion] cenário, é possível automatizar workflows que usam [!DNL ServiceNow], bem como conectá-lo a vários aplicativos e serviços de terceiros.

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

Para usar [!DNL ServiceNow] módulos, você deve ter uma [!DNL ServiceNow] conta.

## Conectar [!DNL ServiceNow] para [!DNL Workfront Fusion]

Para criar uma conexão para o seu [!DNL ServiceNow] módulos:

1. Clique em **[!UICONTROL Adicionar]** ao lado da [!UICONTROL Conexão] ao começar a configurar o primeiro [!DNL ServiceNow] módulo.
1. Insira o seguinte:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nome da Conexão]</p> </td> 
      <td>Insira um nome para o novo [!DNL ServiceNow] conexão</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nome de Usuário]</p> </td> 
      <td>Insira seu [!DNL ServiceNow] usuário.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Senha]</p> </td> 
      <td>Digite sua senha do ServiceNow.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Instância]</p> </td> 
      <td> <p>Digite o endereço do seu [!DNL ServiceNow] conta sem <code>https://</code> (normalmente <code>&lt;company>.service-now.com</code>).</p> </td> 
     </tr> 
    </tbody> 
   </table>

## [!UICONTROL ServiceNow] módulos e seus campos

Ao configurar [!DNL ServiceNow] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL ServiceNow] Os campos podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>Se um registro personalizado for selecionado em um &quot;[!UICONTROL Tipo de registro]&quot;, pode levar algum tempo para carregar os campos personalizados.
>
>Se não houver registros personalizados, a lista suspensa ficará vazia.

* [[!UICONTROL Observar registros]](#watch-records)
* [[!UICONTROL Chamada de API personalizada]](#custom-api-call)
* [[!UICONTROL Ler um registro]](#read-a-record)
* [[!UICONTROL Desativar um usuário]](#deactivate-a-user)
* [[!UICONTROL Baixar um anexo]](#download-an-attachment)
* [[!UICONTROL Fazer upload de um anexo]](#upload-an-attachment)
* [[!UICONTROL Criar um registro]](#create-a-record)
* [[!UICONTROL Atualizar um registro]](#update-a-record)
* [[!UICONTROL Excluir um registro]](#delete-a-record)
* [[!UICONTROL Pesquisar registros]](#search-for-records)

### [!UICONTROL Observar registros]

Esse módulo acionador ativa um cenário quando um registro é criado ou atualizado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Conectar [!DNL ServiceNow] para o [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de tabela]</td> 
   <td>Selecione se a tabela que você deseja observar é uma tabela personalizada ou uma tabela padrão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Selecione o tipo de registro que deseja assistir.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Exibir]</td> 
   <td>Selecione o tipo de valores que deseja exibir.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td>Selecione os campos que devem ser gerados pelo módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td>Selecione se deseja observar novos registros ou registros atualizados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Chamada de API personalizada]

Esse módulo de ação permite fazer uma chamada autenticada personalizada para o [!DNL ServiceNow] API. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pelo outro [!DNL ServiceNow] módulos.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Conectar [!DNL ServiceNow] para o [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL relativa]</td> 
   <td> <p>Digite o endereço no servidor Web com o qual você deseja que o módulo interaja.</p> <p>Você pode digitar um URL relativo, o que significa que não é necessário incluir o protocolo (como <code>http://</code>) no início. Isso sugere ao servidor Web que a interação está ocorrendo no servidor.</p> <p>Por exemplo: <code>[!DNL /api/conversations].create</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   td&gt; <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formulário de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> </td> 
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

### [!UICONTROL Ler um registro]

Este módulo de ação lê uma [!DNL ServiceNow] registro usando a ID do sistema.

O módulo retorna quaisquer campos padrão associados ao registro, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Conectar [!DNL ServiceNow] para o [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do Sistema de Registros]</td> 
   <td>Insira ou mapeie o único [!DNL ServiceNow] ID do registro que você deseja que o módulo leia.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de tabela]</td> 
   <td>Selecione se o registro que deseja ler está em uma tabela personalizada ou em uma tabela padrão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Registro]</td> 
   <td>Selecione o tipo de [!DNL ServiceNow] registre que deseja que o módulo leia.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Exibir]</td> 
   <td>Selecione o tipo de valores que deseja exibir.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td>Selecione os campos que devem ser gerados pelo módulo.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Desativar um usuário]

Este módulo de ação desativa um usuário no [!DNL ServiceNow] usando a ID do sistema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Conectar [!DNL ServiceNow] para o [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Sistema do Usuário]</td> 
   <td> Insira ou mapeie o único [!DNL ServiceNow] ID do usuário que você deseja que o módulo desative.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Baixar um anexo]

Este módulo de ação baixa um anexo em um [!DNL ServiceNow] registro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Conectar [!DNL ServiceNow] para o [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do Sistema de Anexo]</td> 
   <td> Insira ou mapeie o único [!DNL ServiceNow] ID do anexo que você deseja que o módulo baixe.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Fazer upload de um anexo]

Este módulo de ação faz upload de um anexo em um [!DNL ServiceNow] registro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Conectar [!DNL ServiceNow] para o [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome da tabela]</td> 
   <td>Insira ou mapeie o nome da tabela na qual deseja fazer upload do anexo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Sistema]</td> 
   <td>Insira ou mapeie o único [!DNL ServiceNow] ID do sistema no qual você deseja fazer upload do anexo.</td> 
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

Este módulo de ação cria um novo [!DNL ServiceNow] registro.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Conectar [!DNL ServiceNow] para o [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de tabela]</td> 
   <td>Selecione se deseja criar um registro em uma tabela personalizada ou em uma tabela padrão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Registro]</td> 
   <td>Selecione o tipo de [!DNL ServiceNow] registro que você deseja que o módulo crie. Em seguida, é possível preencher os campos disponíveis para esse tipo de registro.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Atualizar um registro]

Este módulo de ação cria um novo [!DNL ServiceNow] registro.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Conectar [!DNL ServiceNow] para o [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do Sistema de Registros]</td> 
   <td>Insira ou mapeie o único [!DNL ServiceNow] ID do registro que você deseja que o módulo atualize.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de tabela]</td> 
   <td>Selecione se o registro que deseja atualizar é uma tabela personalizada ou uma tabela padrão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Registro]</td> 
   <td>Selecione o tipo de [!DNL ServiceNow] registro que você deseja que o módulo atualize. Em seguida, é possível preencher os campos disponíveis para esse tipo de registro.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Excluir um registro]

Este módulo de ação exclui um incidente ou um usuário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Conectar [!DNL ServiceNow] para o [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Registro]</td> 
   <td>Selecione se deseja deletar um incidente ou um usuário.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Sistema]</td> 
   <td>Insira ou mapeie o único [!DNL ServiceNow] ID do registro que você deseja que o módulo exclua.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Pesquisar registros]

Este módulo procura por registros usando os critérios que você selecionar.

O módulo retorna quaisquer campos padrão associados ao registro, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Conectar [!DNL ServiceNow] para o [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de tabela]</td> 
   <td>Selecione se a tabela que você deseja pesquisar é uma tabela personalizada ou uma tabela padrão.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Selecione o tipo de registro que deseja pesquisar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conjunto de resultados]</td> 
   <td>Selecione se deseja que o módulo retorne todos os registros que correspondem aos critérios ou apenas o primeiro registro que corresponda a ele. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contagem máxima de registros]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de pesquisa]</td> 
   <td> <p>Selecione o tipo de pesquisa que deseja que o módulo execute</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Consulta avançada]</strong> </p> 
      <ul> 
       <li> <p>[!UICONTROL Pesquisar Consulta]</p> <p>Insira a consulta de pesquisa personalizada. Para obter informações sobre [!DNL ServiceNow] consultas de pesquisa personalizadas, consulte a <a href="https://docs.servicenow.com/bundle/orlando-platform-user-interface/page/use/common-ui-elements/reference/r_OpAvailableFiltersQueries.html">Documentação de consulta do ServiceNow</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Simples]</strong> </p> 
      <ul> 
       <li> <p>[!UICONTROL Critérios de Pesquisa]</p> <p>Informe os critérios pelos quais deseja que o módulo pesquise. Para obter mais informações sobre a configuração de filtros de pesquisa, consulte <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Adicionar um filtro a um cenário no Adobe Workfront Fusion</a>.</p> </li> 
       <li> <p>[!UICONTROL Classificar por]</p> <p>Indique por qual campo você deseja que o módulo classifique os resultados e se eles devem ser classificados em ordem crescente ou decrescente.</p> </li> 
      </ul> </li> 
    </ul> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Exibir]</td> 
   <td>Selecione o tipo de valores que deseja exibir.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td>Selecione os campos que devem ser gerados pelo módulo.</td> 
  </tr> 
 </tbody> 
</table>
