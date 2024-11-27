---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: módulos Adobe Firefly
description: Em um cenário  [!DNL Adobe Workfront Fusion] , é possível automatizar fluxos de trabalho que usam  [!DNL Adobe Firefly], bem como conectá-los a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 1e131c27-571d-4099-9243-69572bdb3f5a
source-git-commit: f6b00b98d3375e5660d684f1fad682fa721517aa
workflow-type: tm+mt
source-wordcount: '1315'
ht-degree: 0%

---

# [!DNL Adobe Firefly] módulos

Em um cenário [!DNL Adobe Workfront Fusion], você pode automatizar fluxos de trabalho que usam [!DNL Adobe Firefly], bem como conectá-los a vários aplicativos e serviços de terceiros.

Se você precisar de instruções sobre como criar um cenário, consulte [Criar um cenário](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obter informações sobre módulos, consulte [Módulos em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td> <p>Novo: [!UICONTROL Padrão]</p><p>Ou</p><p>Atual: [!UICONTROL Trabalho] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licença**</td> 
   <td>
   <p>Atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Herdados: Qualquer um </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Novo:</p> <ul><li>[!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Workfront] Plano: sua organização deve comprar [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plano: [!DNL Workfront Fusion] está incluído.</li></ul>
   <p>Ou</p>
   <p>Atual: sua organização deve comprar o [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Antes de usar o conector [!DNL Adobe Firefly], verifique se os seguintes pré-requisitos foram atendidos:

* Você deve ter uma conta [!DNL Adobe Firefly] ativa.

## Informações da API do Adobe Campaign

O conector do Adobe Campaign usa o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Tag da API</td> 
   <td>v1.4.24</td> 
  </tr>
 </tbody> 
 </table>

## Criar uma conexão com [!DNL Adobe Firefly]

Para criar uma conexão para seus módulos do [!DNL Adobe Firefly]:

1. Clique em **[!UICONTROL Adicionar]** ao lado da caixa Conexão.

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
        <td>Selecione se você está se conectando a uma conta de serviço ou a uma conta pessoal.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL ID do Cliente]</td>
        <td>Insira sua [!UICONTROL Adobe] [!UICONTROL ID do cliente]. Isso pode ser encontrado na seção de detalhes [!UICONTROL Credentials] do [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Segredo do Cliente]</td>
        <td>Insira seu [!DNL Adobe] [!UICONTROL Segredo do Cliente]. Isso pode ser encontrado na seção de detalhes [!UICONTROL Credentials] do [!DNL Adobe Developer Console].</td>
        </tr>
      </tbody>
    </table>

1. Clique em **[!UICONTROL Continuar]** para salvar a conexão e retornar ao módulo.

## [!DNL Adobe Firefly] módulos e seus campos

Ao configurar módulos do [!DNL Adobe Firefly], o [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos [!DNL Adobe Firefly] adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Fazer uma chamada de API personalizada

Esse módulo de ação faz uma chamada personalizada para a API Firefly.

Para obter as APIs específicas disponíveis, consulte [APIs de Adobe Firefly](https://developer.adobe.com/firefly-services/docs/firefly-api/) na documentação do Adobe Developer.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com [!DNL Adobe Firefly], consulte <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Firefly]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Insira um caminho relativo para <code>https://firefly-api-enterprise-stage.adobe.io/</code>.</p>
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
      <td role="rowheader">[!UICONTROL Corpo]</td>
   <td> <p>Adicione o conteúdo do corpo para a chamada à API na forma de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar instruções condicionais como <code>if</code> em seu JSON, coloque as aspas fora da instrução condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

### Expandir uma imagem

Esse módulo de ação expande uma imagem, opcionalmente com conteúdo de um prompt fornecido.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td>Para obter instruções sobre como criar uma conexão com [!DNL Adobe Campaign], consulte <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Firefly]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Prompt]</td> 
   <td>Insira ou mapeie um prompt para o conteúdo com o qual deseja expandir a imagem. Se nenhum prompt for fornecido, a imagem será expandida com o conteúdo correspondente à imagem original.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número de variações]</td> 
   <td>Insira um número entre 1-4. O módulo gerará esse número de variações de imagem expandidas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato de imagem expandido]</td> 
   <td>Selecione o formato de arquivo com o qual a imagem expandida será salva.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL arquivo Source]</td> 
   <td>  <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome do arquivo de imagem do arquivo de origem e o arquivo de imagem (dados).</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tamanho]</td> 
   <td>Selecione o tamanho desejado para a imagem expandida.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seed]</td> 
   <td>Insira ou mapeie um inteiro. Você pode usar essa mesma semente em outro módulo Expandir uma imagem para gerar uma imagem semelhante com estilos diferentes. </td> 
  </tr> 
 </tbody> 
