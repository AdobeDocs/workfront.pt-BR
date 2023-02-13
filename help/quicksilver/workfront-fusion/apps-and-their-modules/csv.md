---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: CSV
description: Os módulos CSV do Adobe Workfront Fusion permitem criar arquivos CSV e analisar o texto CSV a partir de um valor de texto recebido ou de um arquivo.
author: Becky
feature: Workfront Fusion
exl-id: 4e37482a-e84e-4ab2-a48f-7e7bfbecee56
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 0%

---

# CSV

O [!DNL Adobe Workfront Fusion] [!UICONTROL CSV] Os módulos permitem criar arquivos CSV e analisar o texto CSV a partir de um valor de texto recebido ou de um arquivo.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p>  <p>[!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Criar CSV]

O [!UICONTROL Criar CSV] O Aggregator permite criar um texto csv a partir de valores de texto recebidos.

Para obter mais informações sobre agregadores, consulte [Módulo agregador em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Módulo de origem]</td>
        <td>Selecione o módulo que você está usando para agregar os campos necessários.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Campos agregados]</td>
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
        <td>[!UICONTROL Parar o processamento após uma agregação vazia]</td>
        <td>Selecione essa opção para interromper o cenário quando não houver resultados.</td>
    </tr>
</table>

## [!UICONTROL Criar CSV (avançado)]

O [!UICONTROL Criar CSV (avançado)] O Agregador permite criar um texto CSV a partir de valores de texto recebidos. Ele emprega uma estrutura de dados que define as colunas CSV no arquivo CSV resultante. Depois de definidas, as colunas aparecem como campos na configuração do módulo CSV e podem ser mapeadas para o módulo posterior no cenário.

Para obter mais informações sobre agregadores, consulte [Módulo agregador em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Módulo de origem]</td> 
   <td>Selecione o módulo de aplicativo que você está usando para agregar os campos necessários.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Estrutura de dados]</td> 
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
   <td role="rowheader">[!UICONTROL Parar o processamento após uma agregação vazia] </td> 
   <td>Selecione essa opção para interromper o cenário quando não houver resultados. </td> 
  </tr> 
 </tbody> 
</table>


<p>Considere que você deseja exportar seus contatos do Google para um arquivo CSV com duas colunas "Nome completo" e "Email". O pacote de saída do módulo [!UICONTROL Google Contacts] &gt;[!UICONTROL Obter contatos de um grupo] tem a seguinte estrutura. Os endereços de email são armazenados no <code>[!UICONTROL Emails[]]</code> item, que é uma matriz de coleções, cada coleção contendo dois itens: <code>Label</code> e <code>Email</code>.</p>
<p> <img src="assets/transforming-350x546.png" style="width: 350;height: 546;"> </p>
<p>Se você usar o [!DNL Create CSV] , você recebe uma lista de caixas de seleção correspondentes aos itens de nível superior de um pacote. Se tentar marcar <code>Full name</code> e <code>Emails</code> itens, o módulo [!UICONTROL Criar CSV] produz a seguinte saída, que provavelmente não é o que você deseja:</p>
<p>"emails","fullName"</p>
<p>"[object Object]","Shon Winer"</p>
<p>"[object Object]","Lizeth Fulmore"</p>
<p>"[object Object]","Hilario Gullatt"</p>
<p>"[object Object]","Abby Eisenbarth"</p>
<p>Desde o item <code>Full Name</code> é do tipo simples Texto, é exportado muito bem. Mas o item <code>Emails</code>, que é de um tipo complexo Array of Collections, é exportado como [object Object], que é a forma como as Collections e Arrays são transformadas em texto por padrão. Para obter mais informações, consulte <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Tipos de dados de item no Adobe Workfront Fusion</a>.</p>
<p>Para exportar o conteúdo da <code>Email </code>item da primeira coleção do <code>Emails[]</code> em vez disso, é necessário empregar o módulo [!UICONTROL Criar CSV (avançado)]. O módulo permite definir colunas individuais do seu arquivo CSV e mapear itens para elas, incluindo as aninhadas.</p>
<ol>
<li value="1">Insira o módulo [!UICONTROL Criar CSV (avançado)] em um cenário e abra a configuração.</li>
<li value="2">Clique no botão <strong>[!UICONTROL Adicionar]</strong> botão ao lado do campo [!UICONTROL Data structure] para criar uma nova estrutura de dados.</li>
<li value="3"> <p>Escreva um nome para a estrutura de dados e clique no botão <strong>[!UICONTROL Adicionar item]</strong> para adicionar as colunas individuais. Se quiser exportar duas colunas: "Nome completo" e "Email", a estrutura de dados resultante seria semelhante a:</p> <p> <img src="assets/google-contacts-350x524.png" style="width: 350;height: 524;"> </p> </li>
<li value="4"> <p>Depois de definir com êxito a estrutura de dados, os campos correspondentes a cada coluna individual devem aparecer na configuração do módulo [!UICONTROL Criar CSV (avançado)] para que você possa mapear os itens. Pegue o primeiro item do <code>[!UICONTROL Emails[]]</code> matriz e mapeie seu item <code>Email </code>para o campo/coluna Email:</p> <p> <img src="assets/create-csv-advanced-350x308.png" style="width: 350;height: 308;"> </p> </li>
<li value="5"> <p>Execute o cenário. Desde o item <code>Emails[1]: Email</code> mapeado para a coluna "Email" é do tipo simples Texto, ele exporta corretamente agora:</p> <p>"Nome completo", "Email"</p> <p>"Shon Winer","Shon@Winer.com"</p> <p>"Lizeth Fulmore","Lizeth@Fulmore.com"</p> <p>"Hilario Gullatt","Hilario@Gullatt.com"</p> <p>"Abby Eisenbarth","Abby@Eisenbarth.com"</p> </li>
</ol>
</div>

## [!UICONTROL Analisar CSV]

O [!UICONTROL Analisar CSV] O transformador permite analisar o texto CSV de um valor de texto recebido ou de um arquivo.

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
   <td> <p>Selecione essa opção se a primeira linha do texto CSV contiver cabeçalhos.</p> <p>Observação: O módulo não usa esses cabeçalhos para rotular as colunas na saída. Em vez disso, esse campo garante que os cabeçalhos não sejam incluídos nos dados de saída.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL delimiterType]</td> 
   <td> <p>Selecione o delimitador do arquivo CSV. O delimitador é o caractere de texto que indica o limite entre valores ou campos separados.</p> 
    <ul> 
     <li>[!UICONTROL Vírgula]</li> 
     <li>[!UICONTROL Guia]</li> 
     <li> <p>[!UICONTROL Outro]</p> <p>Se você selecionar [!UICONTROL Outros], insira o caractere delimitador que o arquivo CSV está usando para separar valores. Você deve inserir exatamente um caractere.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Preservar aspas dentro de um campo não cotado]</td> 
   <td>Habilite esta opção para preservar as aspas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV]</td> 
   <td>Insira ou mapeie o arquivo CSV que deseja analisar.<p>Nota: <p>Se os dados vêm em forma binária (normalmente de um arquivo), é necessário usar a função `toString()` para converter os dados binários em [!UICONTROL String]:</p><p><img src="assets/parse-csv-350x123.png" style="width: 350;height: 123;"></p></p></td> 
  </tr> 
 </tbody> 
</table>
