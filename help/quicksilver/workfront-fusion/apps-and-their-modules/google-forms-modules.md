---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Google Forms
description: Os  [!DNL Adobe Workfront Fusion Google Forms] módulos permitem monitorar, selecionar, adicionar, atualizar ou excluir respostas no Google Forms.
author: Becky
feature: Workfront Fusion
exl-id: 45c86879-bc4e-4134-b63c-02410b9de43b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1420'
ht-degree: 0%

---

# [!DNL Google Forms] módulos

Os módulos do [!DNL Adobe Workfront Fusion] [!DNL Google Forms] permitem monitorar, selecionar, adicionar, atualizar ou excluir respostas no [!DNL Google Forms].

Para usar [!DNL Google Docs] com [!DNL Adobe Workfront Fusion], é necessário ter uma conta [!DNL Google]. Se você ainda não tiver uma conta [!DNL Google], crie uma na página de ajuda da Conta [!DNL Google].

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
   <td>
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Para usar módulos [!DNL Google Forms], você deve ter uma conta [!DNL Google].

## Criação de uma planilha a partir do formulário

Para trabalhar com as respostas do formulário, a planilha de suas respostas deve ser criada.

1. Abra o formulário.
1. Vá para a guia **[!UICONTROL Respostas]**.
1. Clique no ícone ![](assets/spreadsheet-icon.png) de **[!UICONTROL Criar Planilha]**.

1. Selecione se deseja criar uma nova planilha ou uma planilha existente
1. Clique em **[!UICONTROL Criar]**.

## [!DNL Google Forms] módulos e seus campos

Ao configurar módulos do [!DNL Google Forms], o [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos [!DNL Google Forms] adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Ações](#actions)
* [Pesquisas](#searches)

### Triggers

#### [!UICONTROL Assistir Respostas]

Verifica se há novas respostas no formulário.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planilha]</td> 
   <td> <p>Selecione a planilha que contém as respostas do formulário a ser observado para novas respostas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planilha]</td> 
   <td> <p> Selecione a planilha que contém as respostas do formulário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Linha com cabeçalhos]</td> 
   <td>Especifique a linha de cabeçalho da tabela. Linha padrão <code>A1:Z1</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Opção de Renderização de Valor]</td> 
   <td> <p>Especifique como deseja que os valores sejam renderizados na saída.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Valor formatado]</strong> </p> <p>Os valores são calculados e formatados na resposta de acordo com a formatação da célula. A formatação se baseia no local da planilha, não no local do usuário solicitante. Por exemplo, se <code>A1</code> for <code>1. 23</code> e <code>A2 </code> for <code>=A1</code> e formatado como moeda, <code>A2</code> retornará <code>$1. 23</code>.</p> </li> 
     <li> <p><strong>[!UICONTROL Valor não formatado]</strong> </p> <p>Os valores são calculados, mas não formatados na resposta. Por exemplo, se <code>A1</code> for <code>1. 23</code> e <code>A2 </code> for <code>=A1</code> e formatado como moeda, <code>A2</code> retornará o número <code>1. 23</code>.</p> </li> 
     <li> <p><strong>[!UICONTROL Fórmula]</strong> </p> <p>Os valores não são calculados. A resposta inclui as fórmulas. Por exemplo, se <code>A1</code> for <code>1. 23</code> e <code>A2 </code> for <code>=A1</code> e formatado como moeda, <code>A2</code> retornará <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Opção de renderização de data e hora]</td> 
   <td>Selecione como deseja que datas, horas e duração sejam representadas na saída. Este campo será ignorado se a [!UICONTROL Opção de Renderização de Valor] estiver definida como [!UICONTROL Valor Formatado].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p> Defina o número máximo de respostas com as quais [!DNL Workfront Fusion] funciona durante um ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [[!UICONTROL Adicionar uma resposta]](#add-a-response)
* [[!UICONTROL Atualizar uma resposta]](#update-a-response)
* [[!UICONTROL Excluir uma resposta]](#delete-a-response)

#### [!UICONTROL Adicionar uma resposta]

Este módulo anexa uma nova resposta à parte inferior da planilha do formulário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planilha]</td> 
   <td> <p>Selecione a planilha que contém a planilha à qual deseja adicionar uma resposta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planilha]</td> 
   <td> <p> Selecione a planilha que contém as respostas do formulário.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Valores]</p> </td> 
   <td> <p>Insira os valores desejados nas colunas da planilha.</p> <p>Para a coluna [!UICONTROL Carimbo de Data/Hora] no formato correto, use o seguinte valor:</p><pre>formatDate(agora;DD/MM/AAAA HH:mm;UTC)</pre> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Opção de entrada de valor]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> Os valores inseridos pelo usuário não são analisados e são armazenados como estão. </p> </li> 
     <li> <p><strong>[!UICONTROL Usuário inserido]</strong></p> <p>Os valores são analisados como se o usuário os tivesse digitado na interface. Os números permanecem números, mas as cadeias de caracteres podem ser convertidas em números, datas ou outros formatos seguindo as mesmas regras aplicadas ao inserir texto em uma célula por meio da interface do usuário do [!DNL Google Sheets].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Inserir opção de dados]</td> 
   <td> <p>Especifique como os dados existentes serão alterados quando novos dados forem inseridos. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Substituir]</strong> </p> <p>Os novos dados substituem os dados existentes nas áreas em que são gravados. A adição de dados ao final da planilha insere novas linhas ou colunas para que os dados possam ser gravados.</p> </li> 
     <li> <p><strong>[!UICONTROL Inserir linhas]</strong></p> <p>São inseridas linhas para os novos dados.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar uma resposta]

