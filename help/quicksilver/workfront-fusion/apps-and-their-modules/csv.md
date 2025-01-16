---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: CSV
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: 4e37482a-e84e-4ab2-a48f-7e7bfbecee56
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 0%

---

# CSV

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [CSV](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/csv.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

Os módulos [!DNL Adobe Workfront Fusion] [!UICONTROL CSV] permitem que você crie arquivos CSV e analise textos CSV de um valor de texto recebido ou de um arquivo.

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

## [!UICONTROL Criar CSV]

O Agregador [!UICONTROL Criar CSV] permite criar um texto csv a partir de valores de texto recebidos.

Para obter mais informações sobre agregadores, consulte [Módulo agregador em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Módulo Source]</td>
        <td>Selecione o módulo que você está usando para agregar os campos necessários.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Campos Agregados]</td>
        <td>Selecione os campos que deseja agregar na lista de campos disponíveis.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Incluir cabeçalhos na primeira linha]</td>
        <td>Selecione essa opção para incluir os cabeçalhos no resultado.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Agrupar por]</td>
        <td>Insira o filtro para agrupar os resultados. Por exemplo, insira uma data.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Parar processamento após uma agregação vazia]</td>
        <td>Selecione esta opção para interromper o cenário quando não houver resultados.</td>
    </tr>
</table>

## [!UICONTROL Criar CSV (avançado)]

O Agregador [!UICONTROL Criar CSV (avançado)] permite criar um texto CSV a partir de valores de texto recebidos. Ele emprega uma estrutura de dados que define as colunas CSV no arquivo CSV resultante. Uma vez definidas, as colunas são exibidas como campos na configuração do módulo CSV e podem ser mapeadas para um módulo posterior no cenário.

Para obter mais informações sobre agregadores, consulte [Módulo agregador em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Módulo Source]</td> 
   <td>Selecione o módulo de aplicativo que você está usando para agregar os campos necessários.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Estrutura de Dados]</td> 
   <td> <p>Selecione a estrutura de dados para agregar os campos da maneira que desejar. Após definir a estrutura de dados, é possível mapear os itens para os campos correspondentes.</p> <p>Para obter mais informações, consulte <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">Estruturas de dados em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Incluir cabeçalhos na primeira linha] </td> 
   <td>Selecione essa opção para incluir os cabeçalhos no resultado. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Agrupar por] </td> 
   <td>Insira o filtro para agrupar os resultados. Por exemplo, insira uma data. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parar processamento após uma agregação vazia] </td> 
   <td>Selecione esta opção para interromper o cenário quando não houver resultados. </td> 
  </tr> 
 </tbody> 
</table>


