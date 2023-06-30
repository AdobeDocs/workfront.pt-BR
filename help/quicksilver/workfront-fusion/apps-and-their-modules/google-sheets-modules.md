---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Google Sheets
description: Para utilizar [!DNL Google Sheets] com [!DNL Adobe Workfront Fusion],you need the [!UICONTROL Workfront Fusion Google Sheets] extensão (opcional, mas necessária para acionadores instantâneos).
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 11d62222-df34-472d-93d7-f0d53eb95c9b
source-git-commit: 6f4e5042054f3936fa0e387bfbebaa1775d16573
workflow-type: tm+mt
source-wordcount: '3941'
ht-degree: 0%

---

# [!DNL Google Sheets] módulos

Em um [!DNL Adobe Workfront Fusion] cenário, é possível automatizar workflows que usam [!DNL Google Sheets], bem como conectá-lo a vários aplicativos e serviços de terceiros.

Para obter instruções sobre como conectar seu [!DNL Google Sheets] conta para [!DNL Workfront Fusion], consulte [Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

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

Para usar [!UICONTROL Planilhas Google] módulos, você deve ter uma [!UICONTROL Google] conta.

## Triggers

### [!UICONTROL Observar linhas]

Recupera valores de cada linha adicionada recentemente na planilha.

O módulo recupera somente novas linhas que não foram preenchidas anteriormente. O disparador não processará uma linha substituída.

>[!IMPORTANT]
>
>Se a planilha contiver uma linha em branco, nenhuma linha após a linha em branco será processada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Sheets] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planilha] </td> 
   <td> <p>Selecione a planilha que contém a planilha que você deseja observar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planilha] </td> 
   <td> <p>Selecione a planilha que deseja observar para uma nova linha.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabela contém cabeçalhos]</td> 
   <td> <p> Selecione se a planilha contém a linha de cabeçalho.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Sim]</strong> </p> <p>O módulo não recupera a linha de cabeçalho como dados de saída. </p> <p>Os nomes das variáveis na saída são chamados pelos cabeçalhos.</p> </li> 
     <li> <p><strong>[!UICONTROL Não]</strong> </p> <p>O módulo também recupera a primeira linha da tabela</p> <p>Os nomes das variáveis na saída são chamados de A, B, C, D e assim por diante.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Linha com cabeçalhos] </td> 
   <td> <p>Informe a faixa da linha de cabeçalho. Por exemplo, <code>A1:F1</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Primeira linha de tabela]</td> 
   <td> <p>Insira o intervalo da primeira linha da tabela. Por exemplo, <code>A1:F1</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Opção de renderização de valor]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Valor formatado]</p> <p>Os valores serão calculados e formatados na resposta de acordo com a formatação da célula. A formatação se baseia no local da planilha, não no local do usuário solicitante. Por exemplo, se <code>A1</code> é <code>1.23</code> e <code>A2</code> é <code>=A1</code> e formatada como moeda, em seguida <code>A2</code> retornaria <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Valor não formatado]</p> <p>Os valores serão calculados, mas não formatados na resposta. Por exemplo, se <code>A1</code> é <code>1.23</code> e <code>A2</code> é <code>=A1</code> e formatada como moeda, em seguida <code>A2</code> retornaria o número <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Fórmula]</p> <p>Os valores não serão calculados. A resposta incluirá as fórmulas. Por exemplo, se <code>A1</code> é <code>1.23</code> e <code>A2</code> é <code>=A1</code> e formatada como moeda, em seguida <code>A2</code> retornaria <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Opção de renderização de data e hora]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Número de série]</p> <p>Instrui os campos date, time, datetime e duration a serem exibidos como duplos no formato "número de série", conforme popularizado pelo Lotus 1-2-3. A parte do número inteiro do valor (à esquerda do decimal) conta os dias desde 30 de dezembro de 1899. A parte fracional (à direita do decimal) conta o tempo como uma fração do dia. Por exemplo, 1º de janeiro de 1900 ao meio-dia seria 2,5, 2 porque é 2 dias depois de 30 de dezembro de 1899, e 0,5 porque o meio-dia é meio dia. 1 de fevereiro de 1900 às 15h seria 33.625. Isso considera corretamente o ano de 1900 como não um ano bissexto.</p> <p style="font-weight: bold;">[!UICONTROL Cadeia de caracteres formatada]</p> <p>Instrui os campos de data, hora, data e hora e duração a serem exibidos como cadeias de caracteres em seu formato de número fornecido (que depende do local da planilha).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite] </td> 
   <td> <p>Defina o número máximo de resultados que [!DNL Workfront Fusion] funcionará com durante um ciclo de execução.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ações

