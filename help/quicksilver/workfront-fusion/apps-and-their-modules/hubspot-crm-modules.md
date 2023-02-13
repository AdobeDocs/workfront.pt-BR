---
title: Módulos CRM do HubSpot
description: O [!DNL Adobe Workfront Fusion] Os módulos CRM do HubSpot permitem monitorar eventos, registros, contatos, envolvimentos, envios de arquivos e formulários, ou criar, recuperar, atualizar e excluir registros, contatos, envolvimentos, eventos ou arquivos em seu [!DNL HubSpot CRM] conta.
author: Becky
feature: Workfront Fusion
exl-id: d58e0c12-a798-495c-8f88-fbf2a532f8a4
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2485'
ht-degree: 0%

---

# [!DNL HubSpot CRM] módulos

O [!DNL Adobe Workfront Fusion] [!DNL HubSpot CRM] os módulos permitem monitorar eventos, registros, contatos, envolvimentos, envios de arquivo e formulário, ou criar, recuperar, atualizar e excluir registros, contatos, envolvimentos, eventos ou arquivos em seu [!DNL HubSpot CRM] conta.

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

Para usar [!DNL HubSpot CRM] módulos, você deve ter um [!DNL HubSpot CRM] conta.

## Connect [!DNL Adobe Workfront Fusion] para [!DNL HubSpot CRM]

Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] para [!DNL Workfront Fusion], consulte [Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL HubSpot CRM] módulos e seus campos

Ao configurar [!DNL Hubspot CRM] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Hubspot CRM] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Objetos CRM](#crm-objects)
* [Registros (Contratos, Contatos e Empresas)](#records-deals-contacts-and-companies)
* [Contatos](#contacts)
* [Contratos](#deals)
* [Empresas](#companies)
* [Arquivos](#files)
* [Ingressos](#tickets)
* [Faça uma chamada de API](#make-an-api-call)

### Objetos CRM

#### [!UICONTROL Pesquisar objetos do CRM]

Esse módulo de pesquisa pesquisa pesquisa objetos CRM por propriedades personalizadas ou por query. Para procurar produtos ou itens de linha, use uma conexão especial com um escopo personalizado necessário.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Insira ou mapeie o número máximo de itens que o módulo retornará em um ciclo de execução.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de objeto para pesquisa]</td> 
   <td>Selecione o tipo de objeto de CRM do Hubspot que deseja pesquisar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Propriedades de saída]</td> 
   <td>Selecione as propriedades que deseja que apareçam na saída do módulo. Os campos disponíveis dependem do objeto selecionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtrar por] </td> 
   <td> <p>Selecione como deseja filtrar a pesquisa</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Consulta]</strong> </p> <p>Inserir ou mapear a consulta</p> </li> 
     <li> <p><strong>[!UICONTROL Propriedades]</strong> </p> <p>Insira os grupos ou filtros para sua pesquisa.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Classificar por]</td> 
   <td> <p>Clique em para classificar os resultados. Se você optar por classificar os resultados, os seguintes campos serão exibidos. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome da propriedade]</strong> </p> <p>Selecione a propriedade pela qual deseja classificar os resultados</p> </li> 
     <li> <p><strong>[!UICONTROL Direção]</strong> </p> <p>Escolha se deseja classificar os resultados em uma direção crescente ou decrescente.</p> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Start Offset</td> 
    <td>Enter or map the ID of the first item you want to retrieve details for. This module only returns up to 5000 results at a time. Setting a start offset allows you to retrieve items other than the first 5000. If the start offset is 5000, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

### Registros (Contratos, Contatos e Empresas)

* [[!UICONTROL Criar um registro (herdado)]](#create-a-record-legacy)
* [[!UICONTROL Obter um registro]](#get-a-record)
* [[!UICONTROL Atualizar um registro]](#update-a-record)
* [[!UICONTROL Excluir um registro]](#delete-a-record)
* [[!UICONTROL Obter uma propriedade de registro]](#get-a-record-property)
* [[!UICONTROL Ver registros]](#watch-records)

#### [!UICONTROL Criar um registro (herdado)]

Esse módulo de ação cria um contato, uma empresa ou um negócio.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione o tipo de registro que deseja criar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Propriedades]</td> 
   <td>Preencha as propriedades que deseja definir para o registro. Os campos disponíveis dependem do tipo de registro que você deseja criar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um registro]

Este módulo de ação obtém detalhes de um contato, uma empresa ou um negócio.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione o tipo de registro.</p> 
    <ul> 
     <li>[!UICONTROL Contato]</li> 
     <li>[!UICONTROL Company] </li> 
     <li>[!UICONTROL Deal]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de pesquisa]</td> 
   <td>Se estiver recebendo um contato, selecione se deseja identificá-lo por ID ou endereço de email.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Insira a ID do contato, da empresa ou do negócio que você deseja recuperar. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>Insira o endereço de email do contato cujos detalhes você deseja recuperar. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar um registro]

Este módulo de ação atualiza um contato, uma empresa ou um negócio.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Selecione o tipo de registro que deseja atualizar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de pesquisa]</td> 
   <td> <p>Se estiver recebendo um contato, selecione como deseja identificar o registro:</p> 
    <ul> 
     <li> <p>[!UICONTROL ID]</p> </li> 
     <li> <p>[!UICONTROL Email]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Insira a ID do contato, empresa ou negócio que deseja atualizar. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>Insira o endereço de email do contato cujos detalhes você deseja atualizar. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Propriedades]</td> 
   <td>Preencha as propriedades que deseja definir para o registro. Os campos disponíveis dependem do tipo de registro que você deseja criar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir um registro]

Esse módulo de ação exclui um contato, uma empresa ou um negócio.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Selecione o tipo de registro que deseja excluir.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Insira a ID do contato, empresa ou negócio que deseja excluir. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter uma propriedade de registro]

