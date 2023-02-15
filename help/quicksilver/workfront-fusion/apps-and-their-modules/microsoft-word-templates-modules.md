---
filename: microsoft-word-templates-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de modelo do Microsoft Word
description: Em um cenário do Adobe Workfront Fusion, é possível automatizar os fluxos de trabalho que usam Modelos do Microsoft Word, bem como conectá-los a vários aplicativos e serviços de terceiros.
author: Becky
source-git-commit: 43b64d1371438909063d2ac81cccb90b97179dfc
workflow-type: tm+mt
source-wordcount: '1286'
ht-degree: 0%

---


# [!DNL Microsoft Word Template] módulos

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL Microsoft Word Templates], bem como conectá-lo a vários aplicativos e serviços de terceiros.

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
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> 
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
     --> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
     --> </td> 
   </tr>
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Para usar [!DNL Miscrosoft Word Templates] com [!DNL Adobe Workfront Fusion], é necessário ter um [!DNL Office 365] conta. Você pode criar um em www.office.com.

## Usando [!DNL Microsoft Word Templates] módulos

Você pode usar um [!DNL Microsoft Word Template] módulo para mesclar dados de vários serviços da Web em um [!DNL Microsoft Word] documento.

Por exemplo, é possível usar essa opção [!DNL Microsoft Word] modelo:

![](assets/word-template-before-filled-350x62.png)

Para criar este documento:

![](assets/word-template-exampled-filled-350x85.png)

## Sobre tags de valor

A [!DNL Microsoft Word] modelo é regular [!DNL Microsoft Word] documento (arquivo .docx) com tags especiais em seu texto que determinam onde e como unir ou preencher os dados. Existem três tipos de tags:

