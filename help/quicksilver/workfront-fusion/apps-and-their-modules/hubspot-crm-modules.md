---
title: Módulos CRM do HubSpot
description: A variável [!DNL Adobe Workfront Fusion] Os módulos CRM do HubSpot permitem monitorar eventos, registros, contatos, compromissos, envios de arquivos e formulários ou criar, recuperar, atualizar e excluir registros, contatos, compromissos, eventos ou arquivos em seu [!DNL HubSpot CRM] conta.
author: Becky
feature: Workfront Fusion
exl-id: d58e0c12-a798-495c-8f88-fbf2a532f8a4
source-git-commit: 1c56cf8aa9da7ec2644955d5533c71f60160d580
workflow-type: tm+mt
source-wordcount: '2615'
ht-degree: 0%

---

# [!DNL HubSpot CRM] módulos

A variável [!DNL Adobe Workfront Fusion] [!DNL HubSpot CRM] Os módulos do permitem monitorar eventos, registros, contatos, compromissos, envios de arquivos e formulários ou criar, recuperar, atualizar e excluir registros, contatos, compromissos, eventos ou arquivos no [!DNL HubSpot CRM] conta.

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

Para usar [!DNL HubSpot CRM] módulos, você deve ter uma [!DNL HubSpot CRM] conta.

## Conectar [!DNL Adobe Workfront Fusion] para [!DNL HubSpot CRM]

Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] conta para [!DNL Workfront Fusion], consulte [Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Ao configurar uma conexão, selecione o **CRM do HubSpot** tipo de conexão. O tipo HubSpot CRM (obsoleto) é compatível com conexões existentes, mas não recomendamos usá-lo para criar novas conexões.

## [!DNL HubSpot CRM] módulos e seus campos

Ao configurar [!DNL Hubspot CRM] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Hubspot CRM] Os campos podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Objetos do CRM](#crm-objects)
* [Registros (Transações, Contatos e Empresas)](#records-deals-contacts-and-companies)
* [Contatos](#contacts)
* [Transações](#deals)
* [Empresas](#companies)
* [Arquivos](#files)
* [Tíquetes](#tickets)
* [Fazer uma chamada de API](#make-an-api-call)

### Objetos do CRM

#### [!UICONTROL Procurar Objetos do CRM]

Este módulo de pesquisa procura objetos do CRM por propriedades personalizadas ou por consulta. Para pesquisar produtos ou itens de linha, use uma conexão especial com um escopo personalizado necessário.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Insira ou mapeie o número máximo de itens que o módulo retornará em um ciclo de execução.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Objeto para Pesquisa]</td> 
   <td>Selecione o tipo de objeto CRM do Hubspot que você deseja pesquisar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Propriedades de saída]</td> 
   <td>Selecione as propriedades que você deseja que apareçam na saída do módulo. Os campos disponíveis dependem do objeto selecionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtrar por] </td> 
   <td> <p>Selecione como deseja filtrar a pesquisa</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Consulta]</strong> </p> <p>Insira ou mapeie a consulta</p> </li> 
     <li> <p><strong>[!UICONTROL Propriedades]</strong> </p> <p>Insira os grupos ou filtros para sua pesquisa.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Classificar por]</td> 
   <td> <p>Clique em para classificar os resultados. Se você optar por classificar os resultados, serão exibidos os seguintes campos. </p> 
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

### Registros (Transações, Contatos e Empresas)

* [[!UICONTROL Criar um registro (herdado)]](#create-a-record-legacy)
* [[!UICONTROL Obter um Registro]](#get-a-record)
* [[!UICONTROL Atualizar um Registro]](#update-a-record)
* [[!UICONTROL Excluir um Registro]](#delete-a-record)
* [[!UICONTROL Obter uma propriedade de registro]](#get-a-record-property)
* [[!UICONTROL Observar registros]](#watch-records)

#### [!UICONTROL Criar um registro (herdado)]

Este módulo de ação cria um contato, uma empresa ou uma negociação.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Registro]</td> 
   <td> <p>Selecione o tipo de registro que deseja criar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Propriedades]</td> 
   <td>Preencha quaisquer propriedades que deseja definir para o registro. Os campos disponíveis dependem do tipo de registro que você deseja criar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um Registro]

Este módulo de ação obtém detalhes de um contato, de uma empresa ou de uma transação.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Registro]</td> 
   <td> <p>Selecione o tipo de registro.</p> 
    <ul> 
     <li>[!UICONTROL Contato]</li> 
     <li>[!UICONTROL Empresa] </li> 
     <li>[!UICONTROL oferta]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Pesquisa]</td> 
   <td>Se você estiver recebendo um contato, selecione se deseja identificá-lo por ID ou por endereço de email.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Insira a ID do contato, empresa ou negócio que você deseja recuperar. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>Insira o endereço de email do contato cujos detalhes você deseja recuperar. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar um Registro]

Este módulo de ação atualiza um contato, uma empresa ou um negócio.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Registro]</td> 
   <td>Selecione o tipo de registro que deseja atualizar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Pesquisa]</td> 
   <td> <p>Se você estiver recebendo um contato, selecione como deseja identificar o registro:</p> 
    <ul> 
     <li> <p>[!UICONTROL ID]</p> </li> 
     <li> <p>[!UICONTROL Email]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Insira a ID do contato, empresa ou negócio que você deseja atualizar. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>Insira o endereço de email do contato cujos detalhes você deseja atualizar. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Propriedades]</td> 
   <td>Preencha quaisquer propriedades que deseja definir para o registro. Os campos disponíveis dependem do tipo de registro que você deseja criar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir um Registro]