Esse módulo de ação obtém metadados para uma propriedade de registro específica pelo nome (interno).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Selecione o tipo de registro que tem a propriedade para a qual deseja recuperar metadados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome da propriedade]</td> 
   <td>Selecione a propriedade para a qual deseja recuperar metadados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Option ID]</td> 
   <td> <p> Algumas propriedades têm um conjunto de opções disponíveis que um usuário pode selecionar como o valor da propriedade. Insira a ID da opção que representa o valor da propriedade que você deseja recuperar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ver registros]

Este módulo de acionador inicia um cenário quando um contato, empresa ou negócio foi modificado ou criado nos últimos 30 dias. A saída é limitada a 10.000 registros.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Selecione o tipo de registro que tem a propriedade que você deseja assistir.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search]</td> 
   <td>Selecione se deseja assistir a registros modificados recentemente ou criados recentemente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Propriedades de saída]</td> 
   <td>Selecione as propriedades que deseja incluir na saída do módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Contatos

* [[!UICONTROL Criar/atualizar um contato (herdado)]](#createupdate-a-contact-legacy)
* [[!UICONTROL Criar/atualizar um grupo de contatos]](#createupdate-a-group-of-contacts)
* [[!UICONTROL Adicionar Contatos a uma Lista]](#add-contacts-to-a-list)
* [[!UICONTROL Remover um Contato de uma Lista]](#remove-a-contact-from-a-list)
* [[!UICONTROL Mesclar contatos]](#merge-contacts)
* [[!UICONTROL Procurar Contatos]](#search-for-contacts)
* [[!UICONTROL Listar Contatos]](#list-contacts)
* [[!UICONTROL Listar Contatos de uma Empresa]](#list-contacts-of-a-company)

#### [!UICONTROL Criar/atualizar um contato (herdado)]

Cria um contato se ele já não existir em um portal ou o atualiza com os valores de propriedade mais recentes, se ele existir em um portal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Propriedades]</td> 
   <td>Preencha as propriedades que deseja definir ou atualizar para o contato. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar/atualizar um grupo de contatos]

Cria um grupo de contatos ou os atualiza caso já existam. O desempenho é melhor quando o tamanho do lote é limitado a 100 contatos ou menos. As alterações feitas por meio desse terminal são processadas de forma assíncrona, portanto, pode levar vários minutos para que as alterações sejam aplicadas aos registros de contato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lote de contatos para criar/atualizar] </td> 
   <td> <p>Adicione o lote de contatos.</p> <p>Clique em <strong>[!UICONTROL Adicionar item]</strong> para adicionar um novo contato. Na janela exibida, insira ou mapeie as seguintes informações:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Tipo de pesquisa]</strong> </p> <p>Selecione como deseja identificar o contato:</p> 
      <ul> 
       <li> <p>[!UICONTROL ID]</p> <p>Insira a ID do contato que deseja criar ou atualizar. </p> </li> 
       <li> <p>[!UICONTROL Email]</p> <p>Insira o endereço de email do contato que deseja criar ou atualizar. </p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Propriedades]</strong> </p> <p>Preencha as propriedades que deseja definir ou atualizar para o contato.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Adicionar Contatos a uma Lista]

Esse módulo adiciona registros de contato que já foram criados no sistema a uma lista de contatos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID] </td> 
   <td>Selecione a ID da lista à qual deseja adicionar o contato. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL IDs/Emails] </td> 
   <td> <p>Selecione como deseja identificar os contatos que deseja adicionar à lista:</p> 
    <ul> 
     <li> <p>[!UICONTROL IDs]</p> <p>Adicione as IDs dos contatos que deseja adicionar à lista.</p> </li> 
     <li> <p>[!UICONTROL Emails]</p> <p>Adicione os endereços de email dos contatos que deseja adicionar à lista.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remover um Contato de uma Lista]

