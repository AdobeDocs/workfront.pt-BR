---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: Analisador de texto
description: Você pode usar a ferramenta Analisador de texto para analisar o texto para uso em outros [!DNL Adobe Workfront Fusion] módulos de cenário. O analisador de texto não requer uma conexão.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d71cf64-4f86-42c5-81e7-8fc15333cbd7
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1010'
ht-degree: 0%

---

# [!UICONTROL Analisador de texto]

Você pode usar o [!UICONTROL Ferramenta Analisador de texto] para analisar o texto para uso em outros [!DNL Adobe Workfront Fusion] módulos de cenário. O [!UICONTROL Analisador de texto] não requer uma conexão.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p> <p>[!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Analisador de texto] módulos e seus campos

Ao configurar [!UICONTROL Analisador de texto] módulos, [!DNL Adobe Workfront Fusion] exibe os campos listados abaixo. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Transformadores

* [[!UICONTROL Obter elementos do HTML]](#get-elements-from-html)
* [[!UICONTROL Obter elementos do texto]](#get-elements-from-text)
* [[!UICONTROL HTML para texto]](#html-to-text)
* [[!UICONTROL Padrão de correspondência]](#match-pattern)
* [[!UICONTROL Substituir]](#replace)

#### [!UICONTROL Obter elementos do HTML]

Recupera os elementos desejados do código HTML.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Continuar a execução da rota mesmo se o módulo não encontrar correspondências]</td> 
   <td> <p>Ative essa opção para garantir que o módulo não interrompa o cenário se não retornar resultados.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de elemento]</td> 
   <td> <p> Selecione o tipo de elemento que deseja recuperar do código de HTML. </p> 
    <ul> 
     <li>[!UICONTROL Imagem]</li> 
     <li>[!UICONTROL Link]</li> 
     <li>[!UICONTROL Elemento(s) do iFrame]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>Insira ou mapeie o código HTML do qual deseja recuperar os tipos de elemento especificados.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter elementos do texto]

Analisa elementos do texto com base no padrão especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Entrada de texto]</td> 
   <td> <p>Insira ou mapeie o texto que deseja analisar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Padrão]</td> 
   <td> <p>Selecione o padrão que reflete os elementos que você deseja analisar do texto.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ignorar ocorrências duplicadas]</td> 
   <td> <p>Marque essa caixa para ignorar ocorrências duplicadas de um elemento de texto.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL HTML para texto]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>Insira o código HTML que você deseja converter em texto sem formatação.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Quebra de linha] </td> 
   <td> <p>Selecione o tipo de nova linha (quebra de linha).</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Cabeçalhos em maiúsculas]</p> </td> 
   <td> <p>Ative essa opção para converter texto delimitado nas tags de cabeçalho (como &lt;h2&gt; &lt;/h2&gt;) em texto maiúsculo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Padrão de correspondência]

O [!UICONTROL Corresponder padrão] permite localizar e extrair elementos de string correspondentes a um padrão de pesquisa de um determinado texto. Esse módulo usa expressões regulares (também conhecidas como regex ou regexp).

Uma expressão regular é uma sequência de caracteres na qual cada caractere é um metacaractere, com um significado especial, ou um caractere regular com um significado literal. Esses caracteres e metacaracteres identificam um padrão que pode ser usado para pesquisar texto. Por exemplo, se você quiser procurar nomes, poderá configurar uma expressão regular para procurar por um padrão que consista em duas palavras consecutivas que começam com letras maiúsculas. Expressões regulares são uma ferramenta poderosa para pesquisar e manipular texto.

Uma discussão sobre expressões regulares está fora do escopo deste artigo. Recomendamos os seguintes recursos:

* Para obter a lista completa de metacaracteres, consulte [Expressões regulares](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions) em documentos da Web MDN.
* Para assistir a um tutorial sobre como criar expressões regulares, recomendamos [RegexOne](https://regexone.com/).
* Para experimentar expressões regulares, recomendamos a variável [Expressões regulares 101](https://regex101.com/) site. Selecione a PALAVRA do ECMAScript (JavaScript) no painel esquerdo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Padrão] </td> 
   <td> <p>Insira o padrão de expressão regular. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span> <code>[+-]?(\d+(\.\d+)?|\.\d+)([eE][+-]?\d+)?</code> extrai todos os numerais no texto fornecido.</p> <p>Nota:  <p>O padrão deve conter pelo menos um grupo de captura entre parênteses <code>()</code>. Se o padrão não contiver grupos de captura, o pacote de saída estará vazio.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Correspondência global]</td> 
   <td> <p>Habilite esta opção para recuperar todas as correspondências no texto. Cada correspondência é emitida em um pacote separado. Se essa opção estiver desativada, o módulo recuperará somente a primeira entrada.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Diferencia maiúsculas de minúsculas]</td> 
   <td> <p> Ative essa opção para que esse módulo trate o texto como diferencia maiúsculas de minúsculas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiline] </td> 
   <td> <p>Habilite esta opção para garantir que os metacaracteres de início e fim (<code>^</code> e <code>$</code>) corresponde ao início ou ao fim de cada linha, não apenas ao início ou ao fim de toda a string de entrada.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Linha única]</td> 
   <td>Ative essa opção para garantir que o ponto (.) corresponde a caracteres de nova linha (<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continuar a execução da rota mesmo se o módulo não retornar nenhum resultado]</td> 
   <td> <p>Ative essa opção para garantir que o módulo não interrompa o cenário se não retornar resultados.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Texto] </td> 
   <td> <p>Insira ou mapeie o texto que deseja corresponder ao padrão.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Substituir]

Pesquisa o texto inserido para um valor especificado ou uma expressão regular e substitui o resultado pelo novo valor.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Padrão] </td> 
   <td> <p>Insira o termo de pesquisa. Também é possível usar uma expressão regular. Para obter mais detalhes sobre a expressão regular, consulte <a href="#match-pattern" class="MCXref xref">[!UICONTROL Corresponder Padrão]</a> módulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Novo valor]</td> 
   <td> <p> Insira um valor que substitua o termo de pesquisa.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Correspondência global]</td> 
   <td> <p>Habilite esta opção para recuperar todas as correspondências no texto. Cada correspondência é emitida em um pacote separado. Se essa opção estiver desativada, o módulo recuperará somente a primeira entrada.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Diferencia maiúsculas de minúsculas]</td> 
   <td> <p> Ative essa opção para que esse módulo trate o texto como diferencia maiúsculas de minúsculas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiline] </td> 
   <td> <p>Habilite esta opção para garantir que os metacaracteres de início e fim (<code>^</code> e <code>$</code>) corresponde ao início ou ao fim de cada linha, não apenas ao início ou ao fim de toda a string de entrada.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Linha única]</td> 
   <td>Ative essa opção para garantir que o ponto (.) corresponde a caracteres de nova linha (<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Texto] </td> 
   <td> <p>Insira o texto a ser pesquisado.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Script de dados

A coleta de dados, às vezes chamada de raspagem da Web, extração de dados ou colheita da Web, é o processo de coleta de dados de sites e seu armazenamento em bancos de dados ou planilhas locais. Se quiser extrair dados de um site e não estiver familiarizado com expressões regulares, use uma ferramenta de rascunho de dados:

* [Apify](https://apify.com/)
* [Melhores ferramentas de criação de dados para 2019](https://www.octoparse.com/blog/best-data-scraping-tools-for-2019-top-10-reviews)

Se a ferramenta de rascunho de dados fornecer uma REST API, você pode se conectar a ela por meio de nossa API universal [[!UICONTROL HTTP] módulos](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md) e [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md) módulos.
