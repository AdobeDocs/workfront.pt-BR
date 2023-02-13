---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos da unidade Google
description: O [!DNL Adobe Workfront Fusion Google Drive] os módulos permitem monitorar, pesquisar, criar, atualizar, excluir e gerenciar os arquivos, as pastas ou as unidades compartilhadas em seu [!DNL Google Drive].
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d620c93-d1bf-4451-9f76-1d6fd850cec9
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2908'
ht-degree: 0%

---

# [!DNL Google Drive] módulos

O [!DNL Adobe Workfront Fusion] [!DNL Google Drive] os módulos permitem monitorar, pesquisar, criar, atualizar, excluir e gerenciar os arquivos, as pastas ou as unidades compartilhadas em seu [!DNL Google Drive].

Em um [!DNL Adobe Workfront Fusion] você pode conectar seu [!DNL Google Drive] para vários aplicativos e serviços de terceiros.

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



## Conexão [!DNL Google Drive] para [!DNL Workfront Fusion]

Se você [!DNL @gmail.com] ou [!DNL @googlemail.com] usuário, é necessário criar um cliente OAuth em [o [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) a fim de obter [!UICONTROL ID do cliente] e [!UICONTROL Segredo do cliente].

Para obter instruções passo a passo sobre como criar o cliente OAuth (e obter [!UICONTROL ID do cliente] e [!UICONTROL Segredo do cliente]), consulte [Connect [!DNL Adobe Workfront Fusion] para [!DNL Google Services] usando um cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Para obter instruções sobre como conectar seu [!DNL Google Drive] para [!UICONTROL Workfront Fusion], consulte [Criar uma conexão com [!UICONTROL Adobe Workfront Fusion] - Instruções básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Google Drive] módulos e seus campos

Ao configurar [!DNL Google Drive] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Google Drive] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)



* [Triggers](#triggers)
* [Ações](#actions)

### Triggers

* [[!UICONTROL Assistir Arquivos Na Pasta]](#watch-files-in-folder)
* [[!UICONTROL Ver todos os arquivos]](#watch-all-files)
* [[!UICONTROL Assista a arquivos compartilhados]](#watch-shared-files)
* [[!UICONTROL Observar comentários]](#watch-comments)

#### [!UICONTROL Assistir Arquivos Na Pasta]

Recupera detalhes do arquivo quando um arquivo é adicionado ou modificado na pasta especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection] </td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Drive] para [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conexão [!DNL Google Drive] para [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Selecionar a pasta a ser assistida]</td>
    <td >Selecione a pasta na sua unidade em que deseja assistir aos arquivos.</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL Quais arquivos devem ser monitorados]</td>
   <td> <p>Selecione o tipo de arquivos que deseja visualizar.</p> 
    <ul> 
     <li>[!UICONTROL Tudo]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL Converter [!DNL Google Documents] arquivos para formatar]</td>
    <td>Selecione o formato de arquivo que deseja converter [!DNL Google Documents] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converter [!DNL Google Spreadsheets] arquivos para formatar]</td>
    <td>Selecione o formato de arquivo que deseja converter [!DNL Google Spreadsheets] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converter [!DNL Google Slides] arquivos para formatar]</td>
    <td>Selecione o formato de arquivo que deseja converter [!DNL Google Slides] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converter [!DNL Google Drawings] arquivos para formatar]</td>
    <td>Selecione o formato de arquivo que deseja converter [!DNL Google Drawings] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Watch]</td>
    <td>Selecione se deseja ver novos arquivos e todas as alterações ou apenas novos arquivos.</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL Número máximo de arquivos baixados]</td>
    <td>Defina o número máximo de resultados que [!DNL Workfront Fusion] será baixado durante um ciclo (o número de repetições por execução de cenário).</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ver todos os arquivos]