Remove um contato de uma lista de contatos.

>[!NOTE]
>
>Não é possível remover manualmente contatos de uma lista dinâmica.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID] </td> 
   <td>Selecione a ID da lista da qual deseja remover o contato. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do contato] </td> 
   <td>Insira a ID do contato que deseja remover da lista. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mesclar contatos]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 1] </td> 
   <td>Insira a ID de um dos contatos que deseja mesclar. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 2] </td> 
   <td>Insira a ID do outro contato que deseja mesclar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Procurar Contatos]

Recupera uma lista de contatos usando a consulta de pesquisa.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Consulta]</td> 
   <td>Insira a consulta de pesquisa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite] </td> 
   <td>Inserir ou mapear o número máximo de contatos [!DNL Workfront Fusion] deve retornar durante um ciclo de execução de cenário. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listar Contatos]

Retorna todos os contatos que foram criados no portal. A saída é limitada a 5000 contatos. Para listar contatos anteriores ou próximos, você pode usar o [!UICONTROL avançado] para deslocar a lista.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>O número máximo de contatos [!DNL Workfront Fusion] deve retornar durante um ciclo de execução de cenário. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Propriedades de saída]</td> 
   <td>Selecione as propriedades que deseja que apareçam na saída do módulo. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL Listar Contatos de uma Empresa]

Recupera uma lista de contatos na empresa. A saída é limitada a 5000 contatos. Para listar contatos anteriores ou próximos, você pode usar o [!UICONTROL avançado] para deslocar a lista.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Insira a ID da empresa cujos contatos você deseja listar. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>O número máximo de contatos [!DNL Workfront Fusion] deve retornar durante um ciclo de execução de cenário. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL Observar contatos adicionados a uma lista]

Este módulo de acionador inicia um cenário quando um novo contato é adicionado a uma lista. Isso está disponível somente para usuários com uma conta de Marketing paga.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td>Insira ou mapeie a ID da lista que contém os contatos que deseja visualizar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Propriedades de saída]</td> 
   <td>Selecione as propriedades que deseja incluir na saída do módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Contratos

* [[!UICONTROL Listar Pipelines de Negociação/Tíquete]](#list-dealticket-pipelines)
* [[!UICONTROL Obter o pipeline de CRM de um contrato]](#get-a-deals-crm-pipeline)

#### [!UICONTROL Listar Pipelines de Negociação/Tíquete]

Retorna todos os pipelines de venda e tíquete de um determinado portal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de objeto] </td> 
   <td>Selecione se deseja listar ofertas ou ingressos.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter o pipeline de CRM de um contrato]

Retorna um pipeline de negócios específico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do pipeline] </td> 
   <td>Insira ou mapeie a ID do pipeline para o qual deseja recuperar detalhes. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stage ID] </td> 
   <td>Insira ou mapeie a ID do estágio para o qual deseja recuperar detalhes. </td> 
  </tr> 
 </tbody> 
