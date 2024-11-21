---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de placas Adobe Workfront
description: Você pode usar o conector de placas Adobe Workfront para automatizar seus processos dentro das placas Workfront e conectá-los a aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: 0b4a25f7-a8f1-47f4-8929-7eff82f1dfdc
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '2647'
ht-degree: 1%

---

# [!DNL Adobe Workfront] módulos de Quadros

>[!NOTE]
>
>O conector de fusão de placas está em status beta. Como resultado, o suporte para este conector é limitado e pode mudar devido ao desenvolvimento futuro das placas. Além disso, pode haver alterações na API do GraphQL sem aviso prévio que podem afetar o processo do conector Fusion.

As placas Adobe Workfront são ferramentas flexíveis que permitem a colaboração em equipe, fornecendo acesso a uma placa compartilhada que contém colunas e cartões.

Você pode usar os módulos Quadros Adobe Workfront para ler ou atualizar registros, fazer uma chamada de API para a API Quadros Workfront ou acionar um cenário quando uma ação ocorre em um quadro.

Para obter informações gerais sobre Workfront Boards, consulte [Visão geral dos painéis](/help/quicksilver/agile/boards-overview.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td>
  <td> <p>Qualquer</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td>
   <td> <p>Novo: Padrão</p><p>Ou</p><p>Atual: [!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licença</td> 
   <td>
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para Automação do Trabalho]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o plano [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], sua organização deve comprar [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).


## Pré-requisitos

Você deve ter configurado um quadro no Adobe Workfront antes de se conectar a ele.

## Informações da API de placas Adobe Workfront

O conector das placas Adobe Workfront usa o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Tag da API</td> 
   <td>v1.23.6</td> 
  </tr>
 </tbody> 
 </table>

## Criar uma conexão com Workfront Boards

>[!NOTE]
>
>Você pode usar uma conexão do Workfront para se conectar a placas Workfront ou criar uma conexão separada de placas Workfront.

Para criar uma conexão com Workfront Boards:

1. Em qualquer módulo [!DNL Adobe Workfront Boards], clique em **[!UICONTROL Adicionar]** ao lado da caixa Conexão.

1. Preencha os seguintes campos:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Nome da Conexão]</td>
          <td>
            <p>Insira um nome para esta conexão.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Ambiente]</td>
          <td>Selecione se você está se conectando a um ambiente de produção ou não produção.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Tipo]</td>
          <td>Selecione se você deseja se conectar a uma conta de serviço ou a uma conta pessoal.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID do Cliente]<p>(Opcional)</p></td>
          <td>Insira sua [!DNL Adobe] [!UICONTROL ID do Cliente]. Isso pode ser encontrado na seção [!UICONTROL Credentials details] do [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Segredo do Cliente]<p>(Opcional)</p></td>
          <td>Insira seu [!DNL Adobe] [!UICONTROL Segredo do Cliente]. Isso pode ser encontrado na seção [!UICONTROL Credentials details] do [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL URL de Autenticação]<p>(Opcional)</p></td>
          <td>Insira o URL que sua instância do Workfront usará para autenticar essa conexão. <p>O valor padrão é <code>https://oauth.my.workfront.com/integrations/oauth2</code>.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Prefixo de host]</td>
          <td>Insira seu prefixo de host.<p>O valor padrão é <code>origin-</code>.</p>
        </tr>
      </tbody>
    </table>
1. Clique em **[!UICONTROL Continuar]** para salvar a conexão e retornar ao módulo.

## Módulos de placas Adobe Workfront e seus campos

