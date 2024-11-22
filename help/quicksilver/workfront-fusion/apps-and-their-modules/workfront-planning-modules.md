---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Adobe Workfront Planning
description: Com os  [!DNL Adobe Workfront Planning] módulos, você pode iniciar um [!DNL Adobe Workfront Fusion] cenário com base nos eventos da sua [!DNL Adobe] conta do Workfront Planning, criar, ler ou atualizar contratos e outros registros, pesquisar registros usando critérios definidos por você e carregar documentos.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 892fdaf3-935e-4e66-a01c-9e9b6e0daf3e
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 0%

---

# [!DNL Adobe Workfront Planning] módulos

Com os módulos [!DNL Adobe Workfront Planning], é possível acionar um cenário quando os eventos ocorrem no Workfront Planning. Você também pode criar, ler, atualizar e excluir registros ou executar uma chamada de API personalizada para sua conta do [!DNL Adobe Workfront Planning].

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
   <p>Requisito atual do produto: se você tiver o plano [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], sua organização deve comprar [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Informações da API do Adobe Workfront Planning

O conector do Adobe Workfront Planning usa o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL base</td> 
   <td>https://&lbrace;&lbrace;connection.host&rbrace;&rbrace;/maestro/api/&lbrace;&lbrace;common.maestroApiVersion&rbrace;&rbrace;/</td> 
  </tr>
  <tr> 
   <td role="rowheader">Tag da API</td> 
   <td>v1.13.7</td> 
  </tr>
 </tbody> 
 </table>

## Criar uma conexão com [!DNL Adobe Workfront Planning]

Você pode criar uma conexão com sua conta do [!DNL Workfront Planning] diretamente de dentro de um módulo do [!DNL Workfront Fusion].

1. Em qualquer módulo [!DNL Adobe Workfront Planning], clique em **[!UICONTROL Adicionar]** ao lado da caixa Conexão.

1. Preencha os seguintes campos:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Nome da Conexão]</td>
          <td>
            <p>Insira um nome para esta conexão.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Ambiente]</td>
          <td>Selecione se você está se conectando a um ambiente de produção ou não produção.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Tipo]</td>
          <td>Selecione se você deseja se conectar a uma conta de serviço ou a uma conta pessoal.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID do Cliente]<p>(Opcional)</p></td>
          <td>Insira sua [!DNL Adobe] [!UICONTROL ID do Cliente]. Isso pode ser encontrado na seção [!UICONTROL Credentials details] do [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Segredo do Cliente]<p>(Opcional)</p></td>
          <td>Insira seu [!DNL Adobe] [!UICONTROL Segredo do Cliente]. Isso pode ser encontrado na seção [!UICONTROL Credentials details] do [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL URL de Autenticação]<p>(Opcional)</p></td>
          <td>Insira o URL que sua instância do Workfront usará para autenticar essa conexão. <p>O valor padrão é <code>https://oauth.my.workfront.com/integrations/oauth2</code>.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Prefixo de host]</td>
          <td>Insira seu prefixo de host.<p>O valor padrão é <code>origin-</code>.</p>
        </tr>
      </tbody>
    </table>
1. Clique em **[!UICONTROL Continuar]** para salvar a conexão e retornar ao módulo.

## [!DNL Adobe Workfront Planning] módulos e seus campos

### Triggers

#### Assistir a eventos