Recupera detalhes do arquivo quando um arquivo em seu [!DNL Google Drive] é adicionado ou modificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Drive] para [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conexão [!DNL Google Drive] para [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Quais arquivos devem ser monitorados]</td> 
   <td> <p>Selecione o tipo de arquivos que deseja visualizar.</p> 
    <ul> 
     <li>[!UICONTROL Tudo]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL Converter [!DNL Google Documents] arquivos para formatar]</td>
    <td>Selecione o formato de arquivo que deseja converter [!DNL Google Documents] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converter [!DNL Google Spreadsheets] arquivos para formatar]</td>
    <td>Selecione o formato de arquivo que deseja converter [!DNL Google Spreadsheets] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converter [!DNL Google Slides] arquivos para formatar]</td>
    <td>Selecione o formato de arquivo que deseja converter [!DNL Google Slides] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converter [!DNL Google Drawings] arquivos para formatar]</td>
    <td>Selecione o formato de arquivo que deseja converter [!DNL Google Drawings] a.</td>
  </tr>  
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>Selecione se deseja ver novos arquivos e todas as alterações ou apenas novos arquivos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de arquivos baixados]</td> 
   <td>Defina o número máximo de resultados que [!DNL Workfront Fusion] será baixado durante um ciclo (o número de repetições por execução de cenário).</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Assista a arquivos compartilhados]

Aciona quando um novo arquivo é compartilhado com você ou quando um arquivo compartilhado existente é atualizado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Drive] para [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conexão [!DNL Google Drive] para [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Selecionar a pasta a ser assistida]</td> 
   <td>Selecione a pasta compartilhada na qual deseja assistir aos arquivos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Quais arquivos devem ser monitorados]</td> 
   <td> <p>Selecione o tipo de arquivos que deseja visualizar.</p> 
    <ul> 
     <li>[!UICONTROL Tudo]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL Converter [!DNL Google Documents] arquivos para formatar]</td>
    <td>Selecione o formato de arquivo que deseja converter [!DNL Google Documents] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converter [!DNL Google Spreadsheets] arquivos para formatar]</td>
    <td>Selecione o formato de arquivo que deseja converter [!DNL Google Spreadsheets] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converter [!DNL Google Slides] arquivos para formatar]</td>
    <td>Selecione o formato de arquivo que deseja converter [!DNL Google Slides] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converter [!DNL Google Drawings] arquivos para formatar]</td>
    <td>Selecione o formato de arquivo que deseja converter [!DNL Google Drawings] a.</td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>Selecione se deseja ver novos arquivos e todas as alterações ou apenas novos arquivos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de arquivos baixados]</td> 
   <td>Defina o número máximo de resultados que [!DNL Workfront Fusion] será baixado durante um ciclo (o número de repetições por execução de cenário).</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Observar comentários]