* [[!UICONTROL Adicionar uma linha]](#add-a-row)
* [[!UICONTROL Atualizar uma linha]](#update-a-row)
* [[!UICONTROL Limpar uma Linha]](#clear-a-row)
* [[!UICONTROL Excluir uma linha]](#delete-a-row)
* [[!UICONTROL Obter uma Célula]](#get-a-cell)
* [[!UICONTROL Atualizar uma Célula]](#update-a-cell)
* [[!UICONTROL Limpar uma Célula]](#clear-a-cell)
* [[!UICONTROL Adicionar uma planilha]](#add-a-sheet)
* [[!UICONTROL Criar uma planilha]](#create-a-spreadsheet)
* [[!UICONTROL Excluir uma Planilha]](#delete-a-sheet)
* [[!UICONTROL Fazer uma chamada de API]](#make-an-api-call)

### [!UICONTROL Adicionar uma linha]

Este módulo anexa adiciona uma linha a uma planilha.

Ao configurar [!DNL Google Sheets] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Google Sheets] Os campos podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Sheets] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modo]</td> 
   <td> <p>Selecione se deseja selecionar a planilha e a planilha manualmente ou por mapeamento.</p> <p>Observação: O mapeamento manual é útil, por exemplo, quando uma nova planilha é criada em um [!DNL Workfront Fusion] e quiser adicionar dados na planilha recém-criada diretamente no cenário.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planilha] </td> 
   <td> <p>Selecione o [!DNL Google] planilha eletrônica.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planilha] </td> 
   <td> <p>Selecione a planilha à qual deseja adicionar uma linha.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Intervalo de Colunas]</td> 
   <td>Selecione o intervalo de colunas com o qual deseja trabalhar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabela contém cabeçalhos]</td> 
   <td> <p> Selecione se a planilha contém a linha de cabeçalho.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Sim]</strong> </p> <p>O módulo não recupera a linha de cabeçalho como dados de saída. </p> <p>Os nomes das variáveis na saída são chamados pelos cabeçalhos.</p> </li> 
     <li> <p><strong>[!UICONTROL Não]</strong> </p> <p>O módulo também recupera a primeira linha da tabela</p> <p>Os nomes das variáveis na saída são chamados de A, B, C, D e assim por diante.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valores] </td> 
   <td> <p>Insira ou mapeie as células desejadas da linha que deseja adicionar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Opção de entrada de valor]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Usuário inserido]</strong></p> <p>Os valores são analisados como se o usuário os tivesse digitado na interface. Os números permanecem números, mas as cadeias de caracteres podem ser convertidas em números, datas ou outros formatos seguindo as mesmas regras aplicadas ao inserir texto em uma célula por meio do [!DNL Google Sheets] IU.</p> </li> 
     <li> <p><strong>[!UICONTROL Bruto]</strong> </p> <p> Os valores inseridos pelo usuário não são analisados e são armazenados como estão. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Inserir opção de dados]</td> 
   <td> <p>Especifique como os dados existentes serão alterados quando novos dados forem inseridos. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir linhas]</strong></p> <p>São inseridas linhas para os novos dados.</p> </li> 
     <li> <p><strong>[!UICONTROL Substituir]</strong> </p> <p>Os novos dados substituem os dados existentes nas áreas em que são gravados. A adição de dados ao final da planilha insere novas linhas ou colunas para que os dados possam ser gravados.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Atualizar uma linha]