Ao configurar módulos de Quadros Workfront, o [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos adicionais dos Workfront Boards podem ser exibidos, dependendo de fatores como nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Cartões](#cards)
* [Quadros](#boards)
* [Colunas](#columns)
* [Tags](#tags)
* [Comentários](#comments)
* [Outro](#other)

<!--

### Watch

#### Watch events

This trigger module starts a scenario when an event occurs on a board.

1. Click **[!UICONTROL Add]** to the right of the **Webhook** box.

1. Configure the webhook in the **[!UICONTROL Add a hook]** box that displays.

   When you are configuring this module, the following fields display.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Webhook name]</td> 
      <td>(Optional) Type a new name for the webhook</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Connection]</td> 
      <td> <p>You can use an existing Workfront connection to connect to Workfront Boards, or you can use a specific Workfront Boards connection. </p><p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Create a connection to Workfront Boards</a> in this article.</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Object type]</td> 
      <td>Select the type of [!DNL Workfront] object that you want the module to watch.</td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Objects to watch]</p> </td> 
      <td> Select whether you want to trigger a scenario when there is a new object, an updated object, a new or updated object, or a deleted object. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>Exclude events made by this connection</td> 
      <td>Enable this option to exclude events created or updated using the same connector that this trigger module uses. This can prevent situations where a scenario might trigger itself, causing it to repeat in an endless loop.</td> 
     </tr> 
    </tbody> 
   </table>

After the webhook is created, you can view the address of the endpoint that events are sent to.

-->

### Cartões

* [Adicionar item da lista de verificação](#add-checklist-item)
* [Adicionar subtarefa](#add-subtask)
* [Criar um cartão](#create-a-card)
* [Mover uma carta](#move-a-card)
* [Ler um cartão](#read-a-card)
* [Atualizar um cartão](#update-a-card)

#### Adicionar item da lista de verificação

Esse módulo de ação adiciona um item de lista de verificação ao cartão especificado.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
      <td> <p>Você pode usar uma conexão Workfront existente para se conectar a Workfront Boards, ou usar uma conexão Workfront Boards específica. </p><p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Criar uma conexão com Workfront Boards</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do Cartão]</td> 
   <td>Insira ou mapeie a ID do cartão ao qual deseja adicionar um item da lista de verificação.<p>Você pode encontrar a ID do cartão no URL ao visualizá-lo no Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Itens da lista de verificação]</td> 
   <td>Para cada item da lista de verificação que você deseja adicionar, clique em Adicionar item, digite o nome do item da lista de verificação e selecione se o item foi concluído.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Adicionar subtarefa

Este módulo de ação adiciona uma subtarefa a um cartão em Quadros. A placa deve ser conectada. A subtarefa também é adicionada à tarefa do Workfront que o cartão representa.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
      <td> <p>Você pode usar uma conexão Workfront existente para se conectar a Workfront Boards, ou usar uma conexão Workfront Boards específica. </p><p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Criar uma conexão com Workfront Boards</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de cartão pai]</td> 
   <td>Insira ou mapeie a ID do cartão ao qual deseja adicionar uma subtarefa.<p>Você pode encontrar a ID do cartão no URL ao visualizá-lo no Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do Quadro]</td> 
   <td>Insira ou mapeie a ID do quadro que contém o cartão ao qual você deseja adicionar uma subtarefa.<p>Você pode encontrar a ID da placa no URL ao visualizar a placa no Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome]</td> 
   <td>Insira ou mapeie um nome para a nova subtarefa.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Criar um cartão

Este módulo de ação cria um novo cartão em um quadro Workfront.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
      <td> <p>Você pode usar uma conexão Workfront existente para se conectar a Workfront Boards, ou usar uma conexão Workfront Boards específica. </p><p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Criar uma conexão com Workfront Boards</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do Quadro]</td> 
   <td>Insira ou mapeie a ID do quadro ao qual você deseja adicionar um cartão.<p>Você pode encontrar a ID da placa no URL ao visualizar a placa no Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Identificação de Coluna]</td> 
   <td>Insira ou mapeie a ID da coluna à qual deseja adicionar uma subtarefa.<p>Você pode encontrar a ID da coluna nas informações retornadas do módulo Leia uma placa.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome]</td> 
   <td>Insira ou mapeie um nome para o novo cartão.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Mover uma carta

Esse módulo de ação move um cartão para uma coluna diferente no mesmo quadro.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
      <td> <p>Você pode usar uma conexão Workfront existente para se conectar a Workfront Boards, ou usar uma conexão Workfront Boards específica. </p><p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Criar uma conexão com Workfront Boards</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do Cartão]</td> 
   <td>Insira ou mapeie a ID do cartão que você deseja mover.<p>Você pode encontrar a ID do cartão no URL ao visualizá-lo no Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do Quadro]</td> 
   <td>Insira ou mapeie a ID do quadro que contém o cartão que você deseja mover.<p>Você pode encontrar a ID do cartão no URL ao visualizá-lo no Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID da coluna de destino]</td> 
   <td>Insira ou mapeie a ID da coluna para a qual deseja mover o cartão.<p>Você pode encontrar a ID da coluna nas informações retornadas do módulo Leia uma placa.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Para índice]</td> 
   <td>Insira ou mapeie a posição que deseja que o cartão tenha na nova coluna.<p>A posição superior na coluna no índice 0.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Ler um cartão

Este módulo de ação recupera informações sobre um cartão específico.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
      <td> <p>Você pode usar uma conexão Workfront existente para se conectar a Workfront Boards, ou usar uma conexão Workfront Boards específica. </p><p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Criar uma conexão com Workfront Boards</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do Cartão]</td> 
   <td>Insira ou mapeie a ID do cartão que deseja ler.<p>Você pode encontrar a ID do cartão no URL ao visualizá-lo no Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Atualizar um cartão

