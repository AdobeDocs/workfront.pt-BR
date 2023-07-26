---
filename: adobe-journey-optimizer-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos do Adobe Journey Optimizer
description: Em um [!DNL Adobe Workfront Fusion] cenário, é possível automatizar workflows que usam [!DNL Adobe Journey Optimizer], bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: 2c1aea46-edbf-42a3-a6e9-f8aea042a48d
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '1602'
ht-degree: 0%

---

# [!DNL Adobe Journey Optimizer] Módulos

<!--
Becky: pull from main, add to TOCs, then push to merge.
-->

Em um [!DNL Adobe Workfront Fusion] cenário, é possível automatizar workflows que usam [!DNL Adobe Journey Optimizer], bem como conectá-lo a vários aplicativos e serviços de terceiros. [!DNL Adobe Journey Optimizer] permitem criar, ler, atualizar ou excluir registros, ou executar uma chamada de API personalizada para o [!DNL Adobe Journey Optimizer] API.


Se precisar de instruções sobre como criar um cenário, consulte [Criar um cenário](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obter informações sobre módulos, consulte [Módulos no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plano*</td>
      <td>
        <p>[!UICONTROL Pro] ou superior</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] licença*</td>
      <td>
        <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p>
      </td>
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

Antes de poder usar o [!DNL Adobe Journey Optimizer] deve garantir que os seguintes pré-requisitos sejam atendidos:

* Você deve ter um ativo [!DNL Adobe Journey Optimizer] conta.

## Criar uma conexão com o [!DNL Adobe Journey Optimizer]

Para criar uma conexão para o seu [!DNL Adobe Journey Optimizer] módulos:

1. Em qualquer [!DNL Adobe Journey Optimizer] , clique em **[!UICONTROL Adicionar]** ao lado da caixa Conexão.

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
          <td role="rowheader">[!UICONTROL ID do Cliente]</td>
          <td>Insira seu [!DNL Adobe] [!UICONTROL ID do Cliente]. Isso pode ser encontrado na seção [!UICONTROL Credenciais detalhes] do [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Segredo do Cliente]</td>
          <td>Insira seu [!DNL Adobe] [!UICONTROL Segredo do Cliente]. Isso pode ser encontrado na seção [!UICONTROL Credenciais detalhes] do [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID da conta técnica]</td>
          <td>Insira seu [!DNL Adobe] [!UICONTROL ID da conta técnica]. Isso pode ser encontrado na seção [!UICONTROL Credenciais detalhes] do [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID da Organização]</td>
          <td>Insira seu [!DNL Adobe] [!UICONTROL ID da Organização]. Isso pode ser encontrado na seção [!UICONTROL Credenciais detalhes] do [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Metaescopos]</td>
          <td>
            Insira todos os metaescopos necessários para a conexão.
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Chave privada]</td>
          <td>
            <p>Insira a chave privada que foi gerada quando suas credenciais foram criadas na [!DNL Adobe Developer Console]. </p>
            <p>Para extrair sua chave privada ou certificado:</p>
            <ol>
              <li value="1">
                <p>Clique em <b>[!UICONTROL Extract]</b>.</p>
              </li>
              <li value="2">
                <p>Selecione o tipo de arquivo que você está extraindo.</p>
              </li>
              <li value="3">
                <p>Selecione o arquivo que contém a chave privada ou o certificado.</p>
              </li>
              <li value="4">
                <p>Digite a senha do arquivo.</p>
              </li>
              <li value="5">
                <p>Clique em <b>[!UICONTROL Salvar]</b> para extrair o arquivo e retornar à configuração da conexão.</p>
              </li>
            </ol>
          </td>
        </tr>
      </tbody>
    </table>
1. Clique em **[!UICONTROL Continuar]** para salvar a conexão e retornar ao módulo.

## [!DNL Adobe Journey Optimizer] módulos e seus campos