Este módulo atualiza a resposta selecionada.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planilha]</td> 
   <td> <p>Selecione a planilha que contém a planilha na qual você deseja atualizar uma resposta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planilha]</td> 
   <td> <p> Selecione a planilha que contém as respostas do formulário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Número de linha]</p> </td> 
   <td> <p>Informe ou mapeie o número da linha que deseja atualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Valores]</p> </td> 
   <td> <p>Insira os novos valores nas colunas desejadas.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Opção de entrada de valor]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> Os valores inseridos pelo usuário não são analisados e são armazenados como estão. </p> </li> 
     <li> <p><strong>[!UICONTROL Usuário inserido]</strong></p> <p>Os valores são analisados como se o usuário os tivesse digitado na interface. Os números permanecem números, mas as cadeias de caracteres podem ser convertidas em números, datas ou outros formatos seguindo as mesmas regras aplicadas ao inserir texto em uma célula por meio da interface do usuário do [!DNL Google Sheets].</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir uma resposta]

Este módulo exclui uma resposta selecionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planilha]</td> 
   <td> <p>Selecione a planilha que contém a planilha da qual deseja excluir uma resposta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planilha]</td> 
   <td> <p> Selecione a planilha que contém as respostas do formulário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Número de linha]</p> </td> 
   <td> <p>Informe ou mapeie o número da linha que deseja deletar.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Pesquisas

* [[!UICONTROL Pesquisar Respostas]](#search-responses)
* [[!UICONTROL Pesquisar Respostas (Avançado])](#search-responses-advanced)

#### [!UICONTROL Pesquisar Respostas]

Este módulo retorna respostas que correspondem aos critérios fornecidos.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
    <td>Conexão</td>
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Planilha]</td>
   <td> <p>Selecione o formulário que deseja pesquisar.</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Planilha] </td>
   <td> <p>Selecione a planilha que contém as respostas do formulário.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Intervalo de colunas]</td>
   <td> <p> Selecione o intervalo de colunas que deseja pesquisar.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Defina o filtro pelo qual deseja pesquisar respostas de respostas.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Ordem de Classificação] </td>
   <td> <p>Selecione se as respostas retornadas devem ser classificadas em ordem crescente ou decrescente.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Ordenar por]</td>
   <td> <p> Selecione a coluna pela qual deseja ordenar as respostas retornadas.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Opção de Renderização de Valor]</td> 
   <td> <p>Especifique como deseja que os valores sejam renderizados na saída.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Valor formatado]</strong></p> <p>Os valores são calculados e formatados na resposta de acordo com a formatação da célula. A formatação se baseia no local da planilha, não no local do usuário solicitante. Por exemplo, se <code>A1</code> for <code>1. 23</code> e <code>A2 </code> for <code>=A1</code> e formatado como moeda, <code>A2</code> retornará <code>$1. 23</code>.</p> </li> 
     <li> <p><strong>[!UICONTROL Valor não formatado]</strong> </p> <p>Os valores são calculados, mas não formatados na resposta. Por exemplo, se <code>A1</code> for <code>1. 23</code> e <code>A2 </code> for <code>=A1</code> e formatado como moeda, <code>A2</code> retornará o número <code>1. 23</code>.</p> </li> 
     <li> <p><strong>[!UICONTROL Fórmula]</strong> </p> <p>Os valores não são calculados. A resposta inclui as fórmulas. Por exemplo, se <code>A1</code> for <code>1. 23</code> e <code>A2 </code> for <code>=A1</code> e formatado como moeda, <code>A2</code> retornará <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Opção de renderização de data e hora]</td>
    <td>Selecione como deseja que datas, horas e duração sejam representadas na saída. Este campo será ignorado se a Opção [!UICONTROL Value Render] estiver definida como Valor Formatado. </td>
  </tr> 
  <tr>
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Número máximo de respostas retornadas]</td>
   <td> <p> Defina o número máximo de respostas que [!DNL Workfront Fusion] retorna durante um ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Respostas de Pesquisa (Avançadas)]

Este módulo executa uma pesquisa usando o [[!DNL Google Charts Query Language]](https://developers.google.com/chart/interactive/docs/querylanguage). Este módulo não retorna um número de linha.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Conexão]</td>
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Planilha]</td>
   <td> <p>Selecione a planilha que contém a planilha que você deseja pesquisar.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Planilha]</td>
   <td> <p> Selecione a planilha que contém as respostas do formulário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Defina a consulta de pesquisa usando o <a href="https://developers.google.com/chart/interactive/docs/querylanguage">[!DNL Google Charts Query Language]</a>.</p> <p>Exemplo: <code>select * where C = "John"</code> recupera todos os valores da linha em que a coluna C é "John".</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Número máximo de linhas retornadas]</td>
   <td> <p> Defina o número máximo de respostas que [!DNL Workfront Fusion] retorna durante um ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>