Dispara quando um comentário é adicionado ou modificado no arquivo selecionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Drive] para [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conexão [!DNL Google Drive] para [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arquivo]</td> 
   <td>Selecione o arquivo que deseja visualizar para comentários.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>Selecione se deseja monitorar todas as alterações ou somente novos comentários</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de comentários retornados]</td> 
   <td>Defina o número máximo de comentários que [!DNL Workfront Fusion] retornará durante um ciclo (o número de repetições por execução de cenário).</td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [[!UICONTROL Fazer upload de um arquivo]](#upload-a-file)
* [[!UICONTROL Atualizar um arquivo]](#update-a-file)
* [[!UICONTROL Copiar um arquivo]](#copy-a-file)
* [[!UICONTROL Excluir um arquivo]](#delete-a-file)
* [[!UICONTROL Mover um arquivo/pasta para a lixeira]](#move-a-filefolder-to-trash)
* [[!UICONTROL Obter um arquivo]](#get-a-file)
* [[!UICONTROL Procurar Ficheiros/Pastas]](#search-for-filesfolders)
* [[!UICONTROL Criar uma pasta]](#create-a-folder)
* [[!UICONTROL Obter um link de compartilhamento]](#get-a-share-link)

#### [!UICONTROL Fazer upload de um arquivo]

Carrega um arquivo para seu [!DNL Google Drive].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Drive] para [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conexão [!DNL Google Drive] para [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Destination]</td> 
   <td> <p>Selecione o destino para o qual deseja fazer upload de um arquivo.</p> 
    <ul> 
     <li>[!DNL My Drive]</li> 
     <li>[!DNL Shared with Me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta de destino]</td> 
   <td>Selecione a pasta para a qual deseja carregar um arquivo. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arquivo de origem]</td> 
   <td>Selecione se deseja usar um arquivo passado de um módulo anterior ou se deseja mapear o arquivo manualmente.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome do arquivo]</td> 
   <td>Selecione o nome do arquivo. Essa opção estará disponível se você selecionar "[!UICONTROL Map]" no campo [!UICONTROL arquivo de origem].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dados]</td> 
   <td>Selecione o arquivo de dados que deseja fazer upload. Essa opção estará disponível se você selecionar "[!UICONTROL Map]" no campo [!UICONTROL arquivo de origem].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Título]</td> 
   <td>Insira um título para o novo arquivo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter um arquivo]</td> 
   <td>Habilitar essa opção permite que o módulo converta arquivos para o [!DNL Google] formato.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar um arquivo]

Atualiza os metadados ou o conteúdo de um arquivo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Drive] para [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conexão [!DNL Google Drive] para [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destino]</td> 
   <td> <p>Selecione o destino para o qual deseja fazer upload de um arquivo.</p> 
    <ul> 
     <li>[!UICONTROL Minha unidade]</li> 
     <li>[!UICONTROL Compartilhado comigo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mover para uma pasta]</td> 
   <td>Para mover o arquivo para uma pasta diferente, selecione a pasta para a qual deseja mover o arquivo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do arquivo]</td> 
   <td>Mapeie a ID do arquivo que deseja atualizar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Título]</td> 
   <td>Insira um título para o arquivo atualizado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Alterar o conteúdo de um arquivo]</td> 
   <td>Selecione se deseja substituir o conteúdo do arquivo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arquivo de origem]</td> 
   <td>Selecione se deseja usar um arquivo passado de um módulo anterior ou se deseja mapear o arquivo manualmente. Este campo estará disponível se você tiver selecionado para alterar o conteúdo do arquivo no campo anterior.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome do arquivo]</td> 
   <td>Selecione o nome do arquivo. Essa opção estará disponível se você selecionar "[!UICONTROL Map]" no campo [!UICONTROL arquivo de origem].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dados]</td> 
   <td>Selecione o arquivo de dados que deseja fazer upload. Essa opção estará disponível se você selecionar "[!UICONTROL Map]" no campo [!UICONTROL arquivo de origem].</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiar um arquivo]

Copia um arquivo para o novo local.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Drive] para [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conexão [!DNL Google Drive] para [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destino]</td> 
   <td> <p>Selecione o destino para o qual deseja fazer upload de um arquivo.</p> 
    <ul> 
     <li>[!UICONTROL Minha unidade]</li> 
     <li>[!UICONTROL Compartilhado comigo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta de destino]</td> 
   <td>Selecione a pasta onde o arquivo que deseja copiar está localizado/</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do arquivo]</td> 
   <td>Mapeie a ID do arquivo que deseja atualizar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL O nome da cópia]</td> 
   <td>Insira um título para o novo arquivo. Deixe esse campo em branco caso não queira alterar o nome do arquivo original.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir um arquivo]

Exclui permanentemente um arquivo ou pasta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Drive] para [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conexão [!DNL Google Drive] para [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do arquivo]</td> 
   <td>Mapeie a ID do arquivo que deseja excluir.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover um arquivo/pasta para a lixeira]

Move um arquivo ou pasta para a lixeira.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Drive] para [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conexão [!DNL Google Drive] para [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do arquivo]</td> 
   <td>Mapeie a ID do arquivo que deseja mover para a lixeira.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um arquivo]

