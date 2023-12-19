---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Adobe Maestri
description: Com o [!DNL Adobe Maestro] módulos, você pode iniciar um [!DNL Adobe Workfront Fusion] cenário com base em eventos no seu [!DNL Adobe] Maestri conta, criar, ler ou atualizar contratos e outros registros, pesquisar registros usando critérios que você definiu e fazer upload de documentos.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
source-git-commit: fe0c867b218879c1d0d969112eb62878782a40ad
workflow-type: tm+mt
source-wordcount: '1007'
ht-degree: 0%

---

# [!DNL Adobe Maestro] módulos

Com o [!DNL Adobe Maestro] você pode acionar um cenário quando eventos ocorrem no Maestro. Você também pode criar, ler, atualizar e excluir registros ou executar uma chamada de API personalizada para o [!DNL Adobe Maestro] conta.

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

## Criar uma conexão com o [!DNL Adobe Maestro]

Você pode criar uma conexão com o seu [!DNL Maestro] conta diretamente de dentro de um [!DNL Workfront Fusion] módulo.

1. Em qualquer [!DNL Maestro] módulo de aplicativo, clique em **[!UICONTROL Adicionar]** ao lado da [!UICONTROL Conexão] caixa.
1. Insira um nome para esta conexão.
1. Selecione se você deseja se conectar a um ambiente de produção ou a um ambiente de não produção.
1. Selecione se você está se conectando a uma conta de serviço ou a uma conta pessoal.
1. Clique em **[!UICONTROL Login do SAML]** para criar a conexão e voltar ao módulo.

## [!DNL Adobe Maestro] módulos e seus campos

### Assistir a eventos

Este módulo de acionamento inicia um cenário quando um registro, tipo de registro ou espaço de trabalho é criado, atualizado ou excluído no Maestro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Webhook]</td>
      <td>Selecione o webhook que deseja usar ou clique em Adicionar para criar um novo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Maestro], consulte <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Maestro]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo de objeto]</td>
      <td>Selecione se deseja observar registros, tipos de registro ou espaços de trabalho.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Objetos a serem observados]</td>
      <td>Selecione se você deseja observar novos. registros atualizados, novos e atualizados ou excluídos.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Excluir atualizações feitas por esta conexão]</p>
      </td>
      <td>Habilite esta opção para impedir que o cenário seja acionado quando uma alteração for feita pela conexão usada por este módulo. Isso impede que outra instância do cenário seja acionada se esse cenário executar uma ação de acionamento.</td> 
      </tr>
  </tbody>
</table>

### Excluir um tipo de registro

Este módulo de ação exclui um único tipo de registro no Maestri por sua ID.

>[!WARNING]
>
>A exclusão de um tipo de registro no Maestro também exclui todos os registros na tabela de tipo de registro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Maestro], consulte <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Maestro]</a> neste artigo.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL ID de tipo de registro]</p>
      </td>
      <td>Insira ou mapeie a ID do campo que deseja excluir.</td> 
      </tr>
  </tbody>
</table>

### Fazer uma chamada de API personalizada

Esse módulo faz uma chamada de API personalizada para o [!DNL Adobe Maestro] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Maestro], consulte <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Maestro]</a> neste artigo.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Caminho]</p>
      </td>
      <td>
        <p>Insira um caminho relativo a https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</p>
      </td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL versão da API]</p>
      </td>
      <td>
        <p>Selecione a versão da API que deseja usar. Se você não selecionar uma versão, a versão mais recente será usada por padrão.</p>
      </td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Substituição de Caminho de API]</p>
      </td>
      <td>
        <p>Insira um caminho relativo a https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Método]</p>
      </td>
   <td> <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cabeçalhos]</td>
      <td>
        <p>Adicione os cabeçalhos da solicitação no formulário de um objeto JSON padrão.</p>
        <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] O adiciona cabeçalhos de autorização automaticamente.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cadeia de Consulta]  </td>
      <td>
        <p>Para cada par de chave/valor que você deseja adicionar à sequência de consulta, clique em <b>Adicionar item</b> e insira a chave e o valor.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Corpo]</td>
   <td> <p>Adicione o conteúdo do corpo para a chamada à API na forma de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

<!--

### Delete a field

This action module deletes a single field in Maestro by its ID.

>[!WARNING]
>
>Deleting a field in Maestro deletes it and any data in it from every object of that record type in Maestro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Field ID]</p>
      </td>
      <td>Enter or map the ID of the record type you want to delete.</td> 
      </tr>
  </tbody>
</table>

### Get a field 


This action module retrieves a single field in Maestro by its ID.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Field ID]</p>
      </td>
      <td>Enter or map the ID of the field you want to delete.</td> 
      </tr>
  </tbody>
</table>

-->

### Criar um registro

Esta ação cria um único registro no Maestro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Maestro], consulte <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Maestro]</a> neste artigo.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL ID de tipo de registro]</p>
      </td>
      <td>Insira ou mapeie o tipo de registro que deseja criar. Os tipos de registros disponíveis são baseados em sua conta do Maestro.</td> 
      </tr>
     <tr>
      <td role="rowheader">
        <p>Outros campos</p>
      </td>
      <td>Esses campos se baseiam no tipo de registro selecionado.</td> 
      </tr>
     <tr>
  </tbody>
</table>

### Excluir um registro

Este módulo de ação exclui o registro especificado no Maestro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Maestro], consulte <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Maestro]</a> neste artigo.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL ID de Registro]</p>
      </td>
      <td>Informe ou mapeie a ID do registro que deseja deletar.</td> 
      </tr>
  </tbody>
</table>

<!--

### Get all records

This action module retrieves all records from an [!DNL Adobe Maestro] account.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned records]</p>
      </td>
      <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td> 
      </tr>
  </tbody>
</table>

-->

### Obter um registro

Este módulo de ação recupera um único registro de [!DNL Adobe Maestro], especificado por sua ID.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Maestro], consulte <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Maestro]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Registro]</td>
      <td>Insira ou mapeie a ID do registro que deseja recuperar.</td>
    </tr>
  </tbody>
</table>

### Obter registros por tipo de registro

Este módulo de ação recupera todos os registros do tipo especificado.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Maestro], consulte <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Maestro]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Selecione ou mapeie o espaço de trabalho que contém os registros que deseja recuperar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo de registro]</td>
      <td>Selecione o tipo de registro que deseja recuperar.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Número máximo de registros retornados]</p>
      </td>
      <td>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</td> 
  </tbody>
</table>

### Obter tipos de registro

Este módulo de ação recupera uma lista de tipos de registros em um [!DNL Adobe Maestro] conta.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Maestro], consulte <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Maestro]</a> neste artigo.</td>
    </tr>
  </tbody>
</table>

### Atualizar registro

Esta ação atualiza um único registro no Maestro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Maestro], consulte <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Maestro]</a> neste artigo.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL ID de Registro]</p>
      </td>
      <td>Insira ou mapeie o tipo de registro que deseja atualizar. Os tipos de registros disponíveis são baseados em sua conta do Maestro.</td> 
      </tr>
     <tr>
      <td role="rowheader">
        <p>Outros campos</p>
      </td>
      <td>Esses campos se baseiam no tipo de registro selecionado.</td> 
      </tr>
     <tr>
  </tbody>
</table>

### Pesquisar registros

Este módulo de ação recupera uma lista de registros com base nos critérios que você especificar.

>[!NOTE]
>
>Este módulo está em construção.

