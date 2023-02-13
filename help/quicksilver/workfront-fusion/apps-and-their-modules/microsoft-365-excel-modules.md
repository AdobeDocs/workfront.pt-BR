---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos Excel do Microsoft Office 365
description: Em um [!DNL Adobe Workfront Fusion] você pode automatizar fluxos de trabalho que usam o Microsoft 365 Excel, bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 9aa3739d-6800-4eb1-a17f-32fdfd8ed0f2
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2577'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Excel] módulos

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL Microsoft 365 Excel], bem como conectá-lo a vários aplicativos e serviços de terceiros.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p>  </td>  
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

Para usar [!DNL Microsoft office 365 Excel], você deve ter uma conta do Microsoft.

## [!DNL Microsoft Office 365 Excel] módulos e seus campos

Ao configurar [!DNL Microsoft 365 Excel] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Microsoft 365 Excel] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Pasta de Trabalho](#workbook)
* [Planilha](#worksheet)
* [Tabela](#table)
* [Outro](#other)

### Pasta de Trabalho

* [Ver pastas de trabalho](#watch-workbooks)
* [Pesquisar pastas de trabalho](#search-workbooks)
* [Baixar uma pasta de trabalho](#download-a-workbook)

#### [!UICONTROL Ver pastas de trabalho]

Esse módulo de acionador inicia um cenário quando uma pasta de trabalho é criada.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta]</td> 
   <td> <p>Selecione a pasta que deseja procurar por novas pastas de trabalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filtro]</p> </td> 
   <td> <p>Você pode definir um filtro para monitorar somente pastas de trabalho que atendem aos critérios selecionados.</p> <p>Para cada filtro, insira o campo que o filtro deve avaliar, o operador e o valor que você deseja que o filtro permita. Você pode usar mais de um filtro adicionando regras AND ou OR.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de pastas de trabalho que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Pesquisar pastas de trabalho]

Esse módulo de ação pesquisa por [!DNL Excel] pastas de trabalho.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta]</td> 
   <td> <p>Selecione a pasta que deseja pesquisar por pastas de trabalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filtro]</p> </td> 
   <td> <p>Você pode definir um filtro para pesquisar apenas pastas de trabalho que atendam aos critérios selecionados.</p> <p>Para cada filtro, insira o campo que o filtro deve avaliar, o operador e o valor que você deseja que o filtro permita. Você pode usar mais de um filtro adicionando regras AND ou OR.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de planilhas que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Baixar uma pasta de trabalho]

Este módulo de ação baixa o conteúdo da pasta de trabalho do Excel especificada.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Baixar uma pasta de trabalho]</td> 
   <td> <p>Selecione como deseja identificar a pasta de trabalho para download do módulo.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserindo uma ID manualmente]</strong> </p> <p>No campo [!UICONTROL ID da pasta de trabalho], insira ou mapeie a ID da pasta de trabalho específica que você deseja que o módulo baixe.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionando no caminho]</strong> </p> <p>No campo [!UICONTROL Pasta de trabalho], selecione a pasta de trabalho que deseja que o módulo baixe.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Planilha

* [[!UICONTROL Ver Linhas da Planilha]](#watch-worksheet-rows)
* [[!UICONTROL Planilhas de Lista]](#list-worksheets)
* [[!UICONTROL Listar Linhas da Planilha]](#list-worksheet-rows)
* [[!UICONTROL Adicionar uma Planilha]](#add-a-worksheet)
* [[!UICONTROL Adicionar uma Linha de Planilha]](#add-a-worksheet-row)
* [[!UICONTROL Atualizar uma Linha da Planilha]](#update-a-worksheet-row)
* [[!UICONTROL Excluir uma Linha de Planilha]](#delete-a-worksheet-row)

#### [!UICONTROL Ver Linhas da Planilha]

Esse módulo de acionamento inicia um cenário quando uma nova linha é adicionada à planilha.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Pasta de trabalho] </td>
   <td> <p>Selecione a pasta de trabalho que contém a planilha que você deseja visualizar para novas linhas.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Planilha] </td>
   <td> <p>Selecione a planilha do Excel que deseja visualizar para novas linhas.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limite]</td>
   <td> <p>Insira ou mapeie o número máximo de linhas de planilha que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Planilhas de Lista]

Esse módulo de ação recupera uma lista de planilhas na pasta de trabalho especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Pasta de trabalho] </td>
   <td> <p>Selecione a pasta de trabalho que contém as planilhas que você deseja que o módulo liste.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limite]</td>
   <td> <p>Insira ou mapeie o número máximo de planilhas que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listar Linhas da Planilha]