</table>

## Preencher uma imagem

Esse módulo de ação preenche a área mascarada de uma imagem, opcionalmente com o conteúdo de um prompt fornecido.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td>Para obter instruções sobre como criar uma conexão com [!DNL Adobe Campaign], consulte <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Firefly]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Prompt]</td> 
   <td>Insira ou mapeie um prompt para o conteúdo com o qual deseja preencher a imagem. Se nenhum prompt for fornecido, a imagem será preenchida com o conteúdo correspondente à imagem original.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número de variações]</td> 
   <td>Insira um número entre 1-4. O módulo gerará esse número de variações de imagem preenchidas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato de imagem preenchido]</td> 
   <td>Selecione o formato de arquivo com o qual a imagem preenchida será salva.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Imagem]</td> 
   <td>  <p> Clique em <b>Adicionar uma imagem</b>. Selecione um arquivo de origem de um módulo anterior ou mapeie o nome do arquivo de origem e os dados de imagem.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Máscara]</td> 
   <td>  <p> Clique em <b>Adicionar uma máscara</b>. Selecione um arquivo de origem de um módulo anterior ou mapeie o nome do arquivo de origem Máscara e os dados da Máscara. O arquivo Mask representa a máscara personalizada que será preenchida com conteúdo gerado.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tamanho]</td> 
   <td>Selecione o tamanho desejado para a imagem preenchida.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seeds]</td> 
   <td>Para cada imagem gerada pelo módulo, clique em <b>Adicionar item<b> e insira ou mapeie um inteiro. Você pode usar essa mesma semente em outro módulo Expandir uma imagem para gerar uma imagem semelhante com estilos diferentes. O número de seeds que você adicionar deve ser igual ao campo Number of variation.</td> 
  </tr> 
 </tbody> 
</table>

## Gerar uma imagem

Esse módulo de ação gera uma imagem e com base em um prompt fornecido. Você também pode fornecer uma imagem de referência opcional, e a imagem gerada corresponderá ao estilo da imagem de referência.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td>Para obter instruções sobre como criar uma conexão com [!DNL Adobe Campaign], consulte <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Firefly]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Prompt]</td> 
   <td>Insira ou mapeie um prompt para a imagem que deseja criar. Mais detalhes no prompt permitirão que você tenha mais controle sobre o que aparece na imagem.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número de variações]</td> 
   <td>Insira um número entre 1-4. O módulo gerará esse número de variações de imagem.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato de imagem gerado]</td> 
   <td>Selecione o formato de arquivo com o qual a imagem expandida será salva. Se você selecionar padrão, o formato de arquivo será JPEG se nenhuma imagem de referência for fornecida. Se uma imagem de referência for fornecida, o formato de arquivo da imagem gerada será igual ao da imagem de referência.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL arquivo Source]</td> 
   <td>  <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome do arquivo de imagem de referência do arquivo de origem e o arquivo de imagem de referência (dados). A imagem gerada será criada para corresponder ao estilo da imagem de referência.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Predefinições]</td> 
   <td>Se quiser usar um estilo predefinido, clique em Adicionar item e insira ou mapeie o estilo que deseja usar.<p>Para obter uma lista de estilos predefinidos, consulte <a href="https://developer.adobe.com/firefly-services/docs/firefly-api/guides/concepts/style-presets/" >Estilos de modelo de imagem</a> na documentação do desenvolvedor do Adobe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Prompt negativo]</td> 
   <td>Insira ou mapeie as palavras que deseja evitar no conteúdo gerado. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Classe de conteúdo]</td> 
   <td>Selecione se você deseja que a imagem gerada seja mais como uma foto ou mais como uma arte criada. <ul><li><b>Foto</b><p>Insira valores para a abertura, velocidade do obturador (em segundos) e campo de visão (em milímetros).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seed]</td> 
   <td>Insira ou mapeie um inteiro. Você pode usar essa mesma semente em outro módulo Expandir uma imagem para gerar uma imagem semelhante com estilos diferentes. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tamanho]</td> 
   <td>Selecione o tamanho que você deseja que a imagem gerada tenha.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fortaleza]</td> 
   <td>Insira ou mapeie um número inteiro que represente a intensidade com que a imagem gerada corresponderá ao estilo da imagem de referência ou de estilo predefinido. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Intensidade visual]</td> 
   <td>Insira ou mapeie um número inteiro que represente a intensidade geral das características visuais existentes da foto. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Localidade]</td> 
   <td>Se um local for fornecido, o módulo gerará conteúdo mais relevante para o local especificado. <p>A localidade deve ser fornecida no código de idioma ISO 639-1 e na região ISO 3166-1.</p><p> Exemplo: <code>en-US</code></p></td> 
  </tr> 
 </tbody> 
</table>
