---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos SharePoint
description: Em um [!DNL Adobe Workfront Fusion] você pode automatizar workflows que usam o SharePoint, bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: 16d49031-06d2-4c86-bac4-f58cd9b2f1f5
source-git-commit: aee0778b08e00b2fc94f6829e6b2cd957ff0fe23
workflow-type: tm+mt
source-wordcount: '2802'
ht-degree: 0%

---

# [!DNL SharePoint] módulos

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL SharePoint], bem como conectá-lo a vários aplicativos e serviços de terceiros.

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

Para usar [!DNL SharePoint] módulos, você deve ter um [!DNL SharePoint] conta.

## Connect [!DNL SharePoint] para [!DNL Workfront Fusion] {#connect-sharepoint-to-workfront-fusion}

* [Connect [!DNL SharePoint] para [!DNL Workfront Fusion] usando um [!DNL Microsoft] account](#connect-sharepoint-to-workfront-fusion-using-a-microsoft-account)
* [Connect [!DNL SharePoint] para [!DNL Workfront Fusion] usando configurações avançadas](#connect-sharepoint-to-workfront-fusion-using-advanced-settings)

### Connect [!DNL SharePoint] para [!DNL Workfront Fusion] usando um [!DNL Microsoft] account

Você pode usar o [!DNL Microsoft] conta para criar uma conexão com [!DNL SharePoint]. Para obter instruções sobre como conectar seu [!DNL Sharepoint] para [!DNL Workfront Fusion], consulte [Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

### Connect [!DNL SharePoint] para [!DNL Workfront Fusion] usando configurações avançadas

Para ligar [!DNL SharePoint] para [!DNL Workfront Fusion] sem um [!DNL Microsoft] , você precisa de uma ID do cliente, um Segredo do cliente e uma ID do locatário.

1. Clique em **[!UICONTROL Adicionar]** perto da parte superior do **[!DNL SharePoint]** para abrir o **[!UICONTROL Criar uma conexão]** caixa.

1. (Opcional) Alterar o padrão **[!UICONTROL Nome da conexão]**.
1. Clique em **[!UICONTROL Mostrar configurações avançadas]**.
1. Insira o [!DNL SharePoint] **[!UICONTROL ID do cliente]** e **[!UICONTROL Segredo do cliente]**.

1. Clique em **[!UICONTROL Continuar]**.
1. Na janela de logon que é exibida, insira suas credenciais para fazer logon no aplicativo, caso ainda não o tenha feito.
1. (Condicional) Se um **[!UICONTROL Permitir]** for exibido, clique no botão para conectar o aplicativo ao [!DNL Workfront Fusion].

## [!DNL SharePoint] módulos e seus campos

Ao configurar [!DNL SharePoint] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL SharePoint] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Item da unidade](#drive-item)
* [Item](#item)
* [Lista](#list)
* [Página (Beta)](#page-beta)
* [Site](#site)
* [Outro](#other)

### Item da unidade

* [Criar um arquivo](#create-a-file)
* [Criar uma pasta](#create-a-folder)
* [Obter um arquivo](#get-a-file)
* [Ver itens da pasta](#watch-folder-items)

#### Obter alterações

Esse módulo retorna alterações que foram feitas no SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL SharePoint] para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir IDs de site, unidade e pasta]</td> 
   <td> <p>Selecione como deseja identificar o local da pasta em que deseja recuperar as alterações.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a variável <strong>[!UICONTROL ID do site]</strong>, <strong>[!UICONTROL List ID]</strong>e <strong>[!UICONTROL ID da pasta]</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista que você segue]</strong> </p> <p>Selecione o local onde deseja recuperar as alterações. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Token]</td> 
   <td> </td> 
  </tr>  </tbody> 
</table>

#### Criar uma pasta

Esse módulo de ação cria uma nova pasta no SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL SharePoint] para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir IDs de site, unidade e pasta]</td> 
   <td> <p>Selecione como deseja identificar o local da pasta que deseja criar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a variável <strong>[!UICONTROL ID do site]</strong>, <strong>[!UICONTROL List ID]</strong>e <strong>[!UICONTROL ID da pasta]</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista que você segue]</strong> </p> <p>Selecione o local onde deseja criar a pasta. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome da pasta]</td> 
   <td>Insira ou mapeie um nome para a nova pasta.</td> 
  </tr>
  </tbody> 
</table>

#### Obter um arquivo

Esse módulo de ação recupera o arquivo SharePoint especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL SharePoint] para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir IDs de site, unidade e pasta]</td> 
   <td> <p>Selecione como deseja identificar o local do arquivo que deseja obter.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a variável <strong>[!UICONTROL ID do site]</strong>, <strong>[!UICONTROL List ID]</strong>e <strong>[!UICONTROL ID do arquivo]</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista que você segue]</strong> </p> <p>Selecione o local do arquivo. </p> </li> 
    </ul> </td> 
  </tr> 