Esse módulo de ação recupera uma lista de linhas na planilha especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Pasta de trabalho] </td>
   <td> <p>Selecione a pasta de trabalho que contém a planilha que inclui as linhas que você deseja listar.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Planilha] </td>
   <td> <p>Selecione a planilha que contém as linhas que deseja listar.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limite]</td>
   <td> <p>Insira ou mapeie o número máximo de linhas de planilha que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Adicionar uma Planilha]

Esse módulo de ação cria uma nova planilha na pasta de trabalho selecionada.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Pasta de trabalho] </td>
   <td> <p>Selecione a pasta de trabalho onde deseja adicionar uma planilha.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Name] </td>
   <td> <p>Insira ou mapeie um nome para a nova planilha.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Adicionar uma Linha de Planilha]

Esse módulo de ação adiciona uma nova linha à planilha selecionada.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Pasta de trabalho] </td>
   <td> <p>Selecione a pasta de trabalho que contém a planilha à qual deseja adicionar uma linha.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Planilha] </td>
   <td> <p>Selecione a planilha à qual deseja adicionar uma linha.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de valores sendo inseridos]</p> </td> 
   <td> <p>Selecione o tipo de valor a ser inserido na planilha. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Fórmulas]</strong> </p> <p> O Excel tenta avaliar a expressão especificada. Os nomes das funções em uma fórmula são em inglês. Exemplo: <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL Fórmulas locais]</strong> </p> <p>O Excel tenta avaliar a expressão especificada. Os nomes das funções estão no idioma do aplicativo Excel. Exemplo: <code>=SUM(A1, 1.5)</code> vs <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[!UICONTROL Valor]</strong> </p> <p>O Excel não avalia o valor. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Linha]</td>
    <td>Para cada coluna, insira o valor que deseja que a coluna tenha na nova linha.</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar uma Linha da Planilha]

Esse módulo de ação atualiza uma linha de planilha existente.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Pasta de trabalho] </td>
   <td> <p>Selecione a pasta de trabalho que contém a planilha que inclui a linha que você deseja atualizar.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Planilha] </td>
   <td> <p>Selecione a planilha que contém a linha que você deseja atualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de valores sendo inseridos]</p> </td> 
   <td> <p>Selecione o tipo de valor a ser inserido na planilha. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Fórmulas]</strong> </p> <p> O Excel tenta avaliar a expressão especificada. Os nomes das funções em uma fórmula são em inglês. Exemplo: <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL Fórmulas locais]</strong> </p> <p>O Excel tenta avaliar a expressão especificada. Os nomes das funções estão no idioma do aplicativo Excel. Exemplo: <code>=SUM(A1, 1.5)</code> vs <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[!UICONTROL Valor]</strong> </p> <p>O Excel não avalia o valor. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da linha]</td> 
   <td>Selecione o número da linha a ser atualizada.</td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Linha]</td>
    <td>Para cada coluna, insira o valor que deseja que a coluna tenha na nova linha.</td>
   —&gt; 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir uma Linha de Planilha]

Esse módulo de ação exclui uma linha de uma planilha.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Pasta de trabalho] </td>
   <td> <p>Selecione a pasta de trabalho que contém a planilha que inclui a linha que você deseja excluir.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Planilha]</td>
   <td> <p> Selecione a planilha que contém a linha que você deseja excluir.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL ID da linha]</td>
   <td>Insira ou mapeie a ID da linha que deseja excluir.</td> 
  </tr> 
 </tbody> 