Esse módulo de ação atualiza as informações de um cartão especificado.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
      <td> <p>Você pode usar uma conexão Workfront existente para se conectar a Workfront Boards, ou usar uma conexão Workfront Boards específica. </p><p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Criar uma conexão com Workfront Boards</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do Cartão]</td> 
   <td>Insira ou mapeie a ID do cartão que deseja atualizar.<p>Você pode encontrar a ID do cartão no URL ao visualizá-lo no Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do Quadro]</td> 
   <td>Insira ou mapeie a ID do quadro que contém o cartão que você deseja atualizar.<p>Você pode encontrar a ID do cartão no URL ao visualizá-lo no Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome]</td> 
   <td>Insira ou mapeie um novo nome para o cartão.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do Cartão]</td> 
   <td>Insira ou mapeie uma nova descrição para o cartão.</p></td> 
  </tr> 
 </tbody> 
</table>

### Quadros

* [Criar um quadro](#create-a-board)
* [Ler um quadro](#read-a-board)

#### Criar um quadro

Este módulo de ação cria um quadro no Workfront. Você pode especificar o tipo de quadro que deseja criar.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
      <td> <p>Você pode usar uma conexão Workfront existente para se conectar a Workfront Boards, ou usar uma conexão Workfront Boards específica. </p><p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Criar uma conexão com Workfront Boards</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board name]</td> 
   <td>Informe ou mapeie um nome para o novo quadro.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo]</td> 
   <td>Selecione o tipo de quadro que deseja criar.</td> 
  </tr> 
 </tbody> 
</table>

#### Ler um quadro

Esse módulo de ação retorna informações sobre um único quadro, como cartões, colunas, tags e membros do quadro.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
      <td> <p>Você pode usar uma conexão Workfront existente para se conectar a Workfront Boards, ou usar uma conexão Workfront Boards específica. </p><p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Criar uma conexão com Workfront Boards</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do Quadro]</td> 
   <td>Informe ou mapeie o ID do quadro para o qual deseja recuperar informações.<p>Você pode encontrar a ID da placa no URL ao visualizar a placa no Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

### Colunas

* [Criar uma coluna](#create-a-column)
* [Pesquisar uma coluna](#search-for-a-column)
* [Atualizar uma coluna](#update-a-column)

#### Criar uma coluna

Esse módulo de ação cria uma nova coluna no quadro especificado.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
      <td> <p>Você pode usar uma conexão Workfront existente para se conectar a Workfront Boards, ou usar uma conexão Workfront Boards específica. </p><p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Criar uma conexão com Workfront Boards</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do Quadro]</td> 
   <td>Informe ou mapeie a ID do quadro ao qual deseja adicionar uma coluna.<p>Você pode encontrar a ID da placa no URL ao visualizar a placa no Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Identificação de Coluna]</td> 
   <td>Insira ou mapeie a ID da coluna que você deseja atualizar.<p>Você pode encontrar a ID da coluna nas informações retornadas do módulo Leia uma placa.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome da coluna]</td> 
   <td>Insira ou mapeie um novo nome para a coluna.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limite de WIP]</td> 
   <td>Informe ou mapeie um novo limite WIP para a coluna.</td> 
  </tr> 
 </tbody> 
</table>

#### Pesquisar uma coluna

Este módulo de pesquisa retorna informações sobre a coluna com o nome especificado.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
      <td> <p>Você pode usar uma conexão Workfront existente para se conectar a Workfront Boards, ou usar uma conexão Workfront Boards específica. </p><p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Criar uma conexão com Workfront Boards</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do Quadro]</td> 
   <td>Informe ou mapeie a ID do quadro que contém a coluna que você deseja recuperar.<p>Você pode encontrar a ID da placa no URL ao visualizar a placa no Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome da Coluna]</td> 
   <td>Insira ou mapeie o nome da coluna que deseja recuperar.</td> 
  </tr> 
 </tbody> 
</table>

#### Atualizar uma coluna

Esse módulo de ação atualiza o nome ou o limite WIP da coluna especificada.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
      <td> <p>Você pode usar uma conexão Workfront existente para se conectar a Workfront Boards, ou usar uma conexão Workfront Boards específica. </p><p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Criar uma conexão com Workfront Boards</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do Quadro]</td> 
   <td>Informe ou mapeie a ID do quadro que contém a coluna que você deseja recuperar.<p>Você pode encontrar a ID da placa no URL ao visualizar a placa no Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome da Coluna]</td> 
   <td>Insira ou mapeie o nome da coluna que deseja recuperar.</td> 
  </tr> 
 </tbody> 
</table>

### Tags