Esse módulo permite alterar o conteúdo da célula em uma linha selecionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Sheets] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modo]</td> 
   <td> <p>Selecione se deseja selecionar a planilha e a planilha manualmente ou por mapeamento.</p> <p>Observação: o mapeamento manual é útil, por exemplo, quando uma nova planilha é criada no cenário do [!UICONTROL Workfront Fusion] e você deseja adicionar dados à planilha recém-criada diretamente no cenário.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planilha] </td> 
   <td> <p>Selecione o [!DNL Google] planilha eletrônica.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planilha] </td> 
   <td> <p>Selecione a planilha na qual deseja atualizar uma linha.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número de linha]</td> 
   <td> <p> Informe o número da linha que deseja atualizar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabela contém cabeçalhos]</td> 
   <td> <p> Selecione se a planilha contém a linha de cabeçalho.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Sim]</strong> </p> <p>O módulo não recupera a linha de cabeçalho como dados de saída. </p> <p>Os nomes das variáveis na saída são chamados pelos cabeçalhos.</p> </li> 
     <li> <p><strong>[!UICONTROL Não]</strong> </p> <p>O módulo também recupera a primeira linha da tabela</p> <p>Os nomes das variáveis na saída são chamados de A, B, C, D e assim por diante.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valores] </td> 
   <td> <p>Insira ou mapeie os valores para as células desejadas da linha que você deseja alterar (atualizar).</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Opção de entrada de valor]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Usuário inserido]</strong></p> <p>Os valores são analisados como se o usuário os tivesse digitado na interface. Os números permanecem números, mas as cadeias de caracteres podem ser convertidas em números, datas ou outros formatos seguindo as mesmas regras aplicadas ao inserir texto em uma célula por meio do [!DNL Google Sheets] IU.</p> </li> 
     <li> <p><strong>[!UICONTROL Bruto]</strong> </p> <p> Os valores inseridos pelo usuário não são analisados e são armazenados como estão. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Limpar uma Linha]

Exclui valores de uma linha especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Sheets] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planilha] </td> 
   <td> <p>Selecione o [!DNL Google] planilha que contém a planilha da qual você deseja limpar uma linha.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planilha] </td> 
   <td> <p> Selecione a planilha cujos dados você deseja limpar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número de linha]</td> 
   <td> <p>Insira o número da linha da qual deseja limpar dados. Por exemplo, <code> 23</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Excluir uma linha]

Exclui uma linha especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Sheets] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planilha] </td> 
   <td> <p>Selecione a planilha do Google que contém a planilha da qual deseja excluir uma linha.</p> </td> 
  </tr> 
  <tr> 
   <td>Planilha </td> 
   <td> <p>Selecione a planilha da qual deseja excluir uma linha.</p> </td> 
  </tr> 
  <tr> 
   <td>Número da linha</td> 
   <td> <p>Informe o número da linha que deseja deletar. Exemplo: <code>23</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Obter uma Célula]