</tbody> 
</table>

#### Ver itens da pasta

Este módulo de acionador inicia um cenário quando um item é atualizado em uma pasta selecionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL SharePoint] para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir IDs de site, unidade e pasta]</td> 
   <td> <p>Selecione como deseja identificar o local do arquivo que deseja obter.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a variável <strong>[!UICONTROL ID do site]</strong>, <strong>[!UICONTROL List ID]</strong>e <strong>[!UICONTROL ID da pasta]</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista que você segue]</strong> </p> <p>Selecione o local da pasta que deseja visualizar. </p> </li> 
    </ul> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Inserir o número máximo de itens [!DNL Workfront Fusion] deve retornar durante um ciclo de execução de cenário.</td> 
  <tr>
  </tr>
</tbody> 
</table>

### Item

* [[!UICONTROL Copiar item]](#copy-an-item)
* [[!UICONTROL Criar um item]](#create-an-item)
* [[!UICONTROL Excluir um item]](#delete-an-item)
* [[!UICONTROL Obter um item]](#get-an-item)
* [[!UICONTROL Listar itens]](#list-items)
* [[!UICONTROL Mover item]](#move-an-item)
* [[!UICONTROL Atualizar um item]](#update-an-item)
* [[!UICONTROL Itens de observação] (Programado)](#watch-items-scheduled)


#### [!UICONTROL Copiar item]

Este módulo de ação copia um item existente em uma lista do SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL SharePoint] para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Inserir IDs de site, unidade e pasta</td> 
   <td> <p>Selecione como deseja identificar o site e a lista que contém o item que deseja copiar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a variável <strong>[!UICONTROL ID do site]</strong>, <strong>[!UICONTROL List ID]</strong>e <strong>[!UICONTROL ID do item]</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar da lista que você segue]</strong> </p> <p>No campo Tipo de item , selecione se você está movendo um campo ou uma pasta.  Selecione o site que contém o item que você deseja copiar, selecione a lista e selecione o item. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de destino]</td> 
   <td> Insira ou mapeie a ID da pasta para a qual deseja copiar o item. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Novo nome]</td> 
   <td>Insira ou mapeie um nome para a nova cópia do item. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar um item]

Esse módulo de ação cria um novo item em uma lista do SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL SharePoint] para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Criar um item]</td> 
   <td> <p>Selecione como deseja identificar o site e a lista onde deseja criar um item.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a variável <strong>[!UICONTROL ID do site]</strong> e <strong>[!UICONTROL List ID]</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione o site que contém a lista onde deseja criar um item e selecione a lista. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos]</td> 
   <td>Para cada campo que deseja definir para o novo item, insira a chave do campo (identifica o campo) e o valor que deseja que o novo item tenha para esse campo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir um item]

Esse módulo de ação exclui um item existente em uma lista do SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL SharePoint] para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Atualizar um item]</td> 
   <td> <p>Selecione como deseja identificar o site e a lista que contém o item que deseja excluir.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a variável <strong>[!UICONTROL ID do site]</strong>, <strong>[!UICONTROL List ID]</strong>e <strong>[!UICONTROL ID do item]</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione o site que contém o item que deseja excluir, selecione a lista e selecione o item. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um item]

