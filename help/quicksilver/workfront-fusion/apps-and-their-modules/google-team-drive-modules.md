---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;agile-and-teams;user-management
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Google Team Drive
description: A variável [!DNL Adobe Workfront Fusion Google Team Drive] Os módulos do permitem monitorar, fazer upload, atualizar, copiar, excluir ou recuperar arquivos e criar pastas no [!DNL Google Shared] Dirija.
author: Becky
feature: Workfront Fusion
exl-id: 8b4c057f-bb98-44d1-9b71-cbeaa402a1c3
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1306'
ht-degree: 0%

---

# [!DNL Google Team Drive] módulos

A variável [!DNL Adobe Workfront Fusion] [!DNL Google Team Drive] Os módulos do permitem monitorar, fazer upload, atualizar, copiar, excluir ou recuperar arquivos e criar pastas no [!DNL Google Shared Drive].

Para utilizar [!DNL Google Team Drive] com [!DNL Adobe Workfront Fusion], é necessário dispor de um [!DNL G Suite] conta. Se você não tiver um, poderá criar um [!DNL G Suite] conta no [[!DNL G Suite] site de inscrição](https://gsuite.google.com/signup/businessstarter/welcome).

Em um [!DNL Adobe Workfront Fusion] cenário, é possível automatizar workflows que usam [!DNL Google Team Drive], bem como conectá-lo a vários aplicativos e serviços de terceiros.

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

Para usar [!DNL Google Team Drive] módulos, você deve ter uma [!DNL Google Team Drive].

## [!DNL Google Team Drive] módulos e seus campos

Ao configurar [!DNL Google Team Drive] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Google Team Drive] Os campos podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Os campos da caixa de diálogo do módulo exibidos em **negrito** (na caixa [!DNL Workfront Fusion] cenário, **não** neste artigo de documentação) são obrigatórios.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Team Drive] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
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
   <td>[!UICONTROL Converter [!DNL Google Documents] arquivos a serem formatados] </td> 
   <td> <p>Selecione o formato que deseja observar [!DNL Google Documents] arquivos convertidos em.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Sheets] arquivos a serem formatados] </td> 
   <td> <p>Selecione o formato que deseja observar [!DNL Google Sheets] arquivos convertidos em.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Slides] arquivos a serem formatados] </td> 
   <td> <p>Selecione o formato que deseja observar [!DNL Google Slides] arquivos convertidos em.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Drawings] arquivos a serem formatados] </td> 
   <td> <p>Selecione o formato que deseja observar [!DNL Google Drawings] arquivos convertidos em.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Observar]</td> 
   <td> <p> Selecione se deseja monitorar a pasta em busca de arquivos novos e modificados ou apenas em busca de novos arquivos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de arquivos baixados]</td> 
   <td> <p> Definir o número máximo de arquivos [!DNL Workfront Fusion] retornará durante um ciclo de execução.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [[!UICONTROL Carregar um arquivo]](#upload-a-file)
* [[!UICONTROL Atualizar um arquivo]](#update-a-file)
* [[!UICONTROL Copiar um arquivo]](#copy-a-file)
* [[!UICONTROL Excluir um arquivo]](#delete-a-file)
* [[!UICONTROL Mover um arquivo para a lixeira]](#move-a-file-to-trash)
* [[!UICONTROL Obter um arquivo]](#get-a-file)
* [[!UICONTROL Obter uma lista de arquivos]](#get-a-file-list)
* [[!UICONTROL Criar uma pasta]](#create-a-folder)

#### [!UICONTROL Carregar um arquivo]

Faz upload de um arquivo para a unidade compartilhada especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Team Drive] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
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
   <td> <p>[!UICONTROL Arquivo de Origem]</p> </td> 
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

#### [!UICONTROL Atualizar um arquivo]

Permite alterar o nome e/ou o conteúdo do arquivo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Team Drive] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
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
   <td> <p>[!UICONTROL Arquivo de Origem]</p> </td> 
   <td>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Título] </td> 
   <td> <p>Insira o novo título para o arquivo atualizado.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter um Arquivo]</td> 
   <td> <p> Habilite esta opção para converter o arquivo para o [!DNL Google] formato na sua pasta compartilhada.</p> </td> 
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
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Team Drive] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
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
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Team Drive] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
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
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Team Drive] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Arquivo]</td> 
   <td> <p> Insira ou mapeie o ID do arquivo que você deseja mover para a lixeira.</p> </td> 
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
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Team Drive] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Documents] arquivos a serem formatados] </td> 
   <td> <p>Selecione o formato que deseja para o [!DNL Google Documents] arquivos convertidos em.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Sheets] arquivos a serem formatados] </td> 
   <td> <p>Selecione o formato que deseja para o [!DNL Google Sheets] arquivos convertidos em.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Slides] arquivos a serem formatados] </td> 
   <td> <p>Selecione o formato que deseja para o [!DNL Google Slides] arquivos convertidos em.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converter [!DNL Google Drawings] arquivos a serem formatados] </td> 
   <td> <p>Selecione o formato que deseja para o [!DNL Google Drawings] arquivos convertidos em.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Arquivo]</td> 
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
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Team Drive] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
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
     <li> <p style="font-weight: bold;">[!UICONTROL Consulta de pesquisa personalizada]</p> <p>Insira o [!DNL Google] termo de consulta de pesquisa. Para obter mais detalhes, consulte [!DNL Google]do <a href="https://developers.google.com/drive/api/v2/ref-search-terms">Pesquisar documentação de consulta</a>. Exemplo: <code>fullText contains '"Hello world"'</code></p> </li> 
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
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Team Drive] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
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
