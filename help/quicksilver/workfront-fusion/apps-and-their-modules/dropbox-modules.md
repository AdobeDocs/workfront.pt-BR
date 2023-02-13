---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos Dropbox
description: Em um [!DNL Adobe Workfront Fusion] você pode automatizar fluxos de trabalho que usam o Dropbox, bem como conectá-lo a vários aplicativos e serviços de terceiros.Isso permite automatizar atividades como monitoramento, pesquisa, recuperação, listagem, criação e edição de arquivos e pastas em seu Dropbox.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: a35631d7-40ac-4e7f-9a37-ad3879c0b6a2
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3013'
ht-degree: 0%

---

# [!DNL Dropbox] módulos

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!UICONTROL Dropbox], bem como conectá-lo a vários aplicativos e serviços de terceiros.Isso permite automatizar atividades como monitoramento, pesquisa, recuperação, listagem, criação e edição de arquivos e pastas em seu [!UICONTROL Dropbox].

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

Para usar [!DNL Dropbox] módulos, você deve ter um [!DNL Dropbox] conta.

## [!DNL Dropbox] módulos e seus campos

Ao configurar [!DNL Dropbox] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Dropbox] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Módulos de acionador](#trigger-modules)
* [Módulos para obter [!DNL Dropbox] arquivos e pastas](#modules-for-getting-dropbox-files-and-folders)
* [Módulos para criação e edição [!DNL Dropbox] arquivos e pastas](#modules-for-creating-and-editing-dropbox-files-and-folders)
* [Outros módulos](#other-modules)

### Módulos de acionador

#### [!UICONTROL Arquivos de monitoramento]

Esse módulo do tipo Trigger retorna detalhes do arquivo quando o arquivo em uma pasta especificada é modificado.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Dropbox] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione a pasta que deseja visualizar as alterações.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL também subpastas]</td> 
   <td> <p> Ative essa opção para também monitorar subpastas na pasta selecionada para arquivos modificados.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limite] </td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Módulos para obter [!DNL Dropbox] arquivos e pastas

* [[!UICONTROL Pesquisar arquivos/pastas]](#search-filesfolders)
* [[!UICONTROL Baixar um arquivo]](#download-a-file)
* [[!UICONTROL Obter metadados de uma pasta]](#get-a-folder-metadata)
* [[!UICONTROL Listar todos os arquivos/subpastas em uma pasta]](#list-all-filessubfolders-in-a-folder)
* [[!UICONTROL Revisões do arquivo de lista]](#list-file-revisions)

#### [!UICONTROL Pesquisar arquivos/pastas]

Este módulo de pesquisa procura registros em um objeto em [!DNL Dropbox] que correspondem à consulta de pesquisa especificada.

Você pode mapear essas informações em módulos subsequentes do cenário.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Dropbox] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>Insira o termo de pesquisa.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione a pasta que deseja pesquisar. Esse módulo pesquisa todo o [!DNL Dropbox] se você não selecionar uma pasta.</p> </td> 
  </tr> 
  <tr> 
   <td>Status do arquivo</td> 
   <td> <p> Selecione o status do arquivo para restringir a pesquisa ao status do arquivo selecionado.</p> </td> 
  </tr> 
  <tr> 
   <td>Categorias de arquivo</td> 
   <td> <p> Selecione as categorias de arquivo para restringir a pesquisa às categorias selecionadas.</p> </td> 
  </tr> 
  <tr> 
   <td>Extensões de arquivo</td> 
   <td> <p> Escolha as extensões de arquivo que deseja pesquisar.</p> </td> 
  </tr> 
  <tr> 
   <td>Limite </td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Baixar um arquivo]

Este módulo de ação baixa um arquivo de uma pasta.

Especifique o arquivo e seu local.

O módulo retorna a ID do arquivo e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

>[!NOTE]
>
>Esse módulo é útil para fornecer arquivos para módulos subsequentes.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Dropbox] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>Como selecionar arquivos</td> 
   <td> <p> Selecione se deseja mapear o caminho do arquivo ou selecione o arquivo manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Caminho / Arquivo do Arquivo</p> </td> 
   <td> <p style="font-weight: bold;">Caminho do arquivo</p> <p>Insira ou mapeie o caminho de destino para o arquivo.</p> <p style="font-weight: bold;">Arquivo</p> <p>Selecione o arquivo no menu .</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter metadados de uma pasta]

Este módulo de ação recupera detalhes da pasta compartilhada.

Especifique a ID da pasta.

O módulo retorna a ID da pasta e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Dropbox] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>ID da pasta compartilhada</td> 
   <td> <p> Insira ou mapeie a ID da pasta sobre a qual deseja recuperar detalhes.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listar todos os arquivos/subpastas em uma pasta]