Ao configurar [!DNL Adobe Journey Optimizer] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Adobe Journey Optimizer] Os campos podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Ações](#actions)
* [Pesquisas](#searches)

### Ações

* [[!UICONTROL Criar um registro]](#create-a-record)
* [[!UICONTROL Fazer uma chamada de API personalizada]](#make-a-custom-api-call)
* [[!UICONTROL Excluir um registro]](#delete-a-record)
* [[!UICONTROL Atualizar um registro]](#update-a-record)

#### [!UICONTROL Criar um registro]

Esse módulo de ação cria uma oferta de posicionamento, regra de decisão, tag, oferta personalizada, coleção ou oferta substituta.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
     <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Journey Optimizer], consulte <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Journey Optimizer]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Tipo de registro]
      </td>
      <td>
        Selecione o tipo de registro que deseja criar
        <ul>
        <li><b>[!UICONTROL Posicionamento]</b>: Continue para <a href="#placement-fields" >Campos de [!UICONTROL Posicionamento]</a>.</li>
        <li><b>[!UICONTROL Regra de decisão]</b>: Continue para <a href="#decision-rule-fields" >Campos da [!UICONTROL Decision rule]</a>.</li>
        <li><b>[!UICONTROL Decisão]</b>: Continue para <a href="#decision-fields" >Campos de [!UICONTROL Decision]</a>.</li>
        <li><b>[!UICONTROL Marca]</b>: Continue para <a href="#tag-fields" >Campos de [!UICONTROL Tag]</a>.</li>
        <li><b>[!UICONTROL Coleção]</b>: Continue para <a href="#collection-fields" >Campos de [!UICONTROL Collection]</a>.</li>
        <li><b>[!UICONTROL Oferta substituta]</b>: Continue para <a href="#fallback-offer-fields" >Campos de [!UICONTROL oferta substituta]</a>.</li>
        <li><b>[!UICONTROL Oferta personalizada]</b>: Continue para <a href="#personalized-offer-fields" >Campos de [!UICONTROL Oferta personalizada]</a>.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Posicionamento] campos

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Nome]</td>
     <td>Insira ou mapeie um nome para o posicionamento.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Descrição]
      </td>
      <td>Insira ou mapeie uma descrição para o posicionamento.
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL Regra de decisão] campos

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Nome]</td>
     <td>Insira ou mapeie um nome para a regra de descrição.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Descrição]
      </td>
      <td>Insira ou mapeie uma descrição para a regra de decisão.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Condição]
      </td>
      <td>Insira ou mapeie a condição da regra de decisão.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Decisão] campos

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Nome]</td>
     <td>Insira ou mapeie um nome para a regra de descrição.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Status]</td>
      <td>Selecione o status da decisão.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Data de início]</td>
      <td><p>Insira ou mapeie a data de início da decisão.</p><p>Para obter uma lista de formatos de data compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerção de tipo em [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Data de término]</td>
      <td><p>Insira ou mapeie a data final da decisão.</p><p>Para obter uma lista de formatos de data compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerção de tipo em [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Posicionamentos]</td>
      <td>Selecionar os posicionamentos a serem adicionados a esta decisão
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Coleção]</td>
      <td>Selecione a coleção de ofertas que contém as ofertas que esta decisão considerará.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Oferta substituta]</td>
      <td>Selecione a oferta substituta que será apresentada aos clientes que não correspondem às regras desta decisão.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Tag] campos

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Nome]</td>
     <td>Insira ou mapeie um nome para a tag.</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Coleção] campos

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Nome]</td>
     <td>Insira ou mapeie um nome para a coleção.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Tipo de Filtro]
      </td>
      <td>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Elementos]
      </td>
      <td>Selecione as tags que serão incluídas na coleção.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Oferta substituta] campos

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Nome]</td>
     <td>Insira ou mapeie um nome para a oferta substituta.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Status]
      </td>
      <td> Selecione o status da oferta substituta.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Posicionamento]
      </td>
      <td>Insira ou mapeie o posicionamento para a oferta substituta.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Oferta personalizada] campos

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Nome]</td>
     <td>Insira ou mapeie um nome para a regra de descrição.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Status]</td>
      <td>Selecione o status da decisão.
      </td>
    </tr>
    <tr>
      <td role="rowheader">Posicionamento</td>
      <td>Selecione o posicionamento para a oferta personalizada.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Data de início]</td>
      <td><p>Insira ou mapeie a data de início da oferta personalizada.</p><p>Para obter uma lista de formatos de data compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerção de tipo em [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Data de término]</td>
      <td><p>Insira ou mapeie a data final da oferta personalizada.</p><p>Para obter uma lista de formatos de data compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerção de tipo em [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Regras de decisão]</td>
      <td>Selecione as regras de decisão a serem adicionadas a esta oferta personalizada.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Prioridade]</td>
      <td>Selecione a prioridade desta oferta. A prioridade afeta se esta oferta será apresentada em vez de outra oferta.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Restrição de limite]</td>
      <td>Insira ou mapeie o número de vezes que esta oferta será apresentada.
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Excluir um registro]

Este módulo de ação exclui um único registro em [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
     <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Journey Optimizer], consulte <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Journey Optimizer]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Tipo de registro]
      </td>
      <td>
        Selecione o tipo de registro que deseja excluir
        <ul>
        <li>[!UICONTROL Posicionamento]</li>
        <li>[!UICONTROL Regra de decisão]</li>
        <li>[!UICONTROL Decisão]</li>
        <li>[!UICONTROL Marca]</li>
        <li>[!UICONTROL Coleção]</li>
        <li>[!UICONTROL Oferta substituta]</li>
        <li>[!UICONTROL Oferta personalizada]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Posicionamento]/[!UICONTROL Regra de decisão]/[!UICONTROL Decisão]/[!UICONTROL Marca]/[!UICONTROL Coleção]/[!UICONTROL Oferta de fallback]/[!UICONTROL Oferta personalizada]
      </td>
      <td>
        Selecione o registro que deseja excluir.
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL Fazer uma chamada de API personalizada]