Esse módulo de ação retorna os dados de um item especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL SharePoint] para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obter um item]</td> 
   <td> <p>Selecione como deseja identificar o site e a lista que contém o item que deseja obter.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a variável <strong>[!UICONTROL ID do site]</strong>, <strong>[!UICONTROL List ID]</strong>e <strong>[!UICONTROL ID do item]</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione o site que contém a lista da qual você deseja recuperar um item, selecione a lista e selecione o item. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listar itens]

Este módulo de ação recupera uma lista de todos os itens em uma lista especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL SharePoint] para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Listar itens]</td> 
   <td> <p>Selecione como deseja identificar a lista da qual deseja recuperar itens.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a variável <strong>[!UICONTROL ID do site]</strong> e <strong>[!UICONTROL List ID]</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione o site que contém a lista da qual você deseja recuperar itens e selecione a lista. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de itens que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover um item]

Este módulo de ação copia um item existente em uma lista do SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL SharePoint] para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Inserir IDs de site, unidade e pasta</td> 
   <td> <p>Selecione como deseja identificar o site e a lista que contém o item que deseja mover.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a variável <strong>[!UICONTROL ID do site]</strong>, <strong>[!UICONTROL List ID]</strong>e <strong>[!UICONTROL ID do item]</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar da lista que você segue]</strong> </p> <p>No campo Tipo de item , selecione se você está movendo um campo ou uma pasta. Selecione o site que contém o item que você deseja copiar, selecione a lista e selecione o item. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de destino]</td> 
   <td> Insira ou mapeie a ID da pasta para a qual deseja mover o item. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Novo nome]</td> 
   <td>Insira ou mapeie um nome para o item movido. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar um item]

Esse módulo de ação atualiza um item existente em uma lista do SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL SharePoint] para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Atualizar um item]</td> 
   <td> <p>Selecione como deseja identificar o site e a lista que contém o item que deseja atualizar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a variável <strong>[!UICONTROL ID do site]</strong>, <strong>[!UICONTROL List ID]</strong>e <strong>[!UICONTROL ID do item]</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione o site que contém o item que você deseja atualizar, selecione a lista e selecione o item. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos]</td> 
   <td>Para cada campo que deseja atualizar para o novo item, insira a chave do campo (identifica o campo) e o novo valor que você deseja que o item tenha para esse campo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Itens de observação] (Programado)

Esse módulo de acionador inicia um cenário quando um item é criado ou modificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL SharePoint] para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Listas de monitoramento]</td> 
   <td>Selecione se deseja ver as listas por tempo de criação (novos itens) ou por tempo de modificação (itens atualizados).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir ID de site e lista]</td> 
   <td> <p>Selecione como deseja identificar o site e a lista que deseja visualizar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a variável <strong>[!UICONTROL ID do site]</strong> e <strong>[!UICONTROL List ID]</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista que você segue]</strong> </p> <p>Selecione o site que deseja visualizar e selecione a lista. Esses menus suspensos recuperam somente os sites seguidos.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de itens que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Lista

* [[!UICONTROL Criar uma lista]](#create-a-list)
* [[!UICONTROL Obter uma lista]](#get-a-list)
* [[!UICONTROL Listas]](#list-lists)
* [[!UICONTROL Listas de monitoramento]](#watch-lists)

#### [!UICONTROL Criar uma lista]

Esse módulo de ação cria uma nova lista no SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL SharePoint] para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir uma ID de site]</td> 
   <td> <p>Selecione como deseja identificar o site e a lista onde deseja criar uma lista.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a variável <strong>[!UICONTROL ID do site]</strong> onde deseja criar uma lista.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione o site onde deseja criar uma lista. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Exibir nome]</td> 
   <td>Insira ou mapeie um nome para a nova lista.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descrição]</td> 
   <td>Insira ou mapeie uma descrição para a nova lista.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adicionar colunas]</td> 
   <td>Para cada coluna que deseja definir para a nova lista, insira um <strong>[!UICONTROL Name]</strong> para o campo e selecione o <strong>[!UICONTROL Tipo]</strong> do valor que você deseja que a nova coluna tenha.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter uma lista]