Este módulo de acionamento inicia um cenário quando um registro, tipo de registro ou espaço de trabalho é criado, atualizado ou excluído no Workfront Planning.

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
      <td>Para obter instruções sobre como criar uma conexão com [!DNL Adobe Workfront Planning], consulte <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Workfront Planning]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo de objeto]</td>
      <td>Selecione se deseja observar registros, tipos de registro ou espaços de trabalho.</td>
    </tr>
     <tr data-mc-conditions=""> 
      <td> <p>[!UICONTROL Eventos filtros]</p> </td> 
      <td> <p>É possível definir filtros para observar apenas os registros que atendem aos critérios selecionados.</p> <p>Para cada filtro, insira o campo que deseja que o filtro avalie, o operador e o valor que deseja que o filtro permita. Você pode usar mais de um filtro adicionando regras AND.</p> <p>Observação: não é possível editar filtros em webhooks [!DNL Workfront] existentes. Para configurar filtros diferentes para assinaturas de evento [!DNL Workfront], remova o webhook atual e crie um novo.</p> <p>Para obter mais informações sobre filtros de evento, consulte <a href="/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#event-subscription-filters-in-the-workfront--watch-events-modules" class="MCXref xref">Filtros de assinatura de evento nos módulos [!DNL Workfront] &gt; [!UICONTROL Watch Events]</a> no artigo sobre módulos do Workfront.</p> </td> 
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

### Ações

* [Excluir um tipo de registro](#delete-a-record-type)
* [Fazer uma chamada de IA personalizada](#make-a-custom-api-call)

#### Excluir um tipo de registro

Este módulo de ação exclui um único tipo de registro no Workfront Planning por sua ID.

>[!WARNING]
>
>A exclusão de um tipo de registro no Workfront Planning também exclui todos os registros na tabela de tipo de registro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com [!DNL Adobe Workfront Planning], consulte <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Workfront Planning]</a> neste artigo.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL ID de tipo de registro]</p>
      </td>
      <td>Insira ou mapeie a ID do campo que deseja excluir.</td> 
      </tr>
  </tbody>
</table>

#### Fazer uma chamada de API personalizada

Este módulo faz uma chamada de API personalizada para a API [!DNL Adobe Workfront Planning].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com [!DNL Adobe Workfront Planning], consulte <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Workfront Planning]</a> neste artigo.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL]</p>
      </td>
      <td>
        <p>Insira um caminho relativo a <code>https://(YOUR_WORKFRONT_DOMAIN)/maestro/api/</code></p>
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
   <td> <p>Adicione o conteúdo do corpo para a chamada à API na forma de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar instruções condicionais como <code>if</code> em seu JSON, coloque as aspas fora da instrução condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

<!--
### Searches

#### Search records

This action module retrieves a list of records based on criteria you specify.

-->

### Sem categoria


#### Criar um registro

Essa ação cria um único registro no Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com [!DNL Adobe Workfront Planning], consulte <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Workfront Planning]</a> neste artigo.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL ID de tipo de registro]</p>
      </td>
      <td>Insira ou mapeie o tipo de registro que deseja criar. Os tipos de registro disponíveis baseiam-se na sua conta do Workfront Planning.</td> 
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

Este módulo de ação exclui o registro especificado no Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com [!DNL Adobe Workfront Planning], consulte <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Workfront Planning]</a> neste artigo.</td>
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

This action module retrieves all records from an [!DNL Adobe Workfront Planning] account.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Workfront Planning], see <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Create a connection to [!DNL Adobe Workfront Planning]</a> in this article.</td>
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

Este módulo de ação recupera um único registro de [!DNL Adobe Workfront Planning], especificado por sua ID.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com [!DNL Adobe Workfront Planning], consulte <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Workfront Planning]</a> neste artigo.</td>
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
      <td>Para obter instruções sobre como criar uma conexão com [!DNL Adobe Workfront Planning], consulte <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Workfront Planning]</a> neste artigo.</td>
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

Este módulo de ação recupera uma lista de tipos de registros em uma conta [!DNL Adobe Workfront Planning].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com [!DNL Adobe Workfront Planning], consulte <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Workfront Planning]</a> neste artigo.</td>
    </tr>
  </tbody>
</table>

### Atualizar registro

Essa ação atualiza um único registro no Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com [!DNL Adobe Workfront Planning], consulte <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Workfront Planning]</a> neste artigo.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL ID de Registro]</p>
      </td>
      <td>Insira ou mapeie o tipo de registro que deseja atualizar. Os tipos de registro disponíveis baseiam-se na sua conta do Workfront Planning.</td> 
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
