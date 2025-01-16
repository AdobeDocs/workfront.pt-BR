---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: Analisador de texto
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d71cf64-4f86-42c5-81e7-8fc15333cbd7
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1097'
ht-degree: 0%

---

# [!UICONTROL Analisador de texto]

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Analisador de texto](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/text-parser.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

Você pode usar a [!UICONTROL Ferramenta de análise de texto] para analisar o texto a ser usado em outros módulos de cenário [!DNL Adobe Workfront Fusion]. O [!UICONTROL analisador de texto] não requer uma conexão.

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
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para Automação do Trabalho]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o plano [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], sua organização deve comprar [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] da [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Informações da API do analisador de texto

O conector do analisador de texto usa o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Tag da API</td> 
   <td>v2</td> 
  </tr>
 </tbody> 
 </table>

## Módulos [!UICONTROL Analisador de texto] e seus campos

Ao configurar módulos do [!UICONTROL Analisador de texto], o [!DNL Adobe Workfront Fusion] exibe os campos listados abaixo. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Transformadores

* [[!UICONTROL Obter Elementos do HTML]](#get-elements-from-html)
* [[!UICONTROL Obter Elementos do texto]](#get-elements-from-text)
* [[!UICONTROL HTML para texto]](#html-to-text)
* [[!UICONTROL Corresponder Padrão]](#match-pattern)
* [[!UICONTROL Substituir]](#replace)

#### [!UICONTROL Obter Elementos do HTML]

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

#### [!UICONTROL Obter Elementos do texto]

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
   <td> <p>Habilite esta opção para converter o texto delimitado nas marcas de cabeçalho (como &lt;h2&gt; &lt;/h2&gt;) em texto em maiúsculas.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Corresponder Padrão]

O módulo [!UICONTROL Padrão de correspondência] permite localizar e extrair elementos de cadeia de caracteres correspondentes a um padrão de pesquisa de um determinado texto. Esse módulo usa expressões regulares (também conhecidas como regex ou regexp).

Uma expressão regular é uma sequência de caracteres na qual cada caractere é um metacaractere, com um significado especial, ou um caractere regular que tem um significado literal. Esses caracteres e metacaracteres identificam um padrão que pode ser usado para pesquisar texto. Por exemplo, se você deseja pesquisar nomes, é possível configurar uma expressão regular para pesquisar um padrão que consiste em duas palavras consecutivas que começam com letras maiúsculas. As expressões regulares são uma ferramenta poderosa para pesquisar e manipular texto.

Uma discussão de expressões regulares está fora do escopo deste artigo. Recomendamos os seguintes recursos:

* Para obter a lista completa de metacaracteres, consulte [Expressões regulares](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions) em documentos da Web do MDN.
* Para um tutorial sobre como criar expressões regulares, recomendamos [RegexOne](https://regexone.com/).
* Para experimentar expressões regulares, recomendamos o site [Expressões regulares 101](https://regex101.com/). Selecione a VARIÁVEL ECMAScript (JavaScript) no painel esquerdo.

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
   <td> <p>Habilite esta opção para garantir que os metacaracteres de início e término (<code>^</code> e <code>$</code>) correspondam ao início ou ao fim de cada linha, não apenas ao início ou ao fim de toda a cadeia de caracteres de entrada.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Linha Simples]</td> 
   <td>Habilite esta opção para garantir que o ponto (.) corresponda aos caracteres de nova linha (<code>\n</code>).</td> 
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
   <td> <p>Insira o termo de pesquisa. Você também pode usar uma expressão regular. Para obter mais detalhes sobre a expressão regular, consulte o módulo <a href="#match-pattern" class="MCXref xref">[!UICONTROL Padrão de Correspondência]</a>.</p> </td> 
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
   <td> <p>Habilite esta opção para garantir que os metacaracteres de início e término (<code>^</code> e <code>$</code>) correspondam ao início ou ao fim de cada linha, não apenas ao início ou ao fim de toda a cadeia de caracteres de entrada.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Linha Simples]</td> 
   <td>Habilite esta opção para garantir que o ponto (.) corresponda aos caracteres de nova linha (<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Texto] </td> 
   <td> <p>Insira o texto a ser pesquisado.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Rascunho de dados

O raspamento de dados, às vezes chamado de raspagem da Web, extração de dados ou coleta da Web, é o processo de coletar dados de sites e armazená-los no banco de dados ou planilhas locais. Se quiser extrair dados de um site e não estiver familiarizado com expressões regulares, você poderá usar uma ferramenta de raspagem de dados.

Se a ferramenta de raspagem de dados fornecer uma REST API, você poderá se conectar a ela por meio de nossos módulos universais [[!UICONTROL HTTP]](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md) e [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).