</table>

### Tabela

* [[!UICONTROL Exibir linhas da tabela]](#watch-table-rows)
* [[!UICONTROL Listar tabelas]](#list-tables)
* [[!UICONTROL Listar linhas de tabela]](#list-table-rows)
* [[!UICONTROL Obter uma tabela]](#get-a-table)
* [[!UICONTROL Adicionar uma tabela]](#add-a-table)
* [[!UICONTROL Adicionar uma linha de tabela]](#add-a-table-row)
* [[!UICONTROL Atualizar uma tabela]](#update-a-table)
* [[!UICONTROL Excluir uma tabela]](#delete-a-table)

#### [!UICONTROL Exibir linhas da tabela]

Esse acionador inicia um cenário quando uma nova linha é adicionada a uma tabela.

>[!NOTE]
>
>A tabela aqui se refere ao elemento de tabela incorporado na Pasta de trabalho. Não a tabela inteira (pasta de trabalho/planilha).

![](assets/embedded-table-350x420.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Pasta de trabalho]</p> </td> 
   <td> <p>Selecione a pasta de trabalho que contém a tabela que você deseja visualizar.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Planilha] </td>
   <td> <p> Selecione a planilha que contém a tabela que você deseja visualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tabela]</p> </td> 
   <td> <p>Selecione a tabela que deseja visualizar.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limite]</td>
   <td> <p>Insira ou mapeie o número máximo de linhas que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listar tabelas]

Esse módulo de pesquisa recupera uma lista de todos os objetos da tabela.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Pasta de trabalho] </td>
   <td> <p>Selecione a pasta de trabalho que contém as tabelas que deseja listar.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Planilha] </td>
   <td> <p>Selecione a planilha que contém as tabelas que deseja listar</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limite]</td>
   <td> <p>Insira ou mapeie o número máximo de tabelas que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listar linhas de tabela]

Esse módulo de pesquisa recupera uma lista de todas as linhas da tabela em uma pasta de trabalho.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Pasta de trabalho] </td>
   <td> <p>Selecione a pasta de trabalho que contém a tabela que inclui as linhas que você deseja listar.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Planilha] </td>
   <td> <p>Selecione a planilha que contém a tabela que inclui as linhas que você deseja listar</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Tabela] </td>
   <td> <p>Selecione a tabela que contém as linhas que deseja listar.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limite]</td>
   <td> <p>Insira ou mapeie o número máximo de linhas da tabela que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter uma tabela]

Esse módulo de ação recupera metadados para a tabela especificada.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
     <p >[!UICONTROL Connection]</p>
   </td> 
   <td> 
     <p>Para obter instruções sobre como conectar sua conta do Office 365 para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p>
    --&gt; </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obter uma tabela]</td> 
   <td> <p>Selecione como deseja identificar a tabela que deseja recuperar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>No campo [!UICONTROL ID da pasta de trabalho], insira ou mapeie a ID da pasta de trabalho que contém a tabela que você deseja recuperar.</p> <p>No campo [!UICONTROL Table Name], insira ou mapeie o nome da tabela que deseja recuperar.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione a pasta de trabalho e a planilha que contêm a tabela que você deseja recuperar e selecione a tabela.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Adicionar uma tabela]

Esse módulo de ação cria um elemento de tabela dentro da planilha do Excel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta de trabalho] </td> 
   <td> <p>Selecione a pasta de trabalho que contém a planilha à qual deseja adicionar uma tabela.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planilha] </td> 
   <td> <p>Selecione a planilha à qual deseja adicionar uma tabela.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tem cabeçalhos]</td> 
   <td> <p>Ative essa opção para definir a primeira linha como cabeçalhos da tabela.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Endereço]</p> </td> 
   <td> <p>Defina o tamanho da tabela indicando as células superior esquerda e inferior direita. Exemplo: <code>A1:C10</code> cria uma tabela com 3 colunas e 10 linhas.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Adicionar uma linha de tabela]

