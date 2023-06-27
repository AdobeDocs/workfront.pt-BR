---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Microsoft OneDrive for Business
description: Em um [!DNL Adobe Workfront Fusion] cenário, é possível automatizar workflows que usam [!DNL Microsoft OneDrive for Business], bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: b7175cb9-aade-49b7-a28b-25fc9805a078
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1087'
ht-degree: 0%

---

# [!DNL Microsoft OneDrive for Business] módulos

Em um [!DNL Adobe Workfront Fusion] cenário, é possível automatizar workflows que usam [!DNL Microsoft OneDrive for Business], bem como conectá-lo a vários aplicativos e serviços de terceiros.

Se precisar de instruções sobre como criar um cenário, consulte [Criar um cenário no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obter informações sobre módulos, consulte [Módulos no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Para usar [!DNL Microsoft OneDrive for Business] com [!DNL Adobe Workfront Fusion], você precisará de um [!DNL Microsoft] conta.

Para obter instruções sobre como conectar seu [!DNL OneDrive for Business] conta para [!DNL Workfront Fusion], consulte [Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Microsoft OneDrive for Business] módulos e seus campos

Ao configurar [!DNL Microsoft OneDrive for Business] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Microsoft OneDrive for Business] Os campos podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Ações](#actions)

### Triggers

* [[!UICONTROL Observar arquivos]](#watch-files)
* [[!UICONTROL Observar pastas]](#watch-folders)

#### [!UICONTROL Observar arquivos]

Esse módulo acionador é ativado quando um novo arquivo é adicionado ou atualizado em uma pasta que está sendo observada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID da Unidade]</p> </td> 
   <td> <p>Selecione a unidade que deseja observar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta]</td> 
   <td> <p> Selecione a pasta que deseja observar. Em um cenário, só é possível monitorar uma pasta.</p> <p>Dica: para rastrear várias pastas, crie um cenário independente para cada uma delas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL que eu quero assistir]</p> </td> 
   <td> <p>Selecione se você deseja observar novos arquivos e todas as alterações ou somente novos arquivos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de linhas retornadas]</td> 
   <td> <p> Defina o número máximo de resultados que [!DNL Workfront Fusion] funcionará com durante um ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Observar pastas]

Esse módulo acionador é ativado quando uma nova pasta é adicionada à pasta que está sendo monitorada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexão]</p> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID da Unidade]</p> </td> 
   <td> <p>Selecione a unidade que deseja observar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta]</td> 
   <td> <p> Selecione a pasta que deseja observar. Em um cenário, só é possível monitorar uma pasta.</p> <p>Dica: para rastrear várias pastas, crie um cenário independente para cada uma delas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL que eu quero assistir]</p> </td> 
   <td> <p>Selecione se deseja observar novas pastas e todas as alterações ou somente novas pastas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de linhas retornadas]</td> 
   <td> <p> Defina o número máximo de resultados que [!DNL Workfront Fusion] funcionará com durante um ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [[!UICONTROL Carregar um arquivo]](#upload-a-file)
* [[!UICONTROL Excluir um arquivo]](#delete-a-file)
* [[!UICONTROL Obter um arquivo]](#get-a-file)
* [[!UICONTROL Criar uma pasta]](#create-a-folder)
* [[!UICONTROL Excluir uma pasta]](#delete-a-folder)
* [[!UICONTROL Obter um link de compartilhamento]](#get-a-sharing-link)

#### [!UICONTROL Carregar um arquivo]

Este módulo de ação faz upload de um arquivo binário ou de texto para uma pasta especificada

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID da Unidade]</td> 
   <td> <p>Selecione a unidade na qual deseja fazer upload de um arquivo.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione a pasta na unidade.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Arquivo de Origem]</p> </td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Se existir um arquivo com o mesmo nome]</td> 
   <td> <p> Selecione o que deseja fazer se um arquivo com o mesmo nome do arquivo do qual você está tentando fazer upload já existir.</p> 
    <ul> 
     <li>[!UICONTROL Substituir o arquivo existente]</li> 
     <li>[!UICONTROL Renomear o novo arquivo]</li> 
     <li>[!UICONTROL Encerra com erro]</li> 
    </ul> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir um arquivo]

Este módulo de ação move o arquivo especificado para a lixeira.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID da Unidade]</td> 
   <td> <p>Selecione a unidade da qual deseja excluir um arquivo.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Arquivo]</td> 
   <td> <p>Informe a ID do arquivo que deseja deletar. </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um arquivo]

Este módulo de ação recupera o arquivo com a ID fornecida.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID da Unidade]</td> 
   <td> <p>Selecione a unidade da qual deseja recuperar um arquivo.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Arquivo]</td> 
   <td> <p>Insira a ID do arquivo que você deseja recuperar. </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar uma pasta]

Cria uma pasta dentro da pasta pai especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!UICONTROL Conexão]</strong> </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL ID da Unidade]</strong> </td> 
   <td> <p>Selecione a unidade na qual deseja criar uma nova pasta.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Pasta]</strong> </td> 
   <td> <p>Selecione a pasta na qual deseja criar uma nova pasta.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Nome da pasta]</strong> </td> 
   <td>Insira ou mapeie um nome para a nova pasta.</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir uma pasta]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID da Unidade]</td> 
   <td> <p>Selecione a unidade da qual deseja excluir um arquivo.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID da Pasta]</td> 
   <td> <p>Insira ou mapeie a ID da pasta que deseja excluir. </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um link de compartilhamento]

Este módulo recupera um link que você pode compartilhar para dar acesso ao arquivo especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID da Unidade]</td> 
   <td> <p>Selecione a unidade na qual deseja fazer upload de um arquivo.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enter]</td> 
   <td> <p>Selecione se deseja escolher um arquivo usando a ID do arquivo ou o caminho do Arquivo. Insira a ID do arquivo ou o caminho no campo exibido.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Tipo de permissão]</p> </td> 
   <td> <p>Selecione se você deseja que as pessoas que recebem o link tenham permissões de leitura/gravação ou somente leitura.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Escopo]</td> 
   <td> <p> Selecione se você deseja que o arquivo seja acessível por qualquer pessoa que tenha o link ou acessível somente aos membros da organização.</p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
