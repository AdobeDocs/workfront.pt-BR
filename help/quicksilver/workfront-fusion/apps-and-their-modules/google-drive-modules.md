---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de drive Google
description: Os  [!DNL Adobe Workfront Fusion Google Drive] módulos permitem que você monitore, pesquise, crie, atualize, exclua e gerencie seus arquivos, pastas ou unidades compartilhadas em seu  [!DNL Google Drive].
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d620c93-d1bf-4451-9f76-1d6fd850cec9
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2941'
ht-degree: 0%

---

# [!DNL Google Drive] módulos

Os módulos do [!DNL Adobe Workfront Fusion] [!DNL Google Drive] permitem que você monitore, pesquise, crie, atualize, exclua e gerencie seus arquivos, pastas ou unidades compartilhadas no [!DNL Google Drive].

Em um cenário do [!DNL Adobe Workfront Fusion], você pode conectar sua conta do [!DNL Google Drive] a vários aplicativos e serviços de terceiros.

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
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).



## Conectando [!DNL Google Drive] a [!DNL Workfront Fusion]

Se você for [!DNL @gmail.com] ou [!DNL @googlemail.com] usuário, precisará criar um cliente OAuth em [the [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) para obter a [!UICONTROL ID do Cliente] e o [!UICONTROL Segredo do Cliente].

Para obter instruções passo a passo sobre como criar o cliente OAuth (e obter a [!UICONTROL ID do Cliente] e o [!UICONTROL Segredo do Cliente]), consulte [Conectar [!DNL Adobe Workfront Fusion] a [!DNL Google Services] usando um cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Para obter instruções sobre como conectar sua conta do [!DNL Google Drive] ao [!UICONTROL Workfront Fusion], consulte [Criar uma conexão com o [!UICONTROL Adobe Workfront Fusion] - Instruções básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Google Drive] módulos e seus campos

Ao configurar módulos do [!DNL Google Drive], o [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos [!DNL Google Drive] adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)



* [Triggers](#triggers)
* [Ações](#actions)

### Triggers

* [[!UICONTROL Observar Arquivos Na Pasta]](#watch-files-in-folder)
* [[!UICONTROL Assistir a Todos os Arquivos]](#watch-all-files)
* [[!UICONTROL Observar arquivos compartilhados]](#watch-shared-files)
* [[!UICONTROL Assistir Comentários]](#watch-comments)

#### [!UICONTROL Observar Arquivos Na Pasta]

Recupera detalhes do arquivo quando ele é adicionado ou modificado na pasta especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Conexão] </td>
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Drive] ao [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conectando o [!DNL Google Drive] ao [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Selecionar a pasta a ser observada]</td>
    <td >Selecione a pasta na unidade em que deseja observar os arquivos.</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL Quais arquivos observar]</td>
   <td> <p>Selecione o tipo de arquivo que deseja observar.</p> 
    <ul> 
     <li>[!UICONTROL Tudo]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL Converter [!DNL Google Documents] arquivos no formato]</td>
    <td>Selecione o formato de arquivo para o qual você deseja converter [!DNL Google Documents].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converter [!DNL Google Spreadsheets] arquivos no formato]</td>
    <td>Selecione o formato de arquivo para o qual você deseja converter [!DNL Google Spreadsheets].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converter [!DNL Google Slides] arquivos no formato]</td>
    <td>Selecione o formato de arquivo para o qual você deseja converter [!DNL Google Slides].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converter [!DNL Google Drawings] arquivos no formato]</td>
    <td>Selecione o formato de arquivo para o qual você deseja converter [!DNL Google Drawings].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Observar]</td>
    <td>Selecione se deseja observar novos arquivos e todas as alterações ou somente novos arquivos.</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL Número máximo de arquivos baixados]</td>
    <td>Defina o número máximo de resultados que [!DNL Workfront Fusion] baixará durante um ciclo (o número de repetições por execução de cenário).</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Assistir a Todos os Arquivos]

