---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do SharePoint
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: 16d49031-06d2-4c86-bac4-f58cd9b2f1f5
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '2929'
ht-degree: 0%

---

# [!DNL SharePoint] módulos

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [módulos do SharePoint](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/sharepoint-modules.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

Em um cenário [!DNL Adobe Workfront Fusion], você pode automatizar fluxos de trabalho que usam [!DNL SharePoint], bem como conectá-los a vários aplicativos e serviços de terceiros.

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
   <p>Requisito atual do produto: se você tiver o plano [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], sua organização deve comprar [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] da [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Para usar módulos [!DNL SharePoint], você deve ter uma conta [!DNL SharePoint].

## Informações da API do SharePoint

O conector do SharePoint usa o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL base</td> 
   <td> https://graph.microsoft.com/v1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Versão da API</td> 
   <td> v1.0 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tag da API</td> 
   <td>v1.14.2</td> 
  </tr>
 </tbody> 
 </table>

## Conectar [!DNL SharePoint] a [!DNL Workfront Fusion] {#connect-sharepoint-to-workfront-fusion}

* [Conectar [!DNL SharePoint] ao [!DNL Workfront Fusion] usando uma [!DNL Microsoft] conta](#connect-sharepoint-to-workfront-fusion-using-a-microsoft-account)
* [Conectar [!DNL SharePoint] a [!DNL Workfront Fusion] usando configurações avançadas](#connect-sharepoint-to-workfront-fusion-using-advanced-settings)

### Conectar [!DNL SharePoint] a [!DNL Workfront Fusion] usando uma conta [!DNL Microsoft]

Você pode usar sua conta [!DNL Microsoft] para criar uma conexão com [!DNL SharePoint]. Para obter instruções sobre como conectar sua conta do [!DNL Sharepoint] ao [!DNL Workfront Fusion], consulte [Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

### Conectar [!DNL SharePoint] a [!DNL Workfront Fusion] usando configurações avançadas

Para conectar [!DNL SharePoint] a [!DNL Workfront Fusion] sem uma conta [!DNL Microsoft], você precisa de uma ID de Cliente, um Segredo de Cliente e uma ID de Locatário.

1. Clique em **[!UICONTROL Adicionar]** próximo à parte superior da caixa **[!DNL SharePoint]** para abrir a caixa **[!UICONTROL Criar uma conexão]**.

1. (Opcional) Altere o **[!UICONTROL Nome da conexão]** padrão.
1. Clique em **[!UICONTROL Mostrar configurações avançadas]**.
1. Insira a [!DNL SharePoint] **[!UICONTROL ID do Cliente]** e o **[!UICONTROL Segredo do Cliente]**.

1. Clique em **[!UICONTROL Continuar]**.
1. Na janela de logon que é exibida, digite suas credenciais para fazer logon no aplicativo, se ainda não tiver feito.
1. (Condicional) Se um botão **[!UICONTROL Permitir]** for exibido, clique no botão para conectar o aplicativo a [!DNL Workfront Fusion].

## [!DNL SharePoint] módulos e seus campos

Ao configurar módulos do [!DNL SharePoint], o [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos [!DNL SharePoint] adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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
* [Observar itens da pasta](#watch-folder-items)

#### Obter alterações

Este módulo retorna as alterações feitas no SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL SharePoint] ao [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir Site, Unidade e IDs de Pasta]</td> 
   <td> <p>Selecione como você deseja identificar o local da pasta na qual deseja recuperar as alterações.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a <strong>[!UICONTROL ID do Site]</strong>, <strong>[!UICONTROL ID da Lista]</strong> e <strong>[!UICONTROL ID da Pasta]</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista que você segue]</strong> </p> <p>Selecione o local onde deseja recuperar as alterações. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Token]</td> 
   <td> </td> 
  </tr>  </tbody> 
</table>

#### Criar uma pasta

Este módulo de ação cria uma nova pasta no SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL SharePoint] ao [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir Site, Unidade e IDs de Pasta]</td> 
   <td> <p>Selecione como deseja identificar o local da pasta que deseja criar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a <strong>[!UICONTROL ID do Site]</strong>, <strong>[!UICONTROL ID da Lista]</strong> e <strong>[!UICONTROL ID da Pasta]</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista que você segue]</strong> </p> <p>Selecione o local em que deseja criar a pasta. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome da pasta]</td> 
   <td>Insira ou mapeie um nome para a nova pasta.</td> 
  </tr>
  </tbody> 
</table>

#### Obter um arquivo

Este módulo de ação recupera o arquivo SharePoint especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL SharePoint] ao [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir Site, Unidade e IDs de Pasta]</td> 
   <td> <p>Selecione como você deseja identificar o local do arquivo que deseja obter.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a <strong>[!UICONTROL ID do Site]</strong>, <strong>[!UICONTROL ID da Lista]</strong> e <strong>[!UICONTROL ID do Arquivo]</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista que você segue]</strong> </p> <p>Selecione o local do arquivo. </p> </li> 
    </ul> </td> 
  </tr> 