Esse módulo faz uma chamada de API personalizada para o [!DNL Adobe Journey Optimizer] API

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Conexão]</td>
     <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Journey Optimizer], consulte <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Journey Optimizer]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Caminho]</p>
      </td>
      <td>
        <p>Insira um caminho relativo a {baseURL} começando com<code>/</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Método]</p>
      </td>
      <td>
   <td> <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cabeçalhos]</td>
      <td>
        <p>Adicione os cabeçalhos da solicitação no formulário de um objeto JSON padrão.</p>
        <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p>
        <p>O Workfront Fusion adiciona cabeçalhos de autorização e cabeçalhos x-api-key automaticamente.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cadeia de Consulta]  </td>
      <td>
        <p>Insira a string de consulta da solicitação.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Corpo]</td>
   <td> <p>Adicione o conteúdo do corpo para a chamada à API na forma de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Limite]  </td>
      <td>
        <p>Insira o número máximo de resultados que você deseja que o módulo retorne em um ciclo de execução.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Excluir um Registro]

Este módulo de ação exclui um único registro em [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Conexão]</td>
     <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Journey Optimizer], consulte <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Journey Optimizer]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Tipo de Registro]
      </td>
      <td>
        Selecione o tipo de registro que deseja excluir
        <ul>
        <li>[!UICONTROL Posicionamento]</li>
        <li>[!UICONTROL Regra de decisão]</li>
        <li>[!UICONTROL Decisão]</li>
        <li>[!UICONTROL Marca]</li>
        <li>[!UICONTROL Coleção]</li>
        <li>[!UICONTROL Oferta substituta]</li>
        <li>[!UICONTROL Oferta personalizada]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Posicionamento]/[!UICONTROL Regra de decisão]/[!UICONTROL Decisão]/[!UICONTROL Marca]/[!UICONTROL Coleção]/[!UICONTROL Oferta de fallback]/[!UICONTROL Oferta personalizada]
      </td>
      <td>
        Selecione o registro que deseja excluir.
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL Atualizar um registro]

Esse módulo de ação cria uma oferta de posicionamento, decisão, regra de decisão, tag, oferta personalizada, coleção ou oferta substituta.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Conexão]</td>
     <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Journey Optimizer], consulte <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Journey Optimizer]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Tipo de registro]
      </td>
      <td>
        Selecione o tipo de registro que deseja atualizar
        <ul>
        <li>[!UICONTROL Posicionamento]</li>
        <li>[!UICONTROL Regra de decisão]</li>
        <li>[!UICONTROL Decisão]</li>
        <li>[!UICONTROL Marca]</li>
        <li>[!UICONTROL Coleção]</li>
        <li>[!UICONTROL Oferta substituta]</li>
        <li>[!UICONTROL Oferta personalizada]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Posicionamento]/[!UICONTROL Regra de decisão]/[!UICONTROL Decisão]/[!UICONTROL Marca]/[!UICONTROL Coleção]/[!UICONTROL Oferta de fallback]/[!UICONTROL Oferta personalizada]
      </td>
      <td>
        Selecione o registro que deseja atualizar.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Campos]
      </td>
      <td>Para cada campo que você deseja atualizar:
      <ol>
      <li>Clique em <b>[!UICONTROL Adicionar]</b>.</li>
      <li>Selecione se deseja adicionar, substituir ou remover valores.</li>
      <li>Insira o campo que deseja atualizar.</li>
      <li>Insira o novo valor para o campo.</li>
      </td>
    </tr>

</tbody>
</table>


### Pesquisas

#### [!UICONTROL Listar registros]

Este módulo de pesquisa lista registros do tipo selecionado, retornando resultados com base nos critérios que você especificar.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Conexão]</td>
     <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Journey Optimizer], consulte <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Journey Optimizer]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Tipo de registro]</p>
      </td>
      <td>
        <p>Selecione o tipo de registro que deseja listar.</p>
        <ul>
        <li>[!UICONTROL Posicionamento]</li>
        <li>[!UICONTROL Regra de decisão]</li>
        <li>[!UICONTROL Decisão]</li>
        <li>[!UICONTROL Marca]</li>
        <li>[!UICONTROL Coleção]</li>
        <li>[!UICONTROL Oferta substituta]</li>
        <li>[!UICONTROL Oferta personalizada]</li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Operador de consulta]</p>
      </td>
      <td>
        <p>Selecione um operador para aplicar aos parâmetros na query</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Campos]</td>
      <td><p>Se quiser limitar a pesquisa a campos específicos, informe os campos. Para cada campo ao qual você deseja limitar a pesquisa, clique em [!UICONTROL Adicionar item] e insira o nome do campo.</p><p>As expressões de caminho estão no formato de caminhos separados por pontos, como <code>_instance.xdm:name</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ordenar por] </td>
      <td>Insira ou mapeie a propriedade pela qual deseja solicitar resultados.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Direção da ordem]</td>
   <td>Selecione se deseja ordenar os resultados em direção crescente ou decrescente.
    </td>
     </tr>
  </tbody>
</table>