Recupera detalhes do arquivo quando um arquivo em seu [!DNL Google Drive] é adicionado ou modificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Drive] ao [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conectando o [!DNL Google Drive] ao [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Quais arquivos observar]</td> 
   <td> <p>Selecione o tipo de arquivo que deseja observar.</p> 
    <ul> 
     <li>[!UICONTROL Tudo]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL Converter [!DNL Google Documents] arquivos no formato]</td>
    <td>Selecione o formato de arquivo para o qual você deseja converter [!DNL Google Documents].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converter [!DNL Google Spreadsheets] arquivos no formato]</td>
    <td>Selecione o formato de arquivo para o qual você deseja converter [!DNL Google Spreadsheets].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converter [!DNL Google Slides] arquivos no formato]</td>
    <td>Selecione o formato de arquivo para o qual você deseja converter [!DNL Google Slides].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converter [!DNL Google Drawings] arquivos no formato]</td>
    <td>Selecione o formato de arquivo para o qual você deseja converter [!DNL Google Drawings].</td>
  </tr>  
  <tr> 
   <td>[!UICONTROL Observar]</td> 
   <td>Selecione se deseja observar novos arquivos e todas as alterações ou somente novos arquivos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de arquivos baixados]</td> 
   <td>Defina o número máximo de resultados que [!DNL Workfront Fusion] baixará durante um ciclo (o número de repetições por execução de cenário).</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Observar arquivos compartilhados]

Dispara quando um novo arquivo é compartilhado com você ou um arquivo compartilhado existente é atualizado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Drive] ao [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conectando o [!DNL Google Drive] ao [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Selecionar a pasta a ser observada]</td> 
   <td>Selecione a pasta compartilhada na qual você deseja observar os arquivos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Quais arquivos observar]</td> 
   <td> <p>Selecione o tipo de arquivo que deseja observar.</p> 
    <ul> 
     <li>[!UICONTROL Tudo]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL Converter [!DNL Google Documents] arquivos no formato]</td>
    <td>Selecione o formato de arquivo para o qual você deseja converter [!DNL Google Documents].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converter [!DNL Google Spreadsheets] arquivos no formato]</td>
    <td>Selecione o formato de arquivo para o qual você deseja converter [!DNL Google Spreadsheets].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converter [!DNL Google Slides] arquivos no formato]</td>
    <td>Selecione o formato de arquivo para o qual você deseja converter [!DNL Google Slides].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converter [!DNL Google Drawings] arquivos no formato]</td>
    <td>Selecione o formato de arquivo para o qual você deseja converter [!DNL Google Drawings].</td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Observar]</td> 
   <td>Selecione se deseja observar novos arquivos e todas as alterações ou somente novos arquivos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de arquivos baixados]</td> 
   <td>Defina o número máximo de resultados que [!DNL Workfront Fusion] baixará durante um ciclo (o número de repetições por execução de cenário).</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Assistir Comentários]