</tbody> 
</table>

#### Observar itens da pasta

Este módulo de acionamento inicia um cenário quando um item é atualizado em uma pasta selecionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL SharePoint] ao [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir Site, Unidade e IDs de Pasta]</td> 
   <td> <p>Selecione como você deseja identificar o local do arquivo que deseja obter.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a <strong>[!UICONTROL ID do Site]</strong>, <strong>[!UICONTROL ID da Lista]</strong> e <strong>[!UICONTROL ID da pasta]</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista que você segue]</strong> </p> <p>Selecione o local da pasta que deseja observar. </p> </li> 
    </ul> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Insira o número máximo de itens que [!DNL Workfront Fusion] deve retornar durante um ciclo de execução de cenário.</td> 
  <tr>
  </tr>
</tbody> 
</table>

### Item

* [[!UICONTROL Copiar um item]](#copy-an-item)
* [[!UICONTROL Criar um item]](#create-an-item)
* [[!UICONTROL Excluir um item]](#delete-an-item)
* [[!UICONTROL Obter um Item]](#get-an-item)
* [[!UICONTROL Listar itens]](#list-items)
* [[!UICONTROL Mover Item]](#move-an-item)
* [[!UICONTROL Atualizar um item]](#update-an-item)
* [[!UICONTROL Itens de observação] (Agendados)](#watch-items-scheduled)


#### [!UICONTROL Copiar item]

Este módulo de ação copia um item existente em uma lista do SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL SharePoint] ao [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Inserir IDs de site, unidade e pasta</td> 
   <td> <p>Selecione como deseja identificar o site e a lista que contém o item que deseja copiar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a <strong>[!UICONTROL ID do Site]</strong>, <strong>[!UICONTROL ID da Lista]</strong> e <strong>[!UICONTROL ID do Item]</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista que você segue]</strong> </p> <p>No campo Tipo de Item, selecione se deseja mover um campo ou uma pasta.  Selecione o site que contém o item que você deseja copiar, selecione a lista e selecione o item. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Destino]</td> 
   <td> Insira ou mapeie a ID da pasta para a qual você deseja copiar o item. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Novo nome]</td> 
   <td>Insira ou mapeie um nome para a nova cópia do item. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar um item]

Este módulo de ação cria um novo item em uma lista do SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL SharePoint] ao [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Criar um Item]</td> 
   <td> <p>Selecione como você deseja identificar o site e a lista onde deseja criar um item.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a <strong>[!UICONTROL ID do Site]</strong> e a <strong>[!UICONTROL ID da Lista]</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione o site que contém a lista onde você deseja criar um item e selecione-a. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos]</td> 
   <td>Para cada campo que você deseja definir para o novo item, insira a chave do campo (identifica o campo) e o valor que você deseja que o novo item tenha para esse campo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir um item]

Este módulo de ação exclui um item existente em uma lista do SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL SharePoint] ao [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Atualizar um Item]</td> 
   <td> <p>Selecione como você deseja identificar o site e a lista que contém o item que você deseja excluir.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a <strong>[!UICONTROL ID do Site]</strong>, <strong>[!UICONTROL ID da Lista]</strong> e <strong>[!UICONTROL ID do Item]</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione o site que contém o item que você deseja excluir, selecione a lista e selecione o item. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um Item]