Esse módulo de ação lista arquivos ou pastas em uma pasta específica.

Especifique a ID da pasta.

O módulo retorna as IDs dos arquivos ou pastas e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Dropbox] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>Lista </td> 
   <td> <p>Selecione se deseja recuperar arquivos ou pastas.</p> </td> 
  </tr> 
  <tr> 
   <td>Mostrar somente arquivos baixáveis</td> 
   <td> <p> Habilite esta opção para retornar somente arquivos baixáveis. Alguns tipos de arquivos, como Google Docs, não podem ser baixados.</p> </td> 
  </tr> 
  <tr> 
   <td>Pasta </td> 
   <td> <p>Insira ou mapeie a pasta da qual deseja recuperar arquivos ou pastas.</p> </td> 
  </tr> 
  <tr> 
   <td>Limite </td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo liste durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Revisões do arquivo de lista]

Este módulo de ação recupera todas as revisões de arquivo (um histórico de versões) de um arquivo específico.\
Especifique a ID do arquivo.

O módulo retorna quaisquer campos padrão associados ao registro, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Dropbox] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>Como selecionar arquivos</td> 
   <td> <p> Selecione se deseja mapear o caminho do arquivo ou selecione o arquivo manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Caminho / Arquivo do Arquivo</p> </td> 
   <td> <p style="font-weight: bold;">Caminho do arquivo</p> <p>Insira ou mapeie o caminho de destino para o arquivo.</p> <p style="font-weight: bold;">Arquivo</p> <p>Selecione o arquivo no menu .</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Limite</p> </td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo liste durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Módulos para criação e edição [!DNL Dropbox] arquivos e pastas

* [[!UICONTROL Upload] um arquivo](#upload-a-file)
* [[!UICONTROL Criar uma pasta]](#create-a-folder)
* [[!UICONTROL Criar/substituir um arquivo de texto]](#createoverwrite-a-text-file)
* [[!UICONTROL Criar/atualizar um link de compartilhamento]](#createupdate-a-share-link)
* [[!UICONTROL Restaurar um arquivo]](#restore-a-file)
* [[!UICONTROL Mover um arquivo/pasta]](#move-a-filefolder)
* [[!UICONTROL Renomear um arquivo/pasta]](#rename-a-filefolder)
* [[!UICONTROL Excluir um arquivo/pasta]](#delete-a-filefolder)

#### [!UICONTROL Fazer upload de um arquivo]

Este módulo de ação carrega um arquivo em uma pasta.

Especifique informações como o local do arquivo, o arquivo que deseja carregar e um novo nome opcional para o arquivo.

O módulo retorna a ID do arquivo e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Dropbox] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta]</td> 
   <td> <p> Selecione a pasta de seu [!DNL Dropbox] você deseja fazer upload do arquivo para o .</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Arquivo de origem]</p> </td> 
   <td> <p>Insira ou mapeie o arquivo que deseja adicionar ao [!DNL Dropbox] pasta selecionada acima.</p> <p style="font-weight: bold;">[!UICONTROL Nome do arquivo]</p> <p>Insira ou mapeie o nome do arquivo, incluindo a extensão de arquivo.</p> <p style="font-weight: bold;">[!UICONTROL Dados do arquivo]</p> <p>Insira ou mapeie os dados do arquivo (do módulo anterior, como [!UICONTROL Google Drive] &gt;[!UICONTROL Obter um arquivo)].</p> <p>Observação: O tamanho máximo do arquivo carregado é de 150 MB.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Substituir um arquivo existente]</td> 
   <td> <p> Habilite esta opção para substituir o arquivo existente pelo novo arquivo. Se essa opção for deixada desativada, o arquivo carregado será renomeado.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar uma pasta]

Esse módulo de ação cria uma nova pasta.

Especifique o caminho e um nome para a pasta.

O módulo retorna a ID da pasta e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Dropbox] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome da pasta] </td> 
   <td> <p>Insira o nome da nova pasta.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Pasta]</p> </td> 
   <td> <p>Insira ou mapeie o caminho onde deseja criar uma nova pasta.</p> <p>Nota:   <p>Se estiver usando um [!DNL Dropbox Business] conta (com espaços de equipe), você deve remover a barra <code>/</code>ou não clique em <strong>[!UICONTROL Clique aqui] para escolher a pasta</strong> para criar uma pasta de equipe na raiz.</p> <p>Se a barra não for removida, um erro <code>[409] path/malformed_path/..</code> é retornado.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Renomear automaticamente]</td> 
   <td> <p> Ative essa opção para renomear a nova pasta se uma pasta com o mesmo nome já existir no local de destino.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar/substituir um arquivo de texto]

