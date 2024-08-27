---
filename: microsoft-word-templates-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Modelo do Microsoft Word
description: Em um cenário do Adobe Workfront Fusion, é possível automatizar workflows que usam Modelos do Microsoft Word, bem como conectá-los a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: 889b417c-04a9-4dbf-9a34-0dab65f11f03
source-git-commit: 0b8a4e3864cf9ca2c179a824bdb87977819c9383
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 0%

---

# [!DNL Microsoft Word Template] módulos

Em um cenário [!DNL Adobe Workfront Fusion], você pode automatizar fluxos de trabalho que usam [!DNL Microsoft Word Templates], bem como conectá-los a vários aplicativos e serviços de terceiros.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
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

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Para usar [!DNL Miscrosoft Word Templates] com [!DNL Adobe Workfront Fusion], é necessário ter uma conta [!DNL Office 365]. Crie um em www.office.com.



## Conectando o serviço [!DNL Office] a [!DNL Workfront Fusion]

Para obter instruções sobre como conectar sua conta do [!DNL Office] ao [!UICONTROL Workfront Fusion], consulte [Criar uma conexão com o [!UICONTROL Adobe Workfront Fusion] - Instruções básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Alguns aplicativos do Microsoft usam a mesma conexão, que está vinculada a permissões de usuário individuais. Portanto, ao criar uma conexão, a tela de consentimento de permissões exibe todas as permissões que foram concedidas anteriormente à conexão deste usuário, além de todas as novas permissões necessárias para o aplicativo atual.
>
>Por exemplo, se um usuário tiver permissões de &quot;Tabela de leitura&quot; concedidas por meio do conector do Excel e criar uma conexão no conector do Outlook para ler emails, a tela de consentimento de permissões mostrará a permissão &quot;Tabela de leitura&quot; já concedida e a permissão &quot;Gravar email&quot; recém-necessária.

## Usando módulos [!DNL Microsoft Word Templates]

Você pode usar um módulo [!DNL Microsoft Word Template] para mesclar dados de vários serviços Web em um documento [!DNL Microsoft Word].

Por exemplo, você poderia usar este modelo [!DNL Microsoft Word]:

![](assets/word-template-before-filled-350x62.png)

Para criar este documento:

![](assets/word-template-exampled-filled-350x85.png)

## Sobre tags de valor

Um modelo [!DNL Microsoft Word] é um documento [!DNL Microsoft Word] comum (arquivo .docx) com marcas especiais em seu texto que determinam onde e como mesclar ou preencher dados. Há três tipos de tags:

* [Marca de valor simples](#simple-value-tag)
* [Marca de condição](#condition-tag)
* [Marca Loop](#loop-tag)

### Marca de valor simples {#simple-value-tag}

Uma tag de valor simples é simplesmente substituída por um valor correspondente. O nome da marca corresponde ao valor do campo [!UICONTROL Chave], que é colocado dentro de chaves duplas; por exemplo, `{{name}}`.

**Exemplo:** Para criar um documento que diga &quot;Olá, Petr!&quot;, você pode usar um módulo [!DNL Microsoft Word Template] para criar o seguinte modelo:

```
> Hi {{name}}!
```

Para fazer isso, você configuraria o módulo da seguinte maneira:

![](assets/word-template-simple-value-350x286.png)

### Tag de condição {#condition-tag}

Você pode usar uma tag de condição para quebrar o texto que deve ser renderizado somente quando determinadas condições forem atendidas. Para quebrar o texto, coloque-o entre as tags de condição de abertura e fechamento, como &quot;hasPhone&quot;, se a condição for se os dados incluem ou não um número de telefone. O nome de uma tag de abertura é anexado ao sinal de hash #; o nome de uma tag de fechamento é anexado a uma barra /, como mostrado no exemplo abaixo.

**Exemplo:** para produzir um documento que inclua o número de telefone de um cliente, se os dados de entrada incluírem um número de telefone, mas nenhum endereço de email, você poderá usar um módulo [!DNL Microsoft Word Template] e criar o seguinte modelo:

```
> {{#hasPhone}}Phone: {{phone}} {{/hasPhone}}
> {{#hasEmail}}Email: {{email}} {{/hasEmail}}
```

Para fazer isso, você configuraria o módulo da seguinte maneira:

![](assets/word-template-conditional-350x501.png)

No documento, o número de telefone seria exibido da seguinte maneira:

```
> Phone: 4445551234
```

### Marca Loop {#loop-tag}

Você pode usar uma tag de loop, também conhecida como tag de seção, para repetir uma seção de texto. Quebrar o texto automaticamente colocando-o entre as tags de loop de abertura e fechamento. O nome de uma tag de abertura é prefixado com um hash sinal #; o nome de uma tag de fechamento é prefixado com uma barra /.

* [Repetir marca com Preencher um módulo de documento](#loop-tag-with-fill-out-a-document-module)
  <!-- [Loop tag with Fill a document with a batch of data module](#loop-tag-with-fill-a-document-with-a-batch-of-data-module)-->

#### Repetir tag com Preencher um módulo de documento {#loop-tag-with-fill-out-a-document-module}

**Exemplo:** Para produzir um documento que liste o nome e o número de telefone de cada contato em uma lista de clientes, você poderia usar um módulo [!DNL Microsoft Word Template] e criar o seguinte modelo:

```
> {{#contact}}
>     {{name}}, {{phone}}
> {{/contact}}
```

Para fazer isso, você configuraria o módulo da seguinte maneira:


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
* [Preencher um documento com um lote de dados](#fill-a-document-with-a-batch-of-data)

### [!UICONTROL Preencher um documento] {#fill-out-a-document}

Esse módulo de transformador permite preencher um documento com os dados especificados. Ele pode ser usado com tags de valores simples, tags condicionais ou tags de loop.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Delimitador de início do texto que está sendo substituído]</td> 
   <td> <p>Insira o(s) caractere(s) que deseja marcar o início do texto que será substituído. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>Digite <code>[[</code> se quiser substituir um texto semelhante a este: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Delimitador de fim do texto que está sendo substituído]</p> </td> 
   <td> <p>Insira o(s) caractere(s) que deseja marcar o final do texto que será substituído. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>Digite <code>]]</code> se quiser substituir um texto semelhante a este: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL arquivo Source]</td> 
   <td> <p> Mapeie o arquivo que você deseja carregar do módulo anterior (por exemplo, o HTTP &gt; Obter um arquivo ou o Dropbox &gt; Obter um módulo de arquivo). Ou insira o arquivo de dados manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do arquivo preenchido]</td> 
   <td>Insira um nome de arquivo (incluindo a extensão) para o arquivo de saída de destino.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fonte de Dados]</td> 
   <td> <p>Selecione uma opção para indicar se os dados que você está usando são de um formulário ou de uma coleção de dados brutos (dados não processados do computador).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valores]</td> 
   <td> <p>Deve ser uma matriz de coleções, em que:</p> 
    <ul> 
     <li>Cada coleção corresponde a uma entrada de dados e contém um item <code>entry</code></li> 
     <li>O item <code>entry </code> contém uma coleção de <code>key </code>e <code>value</code></li> 
     <li>O item <code>key </code> contém o nome da marca</li> 
     <li>o item <code>value </code> contém o valor da marca</li> 
    </ul> 
    <p>Para adicionar uma entrada:</p>
    <ol> 
     <li> Clique em <b>[!UICONTROL Adicionar Item]</b>. </li> 
     <li>Selecione o tipo de valor da entrada.</li> 
     <li>Adicione o nome e o valor. Para obter mais informações, consulte o exemplo do tipo de valor escolhido neste artigo. 
      <ul> 
       <li><a href="#simple-value-tag" class="MCXref xref">Marca de valor simples</a></li> 
       <li><a href="#condition-tag" class="MCXref xref">Tag de condição</a></li> 
       <li><a href="#loop-tag" class="MCXref xref">Marca Loop</a></li> 
      </ul></li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Preencher um documento com um lote de dados] {#fill-a-document-with-a-batch-of-data}

Esse módulo agregador é útil se suas entradas de dados vêm como pacotes separados. Com esse módulo, você pode configurar facilmente a estrutura necessária para o campo Valor e mapear itens para cada item de valor. Ao contrário do módulo Preencher um documento, o campo Valores do módulo Preencher um documento com um lote de dados permite apenas uma única entrada contendo variáveis.

Você também pode usar este módulo se suas entradas de dados vierem como uma matriz, usando o módulo *Iterador* para transformar o conteúdo da matriz em uma série de pacotes.

Os valores reais são criados e preenchidos para cada pacote recebido. O template é produzido depois que todos os pacotes de entrada são processados.

Esse módulo agregador é especialmente útil para criar listas ou relatórios.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Módulo Source]</td> 
   <td>Selecione o módulo que é a fonte do seu texto.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Delimitador de início do texto que está sendo substituído]</td> 
   <td> <p>Insira o(s) caractere(s) que deseja marcar o início do texto que será substituído. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>Digite <code>[[</code> se quiser substituir um texto semelhante a este: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Delimitador de fim do texto que está sendo substituído]</p> </td> 
   <td> <p>Insira o(s) caractere(s) que deseja marcar o final do texto que será substituído. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>Digite <code>]]</code> se quiser substituir um texto semelhante a este: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Agrupar por]</td> 
   <td> Defina uma expressão contendo um ou mais itens mapeados. Os dados agregados são separados em Grupos com o mesmo valor de expressão. Cada Grupo gera um pacote separado contendo uma Chave com a expressão avaliada e o texto agregado. Ao fazer isso, você pode usar a chave como um filtro nos módulos subsequentes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parar processamento após uma agregação vazia]</td> 
   <td>Habilite esta opção para parar o processamento quando uma agregação não contiver pacotes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL arquivo Source]</td> 
   <td> <p> Mapeie o arquivo que você deseja carregar do módulo anterior (por exemplo, o HTTP &gt; Obter um arquivo ou o Dropbox &gt; Obter um módulo de arquivo). Ou insira o arquivo de dados manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do arquivo preenchido]</td> 
   <td>Insira um nome de arquivo (incluindo a extensão) para o arquivo de saída de destino.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fonte de Dados]</td> 
   <td> <p>Selecione uma opção para indicar se os dados que você está usando são de um formulário ou de uma coleção de dados brutos (dados não processados do computador).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valores]</td> 
   <td> <p>Deve ser uma matriz de coleções, em que:</p> 
    <ul> 
     <li>Cada coleção corresponde a uma entrada de dados e contém um item <code>entry</code></li> 
     <li>O item <code>entry </code> contém uma coleção de <code>key </code>e <code>value</code></li> 
     <li>O item <code>key </code> contém o nome da marca</li> 
     <li>o item <code>value </code> contém o valor da marca</li> 
    </ul> 
    <p>Para adicionar uma entrada:</p>
    <ol> 
     <li> Clique em <b>[!UICONTROL Adicionar Item]</b>. </li> 
     <li>Selecione o tipo de valor da entrada.</li> 
     <li>Adicione o nome e o valor. Para obter mais informações, consulte o exemplo do tipo de valor escolhido neste artigo. 
      <ul> 
       <li><a href="#simple-value-tag" class="MCXref xref">Marca de valor simples</a></li> 
       <li><a href="#condition-tag" class="MCXref xref">Tag de condição</a></li> 
       <li><a href="#loop-tag" class="MCXref xref">Marca Loop</a></li> 
      </ul></li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>
