---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;agile-and-teams;user-management
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Google Team Drive
description: Os  [!DNL Adobe Workfront Fusion Google Team Drive] módulos permitem que você monitore, carregue, atualize, copie, exclua ou recupere arquivos e crie pastas em sua  [!DNL Google Shared] unidade.
author: Becky
feature: Workfront Fusion
exl-id: 8b4c057f-bb98-44d1-9b71-cbeaa402a1c3
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1297'
ht-degree: 0%

---

# [!DNL Google Team Drive] módulos

Os módulos do [!DNL Adobe Workfront Fusion] [!DNL Google Team Drive] permitem que você monitore, carregue, atualize, copie, exclua ou recupere arquivos e crie pastas no [!DNL Google Shared Drive].

Para usar [!DNL Google Team Drive] com [!DNL Adobe Workfront Fusion], é necessário ter uma conta [!DNL Google Workspace]. Se você não tiver uma, poderá criar uma conta do [!DNL Google Workspace] no [[!DNL Google Workspace] site de inscrição](https://workspace.google.com/business/signup/welcome).

Em um cenário [!DNL Adobe Workfront Fusion], você pode automatizar fluxos de trabalho que usam [!DNL Google Team Drive], bem como conectá-los a vários aplicativos e serviços de terceiros.

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
   <p>Requisito atual do produto: se você tiver o plano [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], sua organização deve comprar [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Para usar módulos [!DNL Google Team Drive], você deve ter um [!DNL Google Team Drive].

## [!DNL Google Team Drive] módulos e seus campos

Ao configurar módulos do [!DNL Google Team Drive], o [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos [!DNL Google Team Drive] adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Os campos de diálogo do módulo exibidos em **bold** (no cenário [!DNL Workfront Fusion], **não** neste artigo de documentação) são obrigatórios.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Triggers

#### [!UICONTROL Observar arquivos]

Retorna os detalhes do arquivo quando um novo arquivo é adicionado e/ou modificado na pasta especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Team Drive] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unidade de Equipe]</td> 
   <td> <p> Selecione a unidade compartilhada que deseja assistir.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione a pasta na unidade compartilhada.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Quais arquivos observar]</td> 
   <td> <p> Selecione o tipo de arquivo que deseja observar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Documents] arquivos no formato] </td> 
   <td> <p>Selecione o formato para o qual você deseja converter os [!DNL Google Documents] arquivos observados.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Sheets] arquivos no formato] </td> 
   <td> <p>Selecione o formato para o qual você deseja converter os [!DNL Google Sheets] arquivos observados.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Slides] arquivos no formato] </td> 
   <td> <p>Selecione o formato para o qual você deseja converter os [!DNL Google Slides] arquivos observados.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Drawings] arquivos no formato] </td> 
   <td> <p>Selecione o formato para o qual você deseja converter os [!DNL Google Drawings] arquivos observados.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Observar]</td> 
   <td> <p> Selecione se deseja monitorar a pasta em busca de arquivos novos e modificados ou apenas em busca de novos arquivos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de arquivos baixados]</td> 
   <td> <p> Defina o número máximo de arquivos que [!DNL Workfront Fusion] retornará durante um ciclo de execução.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [[!UICONTROL Carregar um arquivo]](#upload-a-file)
* [[!UICONTROL Atualizar um Arquivo]](#update-a-file)
* [[!UICONTROL Copiar um Arquivo]](#copy-a-file)
* [[!UICONTROL Excluir um arquivo]](#delete-a-file)
* [[!UICONTROL Mover um arquivo para a lixeira]](#move-a-file-to-trash)
* [[!UICONTROL Obter um Arquivo]](#get-a-file)
* [[!UICONTROL Obter uma Lista de Arquivos]](#get-a-file-list)
* [[!UICONTROL Criar uma Pasta]](#create-a-folder)

#### [!UICONTROL Carregar um arquivo]

Faz upload de um arquivo para a unidade compartilhada especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Team Drive] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unidade de Equipe] </td> 
   <td> <p>Selecione a unidade compartilhada na qual você deseja fazer upload de um arquivo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione a pasta na unidade compartilhada.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Arquivo Source]</p> </td> 
   <td> <p>Especifique o arquivo que deseja fazer upload na unidade compartilhada.</p> <p>Mapeie o arquivo que você deseja fazer upload do módulo anterior (por exemplo, [!UICONTROL HTTP] &gt;[!UICONTROL Obter um Arquivo] ou [!UICONTROL Dropbox] &gt;[!UICONTROL Obter um arquivo)], ou insira o nome do arquivo e os dados do arquivo manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Título]</td> 
   <td> <p> Insira o título do arquivo que será exibido na pasta compartilhada.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter um Arquivo]</td> 
   <td> <p> Habilite essa opção para converter o arquivo para o formato Google correspondente na pasta compartilhada.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar um Arquivo]

Permite alterar o nome e/ou o conteúdo do arquivo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Team Drive] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unidade de Equipe]</td> 
   <td> <p> Selecione a unidade compartilhada que contém o arquivo que você deseja atualizar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione a pasta na unidade compartilhada.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Arquivo]</td> 
   <td> <p> Insira (mapeie) a ID do arquivo que você deseja atualizar.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Arquivo Source]</p> </td> 
   <td>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Título] </td> 
   <td> <p>Insira o novo título para o arquivo atualizado.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter um Arquivo]</td> 
   <td> <p> Habilite esta opção para converter o arquivo para o formato [!DNL Google] correspondente na pasta compartilhada.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiar um Arquivo]