Aciona quando um comentário é adicionado ou modificado no arquivo selecionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Drive] ao [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conectando o [!DNL Google Drive] ao [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arquivo]</td> 
   <td>Selecione o arquivo que deseja observar para comentários.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Observar]</td> 
   <td>Selecione se você deseja observar todas as alterações ou somente os novos comentários</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de comentários retornados]</td> 
   <td>Defina o número máximo de comentários que [!DNL Workfront Fusion] retornará durante um ciclo (o número de repetições por execução de cenário).</td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [[!UICONTROL Carregar um arquivo]](#upload-a-file)
* [[!UICONTROL Atualizar um Arquivo]](#update-a-file)
* [[!UICONTROL Copiar um Arquivo]](#copy-a-file)
* [[!UICONTROL Excluir um arquivo]](#delete-a-file)
* [[!UICONTROL Mover um Arquivo/Pasta para a Lixeira]](#move-a-filefolder-to-trash)
* [[!UICONTROL Obter um arquivo]](#get-a-file)
* [[!UICONTROL Procurar Arquivos/Pastas]](#search-for-filesfolders)
* [[!UICONTROL Criar uma Pasta]](#create-a-folder)
* [[!UICONTROL Obter um link de compartilhamento]](#get-a-share-link)

#### [!UICONTROL Carregar um arquivo]

Carrega um arquivo no [!DNL Google Drive].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Drive] ao [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conectando o [!DNL Google Drive] ao [!UICONTROL Workfront Fusion]</a></p> </td> 
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
   <td>[!UICONTROL Pasta de Destino]</td> 
   <td>Selecione a pasta na qual deseja fazer upload de um arquivo. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL arquivo Source]</td> 
   <td>Selecione se deseja usar um arquivo passado de um módulo anterior ou se deseja mapear o arquivo manualmente.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome do arquivo]</td> 
   <td>Selecione o nome do arquivo. Essa opção estará disponível se você selecionar "[!UICONTROL Mapa]" no campo [!UICONTROL arquivo de origem].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dados]</td> 
   <td>Selecione o arquivo de dados que deseja fazer upload. Essa opção estará disponível se você selecionar "[!UICONTROL Mapa]" no campo [!UICONTROL arquivo de origem].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Título]</td> 
   <td>Insira um título para o novo arquivo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter um arquivo]</td> 
   <td>Habilitar essa opção permite que o módulo converta arquivos no formato [!DNL Google] correspondente.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar um Arquivo]

Atualiza os metadados ou conteúdo de um arquivo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Drive] ao [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conectando o [!DNL Google Drive] ao [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destino]</td> 
   <td> <p>Selecione o destino para o qual deseja fazer upload de um arquivo.</p> 
    <ul> 
     <li>[!UICONTROL Minha Unidade]</li> 
     <li>[!UICONTROL Compartilhado comigo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mover para uma pasta]</td> 
   <td>Se desejar mover o arquivo para uma pasta diferente, selecione a pasta para onde deseja mover o arquivo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Arquivo]</td> 
   <td>Mapeie a ID do arquivo que você deseja atualizar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Título]</td> 
   <td>Insira um título para o arquivo atualizado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Alterar um conteúdo de arquivo]</td> 
   <td>Selecione se deseja substituir o conteúdo do arquivo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL arquivo Source]</td> 
   <td>Selecione se deseja usar um arquivo passado de um módulo anterior ou se deseja mapear o arquivo manualmente. Este campo estará disponível se você tiver selecionado alterar o conteúdo do arquivo no campo anterior.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome do arquivo]</td> 
   <td>Selecione o nome do arquivo. Essa opção estará disponível se você selecionar "[!UICONTROL Mapa]" no campo [!UICONTROL arquivo de origem].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dados]</td> 
   <td>Selecione o arquivo de dados que deseja fazer upload. Essa opção estará disponível se você selecionar "[!UICONTROL Mapa]" no campo [!UICONTROL arquivo de origem].</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiar um Arquivo]

Copia um arquivo para o novo local.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Drive] ao [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conectando o [!DNL Google Drive] ao [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destino]</td> 
   <td> <p>Selecione o destino para o qual deseja fazer upload de um arquivo.</p> 
    <ul> 
     <li>[!UICONTROL Minha Unidade]</li> 
     <li>[!UICONTROL Compartilhado comigo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta de Destino]</td> 
   <td>Selecione a pasta onde o arquivo que deseja copiar está localizado/</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Arquivo]</td> 
   <td>Mapeie a ID do arquivo que você deseja atualizar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL O nome da cópia]</td> 
   <td>Insira um título para o novo arquivo. Deixe esse campo em branco se não quiser alterar o nome do arquivo original.</td> 
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
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Drive] ao [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conectando o [!DNL Google Drive] ao [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Arquivo]</td> 
   <td>Mapeie a ID do arquivo que deseja excluir.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover um Arquivo/Pasta para a Lixeira]

Move um arquivo ou pasta para o lixo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Drive] ao [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conectando o [!DNL Google Drive] ao [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Arquivo]</td> 
   <td>Mapeie a ID do arquivo que você deseja mover para a lixeira.</td> 
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
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Drive] ao [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conectando o [!DNL Google Drive] ao [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Documents] arquivos no formato]</td> 
   <td>Selecione o formato de arquivo para o qual você deseja converter [!DNL Google Documents].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Spreadsheets] arquivos no formato]</td> 
   <td>Selecione o formato de arquivo para o qual você deseja converter [!DNL Google Spreadsheets].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Slides] arquivos no formato]</td> 
   <td>Selecione o formato de arquivo para o qual você deseja converter [!DNL Google Slides].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Drawings] arquivos no formato]</td> 
   <td>Selecione o formato de arquivo para o qual você deseja converter [!DNL Google Drawings].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Arquivo]</td> 
   <td>Mapeie a ID do arquivo que você deseja recuperar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Procurar Arquivos/Pastas]