Recupera o arquivo com a ID especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Drive] para [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conexão [!DNL Google Drive] para [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Documents] arquivos para formatar]</td> 
   <td>Selecione o formato de arquivo que deseja converter [!DNL Google Documents] a.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Spreadsheets] arquivos para formatar]</td> 
   <td>Selecione o formato de arquivo que deseja converter [!DNL Google Spreadsheets] a.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Slides] arquivos para formatar]</td> 
   <td>Selecione o formato de arquivo que deseja converter [!DNL Google Slides] a.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Drawings] arquivos para formatar]</td> 
   <td>Selecione o formato de arquivo que deseja converter [!DNL Google Drawings] a.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do arquivo]</td> 
   <td>Mapeie a ID do arquivo que deseja recuperar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Procurar Ficheiros/Pastas]

Pesquisa por arquivos ou pastas com base em critérios de pesquisa.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Drive] para [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conexão [!DNL Google Drive] para [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destino]</td> 
   <td> <p>Selecione o destino que deseja pesquisar.</p> 
    <ul> 
     <li>[!UICONTROL Minha unidade]</li> 
     <li>[!UICONTROL Compartilhado comigo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lista uma pasta]</td> 
   <td>Navegue até a pasta que deseja pesquisar pelos arquivos ou pastas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recuperar]</td> 
   <td> <p> Selecione se deseja pesquisar por arquivos, pastas ou ambos.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Search]</p> </td> 
   <td> <p>Selecione o tipo de pesquisa que deseja realizar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Pesquisar em nomes de arquivo/pasta]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Consulta]</strong> </p> <p>Insira uma parte do nome do arquivo ou o nome completo do arquivo (incluindo o sufixo) que você deseja pesquisar.</p> </li> 
       <li> <p><strong>[!UICONTROL Opções de pesquisa]</strong> </p> <p>Selecione se deseja pesquisar o termo exato ou se deseja pesquisar nomes que contenham o termo de pesquisa.</p> </li> 
      </ul> </li> 
     <li> <p><strong>Pesquisa de [!UICONTROL Texto completo]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Consulta]</strong> </p> <p>Insira qualquer termo de pesquisa que você deseja pesquisar em sua [!DNL Google Drive].</p> </li> 
      </ul> </li> 
     <li> <p><strong>Inserir consulta de pesquisa personalizada</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Consulta]</strong> </p> <p>Insira a consulta de pesquisa personalizada. Para obter mais detalhes, consulte a seção [!UICONTROL Pesquisar arquivos] deste artigo.</p> </li> 
       <li> <p><strong>Adicionar a pasta selecionada acima à consulta</strong> </p> <p>Pesquisa a pasta na coleção pai. Isso localiza todos os arquivos e pastas localizados diretamente na pasta selecionada acima.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de resultados retornados]</td> 
   <td>Definir o número máximo de arquivos ou pastas [!DNL Workfront Fusion] retornará durante um ciclo de execução.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continuar a execução da rota mesmo se o módulo não retornar nenhum resultado]</td> 
   <td>Ative essa opção para garantir que o cenário não seja interrompido se o módulo não retornar resultados.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar uma pasta]

Cria uma pasta no local especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Drive] para [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conexão [!DNL Google Drive] para [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destino]</td> 
   <td> <p>Selecione o destino para o qual deseja fazer upload de um arquivo.</p> 
    <ul> 
     <li>[!UICONTROL Minha unidade]</li> 
     <li>[!UICONTROL Compartilhado comigo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Novo local da pasta]</td> 
   <td>Navegue até o local onde deseja criar uma nova pasta.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL O nome da nova pasta]</td> 
   <td>Insira um nome para a pasta que você está criando.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Compartilhar pasta]</td> 
   <td>Selecione esta opção se quiser compartilhar a pasta com qualquer pessoa com o link [!UICONTROL Compartilhar]. Caso contrário, o link de compartilhamento será somente para o proprietário.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um link de compartilhamento]