Este módulo de ação retorna os dados de um item especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL SharePoint] ao [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obter um Item]</td> 
   <td> <p>Selecione como você deseja identificar o site e a lista que contém o item que você deseja obter.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a <strong>[!UICONTROL ID do Site]</strong>, <strong>[!UICONTROL ID da Lista]</strong> e <strong>[!UICONTROL ID do Item]</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione o site que contém a lista da qual você deseja recuperar um item e selecione a lista e, em seguida, o item. </p> </li> 
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
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL SharePoint] ao [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Listar Itens]</td> 
   <td> <p>Selecione como deseja identificar a lista da qual deseja recuperar os itens.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a <strong>[!UICONTROL ID do Site]</strong> e a <strong>[!UICONTROL ID da Lista]</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione o site que contém a lista da qual deseja recuperar itens e selecione-a. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de itens que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover um Item]

Este módulo de ação copia um item existente em uma lista do SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL SharePoint] ao [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Inserir IDs de site, unidade e pasta</td> 
   <td> <p>Selecione como você deseja identificar o site e a lista que contém o item que você deseja mover.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a <strong>[!UICONTROL ID do Site]</strong>, <strong>[!UICONTROL ID da Lista]</strong> e <strong>[!UICONTROL ID do Item]</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista que você segue]</strong> </p> <p>No campo Tipo de Item, selecione se deseja mover um campo ou uma pasta. Selecione o site que contém o item que você deseja copiar, selecione a lista e selecione o item. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Destino]</td> 
   <td> Insira ou mapeie a ID da pasta para onde deseja mover o item. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Novo nome]</td> 
   <td>Insira ou mapeie um nome para o item movido. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar um item]

Este módulo de ação atualiza um item existente em uma lista do SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL SharePoint] ao [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Atualizar um Item]</td> 
   <td> <p>Selecione como você deseja identificar o site e a lista que contém o item que você deseja atualizar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a <strong>[!UICONTROL ID do Site]</strong>, <strong>[!UICONTROL ID da Lista]</strong> e <strong>[!UICONTROL ID do Item]</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione o site que contém o item que você deseja atualizar, selecione a lista e selecione o item. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos]</td> 
   <td>Para cada campo que você deseja atualizar para o novo item, informe a chave do campo (identifica o campo) e o novo valor que você deseja que o item tenha para esse campo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Itens de observação] (Agendados)

Esse módulo de acionamento inicia um cenário quando um item é criado ou modificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL SharePoint] ao [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Listas de Observação]</td> 
   <td>Selecione se deseja monitorar as listas por hora de criação (novos itens) ou por hora de modificação (itens atualizados).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir Site e ID de Lista]</td> 
   <td> <p>Selecione como deseja identificar o site e a lista que deseja observar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a <strong>[!UICONTROL ID do Site]</strong> e a <strong>[!UICONTROL ID da Lista]</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista que você segue]</strong> </p> <p>Selecione o site que deseja observar e selecione a lista. Esses menus suspensos recuperam apenas os sites seguidos.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de itens que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Lista

* [[!UICONTROL Criar uma Lista]](#create-a-list)
* [[!UICONTROL Obter uma Lista]](#get-a-list)
* [[!UICONTROL Listar listas]](#list-lists)
* [[!UICONTROL Listas de Interesse]](#watch-lists)

#### [!UICONTROL Criar uma Lista]

Este módulo de ação cria uma nova lista no SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL SharePoint] ao [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir uma ID de Site]</td> 
   <td> <p>Selecione como deseja identificar o site e a lista em que deseja criar uma lista.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie o <strong>[!UICONTROL ID do Site]</strong> onde deseja criar uma lista.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione o site no qual deseja criar uma lista. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome para Exibição]</td> 
   <td>Insira ou mapeie um nome para a nova lista.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descrição]</td> 
   <td>Insira ou mapeie uma descrição para a nova lista.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adicionar Colunas]</td> 
   <td>Para cada coluna que você deseja definir para a nova lista, insira um <strong>[!UICONTROL Name]</strong> para o campo e selecione o <strong>[!UICONTROL Type]</strong> do valor que você deseja que a nova coluna tenha.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter uma Lista]

