---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Microsoft OneDrive for Business
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: b7175cb9-aade-49b7-a28b-25fc9805a078
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1257'
ht-degree: 0%

---

# [!DNL Microsoft OneDrive for Business] módulos

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Módulos do Microsoft OneDrive for Business](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/microsoft-onedrive-for-business-modules.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

Em um cenário [!DNL Adobe Workfront Fusion], você pode automatizar fluxos de trabalho que usam [!DNL Microsoft OneDrive for Business], bem como conectá-los a vários aplicativos e serviços de terceiros.

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

Para usar [!DNL Microsoft OneDrive for Business] com [!DNL Adobe Workfront Fusion], você precisará de uma conta [!DNL Microsoft].

Para obter instruções sobre como conectar sua conta do [!DNL OneDrive for Business] ao [!DNL Workfront Fusion], consulte [Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)



## Conectando o serviço [!DNL Microsoft OneDrive for Business] a [!DNL Workfront Fusion]

Para obter instruções sobre como conectar sua conta do [!DNL Microsoft OneDrive for Business] ao [!UICONTROL Workfront Fusion], consulte [Criar uma conexão com o [!UICONTROL Adobe Workfront Fusion] - Instruções básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Alguns aplicativos do Microsoft usam a mesma conexão, que está vinculada a permissões de usuário individuais. Portanto, ao criar uma conexão, a tela de consentimento de permissões exibe todas as permissões que foram concedidas anteriormente à conexão deste usuário, além de todas as novas permissões necessárias para o aplicativo atual.
>
>Por exemplo, se um usuário tiver permissões de &quot;Tabela de leitura&quot; concedidas por meio do conector do Excel e criar uma conexão no conector do Outlook para ler emails, a tela de consentimento de permissões mostrará a permissão &quot;Tabela de leitura&quot; já concedida e a permissão &quot;Gravar email&quot; recém-necessária.

## [!DNL Microsoft OneDrive for Business] módulos e seus campos

Ao configurar módulos do [!DNL Microsoft OneDrive for Business], o [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos [!DNL Microsoft OneDrive for Business] adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td> <p> Defina o número máximo de resultados com os quais [!DNL Workfront Fusion] trabalhará durante um ciclo.</p> </td> 
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
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td> <p> Defina o número máximo de resultados com os quais [!DNL Workfront Fusion] trabalhará durante um ciclo.</p> </td> 
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
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td> <p>[!UICONTROL Arquivo Source]</p> </td> 
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
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL ID da Unidade]</strong> </td> 
   <td> <p>Selecione a unidade na qual deseja criar uma nova pasta.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL pasta]</strong> </td> 
   <td> <p>Selecione a pasta na qual deseja criar uma nova pasta.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Nome da Pasta]</strong> </td> 
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
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
