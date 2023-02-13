---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos Forms Google
description: O [!DNL Adobe Workfront Fusion Google Forms] Os módulos permitem monitorar, selecionar, adicionar, atualizar ou excluir respostas no Google Forms.
author: Becky
feature: Workfront Fusion
exl-id: 45c86879-bc4e-4134-b63c-02410b9de43b
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1382'
ht-degree: 0%

---

# [!DNL Google Forms] módulos

O [!DNL Adobe Workfront Fusion] [!DNL Google Forms] os módulos permitem monitorar, selecionar, adicionar, atualizar ou excluir respostas em seu [!DNL Google Forms].

Para usar [!DNL Google Docs] com [!DNL Adobe Workfront Fusion], é necessário ter um [!DNL Google] conta. Se você não tiver um [!DNL Google] ainda assim, você pode criar uma no [!DNL Google] Página de ajuda da conta.

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
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Para usar [!DNL Google Forms] módulos, você deve ter um [!DNL Google] conta.

## Criação de uma planilha no formulário

Para trabalhar com as respostas do formulário, a planilha das respostas deve ser criada.

1. Abra o formulário.
1. Vá para o **[!UICONTROL Respostas]** guia .
1. Clique no botão **[!UICONTROL Criar planilha]** ícone ![](assets/spreadsheet-icon.png).

1. Selecione se deseja criar uma nova planilha ou uma planilha existente
1. Clique em **[!UICONTROL Criar]**.

## [!DNL Google Forms] módulos e seus campos

Ao configurar [!DNL Google Forms] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Google Forms] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Ações](#actions)
* [Pesquisas](#searches)

### Triggers

#### [!UICONTROL Assista às respostas]

Verifica o formulário em busca de novas respostas.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Spreadsheet]</td> 
   <td> <p>Selecione a planilha que contém as respostas do formulário que você deseja visualizar para novas respostas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sheet]</td> 
   <td> <p> Selecione a planilha que contém as respostas do formulário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Linha com cabeçalhos]</td> 
   <td>Especifique a linha de cabeçalho da tabela. A linha padrão é <code>A1:Z1</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Opção de renderização de valor]</td> 
   <td> <p>Especifique como deseja que os valores sejam renderizados na saída.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Valor formatado]</strong> </p> <p>Os valores são calculados e formatados na resposta de acordo com a formatação da célula. A formatação é baseada na localidade da planilha, não na localidade do usuário solicitante. Por exemplo, se <code>A1</code> é <code>1. 23</code> e <code>A2 </code>é <code>=A1</code> e formatada como moeda, <code>A2</code> devoluções <code>$1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL Valor não formatado]</strong> </p> <p>Os valores são calculados, mas não são formatados na resposta. Por exemplo, se <code>A1</code> é <code>1. 23</code> e <code>A2 </code>é <code>=A1</code> e formatada como moeda, <code>A2</code> retorna o número <code>1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL Fórmula]</strong> </p> <p>Os valores não são calculados. A resposta inclui as fórmulas. Por exemplo, se <code>A1</code> é <code>1. 23</code> e <code>A2 </code>é <code>=A1</code> e formatada como moeda, <code>A2</code> devoluções <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Opção de renderização de data e hora]</td> 
   <td>Selecione como deseja que as datas, horas e duração sejam representadas na saída. Este campo será ignorado se [!UICONTROL Value Render Option] estiver definido como [!UICONTROL Valor formatado].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p> Defina o número máximo de respostas que [!DNL Workfront Fusion] funciona durante um ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [[!UICONTROL Adicionar uma resposta]](#add-a-response)
* [[!UICONTROL Atualizar uma resposta]](#update-a-response)
* [[!UICONTROL Excluir uma resposta]](#delete-a-response)

#### [!UICONTROL Adicionar uma resposta]

Esse módulo anexa uma nova resposta à parte inferior da planilha do formulário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Spreadsheet]</td> 
   <td> <p>Selecione a planilha que contém a planilha à qual deseja adicionar uma resposta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sheet]</td> 
   <td> <p> Selecione a planilha que contém as respostas do formulário.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Valores]</p> </td> 
   <td> <p>Insira os valores desejados para as colunas da planilha.</p> <p>Para a coluna [!UICONTROL Carimbo de data e hora] no formato correto, use o seguinte valor:</p><pre>formatDate(now;DD/MM/AAAA HH:mm;UTC)</pre> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Opção de entrada Valor]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL bruto]</strong> </p> <p> Os valores inseridos pelo usuário não são analisados e são armazenados como estão. </p> </li> 
     <li> <p><strong>[!UICONTROL Usuário inserido]</strong></p> <p>Os valores são analisados como se o usuário os tivesse digitado na interface do usuário. Os números permanecem números, mas as sequências de caracteres podem ser convertidas em números, datas ou outros formatos seguindo as mesmas regras que são aplicadas ao inserir texto em uma célula por meio do [!DNL Google Sheets] IU.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Inserir opção de dados]</td> 
   <td> <p>Especifique como os dados existentes são alterados quando são introduzidos novos dados. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Substituir]</strong> </p> <p>Os novos dados substituem os dados existentes nas áreas em que são gravados. Adicionar dados ao final da planilha insere novas linhas ou colunas para que os dados possam ser gravados.</p> </li> 
     <li> <p><strong>[!UICONTROL Inserir linhas]</strong></p> <p>As linhas são inseridas para os novos dados.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar uma resposta]