<p>Suponhamos que você deseje exportar seus contatos do Google para um arquivo CSV com duas colunas "Nome completo" e "Email". O conjunto de saídas do módulo [!UICONTROL Google Contacts] &gt;[!UICONTROL Obter contatos de um grupo] tem a seguinte estrutura. Os endereços de email são armazenados dentro do item <code>[!UICONTROL Emails[]]</code>, que é uma matriz de coleções, cada coleção contendo dois itens: <code>Label</code> e <code>Email</code>.</p>
<p> <img src="assets/transforming-350x546.png" style="width: 350;height: 546;"> </p>
<p>Se você usar o módulo simples [!DNL Create CSV], receberá uma lista de caixas de seleção correspondentes aos itens de nível superior de um pacote. Se você tentar marcar <code>Full name</code> e <code>Emails</code> itens, o módulo [!UICONTROL Criar CSV] produzirá a seguinte saída, que provavelmente não é a que você deseja:</p>
<p>"emails","fullName"</p>
<p>"[object Object]","Shon Winer"</p>
<p>"[object Object]","Lizeth Fulmore"</p>
<p>"[object Object]","Hilario Gullatt"</p>
<p>"[object Object]","Abby Eisenbarth"</p>
<p>Como o item <code>Full Name</code> é do tipo Texto simples, ele é exportado sem problemas. Mas o item <code>Emails</code>, que é de um tipo complexo Matriz de Coleções, é exportado como [object Object], que é como Coleções e Matrizes são transformadas em texto por padrão. Para obter mais informações, consulte <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Tipos de dados de item no Adobe Workfront Fusion</a>.</p>
<p>Para exportar o conteúdo do item <code>Email </code> da primeira coleção da matriz <code>Emails[]</code>, é necessário empregar o módulo [!UICONTROL Criar CSV (avançado)]. O módulo permite definir colunas individuais do arquivo CSV e mapear itens para elas, incluindo as aninhadas.</p>
<ol>
<li value="1">Insira o módulo [!UICONTROL Criar CSV (avançado)] em um cenário e abra sua configuração.</li>
<li value="2">Clique no botão <strong>[!UICONTROL Adicionar]</strong> ao lado do campo [!UICONTROL Estrutura de dados] para criar uma nova Estrutura de dados.</li>
<li value="3"> <p>Escreva um nome para a estrutura de Dados e clique no botão <strong>[!UICONTROL Adicionar item]</strong> para adicionar colunas individuais. Se você quiser exportar duas colunas: "Nome completo" e "Email", a estrutura de dados resultante será semelhante a:</p> <p> <img src="assets/google-contacts-350x524.png" style="width: 350;height: 524;"> </p> </li>
<li value="4"> <p>Depois de definir com êxito a Estrutura de dados, os campos correspondentes a cada coluna individual devem aparecer na configuração do módulo [!UICONTROL Criar CSV (avançado)] para que você possa mapear os itens. Pegue o primeiro item da matriz <code>[!UICONTROL Emails[]]</code> e mapeie seu item <code>Email </code> para o campo/coluna Email:</p> <p> <img src="assets/create-csv-advanced-350x308.png" style="width: 350;height: 308;"> </p> </li>
<li value="5"> <p>Execute o cenário. Como o item <code>Emails[1]: Email</code> mapeado para a coluna "Email" é do tipo simples Texto, ele é exportado corretamente agora:</p> <p>"Nome completo","Email"</p> <p>"Shon Winer","Shon@Winer.com"</p> <p>"Lizeth Fulmore","Lizeth@Fulmore.com"</p> <p>"Hilario Gullatt","Hilario@Gullatt.com"</p> <p>"Abby Eisenbarth","Abby@Eisenbarth.com"</p> </li>
</ol>
</div>

## [!UICONTROL Analisar CSV]

O transformador [!UICONTROL Analisar CSV] permite analisar texto CSV de um valor de texto recebido ou de um arquivo.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número de colunas]</td> 
   <td>Especifique o número de colunas no arquivo CSV.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV contém cabeçalhos]</td> 
   <td> <p>Selecione essa opção se a primeira linha do texto CSV contiver cabeçalhos.</p> <p>Observação: o módulo não usa esses cabeçalhos para rotular as colunas na saída. Em vez disso, esse campo garante que os cabeçalhos não sejam incluídos nos dados de saída.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL tipoDelimitador]</td> 
   <td> <p>Selecione o delimitador para o arquivo CSV. O delimitador é o caractere de texto que indica o limite entre valores ou campos separados.</p> 
    <ul> 
     <li>[!UICONTROL Vírgula]</li> 
     <li>[!UICONTROL Guia]</li> 
     <li> <p>[!UICONTROL Outro]</p> <p>Se você selecionar [!UICONTROL Outro], insira o caractere delimitador que o arquivo CSV está usando para separar valores. Digite exatamente um caractere.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Preservar aspas dentro do campo sem aspas]</td> 
   <td>Habilite esta opção para preservar as aspas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV]</td> 
   <td>Insira ou mapeie o arquivo CSV que você deseja analisar.<p>Nota: <p>Se os dados vierem em formato binário (geralmente de um arquivo), você deverá usar a função "toString()" para converter os dados binários em [!UICONTROL String]:</p><p><img src="assets/parse-csv-350x123.png" style="width: 350;height: 123;"></p></p></td> 
  </tr> 
 </tbody> 
</table>