Pesquisa arquivos ou pastas com base nos critérios de pesquisa.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Drive] ao [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conectando o [!DNL Google Drive] ao [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destino]</td> 
   <td> <p>Selecione o destino que deseja pesquisar.</p> 
    <ul> 
     <li>[!UICONTROL Minha Unidade]</li> 
     <li>[!UICONTROL Compartilhado comigo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Listar uma pasta]</td> 
   <td>Navegue até a pasta na qual deseja pesquisar os arquivos ou pastas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recuperar]</td> 
   <td> <p> Selecione se deseja pesquisar arquivos, pastas ou ambos.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Pesquisar]</p> </td> 
   <td> <p>Selecione o tipo de pesquisa que deseja realizar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Pesquisar em nomes de arquivo/pasta]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Consulta]</strong> </p> <p>Insira uma parte do nome do arquivo ou o nome completo do arquivo (incluindo o sufixo) que deseja pesquisar.</p> </li> 
       <li> <p><strong>[!UICONTROL Opções de Pesquisa]</strong> </p> <p>Selecione se deseja pesquisar o termo exato ou se deseja pesquisar nomes contendo o termo de pesquisa.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Texto Completo] pesquisa</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Consulta]</strong> </p> <p>Digite qualquer termo de pesquisa que você deseja pesquisar em seu [!DNL Google Drive].</p> </li> 
      </ul> </li> 
     <li> <p><strong>Inserir consulta de pesquisa personalizada</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Consulta]</strong> </p> <p>Insira a consulta de pesquisa personalizada. Para obter mais detalhes, consulte a seção [!UICONTROL Pesquisar Arquivos] deste artigo.</p> </li> 
       <li> <p><strong>Adicionar a pasta selecionada acima à consulta</strong> </p> <p>Pesquisa a pasta na coleção pai. Isso encontrará todos os arquivos e pastas localizados diretamente na pasta selecionada acima.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de resultados retornados]</td> 
   <td>Defina o número máximo de arquivos ou pastas que [!DNL Workfront Fusion] retornará durante um ciclo de execução.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continuar a execução da rota mesmo se o módulo não retornar resultados]</td> 
   <td>Ative essa opção para garantir que o cenário não seja interrompido se o módulo não retornar resultados.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar uma Pasta]

Cria uma pasta no local especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Drive] ao [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conectando o [!DNL Google Drive] ao [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destino]</td> 
   <td> <p>Selecione o destino para o qual deseja fazer upload de um arquivo.</p> 
    <ul> 
     <li>[!UICONTROL Minha Unidade]</li> 
     <li>[!UICONTROL Compartilhado comigo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Novo local de pasta]</td> 
   <td>Navegue até o local onde deseja criar uma nova pasta.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL O nome da nova pasta]</td> 
   <td>Insira um nome para a pasta que está sendo criada.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Compartilhar pasta]</td> 
   <td>Selecione esta opção se desejar compartilhar a pasta com qualquer pessoa com o link [!UICONTROL Compartilhar]. Caso contrário, o link de compartilhamento será somente para o proprietário.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um link de compartilhamento]

