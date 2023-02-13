---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;agile-and-teams;user-management
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos da Unidade de Equipe Google
description: O [!DNL Adobe Workfront Fusion Google Team Drive] os módulos permitem monitorar, carregar, atualizar, copiar, excluir ou recuperar arquivos e criar pastas em seu [!DNL Google Shared] Dirija.
author: Becky
feature: Workfront Fusion
exl-id: 8b4c057f-bb98-44d1-9b71-cbeaa402a1c3
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1258'
ht-degree: 0%

---

# [!DNL Google Team Drive] módulos

O [!DNL Adobe Workfront Fusion] [!DNL Google Team Drive] os módulos permitem monitorar, carregar, atualizar, copiar, excluir ou recuperar arquivos e criar pastas em seu [!DNL Google Shared Drive].

Para usar [!DNL Google Team Drive] com [!DNL Adobe Workfront Fusion], é necessário ter um [!DNL G Suite] conta. Se não tiver um, você poderá criar um [!DNL G Suite] na conta do [[!DNL G Suite] inscrever-se no site](https://gsuite.google.com/signup/businessstarter/welcome).

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL Google Team Drive], bem como conectá-lo a vários aplicativos e serviços de terceiros.

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

Para usar [!DNL Google Team Drive] módulos, você deve ter um [!DNL Google Team Drive].

## [!DNL Google Team Drive] módulos e seus campos

Ao configurar [!DNL Google Team Drive] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Google Team Drive] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Os campos de diálogo do módulo exibidos em **bold** na [!DNL Workfront Fusion] , **not** neste artigo de documentação) são obrigatórias.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Triggers

#### [!UICONTROL Arquivos de monitoramento]

Retorna os detalhes do arquivo quando um novo arquivo é adicionado e/ou modificado na pasta especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Team Drive] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> Selecione a unidade compartilhada que deseja assistir.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione a pasta na unidade compartilhada.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Quais arquivos devem ser monitorados]</td> 
   <td> <p> Selecione o tipo de arquivos que deseja visualizar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Documents] arquivos para formatar] </td> 
   <td> <p>Selecione o formato que deseja observar [!DNL Google Documents] arquivos convertidos em.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Sheets] arquivos para formatar] </td> 
   <td> <p>Selecione o formato que deseja observar [!DNL Google Sheets] arquivos convertidos em.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Slides] arquivos para formatar] </td> 
   <td> <p>Selecione o formato que deseja observar [!DNL Google Slides] arquivos convertidos em.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Drawings] arquivos para formatar] </td> 
   <td> <p>Selecione o formato que deseja observar [!DNL Google Drawings] arquivos convertidos em.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td> <p> Selecione se deseja monitorar a pasta para arquivos novos e modificados ou apenas para novos arquivos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de arquivos baixados]</td> 
   <td> <p> Definir o número máximo de arquivos [!DNL Workfront Fusion] retornará durante um ciclo de execução.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [[!UICONTROL Fazer upload de um arquivo]](#upload-a-file)
* [[!UICONTROL Atualizar um arquivo]](#update-a-file)
* [[!UICONTROL Copiar um arquivo]](#copy-a-file)
* [[!UICONTROL Excluir um arquivo]](#delete-a-file)
* [[!UICONTROL Mover um arquivo para a lixeira]](#move-a-file-to-trash)
* [[!UICONTROL Obter um arquivo]](#get-a-file)
* [[!UICONTROL Obter uma lista de arquivos]](#get-a-file-list)
* [[!UICONTROL Criar uma pasta]](#create-a-folder)

#### [!UICONTROL Fazer upload de um arquivo]

Carrega um arquivo na unidade compartilhada especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Team Drive] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive] </td> 
   <td> <p>Selecione a unidade compartilhada na qual deseja fazer upload de um arquivo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione a pasta na unidade compartilhada.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Arquivo de origem]</p> </td> 
   <td> <p>Especifique o arquivo que deseja fazer upload na unidade compartilhada.</p> <p>Mapeie o arquivo que deseja fazer upload do módulo anterior (por exemplo, [!UICONTROL HTTP] &gt;[!UICONTROL Obter um arquivo] ou [!UICONTROL Dropbox] &gt;[!UICONTROL Obter um arquivo)], ou insira o nome do arquivo e os dados do arquivo manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Título]</td> 
   <td> <p> Insira o título do arquivo que será exibido na pasta compartilhada.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter um arquivo]</td> 
   <td> <p> Ative essa opção para converter o arquivo para o formato Google correspondente na pasta compartilhada.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar um arquivo]

Permite alterar o nome do arquivo e/ou o conteúdo do arquivo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Team Drive] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> Selecione a unidade compartilhada que contém o arquivo que você deseja atualizar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione a pasta na unidade compartilhada.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do arquivo]</td> 
   <td> <p> Insira (mapa) a ID do arquivo que deseja atualizar.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Arquivo de origem]</p> </td> 
   <td>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Título] </td> 
   <td> <p>Insira o novo título para o arquivo atualizado.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter um arquivo]</td> 
   <td> <p> Habilite esta opção para converter o arquivo para o arquivo correspondente [!DNL Google] na pasta compartilhada.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiar um arquivo]