Este módulo de ação retorna os dados de uma lista especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL SharePoint] ao [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obter uma Lista]</td> 
   <td> <p>Selecione como você deseja identificar o site e a lista que contém o item que você deseja obter.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a <strong>[!UICONTROL ID do Site]</strong> e a <strong>ID da Lista</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione o site que contém a lista que você deseja recuperar e, em seguida, selecione a lista. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listar listas]

Este módulo de ação recupera uma lista de todos os itens em uma lista especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL SharePoint] ao [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Listas de Listas]</td> 
   <td> <p>Selecione como você deseja identificar o site do qual deseja recuperar listas.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie o <strong>[!UICONTROL ID do Site]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione o site que contém as listas que você deseja recuperar. O menu suspenso recupera apenas os sites que você segue.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de listas que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listas de Interesse]

Esse módulo de acionador inicia um cenário quando uma lista é criada ou modificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL SharePoint] ao [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Listas de Observação]</td> 
   <td>Selecione se deseja monitorar as listas por hora de criação (novos itens) ou por hora de modificação (itens atualizados).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir Site e ID de Lista]</td> 
   <td> <p>Selecione como deseja identificar o site e a lista que deseja observar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie o <strong>[!UICONTROL ID do Site]</strong> onde a lista que você deseja assistir está localizada.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista que você segue]</strong> </p> <p>Selecione o site que deseja assistir. O menu suspenso recupera apenas o site que você segue.</p> </li> 
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
>As APIs na versão `beta` em [!DNL Microsoft Graph] estão sujeitas a alterações. O uso dessas APIs em aplicativos de produção não é compatível.

#### [!UICONTROL Obter uma página]

Este módulo de ação retorna os dados de uma página especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL SharePoint] ao [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obter uma Página]</td> 
   <td> <p>Selecione como você deseja identificar a página que deseja recuperar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a <strong>[!UICONTROL ID do Site]</strong>e <strong>[!UICONTROL ID da Página]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione o site que contém a página que você deseja recuperar e selecione a página.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Site

* [[!UICONTROL Obter um site]](#get-a-site)
* [[!UICONTROL Pesquisar Sites]](#search-sites)

#### [!UICONTROL Obter um site]

Este módulo de ação retorna os dados de um site especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL SharePoint] ao [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obter um Site]</td> 
   <td> <p>Selecione como você deseja identificar a página que deseja recuperar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie o <strong>[!UICONTROL ID do Site]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione o site que deseja recuperar.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Pesquisar Sites]

Esse módulo de ação pesquisa sites por um parâmetro especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL SharePoint] ao [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Palavra-chave do Nome para Exibição]</td> 
   <td> <p>Insira ou mapeie o termo de pesquisa que você deseja pesquisar nos sites.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de sites que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Outro

* [Obter alterações](#get-changes)
* [Fazer uma chamada de API](#make-an-api-call)
* [Assistir a eventos](#watch-events)

#### Obter alterações

Este módulo recupera adições, atualizações e exclusões feitas na pasta do SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL SharePoint] ao [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir Site, Unidade e IDs de Pasta]</td> 
   <td> <p>Selecione como você deseja identificar o site e a lista que contém o item que você deseja atualizar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a <strong>[!UICONTROL ID do Site]</strong>, <strong>[!UICONTROL ID da Unidade]</strong> e <strong>[!UICONTROL ID da Pasta]</strong> nos campos exibidos.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione o site que contém o item que você deseja atualizar, selecione a unidade e selecione a pasta. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Token]</td> 
   <td> O token identifica a partir de que ponto o módulo deve começar a recuperar as alterações.  </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Fazer uma chamada de API]

Este módulo permite executar uma chamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL SharePoint] ao [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Insira um caminho relativo para <code>https://graph.microsoft.com</code>. Exemplo:<code> /beta/sites</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   <td> <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação na forma de um objeto JSON padrão. Por exemplo, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] adiciona os cabeçalhos de autorização para você.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadeia de Consulta]</td> 
   <td> <p> Adicione a consulta da chamada à API na forma de um objeto JSON padrão.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo]</td> 
   <td>Selecione o tipo de dados que deseja enviar na chamada de API.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada à API na forma de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar instruções condicionais como <code>if</code> em seu JSON, coloque as aspas fora da instrução condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Assistir a eventos

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