Este módulo de ação exclui um contato, uma empresa ou uma negociação.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Registro]</td> 
   <td>Selecione o tipo de registro que deseja deletar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Insira a ID do contato, empresa ou negócio que deseja excluir. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter uma propriedade de registro]

Esse módulo de ação obtém metadados para uma propriedade de registro específica por seu nome (interno).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Registro]</td> 
   <td>Selecione o tipo de registro que tem a propriedade para a qual você deseja recuperar metadados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome da Propriedade]</td> 
   <td>Selecione a propriedade para a qual deseja recuperar metadados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificação de Opção]</td> 
   <td> <p> Algumas propriedades têm um conjunto de opções disponíveis que um usuário pode selecionar como o valor da propriedade. Insira a ID da opção que representa o valor da propriedade que você deseja recuperar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Observar registros]

Este módulo de acionador inicia um cenário quando um contato, empresa ou negócio foi modificado ou criado nos últimos 30 dias. A saída é limitada a 10.000 registros.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Registro]</td> 
   <td>Selecione o tipo de registro que tem a propriedade que você deseja observar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pesquisar]</td> 
   <td>Selecione se deseja observar registros modificados recentemente ou criados recentemente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Propriedades de Saída]</td> 
   <td>Selecione as propriedades que deseja incluir na saída do módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Contatos