Copia um arquivo especificado para a pasta selecionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Team Drive] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> Selecione a unidade compartilhada que contém o arquivo que você deseja copiar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione a pasta de destino para a qual deseja copiar o arquivo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do arquivo]</td> 
   <td> <p> Insira (mapa) a ID do arquivo que deseja copiar.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL O nome do arquivo de cópia]</p> </td> 
   <td> <p>Insira o novo nome de arquivo se desejar que ele seja alterado no local de destino.</p> </td> 
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
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Team Drive] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do arquivo]</td> 
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
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Team Drive] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do arquivo]</td> 
   <td> <p> Insira ou mapeie a ID do arquivo que deseja mover para a lixeira.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um arquivo]

Recupera detalhes sobre o arquivo especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Team Drive] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Documents] arquivos para formatar] </td> 
   <td> <p>Selecione o formato no qual deseja [!DNL Google Documents] arquivos convertidos em.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Sheets] arquivos para formatar] </td> 
   <td> <p>Selecione o formato no qual deseja [!DNL Google Sheets] arquivos convertidos em.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Slides] arquivos para formatar] </td> 
   <td> <p>Selecione o formato no qual deseja [!DNL Google Slides] arquivos convertidos em.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Drawings] arquivos para formatar] </td> 
   <td> <p>Selecione o formato no qual deseja [!DNL Google Drawings] arquivos convertidos em.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do arquivo]</td> 
   <td> <p> Insira ou mapeie a ID do arquivo que deseja recuperar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter uma lista de arquivos]

Recupera detalhes de arquivos e/ou pastas com base no termo de pesquisa.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Team Drive] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> Selecione a unidade compartilhada da qual deseja listar os arquivos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione a pasta da qual deseja listar arquivos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>Selecione o tipo de pesquisa que deseja realizar - veja abaixo.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Consulta]</p> </td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>[!UICONTROL Pesquisar em nomes de arquivo]</p> <p style="font-weight: normal;">Insira o nome do arquivo (incluindo a extensão de arquivo) quando a opção [!UICONTROL Pesquisar por pesquisa de termo exato] estiver selecionada ou insira a parte do nome quando a opção [!UICONTROL Pesquisar por nomes que contenham o termo pesquisado] estiver selecionada.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Pesquisa de texto completo]</p> <p>Insira o termo de pesquisa para pesquisar pelos nomes, descrições e conteúdos dos arquivos.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Consulta de pesquisa personalizada]</p> <p>Insira o [!DNL Google] pesquisar termo de consulta. Para obter mais detalhes, consulte [!DNL Google]'s <a href="https://developers.google.com/drive/api/v2/ref-search-terms">Documentação da Consulta de Pesquisa</a>. Exemplo: <code>fullText contains '"Hello world"'</code></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recuperar]</td> 
   <td>Selecione se deseja recuperar arquivos, pasta ou ambos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de resultados retornados]</td> 
   <td> <p> Definir o número máximo de arquivos ou pastas [!DNL Workfront Fusion] retornará durante um ciclo de execução.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar uma pasta]

Cria uma nova pasta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Team Drive] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
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