Recupera um valor de uma célula selecionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Sheets] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planilha] </td> 
   <td> <p>Selecione o [!DNL Google] planilha eletrônica.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planilha] </td> 
   <td> <p>Selecione a planilha que contém a célula da qual deseja recuperar dados.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Célula] </td> 
   <td> <p>Insira a ID da célula da qual deseja recuperar dados. Exemplo: <code>A6</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Opção de renderização de valor]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Valor formatado]</p> <p>Os valores serão calculados e formatados na resposta de acordo com a formatação da célula. A formatação se baseia no local da planilha, não no local do usuário solicitante. Por exemplo, se <code>A1</code> é <code>1.23</code> e <code>A2</code> é <code>=A1</code> e formatada como moeda, em seguida <code>A2</code> retornaria <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!DNL Unformatted value]</p> <p>Os valores serão calculados, mas não formatados na resposta. Por exemplo, se <code>A1</code> é <code>1.23</code> e <code>A2</code> é <code>=A1</code> e formatada como moeda, em seguida <code>A2</code> retornaria o número <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!DNL Formula]</p> <p>Os valores não serão calculados. A resposta incluirá as fórmulas. Por exemplo, se <code>A1</code> é <code>1.23</code> e <code>A2</code> é <code>=A1</code> e formatada como moeda, em seguida <code>A2</code> retornaria <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Date and time render option]</td> 
   <td> <p style="font-weight: bold;">[!DNL Serial number]</p> <p>Instrui os campos date, time, datetime e duration a serem exibidos como duplos no formato "número de série", conforme popularizado pelo Lotus 1-2-3. A parte do número inteiro do valor (à esquerda do decimal) conta os dias desde 30 de dezembro de 1899. A parte fracional (à direita do decimal) conta o tempo como uma fração do dia. Por exemplo, 1º de janeiro de 1900 ao meio-dia seria 2,5, 2 porque é 2 dias depois de 30 de dezembro de 1899, e 0,5 porque o meio-dia é meio dia. 1 de fevereiro de 1900 às 15h seria 33.625. Isso considera corretamente o ano de 1900 como não um ano bissexto.</p> <p style="font-weight: bold;">[!DNL Formatted string]</p> <p>Instrui os campos de data, hora, data e hora e duração a serem exibidos como cadeias de caracteres em seu formato de número fornecido (que depende do local da planilha).</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Atualizar uma Célula]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Sheets] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planilha] </td> 
   <td> <p>Selecione o [!DNL Google] planilha eletrônica.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Célula] </td> 
   <td> <p>Insira a ID da célula que deseja atualizar. Exemplo: <code>A5</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valor]</td> 
   <td> <p>Insira o novo valor para a célula.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Opção de entrada de valor]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Usuário inserido]</strong></p> <p>Os valores são analisados como se o usuário os tivesse digitado na interface. Os números permanecem números, mas as cadeias de caracteres podem ser convertidas em números, datas ou outros formatos seguindo as mesmas regras aplicadas ao inserir texto em uma célula por meio do [!DNL Google Sheets] IU.</p> </li> 
     <li> <p><strong>[!UICONTROL Bruto]</strong> </p> <p> Os valores inseridos pelo usuário não são analisados e são armazenados como estão. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Limpar uma Célula]

Exclui um valor de uma célula especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Sheets] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planilha] </td> 
   <td> <p>Selecione a planilha do Google que contém a planilha da qual você deseja limpar uma célula.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planilha] </td> 
   <td> <p>Selecione a planilha da qual deseja limpar uma célula.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Célula] </td> 
   <td> <p>Insira a ID da célula que deseja limpar. Exemplo: <code>A5</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Adicionar uma planilha]