</table>

### Empresas

#### [!UICONTROL Pesquisar Empresas por domínio]

Recupera uma lista de empresas com base em uma correspondência exata da propriedade de domínio.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Domínio] </td> 
   <td>Insira o domínio das empresas que deseja pesquisar, como <code>[!DNL hubspot].com</code>. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>O número máximo de empresas [!DNL Workfront Fusion] deve retornar durante um ciclo de execução de cenário. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Propriedades de saída]</td> 
   <td>Selecione as propriedades que deseja que apareçam na saída do módulo. </td> 
  </tr> 
 </tbody> 
</table>

### Arquivos

* [[!UICONTROL Criar uma pasta]](#create-a-folder)
* [[!UICONTROL Excluir uma pasta]](#delete-a-folder)
* [[!UICONTROL Mover um arquivo]](#move-a-file)

#### [!UICONTROL Criar uma pasta]

Esse módulo cria uma pasta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome da pasta] </td> 
   <td>Insira ou mapeie um nome para a nova pasta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da pasta pai] </td> 
   <td>Selecione a ID da pasta pai da pasta que você está criando. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir uma pasta]

Marca uma pasta como excluída.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Insira o ID da pasta que deseja excluir.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover um arquivo]

Move um arquivo para uma pasta diferente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do arquivo] </td> 
   <td>Insira ou mapeie a ID do arquivo que deseja mover. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da pasta] </td> 
   <td>Selecione a ID da pasta onde deseja mover o arquivo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Insira um nome para o arquivo movido.</td> 
  </tr> 
 </tbody> 
</table>

### Ingressos

#### [!UICONTROL Excluir um tíquete]

Exclui um tíquete existente por sua ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Insira a ID do tíquete que deseja excluir. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Faça uma chamada de API]

Permite executar uma chamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Insira um caminho relativo a https://api.hubapi.com/. Por exemplo, /contacts/v1/lists/all/contacts/all</p> <p>Para obter a lista de endpoints disponíveis, consulte <a href="https://legacydocs.hubspot.com/docs/overview">[!DNL HubSpot] Documentação da API</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   <td> <p>Selecione o método HTTP que deseja usar:</p> <p>[!UICONTROL GET]</p> <p>para recuperar informações de uma entrada.</p> <p>[!UICONTROL POST]</p> <p>para criar uma nova entrada.</p> <p>[!UICONTROL PUT]</p> <p>para atualizar/substituir uma entrada existente.</p> <p>[!UICONTROL PATCH]</p> <p>para fazer uma atualização de entrada parcial.</p> <p>[!UICONTROL DELETE]</p> <p>para excluir uma entrada.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p> Insira os cabeçalhos da solicitação desejada. Você não precisa adicionar cabeçalhos de autorização; já fizemos isso por você.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sequência de consulta]</td> 
   <td> <p> Insira a sequência de consulta da solicitação.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada da API no formato de um objeto JSON padrão.Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemplo:** A chamada de API a seguir retorna todos os contatos em seu [!DNL HubSpot] conta:
>
>**URL**: `/contacts/v1/lists/all/contacts/all`
>
>**Método**: `GET`
>
>![](assets/hubspot-api-config.png)
>
>As correspondências da pesquisa podem ser encontradas na Saída do módulo em [!UICONTROL Pacote] > [!UICONTROL Corpo] > [!UICONTROL contatos].
>
>Em nosso exemplo, 3 contatos foram retornados:
>
>![](assets/hubspot-api-output.png)

## Criar um novo aplicativo

1. Faça logon no [!DNL HubSpot] conta do desenvolvedor.
1. Selecione o **[!UICONTROL Criar um aplicativo]** opção.
1. Insira o nome do aplicativo e [!UICONTROL Salvar] na caixa de diálogo.
1. Selecione os escopos necessários para o seu webhook.

   Por exemplo, adicione escopos de contatos para acionar o módulo quando um novo contato for criado ou excluído.

   O [!UICONTROL escopo de contatos] é tudo que você precisa para receber contatos, ofertas e webhooks de eventos da empresa.

   >[!IMPORTANT]
   >
   >Não preencha o [!UICONTROL Redirecionar URL] campo.