Esse módulo de ação cria um arquivo DOC ou substitui o conteúdo de um existente.

Especifique o arquivo de origem e a pasta .

O módulo retorna a ID da pasta e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Dropbox] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Selecionar para]</td> 
   <td> <p> Selecione se deseja criar ou substituir um arquivo DOC.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione o local de destino onde deseja criar um arquivo.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Arquivo de origem]</p> </td> 
   <td> <p>Insira ou mapeie o arquivo que deseja adicionar ao [!DNL Dropbox] pasta.</p> <p style="font-weight: bold;">Nome do arquivo</p> <p>Insira o nome do arquivo para o novo arquivo DOC (sem uma extensão).</p> <p style="font-weight: bold;">Conteúdo do arquivo</p> <p>Insira o conteúdo de texto do arquivo DOC.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar/atualizar um link de compartilhamento]

Este módulo de ação cria um link público para um arquivo.

Especifique o arquivo e as informações sobre o link.

O módulo retorna a ID do link e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Dropbox] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modo de seleção de arquivos]</td> 
   <td> <p> Selecione se deseja mapear ou inserir o caminho do arquivo ou selecione o arquivo manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Caminho / Arquivo do arquivo]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Caminho do arquivo]</p> <p>Insira ou mapeie o caminho de destino para o arquivo.</p> <p style="font-weight: bold;">[!UICONTROL Arquivo]</p> <p>Selecione o arquivo no menu .</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Visibilidade solicitada]</p> </td> 
   <td> <p>Selecione se o link é público, para equipe ou senha restrita.</p> <p>Observação: As opções [!UICONTROL Team only] e [!UICONTROL Access with password] só estão disponíveis para usuários que tenham [!DNL Dropbox Pro] ou versão superior.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de expiração do link]</td> 
   <td> <p> Insira a data e a hora em que o link expirará e não estará mais acessível. Se esse campo ficar vazio, o link não expirará. Para obter uma lista de formatos de data e hora compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Coação de tipo em [!DNL Adobe Workfront Fusion]</a>.</p> <p>Observação: As opções [!UICONTROL Team only] e [!UICONTROL Access with password] só estão disponíveis para usuários que têm o [!UICONTROL Dropbox Pro] ou versões superiores.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Nível de acesso do link]</p> </td> 
   <td> <p>Defina a permissão para o destinatário do link.</p> <p><strong>[!UICONTROL Viewer]</strong> Os usuários que usam o link podem exibir e comentar o conteúdo.</p> <p><strong>[!UICONTROL Editor]</strong> Os usuários que usam o link podem editar, exibir e comentar o conteúdo.</p> <p><strong>[!UICONTROL Máx.]</strong> Os usuários que usam o link recebem o nível máximo de acesso que você pode definir para.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Restaurar um arquivo]