* [[!UICONTROL Criar/atualizar um contato (herdado)]](#createupdate-a-contact-legacy)
* [[!UICONTROL Criar/Atualizar um Grupo de Contatos]](#createupdate-a-group-of-contacts)
* [[!UICONTROL Adicionar Contatos a uma Lista]](#add-contacts-to-a-list)
* [[!UICONTROL Remover um Contato de uma Lista]](#remove-a-contact-from-a-list)
* [[!UICONTROL Mesclar contatos]](#merge-contacts)
* [[!UICONTROL Procurar Contatos]](#search-for-contacts)
* [[!UICONTROL Listar Contatos]](#list-contacts)
* [[!UICONTROL Listar Contatos de uma Empresa]](#list-contacts-of-a-company)

#### [!UICONTROL Criar/atualizar um contato (herdado)]

Cria um contato se ele ainda não existir em um portal ou o atualiza com os valores de propriedade mais recentes se ele existir em um portal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Propriedades]</td> 
   <td>Preencha todas as propriedades que deseja definir ou atualizar para o contato. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar/Atualizar um Grupo de Contatos]

Cria um grupo de contatos ou os atualiza quando já existem. O desempenho é melhor quando o tamanho do lote é limitado a 100 contatos ou menos. As alterações feitas por meio desse endpoint são processadas de forma assíncrona, portanto, pode levar vários minutos para que as alterações sejam aplicadas a registros de contato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lote de Contatos a ser criado/atualizado] </td> 
   <td> <p>Adicione o lote de contatos.</p> <p>Clique em <strong>[!UICONTROL Adicionar item]</strong> para adicionar um novo contato. Na janela exibida, insira ou mapeie as seguintes informações:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Tipo de Pesquisa]</strong> </p> <p>Selecione como deseja identificar o contato:</p> 
      <ul> 
       <li> <p>[!UICONTROL ID]</p> <p>Insira a ID do contato que você deseja criar ou atualizar. </p> </li> 
       <li> <p>[!UICONTROL Email]</p> <p>Insira o endereço de email do contato que deseja criar ou atualizar. </p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Propriedades]</strong> </p> <p>Preencha todas as propriedades que deseja definir ou atualizar para o contato.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Adicionar Contatos a uma Lista]

Este módulo adiciona registros de contato que já foram criados no sistema a uma lista de contatos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Lista] </td> 
   <td>Selecione a ID da lista à qual você deseja adicionar o contato. </td> 
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
>Não é possível remover contatos manualmente de uma lista dinâmica.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Lista] </td> 
   <td>Selecione a ID da lista da qual deseja remover o contato. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Contato] </td> 
   <td>Digite a ID do contato que você deseja remover da lista. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mesclar contatos]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 1] </td> 
   <td>Digite a ID de um dos contatos que você deseja mesclar. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 2] </td> 
   <td>Insira a ID do outro contato que você deseja mesclar.</td> 
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
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Consulta]</td> 
   <td>Insira a consulta de pesquisa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite] </td> 
   <td>Insira ou mapeie o número máximo de contatos [!DNL Workfront Fusion] deve retornar durante um ciclo de execução de cenário. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listar Contatos]

Retorna todos os contatos que foram criados no portal. A saída é limitada a 5000 contatos. Para listar contatos anteriores ou seguintes, você pode usar o [!UICONTROL avançado] para deslocar a lista.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>O número máximo de contatos [!DNL Workfront Fusion] deve retornar durante um ciclo de execução de cenário. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Propriedades de saída]</td> 
   <td>Selecione as propriedades que você deseja que apareçam na saída do módulo. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL Listar Contatos de uma Empresa]

Recupera uma lista de contatos na empresa. A saída é limitada a 5000 contatos. Para listar contatos anteriores ou seguintes, você pode usar o [!UICONTROL avançado] para deslocar a lista.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Informe a ID da empresa cujos contatos você deseja listar. </td> 
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

#### [!UICONTROL Assistir contatos adicionados a uma lista]

Este módulo de acionamento inicia um cenário quando um novo contato é adicionado a uma lista. Isso está disponível somente para usuários com uma conta de marketing paga.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Lista]</td> 
   <td>Insira ou mapeie a ID da lista que contém os contatos que você deseja assistir.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Propriedades de Saída]</td> 
   <td>Selecione as propriedades que deseja incluir na saída do módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Transações

* [[!UICONTROL Listar pipelines de oferta/tíquete]](#list-dealticket-pipelines)
* [[!UICONTROL Obter um pipeline de CRM do contrato]](#get-a-deals-crm-pipeline)

#### [!UICONTROL Listar pipelines de oferta/tíquete]

Retorna todos os pipelines de negócios e tíquetes de um determinado portal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Objeto] </td> 
   <td>Selecione se deseja listar ofertas ou tickets.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um pipeline de CRM do contrato]

Retorna um pipeline de negociação específico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Pipeline] </td> 
   <td>Insira ou mapeie a ID do pipeline do qual deseja recuperar detalhes. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Estágio] </td> 
   <td>Insira ou mapeie a ID do estágio para o qual deseja recuperar detalhes. </td> 
  </tr> 
 </tbody> 
</table>

### Empresas

#### [!UICONTROL Procurar Empresas por Domínio]

Recupera uma lista de empresas com base em uma correspondência exata com a propriedade de domínio.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
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
   <td>Selecione as propriedades que você deseja que apareçam na saída do módulo. </td> 
  </tr> 
 </tbody> 