Recupera o link de compartilhamento de um arquivo na unidade Google.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Drive] para [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conexão [!DNL Google Drive] para [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do arquivo]</td> 
   <td>Mapeie a ID do arquivo para o qual você deseja obter o link de compartilhamento.</td> 
  </tr> 
 </tbody> 
</table>

## Solução de problemas

### Não é possível carregar ou atualizar um arquivo

Há várias situações em que o upload ou a atualização de um arquivo falha:

* O arquivo carregado é muito grande e excede o limite máximo de tamanho de arquivo permitido para sua [!DNL Google Drive] ou você excedeu seu [!DNL Google Drive] limite de armazenamento. Você pode atualizar seu plano de armazenamento ou excluir arquivos existentes do [!DNL Google Drive] serviço.
* A pasta selecionada na qual o arquivo deveria ser carregado não existe mais. O cenário é interrompido e é necessário selecionar uma pasta de destino novamente.

## Procurar ficheiros

No módulo Lista arquivos em uma pasta, você pode usar sua própria query que consiste nessas partes:

* **[!UICONTROL Campo]** - Atributo do arquivo que está sendo pesquisado, por exemplo, o atributo `name` do arquivo.

* **[!UICONTROL Operador]** - Teste que é executado nos dados para fornecer uma correspondência, por exemplo, `contains`.

* **[!UICONTROL Valor]** - O conteúdo do atributo testado, por exemplo, o nome do arquivo `My cool document`.

Combinar cláusulas com as conjunções `and` ou `or`e negar a consulta com `not`.

* [Campos](#fields)
* [Tipos de valor](#value-types)
* [Operadores](#operators)
* [Exemplos](#examples)

### Campos

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Campo </th> 
   <th>Tipo de valor </th> 
   <th>Operadores</th> 
   <th> <p> Descrição</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>[!UICONTROL title]</code></td> 
   <td>string</td> 
   <td><code>contains</code><sup>1</sup>, <code>=</code>, <code>!=</code></td> 
   <td> <p> Nome do arquivo.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL fullText]</code> </td> 
   <td>string </td> 
   <td><code>contains</code><sup>2, 3</sup> </td> 
   <td> <p> Texto completo do arquivo, incluindo nome, descrição, conteúdo e texto indexável.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL mimeType]</code> </td> 
   <td> string</td> 
   <td><code>contains</code>, <code>=</code>, <code>!=</code></td> 
   <td> <p> Tipo MIME do arquivo.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL modifiedDate]</code> </td> 
   <td> data<sup>4</sup></td> 
   <td><code> &lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>></code>, <code>>=</code></td> 
   <td> <p> Data da última modificação do arquivo.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL lastViewedByMeDate]</code> </td> 
   <td> data<sup>4</sup></td> 
   <td><code>&lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>></code>, <code>>=</code></td> 
   <td> <p> Data em que o usuário visualizou um arquivo pela última vez.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL trashed]</code></td> 
   <td>booleano </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p> Se o arquivo está na lixeira ou não.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL starred]</code></td> 
   <td>booleano </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p>Se o arquivo é iniciado ou não.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL parents]</code></td> 
   <td>coleção </td> 
   <td><code>in </code> </td> 
   <td> <p>Se a coleção [!UICONTROL pais] contém a ID especificada.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL owners]</code></td> 
   <td>coleção </td> 
   <td><code>in </code> </td> 
   <td> <p>Usuários que são proprietários do arquivo.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL writers]</code></td> 
   <td>coleção </td> 
   <td><code>in </code> </td> 
   <td> <p>Usuários que têm permissão para modificar o arquivo.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL readers] </code> </td> 
   <td>coleção </td> 
   <td><code>in </code> </td> 
   <td> <p>Usuários que têm permissão para ler o arquivo.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL sharedWithMe]</code> </td> 
   <td>booleano </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p> Arquivos que estão na coleção "Compartilhado comigo" do usuário.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL properties] </code> </td> 
   <td>coleção</td> 
   <td><code>has </code> </td> 
   <td> <p> Propriedades de arquivo personalizado público.</p> </td> 
  </tr> 
 </tbody> 