Este módulo de ação modifica uma tabela existente.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Pasta de trabalho] </td>
   <td> <p>Selecione a pasta de trabalho que contém a tabela à qual deseja adicionar uma linha.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Planilha] </td>
   <td> <p>Selecione a planilha que contém a tabela à qual deseja adicionar uma linha.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Tabela]</td>
   <td>Selecione a tabela à qual deseja adicionar uma linha.</td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Linha]</td>
    <td>Para cada coluna, insira o valor que deseja que a coluna tenha na nova linha.</td>
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID da linha]</p> </td> 
   <td> <p>Para adicionar uma linha em um local específico na tabela, digite ou mapeie um número de linha. O módulo insere a nova linha após essa linha.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar uma tabela]

Este módulo de ação atualiza uma tabela existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Atualizar uma tabela]</td> 
   <td> <p>Selecione como deseja identificar a tabela que deseja atualizar.</p> 
    <ul> 
     <li> <p><strong>Inserir manualmente</strong> </p> <p>No campo [!UICONTROL ID da pasta de trabalho], insira ou mapeie a ID da pasta de trabalho que contém a tabela que você deseja atualizar.</p> <p>No campo [!UICONTROL Table Name], insira ou mapeie o nome da tabela que deseja atualizar.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione a pasta de trabalho e a planilha que contêm a tabela que você deseja atualizar e selecione a tabela.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabela] </td> 
   <td> <p>Selecione a tabela que deseja atualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td> <p>Se quiser renomear a tabela, insira ou mapeie um novo nome para a tabela.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar cabeçalhos]</td> 
   <td> <p>Ative essa opção para mostrar os cabeçalhos da tabela atualizada.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar totais]</td> 
   <td>Ative essa opção para mostrar os valores totais da tabela.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Estilo]</td> 
   <td>Escolha um estilo para a nova tabela.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir uma tabela]

Esse módulo de ação exclui a tabela especificada de um [!DNL Excel] planilha.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obter uma tabela]</td> 
   <td> <p>Selecione como deseja identificar a tabela que deseja excluir.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>No campo [!UICONTROL ID da pasta de trabalho], insira ou mapeie a ID da pasta de trabalho que contém a tabela que você deseja excluir.</p> <p>No campo [!UICONTROL Table Name], insira ou mapeie o nome da tabela que deseja excluir.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione a pasta de trabalho e a planilha que contêm a tabela que você deseja excluir, em seguida, selecione a tabela.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Outro

* [[!UICONTROL Recuperar dados]](#retrieve-data)
* [[!UICONTROL Faça uma chamada de API]](#make-an-api-call)

#### [!UICONTROL Recuperar dados]

Essa ação recupera dados do intervalo de planilhas definido e retorna um pacote para cada linha.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta de trabalho] </td> 
   <td> <p>Selecione a pasta de trabalho que contém os dados que deseja recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planilha] </td> 
   <td> <p>Selecione a planilha que contém os dados que deseja recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Intervalo] </td> 
   <td> <p>Especifique a área da planilha da qual deseja recuperar dados, indicando as células superior esquerda e inferior direita. Exemplo: <code>A1:D10</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Faça uma chamada de API]

Esse módulo de ação permite fazer uma chamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Insira um caminho relativo a <code>https://graph.microsoft.com</code>. Exemplo:<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   td&gt; <p>Selecione o método de solicitação HTTP que você precisa configurar a chamada da API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> <p>O Workfront Fusion adiciona os cabeçalhos de autorização para você.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sequência de consulta]</td> 
   <td> <p>Adicione a query para a chamada de API no formato de um objeto JSON padrão.</p> <p>Por exemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada da API no formato de um objeto JSON padrão.</p> <p>Nota:   <p>Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