</table>

### Arquivos

* [[!UICONTROL Criar uma pasta]](#create-a-folder)
* [[!UICONTROL Excluir uma pasta]](#delete-a-folder)
* [[!UICONTROL Mover um arquivo]](#move-a-file)

#### [!UICONTROL Criar uma pasta]

Este módulo cria uma pasta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome da Pasta] </td> 
   <td>Insira ou mapeie um nome para a nova pasta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Pasta Pai] </td> 
   <td>Selecione a ID da pasta principal da pasta que você está criando. </td> 
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
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Informe a ID da pasta que deseja deletar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover um arquivo]

Move um arquivo para outra pasta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Arquivo] </td> 
   <td>Insira ou mapeie a ID do arquivo que deseja mover. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Pasta] </td> 
   <td>Selecione a ID da pasta para onde deseja mover o arquivo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome]</td> 
   <td>Insira um nome para o arquivo movido.</td> 
  </tr> 
 </tbody> 
</table>

### Tíquetes

#### [!UICONTROL Excluir um tíquete]

Exclui um tíquete existente por sua ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Digite a ID do ticket que você deseja excluir. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Fazer uma chamada de API]

Permite executar uma chamada de API personalizada.

>[!NOTE]
>
>Os seguintes endpoints foram descontinuados na API HubSpot em 31 de agosto de 2023 e não podem mais ser usados em módulos do Fusion.
>
>* Listar eventos de conteúdo
>* Listar eventos sociais
>* Listar eventos de tarefas do calendário
>* Listar todos os eventos do calendário
>* Criar tarefa de calendário
>* Obter tarefa de calendário por ID
>* Atualizar tarefa de calendário
>* Excluir uma tarefa de calendário

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL HubSpot CRM] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Insira um caminho relativo para https://api.hubapi.com/. Por exemplo, /contacts/v1/lists/all/contacts/all</p> <p>Para obter a lista de endpoints disponíveis, consulte o <a href="https://legacydocs.hubspot.com/docs/overview">[!DNL HubSpot] Documentação da API</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   <td> <p>Selecione o método HTTP que deseja usar:</p> <p>[!UICONTROL GET]</p> <p>para recuperar informações de uma entrada.</p> <p>[!UICONTROL POST]</p> <p>para criar uma nova entrada.</p> <p>[!UICONTROL PUT]</p> <p>para atualizar/substituir uma entrada existente.</p> <p>[!UICONTROL PATCH]</p> <p>para fazer uma atualização de entrada parcial.</p> <p>[!UICONTROL DELETE]</p> <p>para deletar uma entrada.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p> Insira os cabeçalhos de solicitação desejados. Não é necessário adicionar cabeçalhos de autorização; já fizemos isso para você.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadeia de Consulta]</td> 
   <td> <p> Insira a string de consulta da solicitação.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada de API na forma de um objeto JSON padrão. Ao usar declarações condicionais, como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemplo:** A chamada de API a seguir retorna todos os contatos da [!DNL HubSpot] conta:
>
>**URL**: `/contacts/v1/lists/all/contacts/all`
>
>**Método**: `GET`
>
>![](assets/hubspot-api-config.png)
>
>As correspondências da pesquisa podem ser encontradas na Saída do módulo em [!UICONTROL Pacote] > [!UICONTROL Corpo] > [!UICONTROL contatos].
>
>No nosso exemplo, 3 contatos foram retornados:
>
>![](assets/hubspot-api-output.png)

## Criar um novo aplicativo

1. Faça logon no [!DNL HubSpot] conta de desenvolvedor.
1. Selecione o **[!UICONTROL Criar um aplicativo]** opção.
1. Insira o nome do aplicativo e [!UICONTROL Salvar] a caixa de diálogo.
1. Selecione os escopos necessários para o webhook.

   Por exemplo, adicione escopos de contatos para acionar o módulo quando um novo contato for criado ou excluído.

   A variável [!UICONTROL escopo de contatos] é tudo o que você precisa para receber contatos, ofertas e webhooks de eventos da empresa.

   >[!IMPORTANT]
   >
   >Não preencha o [!UICONTROL URL de redirecionamento] campo.