Cria uma nova planilha em uma planilha selecionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Sheets] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planilha] </td> 
   <td> <p>Selecione a planilha do Google à qual deseja adicionar uma planilha.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Propriedades]</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">[!UICONTROL Título]</p> <p>Digite o nome da nova planilha.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Índice]</p> <p>Insira a posição da planilha. O padrão é 0 (coloca a planilha no primeiro lugar)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Criar uma planilha]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Sheets] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Título] </td> 
   <td> <p>Insira o nome de uma nova planilha.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Localidade]</td> 
   <td> <p>Informe o local da planilha em um dos seguintes formatos:</p> 
    <ul> 
     <li>um código de idioma ISO 639-1, como <code>en</code></li> 
     <li>um código de idioma ISO 639-2, como <code>haw</code>, se não existir o código 639-1</li> 
     <li>uma combinação do código ISO de idioma e do código do país, como <code>en_US</code></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Intervalo de recálculo]</td> 
   <td> <p>O tempo de espera antes que as funções voláteis sejam recalculadas:</p> <p style="font-weight: bold;">[!UICONTROL Na alteração]</p> <p>Funções voláteis são atualizadas a cada mudança.</p> <p style="font-weight: bold;">[!UICONTROL Em alteração e a cada minuto]</p> <p>Funções voláteis são atualizadas a cada mudança e a cada minuto.</p> <p style="font-weight: bold;">[!UICONTROL Em alteração e a cada hora]</p> <p>As funções voláteis são atualizadas a cada mudança e a cada hora.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fuso horário]</td> 
   <td> <p> Selecione o fuso horário da planilha.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Formato de número]</td> 
   <td> <p>Selecione o formato padrão de todas as células da planilha.</p> <p><strong>[!UICONTROL Texto]</strong>: Formatação de texto. Exemplo: <code>1000. 12</code></p> <p><strong>[!UICONTROL Número]</strong>: Formatação de números. Exemplo: <code>1,000.12</code></p> <p><strong>[!UICONTROL Porcentagem]</strong>: formatação de porcentagem. Exemplo: <code>10. 12%</code></p> <p><strong>[!UICONTROL Moeda]</strong>: formatação de moeda. Exemplo: <code>$1,000.12</code></p> <p><strong>[!UICONTROL Data]</strong>: Formatação de data. Exemplo: <code>9/26/2008</code></p> <p><strong>[!UICONTROL Hora]</strong>: Formatação de hora. Exemplo: <code>3:59:00 PM</code></p> <p><strong>[!UICONTROL Data e hora]</strong>: formatação de data e hora. Exemplo: <code>9/26/08 15:59:00</code> </p> <p><strong>[!UICONTROL Científico]</strong>Formatação científica de números. Exemplo: <code>1. 01E+03</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planilhas] </td> 
   <td> <p>Clique em <strong>[!UICONTROL Adicionar]</strong> para adicionar uma planilha à planilha. Para cada planilha, insira ou mapeie um título para a planilha e o índice da planilha. Um índice de 0 representa a primeira planilha.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Excluir uma Planilha]

Exclui uma planilha específica.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Sheets] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planilha] </td> 
   <td> <p>Selecione o [!DNL Google] planilha eletrônica.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planilha] </td> 
   <td> <p>Selecione a planilha que deseja excluir.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Fazer uma chamada de API]

Esse módulo de ação permite executar uma chamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [Fusion App] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td>Insira um caminho relativo a <code>https://sheets.googleapis.com/v4/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   <td> <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão. Por exemplo, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] O adiciona os cabeçalhos de autorização para você.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadeia de Consulta]</td> 
   <td> <p> Adicione a consulta da chamada à API na forma de um objeto JSON padrão.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada à API na forma de um objeto JSON padrão.</p> <p>Nota:   <p>Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Pesquisas

