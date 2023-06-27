---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Box
description: Em um [!DNL Adobe Workfront Fusion] Você pode automatizar fluxos de trabalho que usam o Box, bem como conectá-lo a vários aplicativos e serviços de terceiros. monitora uma pasta especificada para verificar alterações em arquivos, modificar e excluir arquivos existentes ou fazer upload de novos arquivos para uma pasta.
author: Becky
feature: Workfront Fusion
exl-id: 965ce570-40bf-474d-b318-0d2de8be6b9d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1070'
ht-degree: 0%

---

# Módulos do Box

Em um [!DNL Adobe Workfront Fusion] cenário, é possível automatizar workflows que usam [!DNL Box], bem como conectá-lo a vários aplicativos e serviços de terceiros. monitora uma pasta especificada para verificar alterações em arquivos, modificar e excluir arquivos existentes ou fazer upload de novos arquivos para uma pasta.

Se precisar de instruções sobre como criar um cenário, consulte [Criar um cenário no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Para obter informações sobre módulos, consulte [Módulos no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Para usar [!DNL Box] módulos, você deve ter uma [!DNL Box] conta.

## [!DNL Box] módulos e seus campos

Ao configurar [!DNL Box] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Box] Os campos podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Triggers

* [[!UICONTROL Novo evento]](#new-event)
* [[!UICONTROL Observar arquivos]](#watch-files)

#### [!UICONTROL Novo evento]

Esse módulo de acionador instantâneo inicia um cenário quando um arquivo é adicionado, movido, copiado, excluído, bloqueado ou desbloqueado.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Selecione o webhook que deseja usar para assistir mensagens de saída. Para adicionar um webhook, clique em <strong>[!UICONTROL Adicionar]</strong> e digite o nome e a conexão do webhook.</p> <p> Para obter instruções sobre como conectar a conta da [!UICONTROL Box] ao [!UICONTROL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!UICONTROL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Número máximo de eventos retornados]</p> </td> 
   <td> <p>Insira o maior número de eventos que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Observar arquivos]

Este módulo de acionamento inicia um cenário quando um novo arquivo é adicionado ou um arquivo existente é atualizado em uma pasta que está sendo observada.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Box] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  <tr> 
   <td role="rowheader">Observar</td> 
   <td> <p>Selecione o tipo de arquivo que deseja observar.</p> 
    <ul> 
     <li> <p><strong>Somente arquivos novos</strong> </p> <p>O cenário será iniciado quando um novo arquivo for adicionado.</p> </li> 
     <li> <p><strong>Novos arquivos e todas as alterações</strong> </p> <p>O cenário começa quando um arquivo é adicionado ou quando o conteúdo do arquivo ou um atributo de arquivo (como seu nome) é modificado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Número máximo de arquivos baixados</p> </td> 
   <td> <p>Insira o maior número de arquivos que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [[!UICONTROL Carregar] um arquivo](#upload-a-file)
* [[!UICONTROL Atualizar um arquivo]](#update-a-file)
* [[!UICONTROL Excluir um arquivo]](#delete-a-file)
* [[!UICONTROL Obter um arquivo]](#get-a-file)

#### [!UICONTROL Carregar um arquivo]

Este módulo de ação carrega um arquivo.

Especifique o arquivo. Você também pode fornecer um novo nome para o arquivo.

O módulo retorna a ID do arquivo e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Box] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Se esse módulo não for bem-sucedido, considere o seguinte:
>
>* O tamanho do arquivo pode exceder o limite máximo de tamanho para o [!DNL Box] ou você pode ter usado todos os seus [!DNL Box] cota de armazenamento da conta. Para obter mais espaço de armazenamento, exclua arquivos existentes de [!DNL Box] ou atualize seu [!DNL Box] conta.
>* [!DNL Box] O não carrega mais de um arquivo com o mesmo nome em uma única pasta. Se a pasta de destino contiver um arquivo com o mesmo nome do arquivo que está sendo carregado, a execução do cenário será encerrada com um erro. Para evitar isso, renomear o arquivo. Se quiser atualizar o arquivo, use o **[!UICONTROL Atualizar um arquivo]** módulo.

#### [!UICONTROL Atualizar um arquivo]

Este módulo de ação atualiza um arquivo.

Especifique a ID do arquivo.

O módulo retorna a ID do arquivo e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Box] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Arquivo]</td> 
   <td>Insira ou mapeie o identificador exclusivo do arquivo que você deseja que o módulo atualize.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir um arquivo]

Este módulo de ação exclui um arquivo.

Especifique a ID do arquivo.

O módulo retorna a ID do arquivo e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Box] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Arquivo]</td> 
   <td>Insira ou mapeie o identificador exclusivo do arquivo que você deseja que o módulo atualize.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um arquivo]

Este módulo de ação baixa um arquivo.

Especifique a ID do arquivo.

O módulo retorna a ID do arquivo e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

>[!NOTE]
>
>Esse módulo é útil para fornecer arquivos aos módulos subsequentes.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Box] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Arquivo]</td> 
   <td>Insira ou mapeie o identificador exclusivo do arquivo que você deseja que o módulo atualize.</td> 
  </tr> 
 </tbody> 
</table>

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Possible problems</h2>
-->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This is drafted out because we don't have a download module for Box yet</p>
-->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Watch files trigger module doesn't download a file contained in the folder.</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">There are several situations when downloading a file fails:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The current file lock setting does not allow the file to be downloaded or the downloading of the file is disabled. In this case, the file is ignored.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">When the scenario started, the file was being uploaded to the server and was not ready to be downloaded. The scenario run gets stopped and Workfront Fusion tries downloading the file again during the next execution of the scenario.</li>
  -->