* [Tag de valor simples](#simple-value-tag)
* [Tag de condição](#condition-tag)
* [Tag de loop](#loop-tag)

### Tag de valor simples {#simple-value-tag}

Uma tag de valor simples é simplesmente substituída por um valor correspondente. O nome da tag corresponde à variável [!UICONTROL Chave] valor do campo, que é colocado dentro de chaves duplas; por exemplo,


<pre>&#123;&#123;name&#125;&#125;</pre>


.

**Exemplo:** Para criar um documento que diga &quot;Oi, Petr!&quot;, você pode usar um [!DNL Microsoft Word Template] para criar o seguinte template:

<pre>&gt; Olá &#123;&#123;name&#125;&#125;!</pre>

Para fazer isso, configure o módulo da seguinte maneira:

![](assets/word-template-simple-value-350x286.png)

### Tag de condição {#condition-tag}

Você pode usar uma tag de condição para envolver o texto que deve ser renderizado apenas quando determinadas condições forem atendidas. Para quebrar o texto, coloque-o entre tags de condição de abertura e fechamento, como &quot;hasPhone&quot;, se a condição for se os dados incluem ou não um número de telefone. O nome de uma tag de abertura é anexado a um sinal de hash #, o nome de uma tag de fechamento é anexado a uma barra /, como mostrado no exemplo abaixo.

**Exemplo:** Para produzir um documento que inclua o número de telefone de um cliente, se os dados de entrada incluírem um número de telefone, mas nenhum endereço de email, você pode usar um [!DNL Microsoft Word Template] e crie o seguinte template:
<pre><pre>> &#123;&#123;#hasPhone&#125;&#125;Telefone: &#123;&#123;phone&#125;&#125; &#123;&#123;/hasPhone&#125;&#125;</pre><pre>> &#123;&#123;#hasEmail&#125;&#125;Email: &#123;&#123;email&#125;&#125; &#123;&#123;/hasEmail&#125;&#125;</pre>Para fazer isso, configure o módulo da seguinte maneira:

![](assets/word-template-conditional-350x501.png)

No documento, o número de telefone aparece da seguinte maneira:
<pre>&gt; Telefone: 444551234</pre>

### Tag de loop {#loop-tag}

Você pode usar uma tag de loop, também conhecida como tag de seção, para repetir uma seção de texto. Encapsule o texto colocando-o entre as tags de loop de abertura e fechamento. O nome de uma tag de abertura é anexado com um sinal de hash #; o nome de uma tag de fechamento é anexado a uma barra /.

* [Carregar tag com Preencher um módulo de documento](#loop-tag-with-fill-out-a-document-module)

<!-- [Loop tag with Fill a document with a batch of data module](#loop-tag-with-fill-a-document-with-a-batch-of-data-module)-->

#### Carregar tag com Preencher um módulo de documento {#loop-tag-with-fill-out-a-document-module}

**Exemplo:** Para produzir um documento que lista o nome e o número de telefone de cada contato em uma lista de clientes, você pode usar um [!DNL Microsoft Word Template] e crie o seguinte template:

<pre>> &#123;&#123;#contact&#125;&#125;</pre><pre>> &#123;&#123;name&#125;&#125;, &#123;&#123;phone&#125;&#125;</pre><pre>> &#123;&#123;/contact&#125;&#125;</pre>

Para fazer isso, configure o módulo da seguinte maneira:


![](assets/word-template-fill-out-a-document-350x732.png)

O módulo criaria o seguinte documento:

```
> Jan Toman, 4445551234
> Eduard Salo, 4445552345
```

<!--

#### Loop tag with Fill a document with a batch of data module {#loop-tag-with-fill-a-document-with-a-batch-of-data-module}

**Example:** You can export Google contacts into a table that you create using loop tags.

The first module loads the template. The next module retrieves all contacts from the group you specify in [!DNL Google Contacts]. The aggregator module aggregates all values retrieved from Google Contacts and merges them into the template. And the last module saves the filled template to the desired location.

![](assets/word-template-batch-scenario-350x124.png)

You could use this scenario with the following template:

![](assets/word-template-batch-template-350x26.png)

To do this, you would set up the module as follows:

![](assets/word-template-batch-module-setup-350x323.png)

The module would create the following document:

![](assets/word-template-batch-document-350x46.png)
-->

## [!DNL Microsoft Word Template] módulos

Esses módulos não exigem uma conexão.

* [Preencher um documento](#fill-out-a-document)
* [Preencha um documento com um lote de dados](#fill-a-document-with-a-batch-of-data)

### [!UICONTROL Preencher um documento] {#fill-out-a-document}

Esse módulo transformador permite preencher um documento com os dados especificados. Ele pode ser usado com valores simples, tags condicionais ou tags de loop.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Delimitador de início do texto sendo substituído]</td> 
   <td> <p>Insira os caracteres que você deseja marcar o início do texto que está sendo substituído. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>Enter <code>[[</code> se quiser substituir um texto semelhante a este: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Delimitador final do texto que está sendo substituído]</p> </td> 
   <td> <p>Insira os caracteres que você deseja marcar o final do texto que está sendo substituído. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>Enter <code>]]</code> se quiser substituir um texto semelhante a este: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td> <p> Mapeie o arquivo que deseja fazer upload do módulo anterior (por exemplo, o HTTP &gt; Obter um arquivo ou Dropbox &gt; Obter um módulo de arquivo). Ou insira o arquivo de dados manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do arquivo preenchido]</td> 
   <td>Insira um nome de arquivo (incluindo extensão) para o arquivo de saída do target.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fonte de dados]</td> 
   <td> <p>Selecione uma opção para indicar se os dados que você está usando são de um formulário ou de uma coleta de dados brutos (dados de computador não processados).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valores]</td> 
   <td> <p>Deve ser uma matriz de coleções, onde:</p> 
    <ul> 
     <li>Cada coleção corresponde a uma entrada de dados e contém um item <code>entry</code></li> 
     <li>Item <code>entry </code>contém uma coleção de <code>key </code>e <code>value</code></li> 
     <li>Item <code>key </code>contém o nome da tag</li> 
     <li>item <code>value </code>contém o valor da tag</li> 
    </ul> 
    <p>Para adicionar uma entrada:</p>
    <ol> 
     <li> Clique em <b>[!UICONTROL Adicionar item]</b>. </li> 
     <li>Selecione o tipo de valor da entrada.</li> 
     <li>Adicione o nome e o valor. Para obter mais informações, consulte o exemplo do tipo de valor escolhido neste artigo. 
      <ul> 
       <li><a href="#simple-value-tag" class="MCXref xref">Tag de valor simples</a></li> 
       <li><a href="#condition-tag" class="MCXref xref">Tag de condição</a></li> 
       <li><a href="#loop-tag" class="MCXref xref">Tag de loop</a></li> 
      </ul></li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Preencha um documento com um lote de dados] {#fill-a-document-with-a-batch-of-data}

Esse módulo agregador é útil se suas entradas de dados vêm como pacotes separados. Com esse módulo, você pode configurar facilmente a estrutura necessária para o campo Valor e ele mapeia itens para cada item de valor. Em contraste com o módulo Fill out a document , o campo Values no campo Fill a document with a batch of data permite apenas uma única entrada contendo variáveis.

Também é possível usar esse módulo se suas entradas de dados vierem como uma matriz, usando o *Iterador* para transformar o conteúdo da matriz em uma série de pacotes.

Os valores reais são criados e preenchidos para cada pacote de entrada. O modelo é produzido depois que todos os pacotes de entrada são processados.

Esse módulo agregador é útil principalmente para criar listas ou relatórios.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Módulo de origem]</td> 
   <td>Selecione o módulo que é a fonte do texto.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Delimitador de início do texto sendo substituído]</td> 
   <td> <p>Insira os caracteres que você deseja marcar o início do texto que está sendo substituído. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>Enter <code>[[</code> se quiser substituir um texto semelhante a este: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Delimitador final do texto que está sendo substituído]</p> </td> 
   <td> <p>Insira os caracteres que você deseja marcar o final do texto que está sendo substituído. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>Enter <code>]]</code> se quiser substituir um texto semelhante a este: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Agrupar por]</td> 
   <td> Defina uma expressão contendo um ou mais itens mapeados. Os dados agregados são separados em Grupos com o valor da mesma expressão. Cada Grupo gera como um pacote separado contendo uma Chave com a expressão avaliada e o texto agregado. Ao fazer isso, você pode usar a Chave como filtro em módulos subsequentes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parar o processamento após uma agregação vazia]</td> 
   <td>Ative essa opção para parar o processamento quando um agregado não contiver pacotes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td> <p> Mapeie o arquivo que deseja fazer upload do módulo anterior (por exemplo, o HTTP &gt; Obter um arquivo ou Dropbox &gt; Obter um módulo de arquivo). Ou insira o arquivo de dados manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do arquivo preenchido]</td> 
   <td>Insira um nome de arquivo (incluindo extensão) para o arquivo de saída do target.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fonte de dados]</td> 
   <td> <p>Selecione uma opção para indicar se os dados que você está usando são de um formulário ou de uma coleta de dados brutos (dados de computador não processados).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valores]</td> 
   <td> <p>Deve ser uma matriz de coleções, onde:</p> 
    <ul> 
     <li>Cada coleção corresponde a uma entrada de dados e contém um item <code>entry</code></li> 
     <li>Item <code>entry </code>contém uma coleção de <code>key </code>e <code>value</code></li> 
     <li>Item <code>key </code>contém o nome da tag</li> 
     <li>item <code>value </code>contém o valor da tag</li> 
    </ul> 
    <p>Para adicionar uma entrada:</p>
    <ol> 
     <li> Clique em <b>[!UICONTROL Adicionar item]</b>. </li> 
     <li>Selecione o tipo de valor da entrada.</li> 
     <li>Adicione o nome e o valor. Para obter mais informações, consulte o exemplo do tipo de valor escolhido neste artigo. 
      <ul> 
       <li><a href="#simple-value-tag" class="MCXref xref">Tag de valor simples</a></li> 
       <li><a href="#condition-tag" class="MCXref xref">Tag de condição</a></li> 
       <li><a href="#loop-tag" class="MCXref xref">Tag de loop</a></li> 
      </ul></li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