* [Adicionar uma tag a um cartão](#add-card-tag)
* [Criar uma tag](#create-a-tag)

#### Adicionar uma tag a um cartão

Esse módulo de ação adiciona uma tag a um cartão.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
      <td> <p>Você pode usar uma conexão Workfront existente para se conectar a Workfront Boards, ou usar uma conexão Workfront Boards específica. </p><p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Criar uma conexão com Workfront Boards</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do Cartão]</td> 
   <td>Insira ou mapeie a ID do cartão ao qual deseja adicionar uma tag.<p>Você pode encontrar a ID do cartão no URL ao visualizá-lo no Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do Quadro]</td> 
   <td>Insira ou mapeie a ID do quadro que contém o cartão ao qual deseja adicionar uma tag.<p>Você pode encontrar a ID da placa no URL ao visualizar a placa no Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Marca]</td> 
   <td>Insira ou mapeie a ID da tag que deseja adicionar.<p>Você pode encontrar a ID da tag nas informações retornadas do módulo Leia uma placa.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Criar uma tag

Esse módulo de ação cria uma nova tag e a atribui a uma cor.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
      <td> <p>Você pode usar uma conexão Workfront existente para se conectar a Workfront Boards, ou usar uma conexão Workfront Boards específica. </p><p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Criar uma conexão com Workfront Boards</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do Quadro]</td> 
   <td>Insira ou mapeie a ID do quadro para o qual você deseja criar uma tag.<p>Você pode encontrar a ID da placa no URL ao visualizar a placa no Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Marca nome]</td> 
   <td>Insira ou mapeie um nome para a nova tag.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cor da Marca]</td> 
   <td>Selecione a cor para esta tag.</td> 
  </tr> 
 </tbody> 
</table>

### Comentários

* [Criar um comentário](#create-a-comment)
* [Ler comentários do cartão](#read-card-comments)

#### Criar um comentário

Esse módulo de ação criou um comentário no cartão especificado.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
      <td> <p>Você pode usar uma conexão Workfront existente para se conectar a Workfront Boards, ou usar uma conexão Workfront Boards específica. </p><p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Criar uma conexão com Workfront Boards</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do Cartão]</td> 
   <td>Insira ou mapeie a ID do cartão ao qual deseja adicionar um comentário.<p>Você pode encontrar a ID do cartão no URL ao visualizá-lo no Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comentário]</td> 
   <td>Insira ou mapeie o texto do comentário que deseja adicionar.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Ler comentários do cartão

Esse módulo de ação recupera os comentários do cartão especificado.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
      <td> <p>Você pode usar uma conexão Workfront existente para se conectar a Workfront Boards, ou usar uma conexão Workfront Boards específica. </p><p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Criar uma conexão com Workfront Boards</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do Cartão]</td> 
   <td>Insira ou mapeie a ID do cartão para o qual deseja recuperar os comentários.<p>Você pode encontrar a ID do cartão no URL ao visualizá-lo no Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limite]</td> 
   <td>Insira o número máximo de comentários que você deseja que o módulo retorne em um ciclo de execução.</p></td> 
  </tr> 
 </tbody> 
</table>

### Outro

#### Fazer uma chamada de API personalizada

Esse módulo de ação faz uma chamada personalizada para a API de placas do Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
      <td> <p>Você pode usar uma conexão Workfront existente para se conectar a Workfront Boards, ou usar uma conexão Workfront Boards específica. </p><p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Criar uma conexão com Workfront Boards</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Insira um caminho relativo a <code> https://&lt;WORKFRONT_DOMAIN&gt;/boards-service/graphql?</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p><p>Para a maioria das chamadas de placas, o método é POST. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formulário de um objeto JSON padrão. Isso determina o tipo de conteúdo da solicitação.</p> <p>Por exemplo,<code> { "Content-type":"application/json-stringify()"}</code></p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadeia de Consulta]</td> 
   <td> <p>Adicione a consulta da chamada à API na forma de um objeto JSON padrão.</p> <p>Para Workfront Boards, essa seção geralmente fica vazia.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada de API na forma de um Graphql incorporado JSON </p> <p>Exemplo:</p><p>Este exemplo atualiza um nome de coluna. Você pode incluir o <code>boardId</code> e <code>columnId</code> como GUIDs codificados ou mapeados de um módulo anterior.<p><pre>{

  &quot;query&quot;: &quot;mutation { updateColumn(boardId: \&quot;\&quot;, columnId: \&quot;\&quot;, updateColumnInput: { name: \&quot;\&quot; }) { id name }}&quot;

}</pre><p>Nota:  <p>Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.</p>
<div class="example" data-mc-autonum="<b>Example: </b>">
<p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p>
</div> </p> </td>
</tr> 
 </tbody> 
</table>