* [[!UICONTROL Pesquisar Linhas]](#search-rows)
* [[!UICONTROL Pesquisar Linhas (Avançado)]](#search-rows-advanced)
* [[!UICONTROL Obter valores de intervalo]](#get-range-values)
* [[!UICONTROL Listar Planilhas]](#list-sheets)

### [!UICONTROL Pesquisar Linhas]

Pesquisa linhas usando as opções de filtro.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [Fusion App] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planilha] </td> 
   <td> <p>Selecione o [!DNL Google] planilha eletrônica.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planilha] </td> 
   <td> <p>Selecione a planilha na qual deseja pesquisar as linhas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabela contém cabeçalhos]</td> 
   <td> <p> Selecione se a planilha contém a linha de cabeçalho. Se a opção [!UICONTROL Sim] estiver selecionada, o módulo não recuperará a linha de cabeçalho, pois os dados de saída e os nomes de variáveis na saída são chamados pelos cabeçalhos. Se a opção [!UICONTROL Não] estiver selecionada, o módulo também recuperará a primeira linha da tabela e os nomes de variáveis na saída serão chamados apenas de A, B, C, D e assim por diante.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Intervalo de colunas]</td> 
   <td>Selecione o intervalo de colunas com o qual trabalhar. Exemplo: <code>A-F</code></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Filtro]</td> 
   <td> <p>Defina o filtro para a linha a ser pesquisada.</p> <p>Para obter mais informações sobre filtros, consulte <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Adicionar um filtro a um cenário no [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordem de classificação]</td> 
   <td>Selecione se deseja classificar em ordem crescente ou decrescente.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordenar por]</td> 
   <td>Escolha a coluna pela qual deseja classificar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Opção de renderização de valor]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Valor formatado]</p> <p>Os valores serão calculados e formatados na resposta de acordo com a formatação da célula. A formatação se baseia no local da planilha, não no local do usuário solicitante. Por exemplo, se <code>A1</code> é <code>1.23</code> e <code>A2</code> é <code>=A1</code> e formatada como moeda, em seguida <code>A2</code> retornaria <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Valor não formatado]</p> <p>Os valores serão calculados, mas não formatados na resposta. Por exemplo, se <code>A1</code> é <code>1.23</code> e <code>A2</code> é <code>=A1</code> e formatada como moeda, em seguida <code>A2</code> retornaria o número <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Fórmula]</p> <p>Os valores não serão calculados. A resposta incluirá as fórmulas. Por exemplo, se <code>A1</code> é <code>1.23</code> e <code>A2</code> é <code>=A1</code> e formatada como moeda, em seguida <code>A2</code> retornaria <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Opção de renderização de data e hora]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Número de série]</p> <p>Instrui os campos date, time, datetime e duration a serem exibidos como duplos no formato "número de série", conforme popularizado pelo Lotus 1-2-3. A parte do número inteiro do valor (à esquerda do decimal) conta os dias desde 30 de dezembro de 1899. A parte fracional (à direita do decimal) conta o tempo como uma fração do dia. Por exemplo, 1º de janeiro de 1900 ao meio-dia seria 2,5, 2 porque é 2 dias depois de 30 de dezembro de 1899, e 0,5 porque o meio-dia é meio dia. 1 de fevereiro de 1900 às 15h seria 33.625. Isso considera corretamente o ano de 1900 como não um ano bissexto.</p> <p style="font-weight: bold;">[!UICONTROL Cadeia de caracteres formatada]</p> <p>Instrui os campos de data, hora, data e hora e duração a serem exibidos como cadeias de caracteres em seu formato de número fornecido (que depende do local da planilha).</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de linhas retornadas]</td> 
   <td>Defina o número máximo de linhas que [!DNL Workfront Fusion] retornará durante um ciclo de execução.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Pesquisar Linhas (Avançado)]

