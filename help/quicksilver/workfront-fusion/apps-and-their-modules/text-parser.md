---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: Analisador de texto
description: Você pode usar a ferramenta Analisador de texto para analisar o texto para uso em outros [!DNL Adobe Workfront Fusion] módulos de cenário. O analisador de Texto não requer uma conexão.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d71cf64-4f86-42c5-81e7-8fc15333cbd7
source-git-commit: 54d1753b9062b6d4910e4478c1f072b7fedc87eb
workflow-type: tm+mt
source-wordcount: '996'
ht-degree: 0%

---

# [!UICONTROL Analisador de texto]

Você pode usar o [!UICONTROL Ferramenta Analisador de texto] para analisar o texto para uso em outros [!DNL Adobe Workfront Fusion] módulos de cenário. A variável [!UICONTROL Analisador de texto] não requer uma conexão.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para Automação e integração do trabalho] </p> <p>[!UICONTROL [!DNL Workfront Fusion] para automação de trabalho]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Analisador de texto] módulos e seus campos

Ao configurar [!UICONTROL Analisador de texto] módulos, [!DNL Adobe Workfront Fusion] exibe os campos listados abaixo. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Transformadores

* [[!UICONTROL Obter elementos do HTML]](#get-elements-from-html)
* [[!UICONTROL Obter elementos de texto]](#get-elements-from-text)
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
   <td> <p> Selecione o tipo de elemento que deseja recuperar do código HTML. </p> 
    <ul> 
     <li>[!UICONTROL Imagem]</li> 
     <li>[!UICONTROL Link]</li> 
     <li>[!UICONTROL elemento(s) iFrame]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>Insira ou mapeie o código de HTML do qual você deseja recuperar os tipos de elemento especificados.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter elementos de texto]

Analisa os elementos do texto com base no padrão fornecido.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Texto de entrada]</td> 
   <td> <p>Insira ou mapeie o texto que deseja analisar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Padrão]</td> 
   <td> <p>Selecione o padrão que reflete os elementos que você deseja analisar do texto.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ignorar Ocorrências Duplicadas]</td> 
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
   <td> <p>Insira o código de HTML que deseja converter em texto sem formatação.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Quebra de linha] </td> 
   <td> <p>Selecione o tipo de nova linha (quebra de linha).</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Cabeçalhos em maiúsculas]</p> </td> 
   <td> <p>Habilite essa opção para converter o texto delimitado nas tags de cabeçalho (como &lt;h2&gt; &lt;/h2&gt;) em texto em maiúsculas.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Padrão de correspondência]

A variável [!UICONTROL Padrão de correspondência] O módulo permite localizar e extrair elementos de string que correspondam a um padrão de pesquisa de um determinado texto. Esse módulo usa expressões regulares (também conhecidas como regex ou regexp).

Uma expressão regular é uma sequência de caracteres na qual cada caractere é um metacaractere, com um significado especial, ou um caractere regular que tem um significado literal. Esses caracteres e metacaracteres identificam um padrão que pode ser usado para pesquisar texto. Por exemplo, se você deseja pesquisar nomes, é possível configurar uma expressão regular para pesquisar um padrão que consiste em duas palavras consecutivas que começam com letras maiúsculas. As expressões regulares são uma ferramenta poderosa para pesquisar e manipular texto.

Uma discussão de expressões regulares está fora do escopo deste artigo. Recomendamos os seguintes recursos:

* Para obter a lista completa de metacaracteres, consulte [Expressões regulares](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions) em documentos da Web do MDN.
* Para obter um tutorial sobre como criar expressões regulares, recomendamos [RegexOne](https://regexone.com/).
* Para experimentar expressões regulares, recomendamos o [Expressões regulares 101](https://regex101.com/) site. Selecione a VARIÁVEL ECMAScript (JavaScript) no painel esquerdo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Padrão] </td> 
   <td> <p>Insira o padrão de expressão regular. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span> <code>[+-]?(\d+(\.\d+)?|\.\d+)([eE][+-]?\d+)?</code> extrai todos os numerais no texto fornecido.</p> <p>Nota:  <p>O padrão deve conter pelo menos um grupo de captura entre parênteses <code>()</code>. Se o padrão não contiver nenhum grupo de captura, o pacote de saída estará vazio.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Correspondência global]</td> 
   <td> <p>Habilite esta opção para recuperar todas as correspondências no texto. Cada correspondência é gerada em um pacote separado. Se essa opção estiver desativada, o módulo recuperará somente a primeira entrada.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Diferencia maiúsculas de minúsculas]</td> 
   <td> <p> Habilite esta opção para que este módulo trate o texto como sensível a maiúsculas e minúsculas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Várias Linhas] </td> 
   <td> <p>Ative esta opção para garantir que os metacaracteres iniciais e finais (<code>^</code> e <code>$</code>) corresponde ao início ou ao fim de cada linha, não apenas ao início ou ao fim de toda a string de entrada.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Linha Simples]</td> 
   <td>Habilite essa opção para garantir que o ponto (.) corresponde a caracteres de nova linha (<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continuar a execução da rota mesmo se o módulo não retornar resultados]</td> 
   <td> <p>Ative essa opção para garantir que o módulo não interrompa o cenário se não retornar resultados.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Texto] </td> 
   <td> <p>Insira ou mapeie o texto que deseja corresponder ao padrão.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Substituir]

Pesquisa no texto inserido um valor especificado ou uma expressão regular e substitui o resultado pelo novo valor.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Padrão] </td> 
   <td> <p>Insira o termo de pesquisa. Você também pode usar uma expressão regular. Para obter mais detalhes sobre a expressão regular, consulte as <a href="#match-pattern" class="MCXref xref">[!UICONTROL Padrão de Correspondência]</a> módulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Novo valor]</td> 
   <td> <p> Insira um valor que substitua o termo de pesquisa.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Correspondência global]</td> 
   <td> <p>Habilite esta opção para recuperar todas as correspondências no texto. Cada correspondência é gerada em um pacote separado. Se essa opção estiver desativada, o módulo recuperará somente a primeira entrada.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Diferencia maiúsculas de minúsculas]</td> 
   <td> <p> Habilite esta opção para que este módulo trate o texto como sensível a maiúsculas e minúsculas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Várias Linhas] </td> 
   <td> <p>Ative esta opção para garantir que os metacaracteres iniciais e finais (<code>^</code> e <code>$</code>) corresponde ao início ou ao fim de cada linha, não apenas ao início ou ao fim de toda a string de entrada.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Linha Simples]</td> 
   <td>Habilite essa opção para garantir que o ponto (.) corresponde a caracteres de nova linha (<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Texto] </td> 
   <td> <p>Insira o texto a ser pesquisado.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Rascunho de dados

O raspamento de dados, às vezes chamado de raspagem da Web, extração de dados ou coleta da Web, é o processo de coletar dados de sites e armazená-los no banco de dados ou planilhas locais. Se quiser extrair dados de um site e não estiver familiarizado com expressões regulares, você poderá usar uma ferramenta de raspagem de dados.

Se a ferramenta de raspagem de dados fornecer uma API REST, você poderá se conectar a ela por meio de nosso [[!UICONTROL HTTP] módulos](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md) e [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md) módulos.