Copia um arquivo especificado para a pasta selecionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Team Drive] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unidade de Equipe]</td> 
   <td> <p> Selecione a unidade compartilhada que contém o arquivo a ser copiado.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione a pasta de destino para a qual deseja copiar o arquivo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Arquivo]</td> 
   <td> <p> Insira (mapeie) a ID do arquivo que deseja copiar.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL O nome do arquivo de cópia]</p> </td> 
   <td> <p>Informe o novo nome do arquivo se quiser que ele seja alterado no local de destino.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir um arquivo]

Exclui um arquivo especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Team Drive] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Arquivo]</td> 
   <td> <p> Insira ou mapeie a ID do arquivo que deseja excluir.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover um arquivo para a lixeira]

Move um arquivo especificado para a lixeira.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Team Drive] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Arquivo]</td> 
   <td> <p> Insira ou mapeie o ID do arquivo que você deseja mover para a lixeira.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um Arquivo]

Recupera detalhes sobre o arquivo especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Team Drive] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Documents] arquivos no formato] </td> 
   <td> <p>Selecione o formato para o qual você deseja converter os arquivos [!DNL Google Documents].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Sheets] arquivos no formato] </td> 
   <td> <p>Selecione o formato para o qual você deseja converter os arquivos [!DNL Google Sheets].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Slides] arquivos no formato] </td> 
   <td> <p>Selecione o formato para o qual você deseja converter os arquivos [!DNL Google Slides].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Drawings] arquivos no formato] </td> 
   <td> <p>Selecione o formato para o qual você deseja converter os arquivos [!DNL Google Drawings].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Arquivo]</td> 
   <td> <p> Insira ou mapeie a ID do arquivo que deseja recuperar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter uma Lista de Arquivos]

Recupera detalhes de arquivos e/ou pastas com base no termo de pesquisa.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Team Drive] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unidade de Equipe]</td> 
   <td> <p> Selecione a unidade compartilhada da qual deseja listar arquivos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione a pasta da qual deseja listar arquivos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pesquisar] </td> 
   <td> <p>Selecione o tipo de pesquisa que deseja realizar - veja abaixo.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Consulta]</p> </td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>[!UICONTROL Pesquisar em nomes de arquivo]</p> <p style="font-weight: normal;">Insira o nome do arquivo (incluindo a extensão de arquivo) quando a opção [!UICONTROL Pesquisar termo exato] for selecionada ou insira a parte do nome quando a opção [!UICONTROL Pesquisar nomes contendo o termo pesquisado] for selecionada.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Pesquisa de texto completo]</p> <p>Insira o termo de pesquisa para pesquisar pelos nomes de arquivo, descrições e conteúdo.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Consulta de pesquisa personalizada]</p> <p>Insira o termo de consulta de pesquisa [!DNL Google]. Para obter mais detalhes, consulte a <a href="https://developers.google.com/drive/api/v2/ref-search-terms">Documentação de Consulta de Pesquisa</a> de [!DNL Google]. Exemplo: <code>fullText contains '"Hello world"'</code></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recuperar]</td> 
   <td>Selecione se deseja recuperar arquivos, pasta ou ambos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de resultados retornados]</td> 
   <td> <p> Defina o número máximo de arquivos ou pastas que [!DNL Workfront Fusion] retornará durante um ciclo de execução.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar uma Pasta]

Cria uma nova pasta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Team Drive] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unidade de Equipe]</td> 
   <td> <p> Selecione a unidade compartilhada na qual deseja criar uma pasta.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione a pasta na qual deseja criar uma pasta.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL O nome da nova pasta]</td> 
   <td> <p> Insira o nome da nova pasta.</p> </td> 
  </tr> 
 </tbody> 
</table>