Retorna resultados que correspondem aos critérios fornecidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Sheets] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planilha] </td> 
   <td> <p>Selecione a planilha do Google que contém a planilha que você deseja pesquisar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planilha] </td> 
   <td> <p>Selecione a planilha que contém as linhas que você deseja pesquisar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Consulta]</td> 
   <td> <p>Use o [!DNL Google Charts Query Language]. Exemplo: <code>select * where B = "John"</code></p> <p>Para obter mais informações sobre [!DNL Google Charts Query Language], consulte <a href="https://developers.google.com/chart/interactive/docs/querylanguage">Referência da linguagem de consulta</a> no [!DNL Google] documentação.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Obter valores de intervalo]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Sheets] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planilha] </td> 
   <td> <p>Selecione o [!DNL Google] planilha eletrônica.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planilha] </td> 
   <td> <p>Selecione a planilha da qual deseja obter o conteúdo do intervalo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Intervalo] </td> 
   <td> <p>Insira o intervalo que deseja obter. Exemplo: <code>A1:D25</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabela contém cabeçalhos]</td> 
   <td> <p>Marque esta caixa se a planilha tiver uma linha de cabeçalho</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Linha com cabeçalhos]</td> 
   <td>Insira o intervalo dos cabeçalhos da tabela. Exemplo <code>A1:F1</code>. Se você deixar o campo vazio, [!DNL Workfront Fusion] suporá que o cabeçalho esteja na primeira linha do intervalo especificado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Opção de renderização de valor]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Valor formatado]</p> <p>Os valores serão calculados e formatados na resposta de acordo com a formatação da célula. A formatação se baseia no local da planilha, não no local do usuário solicitante. Por exemplo, se <code>A1</code> é <code>1.23</code> e <code>A2</code> é <code>=A1</code> e formatada como moeda, em seguida <code>A2</code> retornaria <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Valor não formatado]</p> <p>Os valores serão calculados, mas não formatados na resposta. Por exemplo, se <code>A1</code> é <code>1.23</code> e <code>A2</code> é <code>=A1</code> e formatada como moeda, em seguida <code>A2</code> retornaria o número <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Fórmula]</p> <p>Os valores não serão calculados. A resposta incluirá as fórmulas. Por exemplo, se <code>A1</code> é <code>1.23</code> e <code>A2</code> é <code>=A1</code> e formatada como moeda, em seguida <code>A2</code> retornaria <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Opção de renderização de data e hora]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Número de série]</p> <p>Instrui os campos date, time, datetime e duration a serem exibidos como duplos no formato "número de série", conforme popularizado pelo Lotus 1-2-3. A parte do número inteiro do valor (à esquerda do decimal) conta os dias desde 30 de dezembro de 1899. A parte fracional (à direita do decimal) conta o tempo como uma fração do dia. Por exemplo, 1º de janeiro de 1900 ao meio-dia seria 2,5, 2 porque é 2 dias depois de 30 de dezembro de 1899, e 0,5 porque o meio-dia é meio dia. 1 de fevereiro de 1900 às 15h seria 33.625. Isso considera corretamente o ano de 1900 como não um ano bissexto.</p> <p style="font-weight: bold;">[!UICONTROL Cadeia de caracteres formatada]</p> <p>Instrui os campos de data, hora, data e hora e duração a serem exibidos como cadeias de caracteres em seu formato de número fornecido (que depende do local da planilha).</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Listar Planilhas]

Este módulo retorna uma lista de todas as planilhas em uma planilha.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Sheets] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planilha] </td> 
   <td> <p>Selecione o [!DNL Google] planilha que contém as planilhas que você deseja listar.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Limites de uso

Se o erro `429: RESOURCE_EXHAUSTED` ocorrer, você excedeu o limite de taxa da API.

A variável [!DNL Google Sheets] A API tem um limite de 500 solicitações por 100 segundos por projeto e 100 solicitações por 100 segundos por usuário. Os limites para leituras e gravações são rastreados separadamente. Não há limite de uso diário.