Este módulo de ação restaura uma versão anterior de um arquivo.

Especifique o arquivo e o número da revisão desejada.

O módulo retorna a ID da versão e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Dropbox] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modo de seleção de arquivos]</td> 
   <td> <p> Selecione se deseja mapear ou inserir o caminho do arquivo ou selecione o arquivo manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Caminho do arquivo] / [!UICONTROL Arquivo]</p> </td> 
   <td> <p><strong>[!UICONTROL Caminho do arquivo]</strong> </p> <p>Insira ou mapeie o caminho de destino para o arquivo.</p> <p><strong>[!UICONTROL Arquivo]</strong> </p> <p>Selecione o arquivo no menu .</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Revisão]</p> </td> 
   <td> <p>Insira ou mapeie o número da revisão da revisão que você deseja restaurar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover um arquivo/pasta]

Esse módulo de ação move um arquivo ou pasta para um local diferente.

Especifique o arquivo ou pasta e como e onde deseja movê-lo.

O módulo retorna a ID do arquivo ou pasta e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Dropbox] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modo de seleção de arquivos] </td> 
   <td> <p>Selecione se deseja mapear ou inserir o caminho do arquivo ou selecione o arquivo manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Arquivo/Caminho da pasta] / [!UICONTROL Arquivo/Pasta]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Arquivo/Caminho da pasta]</p> <p>Insira ou mapeie o caminho de destino para o arquivo ou pasta.</p> <p style="font-weight: bold;">[!UICONTROL Arquivo/Pasta]</p> <p>Selecione o arquivo ou pasta no menu .</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Na Pasta]</p> </td> 
   <td> <p>Insira ou mapeie o local de destino do arquivo ou pasta.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Novo nome]</p> </td> 
   <td> <p>Insira o novo nome para o arquivo ou pasta no novo local.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Renomear automaticamente]</p> </td> 
   <td> <p>Ative essa opção para garantir que, se houver um arquivo ou pasta com o mesmo nome, o módulo renomeie o novo arquivo ou pasta adicionando ([!UICONTROL NUMBER]) após o nome do arquivo ou da pasta. Caso contrário, o arquivo ou a pasta no local de destino será substituído.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Permitir transferência de propriedade]</p> </td> 
   <td> <p>Ative essa opção para permitir movimentações por proprietário, mesmo que isso resultasse em uma transferência de propriedade do conteúdo que estivesse sendo movido.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Renomear um arquivo/pasta]

Esse módulo de ação renomeia um arquivo ou pasta.

Especifique o arquivo ou pasta e o novo nome.

O módulo retorna a ID do arquivo ou pasta e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Dropbox] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>Como selecionar arquivos</td> 
   <td> <p> Selecione se deseja mapear ou inserir o caminho do arquivo ou selecione o arquivo manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Caminho/Arquivo/Pasta</p> </td> 
   <td> <p style="font-weight: bold;">Caminho do arquivo/pasta</p> <p>Insira ou mapeie o caminho de destino para o arquivo ou pasta.</p> <p style="font-weight: bold;">Arquivo/Pasta</p> <p>Selecione o arquivo ou pasta no menu .</p> </td> 
  </tr> 
  <tr> 
   <td>Renomear </td> 
   <td> <p>Insira o [!UICONTROL target name] para o arquivo, incluindo a extensão de arquivo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir um arquivo/pasta]

Esse módulo de ação exclui um arquivo ou pasta.

Especifique o arquivo ou pasta.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Dropbox] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modo de seleção de arquivos]</td> 
   <td> <p> Selecione se deseja mapear ou inserir o caminho do arquivo ou selecione o arquivo manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Caminho do arquivo] / [!UICONTROL Arquivo]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Caminho do arquivo]</p> <p>Insira ou mapeie o caminho de destino para o arquivo.</p> <p style="font-weight: bold;">[!UICONTROL Arquivo]</p> <p>Selecione o arquivo no menu .</p> </td> 
  </tr> 
 </tbody> 