</table>

Considere o seguinte sobre os operadores nesses campos:

* O `contains` O operador só executa a correspondência de prefixos para um `title`.

   Por exemplo, o título &quot;HelloWorld&quot; corresponde a `title contains 'Hello'` mas não para `title contains 'World'`.

* O `contains` O operador só executa a correspondência em tokens de cadeia de caracteres inteiros para `fullText`.

   Por exemplo, se o texto completo de um documento contiver a string &quot;HelloWorld&quot; somente a query `fullText contains 'HelloWorld'` retorna um resultado. Queries como `fullText contains 'Hello'` não retornaria resultados neste cenário.

* O `contains` corresponde a uma frase alfanumérica exata se estiver entre aspas duplas.

   Por exemplo, se a variável `fullText` de um documento contém a string &quot;Olá lá mundo&quot;, em seguida o query `fullText contains '"Hello there"'` retorna um resultado, mas a query `fullText contains '"Hello world"'` não.

   Além disso, como a pesquisa é alfanumérica, se a variável `fullText` de um documento contém a string &quot;Hello_world&quot;, então o query `fullText contains '"Hello world"'` retorna um resultado.

* Campos de `type` no momento, as datas não são comparáveis umas às outras, apenas a datas constantes.

### Tipos de valor

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de valor</th> 
   <th> <p> Notas</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>String </td> 
   <td> <p>Marque com aspas simples '. Evitar aspas simples em queries com <code>\'</code>, por exemplo,<code> 'Valentine\'s Day'</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Booleano </td> 
   <td> <p><code>true </code>ou <code>false</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Data </td> 
   <td> <p>Formato RFC 3339, o fuso horário padrão é UTC, por exemplo, <code>2012-06-04T12:00:00-08:00</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Operadores

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Operador </th> 
   <th> <p>Notas</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>contains</code></td> 
   <td> <p>O conteúdo de uma string está presente na outra.</p> </td> 
  </tr> 
  <tr> 
   <td><code>=</code> </td> 
   <td> <p> O conteúdo de uma string ou booleano é igual ao outro.</p> </td> 
  </tr> 
  <tr> 
   <td><code>!=</code> </td> 
   <td> <p> O conteúdo de uma string ou booleano não é igual ao outro.</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;</code> </td> 
   <td> <p> Uma data é anterior a outra.</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;=</code> </td> 
   <td> <p> Uma data é anterior ou igual a outra.</p> </td> 
  </tr> 
  <tr> 
   <td><code>></code> </td> 
   <td> <p> Uma data é posterior a outra.</p> </td> 
  </tr> 
  <tr> 
   <td><code>>=</code> </td> 
   <td> <p> Uma data é posterior ou igual a outra.</p> </td> 
  </tr> 
  <tr> 
   <td><code>in </code> </td> 
   <td> <p>Um elemento está contido em uma coleção.</p> </td> 
  </tr> 
  <tr> 
   <td><code>and </code> </td> 
   <td> <p>Retorna arquivos que correspondem a ambas as cláusulas.</p> </td> 
  </tr> 
  <tr> 
   <td><code>or </code> </td> 
   <td> <p>Retorna arquivos que correspondem a qualquer cláusula.</p> </td> 
  </tr> 
  <tr> 
   <td><code>not </code> </td> 
   <td> <p>Nega uma cláusula de pesquisa.</p> </td> 
  </tr> 
  <tr> 
   <td><code>has </code> </td> 
   <td> <p>Uma coleção contém um elemento correspondente aos parâmetros.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para cláusulas compostas, você pode usar parênteses para agrupar cláusulas. Por exemplo:
`modifiedDate > '2012-06-04T12:00:00' and (mimeType contains 'image/' or mimeType contains 'video/')` Essa pesquisa retorna todos os arquivos com um tipo MIME de imagem ou vídeo que tiveram sua última modificação depois de 4 de junho de 2012. Porque `and` e `or` Os operadores são avaliados da esquerda para a direita, sem parênteses, o exemplo acima retornaria somente imagens modificadas após 4 de junho de 2012, mas retornaria todos os vídeos, mesmo aqueles antes de 4 de junho de 2012.

### Exemplos

Todos os exemplos nesta página mostram os não codificados `<q>q</q>` , onde `title = 'hello'` é codificado como `title+%3d+%27hello%27`. As bibliotecas de clientes lidam com essa codificação automaticamente.

* Procure arquivos com o nome &quot;hello&quot;

   <pre>title = 'hello'</pre>
* Pesquise por pastas usando o tipo MIME específico da pasta

   <pre>mimeType = 'application/vnd.google-apps.folder'</pre>
* Procurar ficheiros que não sejam pastas

   <pre>mimeType != 'application/vnd.google-apps.folder'</pre>
* Procure por arquivos com um nome contendo as palavras &quot;hello&quot; e &quot;goodbye&quot;

   <pre>título contém 'hello' e [!UICONTROL name] contém 'goodbye'</pre>
* Procure por arquivos com um nome que não contenha a palavra &quot;Olá&quot;

   <pre>não título contém 'hello'</pre>
* Procure por arquivos que contenham a palavra &quot;hello&quot; no conteúdo

   <pre>fullText contém 'hello'</pre>
* Procure arquivos que não contenham a palavra &quot;hello&quot; no conteúdo

   <pre>not fullText contém 'hello'</pre>
* Pesquise por arquivos que contenham a frase exata &quot;mundo da saudação&quot; no conteúdo

   <pre>fullText contém '"hello world"'fullText contém '"hello_world"'</pre>
* Procure por arquivos com uma consulta contendo o caractere &quot;\&quot; (por exemplo, &quot;\authors&quot;)

   <pre>fullText contém '\\authors'</pre>
* Procure arquivos graváveis pelo usuário &quot;test@example.org&quot;

   <pre>'test@example.org' em [!DNL writers]</pre>
* Pesquisar a ID `1234567` no `parents` coleção. Isso localiza todos os arquivos e pastas localizados diretamente na pasta cuja ID é `1234567`.

   <pre>'1234567' em [!UICONTROL pais]</pre>
* Procure pela ID de alias `appDataFolder` no `parents` coleção. Isso localiza todos os arquivos e pastas localizados diretamente no [Pasta Dados do aplicativo](https://developers.google.com/drive/api/v2/appdata).

   <pre>'appDataFolder' nos pais</pre>
* Procure arquivos graváveis pelos usuários &quot;test@example.org&quot; e &quot;test2@example.org&quot;

   <pre>'test@example.org' em escritores e 'test2@example.org' em escritores</pre>
* Procure por arquivos que contenham o texto &quot;importante&quot; que estejam na lixeira

   <pre>fullText contém 'important' e lixeira = true</pre>
* Pesquisar arquivos modificados após 4 de junho de 2012

   <pre>modifiedDate &gt; '2012-06-04T12:00:00' // o fuso horário padrão é UTC</pre><pre>modifiedDate &gt; '2012-06-04T12:00:00-08:00'</pre>
* Procure arquivos compartilhados com o usuário autorizado com &quot;hello&quot; no nome

   <pre>sharedWithMe e title contém 'hello'</pre>
* Procure por arquivos com uma [propriedade de arquivo personalizado](https://developers.google.com/drive/api/v2/properties) nomeado `additionalID` com o valor `8e8aceg2af2ge72e78`.

   <pre>As propriedades têm { key='additionalID' e value='8e8aceg2af2ge72e78' e visibility='PRIVATE' }</pre>

A fonte deste guia é [[!DNL Google Drive] documentação](https://developers.google.com/drive/api/v2/search-shareddrives).