Veja mais detalhes em [developers.google.com/sheets/api/limits](https://developers.google.com/sheets/api/limits).

## Dicas e truques

* [Como obter células vazias de um [!DNL Google] Planilha](#how-to-get-empty-cells-from-a-google-sheet)
* [Adicionar um botão em uma planilha para executar um cenário](#add-a-button-in-a-sheet-to-run-a-scenario)

### Como obter células vazias de um [!DNL Google Sheet]

Use o [!UICONTROL Pesquisar Linhas (Avançado)] módulo &amp; use esta fórmula para obter as colunas que estão vazias.
<pre>selecione * onde E é nulo</pre>Aqui, "E" é a coluna e "é nulo" é a condição. Você pode criar uma consulta mais avançada usando o [Google Query Lang](https://developers.google.com/chart/interactive/docs/querylanguage).

### Adicionar um botão em uma planilha para executar um cenário

1. Entrada [!DNL Workfront Fusion], insira o **[!UICONTROL Webhook]** > **[!UICONTROL Webhooks personalizados]** módulo/acionador no cenário e configure-o (consulte [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md)).

1. Copie o URL do webhook.
1. Execute o cenário.
1. No Google Sheets, escolha **[!UICONTROL Inserir]** > **[!UICONTROL Desenho]**... no menu principal.

1. No [!UICONTROL Desenho] Clique na guia **[!UICONTROL Caixa de texto]** ícone ![](assets/text-box.png) perto da parte superior da janela.
1. Crie um botão e clique no botão **[!UICONTROL Salvar e fechar]** no canto superior direito:
1. O botão será colocado em sua planilha. Clique nos três pontos verticais no canto superior direito do botão:
1. Escolher **[!UICONTROL Atribuir script..].** no menu.
1. Insira o nome do script (função), por exemplo `runScenario` e clique em **[!UICONTROL OK]**:
1. Escolher **[!UICONTROL Ferramentas]** > **[!UICONTROL Editor de script]** na barra do menu principal.

1. Insira o seguinte código:

   * O nome da função deve corresponder ao nome especificado na etapa 9.
   * Substitua o URL pelo URL do webhook copiado na etapa 2.

     <pre>função runScenario() {</pre><pre>UrlFetchApp.fetch("<webhook you copied>");</pre><pre>}</pre>

1. Pressione **[!UICONTROL Ctrl+S]** para salvar o arquivo de script, digite um nome de projeto e clique em **[!UICONTROL OK]**.

1. Voltar para [!DNL Google Sheets] e clique no novo botão.
1. Conceda a autorização necessária para o script:
1. Entrada [!DNL Workfront Fusion], verifique se o cenário foi executado com êxito.

## Armazenamento de datas em uma planilha

Se você armazenar um valor Date em uma planilha sem qualquer formatação, ele será exibido na planilha como texto no formato ISO 8601. No entanto, [!DNL Google Sheets] fórmulas ou funções que funcionam com datas que não compreendem esse texto (Exemplo: fórmula `=A1+10`) exibirá o seguinte erro:

![](assets/mceclip6-350x87.png)

Para ajudar a permitir [!DNL Google Sheets] para entender a data, formate-a com a variável [[!UICONTROL formatDate] (data; formato; [fuso horário])](../../workfront-fusion/functions/date-and-time-functions.md#formatda) função. O formato correto passado para a função como o segundo argumento depende das configurações de localidade da planilha.

Para determinar o formato correto:

1. Escolher **[!UICONTROL Arquivo]** > **[!UICONTROL Planilha]** configurações do menu principal para verificar/definir o local.

1. Depois de verificar/definir o local adequado, determine o formato de data e hora correspondente, escolhendo **[!UICONTROL Formato]** > **[!UICONTROL Número]** no menu principal. O formato é exibido ao lado do item de menu Data e hora:

1. Para compor o formato correto que deve ser passado para o [!UICONTROL formatDate()] consulte a lista de [Tokens para formatação de data e hora no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md).

**Exemplo:** A utilização de `MM/DD/YYYY HH:mm:ss` formato da localidade dos Estados Unidos:

![](assets/locale-time-350x83.png)

## Explorar [!DNL Google Sheets] funções

Se você perder uma função integrada, mas ela for apresentada por [!DNL Google Sheets], você poderá explorá-lo. Para obter mais informações, consulte [Uso [!DNL Google Sheets] funções](../../workfront-fusion/functions/map-using-functions.md#exploiti) in [Mapear itens usando funções no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/map-using-functions.md) .

## Manter [!DNL Google Sheets] de alterar números para datas

Talvez você descubra que uma sequência de números usada como texto está sendo interpretada como uma data em uma [!DNL Google] planilha. Por exemplo, você digita 1-2019, com a intenção de texto, mas o Google o interpreta como uma data. Você pode pré-formatar o número como texto simples para evitar isso.

1. Entrada [!DNL Google Sheets], realce a coluna ou célula que contém o número ou os números.
1. Clique em **[!UICONTROL Formato]** > **[!UICONTROL Número]** > **[!UICONTROL Texto sem formatação]**.

Outra solução alternativa em [!DNL Workfront Fusion] é digitar um apóstrofo (&#39;) antes de um número, por exemplo, &#39;1-2019 ou &#39;1/47. O apóstrofo não é exibido na célula após os dados serem enviados de [!DNL Workfront Fusion].