</table>

### Outros módulos

#### [!UICONTROL Faça uma chamada de API]

Esse módulo de ação permite que você faça uma chamada autenticada personalizada para o [!DNL Dropbox] API. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pela outra [!DNL Dropbox] módulos.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Dropbox] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Insira um caminho relativo a Enter um caminho relativo a <code>https://api.dropboxapi.com</code>. Por exemplo, <code>/2/files/list_folder</code></p> <p>Observação: Para obter a lista de endpoints disponíveis, consulte <a href="https://www.dropbox.com/developers/documentation/http/documentation">Documentação da API v2 do Dropbox</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Método]</p> </td> 
   <td> <p>Selecione o método de solicitação HTTP que você precisa configurar a chamada da API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cabeçalhos] </td> 
   <td> <p>Insira os cabeçalhos da solicitação desejada. [!DNL Workfront Fusion] adiciona cabeçalhos de autorização automaticamente.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sequência de consulta]</td> 
   <td> <p> Insira a sequência de consulta da solicitação.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Corpo] </td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada da API no formato de um objeto JSON padrão.</p> <p>Nota:   <p>Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemplo:** A chamada de API a seguir retorna os primeiros 10 arquivos do [!DNL /Text files] na sua pasta [!DNL Dropbox] conta:
>
>URL: `/2/files/list_folder`
>
>Corpo:
> 
>`{`
>
>`"path": "/Text files",`
>
>`"limit": 10,`
>
>`"recursive": false,`
>
>`"include_deleted": false`
>
>`}`
>
>As correspondências da pesquisa podem ser encontradas na Saída do módulo em [!UICONTROL Pacote] > [!UICONTROL Corpo] > entradas.
>
>Em nosso exemplo, 10 tíquetes foram retornados:

## Problemas comuns

* [Não é possível carregar ou atualizar um arquivo](#unable-to-upload-or-update-a-file)
* [Imagem referenciada por um link compartilhado não é renderizada](#image-referenced-via-a-shared-link-does-not-render)

### Não é possível carregar ou atualizar um arquivo

Há várias situações em que o upload ou a atualização de um arquivo falha:

* O arquivo carregado é muito grande e excede o tamanho máximo permitido para o arquivo [!DNL Dropbox] planejar, ou você tiver usado todos os seus [!DNL Dropbox] cota de armazenamento da conta. Você deve excluir os arquivos existentes da [!DNL Dropbox] ou atualize seu plano.
* A pasta selecionada anteriormente, para a qual o arquivo está sendo carregado, não existe mais. O cenário é interrompido e você deve selecionar a pasta de destino novamente.

### Imagem referenciada por um link compartilhado não é renderizada

O URL retornado pelo [!UICONTROL Dropbox] >[!UICONTROL Criar um link compartilhado] não se vincula diretamente a uma imagem, mas a um [!DNL Dropbox] página. Para forçar o download da imagem, substitua o `?dl=0` com `?dl=1`. Para forçar a renderização da imagem (por exemplo, em um navegador da Web ou no Facebook Messenger), anexe `&raw=1` ao URL.

Se você precisar obter o link direto ou bruto da imagem para o seu site ou para outros [!DNL Workfront Fusion] , você deve modificar o URL compartilhado inicial da seguinte maneira:

URL original:

`https://www.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png?dl=0`

1. Substituir `www` com `dl`.
1. Remover `?dl=0`.

URL final:

`https://dl.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png`

Para modificar automaticamente o URL, você pode usar o `replace()` função duas vezes:

* Substituir www por dl

   ![](assets/www-to-dl-350x32.png)

* E para remover ?dl=0

   ![](assets/remove-dl0-350x33.png)

Para fazer isso em uma etapa, combine essas funções:

![](assets/replace-both-350x47.png)

Também é possível copiá-lo e colá-lo no campo. Substituir `1.url` com o URL.

```
{{replace(replace(1.url; "?dl=0"; ""); "www"; "dl")}}
```