Esse módulo atualiza a resposta selecionada.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Spreadsheet]</td> 
   <td> <p>Selecione a planilha que contém a planilha na qual você deseja atualizar uma resposta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sheet]</td> 
   <td> <p> Selecione a planilha que contém as respostas do formulário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Número da linha]</p> </td> 
   <td> <p>Insira ou mapeie o número da linha que deseja atualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Valores]</p> </td> 
   <td> <p>Insira os novos valores nas colunas desejadas.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Opção de entrada Valor]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL bruto]</strong> </p> <p> Os valores inseridos pelo usuário não são analisados e são armazenados como estão. </p> </li> 
     <li> <p><strong>[!UICONTROL Usuário inserido]</strong></p> <p>Os valores são analisados como se o usuário os tivesse digitado na interface do usuário. Os números permanecem números, mas as sequências de caracteres podem ser convertidas em números, datas ou outros formatos seguindo as mesmas regras que são aplicadas ao inserir texto em uma célula por meio do [!DNL Google Sheets] IU.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir uma resposta]

Esse módulo exclui uma resposta selecionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Spreadsheet]</td> 
   <td> <p>Selecione a planilha que contém a planilha na qual você deseja excluir uma resposta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sheet]</td> 
   <td> <p> Selecione a planilha que contém as respostas do formulário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Número da linha]</p> </td> 
   <td> <p>Insira ou mapeie o número da linha que deseja excluir.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Pesquisas

* [[!UICONTROL Respostas de pesquisa]](#search-responses)
* [[!UICONTROL Respostas de pesquisa (Avançadas)])](#search-responses-advanced)

#### [!UICONTROL Respostas de pesquisa]

Esse módulo retorna respostas correspondentes aos critérios fornecidos.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
    <td>Conexão</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Spreadsheet]</td>
   <td> <p>Selecione o formulário que deseja pesquisar.</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Sheet] </td>
   <td> <p>Selecione a planilha que contém as respostas do formulário.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Intervalo de colunas]</td>
   <td> <p> Selecione o intervalo de colunas que deseja pesquisar.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Defina o filtro pelo qual deseja pesquisar as respostas.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Ordem de classificação] </td>
   <td> <p>Selecione se deseja classificar as respostas retornadas em ordem crescente ou decrescente.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Pedido por]</td>
   <td> <p> Selecione a coluna pela qual deseja ordenar as respostas retornadas.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Opção de renderização de valor]</td> 
   <td> <p>Especifique como deseja que os valores sejam renderizados na saída.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Valor formatado]</strong></p> <p>Os valores são calculados e formatados na resposta de acordo com a formatação da célula. A formatação é baseada na localidade da planilha, não na localidade do usuário solicitante. Por exemplo, se <code>A1</code> é <code>1. 23</code> e <code>A2 </code>é <code>=A1</code> e formatada como moeda, <code>A2</code> devoluções <code>$1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL Valor não formatado]</strong> </p> <p>Os valores são calculados, mas não são formatados na resposta. Por exemplo, se <code>A1</code> é <code>1. 23</code> e <code>A2 </code>é <code>=A1</code> e formatada como moeda, <code>A2</code> retorna o número <code>1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL Fórmula]</strong> </p> <p>Os valores não são calculados. A resposta inclui as fórmulas. Por exemplo, se <code>A1</code> é <code>1. 23</code> e <code>A2 </code>é <code>=A1</code> e formatada como moeda, <code>A2</code> devoluções <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Opção de renderização de data e hora]</td>
    <td>Selecione como deseja que as datas, horas e duração sejam representadas na saída. Este campo será ignorado se a opção [!UICONTROL Value Render] estiver definida como Valor formatado. </td>
  </tr> 
  <tr>
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Número máximo de respostas]</td>
   <td> <p> Defina o número máximo de respostas que [!DNL Workfront Fusion] retorna durante um ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Respostas de pesquisa (Avançadas)]

Esse módulo realiza uma pesquisa usando o [[!DNL Google Charts Query Language]](https://developers.google.com/chart/interactive/docs/querylanguage). Esse módulo não retorna um número de linha.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Spreadsheet]</td>
   <td> <p>Selecione a planilha que contém a planilha que você deseja pesquisar.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Sheet]</td>
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