Recupera o link de compartilhamento de um arquivo no Google Drive.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Drive] ao [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conectando o [!DNL Google Drive] ao [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Arquivo]</td> 
   <td>Mapeie a ID do arquivo para o qual você deseja obter o link de compartilhamento.</td> 
  </tr> 
 </tbody> 
</table>

## Solução de problemas

### Não é possível carregar ou atualizar um arquivo

Há várias situações em que ocorre uma falha no upload ou na atualização de um arquivo:

* O arquivo carregado é muito grande e excede o limite de tamanho máximo de arquivo permitido para o plano [!DNL Google Drive] ou você excedeu o limite de armazenamento de [!DNL Google Drive]. Você pode atualizar seu plano de armazenamento ou excluir arquivos existentes do serviço [!DNL Google Drive].
* A pasta selecionada para onde o arquivo deveria ser carregado não existe mais. O cenário é interrompido e, em seguida, é necessário selecionar uma pasta de destino novamente.

## Procurar arquivos

No módulo Listar arquivos em uma pasta, você pode usar sua própria consulta, que consiste nestas partes:

* **[!UICONTROL Campo]** - Atributo do arquivo que está sendo pesquisado, por exemplo, o atributo `name` do arquivo.

* **[!UICONTROL Operador]** - Teste executado nos dados para fornecer uma correspondência, por exemplo, `contains`.

* **[!UICONTROL Valor]** - O conteúdo do atributo testado, por exemplo, o nome do arquivo `My cool document`.

Combine cláusulas com as conjunções `and` ou `or` e negue a consulta com `not`.

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
   <td> <p> Texto completo do arquivo incluindo nome, descrição, conteúdo e texto indexável.</p> </td> 
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
   <td> <p> Data da última modificação no arquivo.</p> </td> 
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
   <td> <p> Se o arquivo está no lixo ou não.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL starred]</code></td> 
   <td>booleano </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p>Se o arquivo é estrelado ou não.</p> </td> 
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
   <td> <p>Usuários proprietários do arquivo.</p> </td> 
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
   <td> <p> Propriedades do arquivo personalizado público.</p> </td> 
  </tr> 
 </tbody> 
</table>

Considere o seguinte sobre operadores nestes campos:

* O operador `contains` executa apenas a correspondência de prefixos para `title`.

  Por exemplo, o título &quot;HelloWorld&quot; corresponde a `title contains 'Hello'`, mas não a `title contains 'World'`.

* O operador `contains` executa apenas a correspondência em tokens de cadeia de caracteres inteira para `fullText`.

  Por exemplo, se o texto completo de um documento contiver a cadeia de caracteres &quot;HelloWorld&quot;, somente a consulta `fullText contains 'HelloWorld'` retornará um resultado. Consultas como `fullText contains 'Hello'` não retornariam resultados neste cenário.

* O operador `contains` corresponde a uma frase alfanumérica exata se estiver entre aspas duplas.

  Por exemplo, se o `fullText` de um documento contiver a cadeia de caracteres &quot;Olá, mundo&quot;, a consulta `fullText contains '"Hello there"'` retornará um resultado, mas a consulta `fullText contains '"Hello world"'` não.

  Além disso, como a pesquisa é alfanumérica, se o `fullText` de um documento contiver a cadeia de caracteres &quot;Hello_world&quot;, a consulta `fullText contains '"Hello world"'` retornará um resultado.

* Atualmente, os campos de data `type` não são comparáveis entre si, apenas a datas constantes.

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
   <td> <p>Circundar com aspas simples '. Evitar aspas simples em consultas com <code>\'</code>, por exemplo, <code> 'Valentine\'s Day'</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Booleano </td> 
   <td> <p><code>true </code>ou <code>false</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Data </td> 
   <td> <p>Formato RFC 3339. O fuso horário padrão é UTC; por exemplo, <code>2012-06-04T12:00:00-08:00</code>.</p> </td> 
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
   <td> <p>O conteúdo de uma cadeia de caracteres está presente na outra.</p> </td> 
  </tr> 
  <tr> 
   <td><code>=</code> </td> 
   <td> <p> O conteúdo de uma string ou booleano é igual ao outro.</p> </td> 
  </tr> 
  <tr> 
   <td><code>!=</code> </td> 
   <td> <p> O conteúdo de uma cadeia de caracteres ou booleano não é igual ao outro.</p> </td> 
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
   <td> <p>Retorne arquivos que correspondam a ambas as cláusulas.</p> </td> 
  </tr> 
  <tr> 
   <td><code>or </code> </td> 
   <td> <p>Retorne arquivos que correspondam a qualquer uma das cláusulas.</p> </td> 
  </tr> 
  <tr> 
   <td><code>not </code> </td> 
   <td> <p>Nega uma cláusula de pesquisa.</p> </td> 
  </tr> 
  <tr> 
   <td><code>has </code> </td> 
   <td> <p>Uma coleção contém um elemento que corresponde aos parâmetros.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para cláusulas compostas, você pode usar parênteses para agrupar cláusulas. Por exemplo:
`modifiedDate > '2012-06-04T12:00:00' and (mimeType contains 'image/' or mimeType contains 'video/')` Esta pesquisa retorna todos os arquivos com um tipo MIME de imagem ou vídeo cuja última modificação foi após 4 de junho de 2012. Como os operadores `and` e `or` são avaliados da esquerda para a direita, sem parênteses, o exemplo acima retornaria somente imagens modificadas após 4 de junho de 2012, mas retornaria todos os vídeos, mesmo os anteriores a 4 de junho de 2012.

### Exemplos

Todos os exemplos nesta página mostram o parâmetro `<q>q</q>` não codificado, em que `title = 'hello'` está codificado como `title+%3d+%27hello%27`. As bibliotecas de clientes lidam com essa codificação automaticamente.

* Pesquisar arquivos com o nome &quot;Olá&quot;
  <pre>title = 'olá'</pre>
* Procurar pastas usando o tipo MIME específico da pasta
  <pre>mimeType = 'application/vnd.google-apps.folder'</pre>
* Procurar arquivos que não sejam pastas
  <pre>mimeType!= 'application/vnd.google-apps.folder'</pre>
* Procure arquivos com um nome contendo as palavras &quot;olá&quot; e &quot;adeus&quot;
  <pre>título contém 'olá' e [!UICONTROL name] contém 'adeus'</pre>
* Procure arquivos com um nome que não contenha a palavra &quot;olá&quot;
  <pre>não o título contém 'olá'</pre>
* Pesquisar arquivos que contenham a palavra &quot;olá&quot; no conteúdo
  <pre>fullText contém 'olá'</pre>
* Pesquisar arquivos que não contenham a palavra &quot;Olá&quot; no conteúdo
  <pre>não fullText contém 'hello'</pre>
* Procure arquivos que contenham a frase exata &quot;olá mundo&quot; no conteúdo
  <pre>fullText contém '"olá mundo"'fullText contém '"olá_mundo"'</pre>
* Procure arquivos com uma consulta que contenha o caractere &quot;\&quot; (por exemplo, &quot;\autores&quot;)
  <pre>fullText contém '\\autores'</pre>
* Procurar arquivos graváveis pelo usuário &quot;test@example.org&quot;
  <pre>'test@example.org' em [!DNL writers]</pre>
* Procure a ID `1234567` na coleção `parents`. Isso localiza todos os arquivos e pastas localizados diretamente na pasta cuja ID é `1234567`.
  <pre>'1234567' em [!UICONTROL pais]</pre>
* Procure a ID de alias `appDataFolder` na coleção `parents`. Isso localiza todos os arquivos e pastas localizados diretamente na [pasta Dados de Aplicativos](https://developers.google.com/drive/api/v2/appdata).
  <pre>'appDataFolder' nos pais</pre>
* Procurar arquivos graváveis pelos usuários &quot;test@example.org&quot; e &quot;test2@example.org&quot;
  <pre>'test@example.org' em escritores e 'test2@example.org' em escritores</pre>
* Procurar por arquivos contendo o texto &quot;importante&quot; que estejam na lixeira
  <pre>fullText contém 'important' e trash = true</pre>
* Procurar arquivos modificados após 4 de junho de 2012
  <pre>modifiedDate &gt; '2012-06-04T12:00:00' // o fuso horário padrão é UTC</pre><pre>modifiedDate &gt; '06-04T12:00:00-08:00'</pre>
* Procure arquivos compartilhados com o usuário autorizado com &quot;Olá&quot; no nome
  <pre>sharedWithMe e o título contêm 'hello'</pre>
* Pesquise arquivos com uma [propriedade de arquivo personalizada](https://developers.google.com/drive/api/v2/properties) chamada `additionalID` com o valor `8e8aceg2af2ge72e78`.
  <pre>properties tem { key='additionalID' e value='8e8aceg2af2ge72e78' e visibility='PRIVATE' }</pre>

O Source deste guia é a [[!DNL Google Drive] documentação](https://developers.google.com/drive/api/v2/search-shareddrives).