Esse módulo de ação retorna os dados de uma lista especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL SharePoint] para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obter uma lista]</td> 
   <td> <p>Selecione como deseja identificar o site e a lista que contém o item que deseja obter.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a variável <strong>[!UICONTROL ID do site]</strong> e <strong>ID da lista</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione o site que contém a lista que você deseja recuperar e selecione a lista. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listas]

Este módulo de ação recupera uma lista de todos os itens em uma lista especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL SharePoint] para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lista Listas]</td> 
   <td> <p>Selecione como deseja identificar o site do qual deseja recuperar listas.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a variável <strong>[!UICONTROL ID do site]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione o site que contém as listas que você deseja recuperar. A lista suspensa recupera somente os sites que você seguir.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de listas que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listas de monitoramento]

Esse módulo de acionador inicia um cenário quando uma lista é criada ou modificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL SharePoint] para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Listas de monitoramento]</td> 
   <td>Selecione se deseja ver as listas por tempo de criação (novos itens) ou por tempo de modificação (itens atualizados).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir ID de site e lista]</td> 
   <td> <p>Selecione como deseja identificar o site e a lista que deseja visualizar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a variável <strong>[!UICONTROL ID do site]</strong> onde a lista que você deseja assistir está localizada.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista que você segue]</strong> </p> <p>Selecione o site que deseja visualizar. A lista suspensa recupera apenas o site que você seguir.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de listas que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Página (Beta)

>[!NOTE]
>
>As APIs no `beta` versão em [!DNL Microsoft Graph] estão sujeitas a alterações. O uso dessas APIs em aplicativos de produção não é suportado.

#### [!UICONTROL Obter uma página]

Esse módulo de ação retorna os dados de uma página especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL SharePoint] para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obter uma página]</td> 
   <td> <p>Selecione como você deseja identificar a página que deseja recuperar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a variável <strong>[!UICONTROL ID do site]</strong>e <strong>[!UICONTROL ID da página]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione o site que contém a página que você deseja recuperar e selecione a página.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Site

* [[!UICONTROL Obter um site]](#get-a-site)
* [[!UICONTROL Sites de pesquisa]](#search-sites)

#### [!UICONTROL Obter um site]

Esse módulo de ação retorna os dados de um site especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL SharePoint] para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obter um site]</td> 
   <td> <p>Selecione como você deseja identificar a página que deseja recuperar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a variável <strong>[!UICONTROL ID do site]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione o site que deseja recuperar.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Sites de pesquisa]

Este módulo de ação pesquisa sites por um parâmetro especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL SharePoint] para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Palavra-chave de nome de exibição]</td> 
   <td> <p>Insira ou mapeie o termo de pesquisa que deseja pesquisar nos sites.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de sites que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Outro

#### Obter alterações

Esse módulo recupera adições, atualizações e exclusões feitas na pasta SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL SharePoint] para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir IDs de site, unidade e pasta]</td> 
   <td> <p>Selecione como deseja identificar o site e a lista que contém o item que deseja atualizar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a variável <strong>[!UICONTROL ID do site]</strong>, <strong>[!UICONTROL ID da unidade]</strong>e <strong>[!UICONTROL ID da pasta]</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione o site que contém o item que você deseja atualizar, selecione a unidade e selecione a pasta. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Token]</td> 
   <td> O token identifica a partir de que ponto o módulo deve começar a recuperar as alterações.  </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Faça uma chamada de API]

Esse módulo permite executar uma chamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL SharePoint] para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Insira um caminho relativo a <code>https://graph.microsoft.com</code>. Exemplo:<code> /beta/sites</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   <td> <p>Selecione o método de solicitação HTTP que você precisa configurar a chamada da API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão. Por exemplo, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] adiciona os cabeçalhos de autorização para você.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sequência de consulta]</td> 
   <td> <p> Adicione a query para a chamada de API no formato de um objeto JSON padrão.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo]</td> 
   <td>Selecione o tipo de dados que deseja enviar na chamada de API.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada da API no formato de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Monitoramento de eventos

Esse módulo de acionador instantâneo inicia um cenário quando um item é adicionado, atualizado ou excluído no SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
  <!--
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL SharePoint] account to [!DNL Workfront Fusion], see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  -->
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Selecione um webhook existente ou clique em Adicionar para criar um novo webhook.</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

