---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Microsoft OneDrive
description: Em um [!DNL Adobe Workfront Fusion] você pode automatizar fluxos de trabalho que usam o OneDrive, bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: 13a25c6c-bdf1-467d-bd90-ebd763c59235
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3934'
ht-degree: 0%

---

# [!DNL Microsoft OneDrive] módulos

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL OneDrive], bem como conectá-lo a vários aplicativos e serviços de terceiros.

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

Para usar [!DNL OneDrive] módulos, você deve ter um [!DNL Microsoft OneDrive] conta.

## Conectando o [!DNL OneDrive] para [!DNL Workfront Fusion]

Para obter instruções sobre como conectar seu [!DNL OneDrive] para [!UICONTROL Workfront Fusion], consulte [Criar uma conexão com [!UICONTROL Adobe Workfront Fusion] - Instruções básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Microsoft OneDrive] módulos e seus campos

Ao configurar [!DNL OneDrive] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL OneDrive] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Arquivo/Pasta](#filefolder)
* [Outro](#other)

### Arquivo/Pasta

* [[!UICONTROL Assistir arquivos/pastas]](#watch-filesfolders)
* [[!UICONTROL Pesquisar arquivos/pastas]](#search-filesfolders)
* [[!UICONTROL Obter um arquivo]](#get-a-file)
* [[!UICONTROL Baixar um arquivo]](#download-a-file)
* [[!UICONTROL Carregar um arquivo]](#upload-a-file)
* [[!UICONTROL Criar uma pasta]](#create-a-folder)
* [[!UICONTROL Obter um link de compartilhamento]](#get-a-share-link)
* [[!UICONTROL Mover um arquivo/pasta]](#move-a-filefolder)
* [[!UICONTROL Copiar um arquivo]](#copy-a-file)
* [[!UICONTROL Excluir um arquivo/pasta]](#delete-a-filefolder)

#### [!UICONTROL Assistir arquivos/pastas]

Esse módulo de acionador inicia um cenário quando um arquivo ou pasta é criado ou atualizado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obter instruções sobre como conectar seu [!DNL OneDrive] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assistir arquivos/pastas]</td> 
   <td> <p>Selecione como deseja assistir a arquivos ou pastas:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Por Hora De Criação]</b> </p> <p>Fique atento a novos arquivos ou pastas.</p> </li> 
     <li> <p><b>[!UICONTROL Por Hora Atualizada]</b> </p> <p>Fique atento a arquivos ou pastas existentes atualizados.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolha sua [!DNL OneDrive] localização]</td> 
   <td> <p>Selecione o local que deseja observar:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Minha unidade]</b> </p> <p>Selecione se o módulo deve ser habilitado para inserir uma ID de unidade.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sim]</b> </p> <p>Insira a ID da unidade que você deseja que o módulo observe.</p> </li> 
       <li> <p><b>[!UICONTROL n.o]</b> </p> <p>Navegue até a pasta que você deseja que o módulo assista. Você também pode inserir uma query para filtrar os resultados retornados.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Compartilhado Comigo]</b> </p> <p>O módulo assiste arquivos que foram compartilhados com o proprietário da unidade.</p> </li> 
     <li> <p><b>[!UICONTROL Unidade do site]</b> </p> <p>Selecione o Site do SharePoint que você deseja que o módulo assista. Sites disponíveis são Sites seguidos pelo usuário conectado.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Selecione o grupo cuja unidade você deseja que o módulo assista.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher um tipo de item]</td> 
   <td> <p>Selecione se deseja assistir a arquivos, pastas ou ambos.</p> <p>Observação: Não é possível procurar pastas em uma unidade [!UICONTROL compartilhada comigo].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>



#### [!UICONTROL Pesquisar arquivos/pastas]

Esse módulo de pesquisa retorna arquivos e pastas com base nos critérios definidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obter instruções sobre como conectar seu [!DNL OneDrive] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolha sua [!DNL OneDrive] localização]</td> 
   <td> <p>Selecione o local que deseja pesquisar:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Minha unidade]</b> </p> <p>Selecione se o módulo deve ser habilitado para inserir uma ID de unidade.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sim]</b> </p> <p>Insira a ID da unidade que você deseja que o módulo pesquise.</p> </li> 
       <li> <p><b>[!UICONTROL n.o]</b> </p> <p>Navegue até a pasta que deseja que o módulo pesquise. Você também pode inserir uma query para filtrar os resultados retornados.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Compartilhado Comigo]</b> </p> <p>O módulo pesquisa arquivos que foram compartilhados com o proprietário da unidade.</p> </li> 
     <li> <p><b>[!UICONTROL Unidade do site]</b> </p> <p>Selecione o [!DNL SharePoint] Site que você deseja que o módulo pesquise. Sites disponíveis são Sites seguidos pelo usuário conectado.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Selecione o grupo cuja unidade você deseja que o módulo pesquise.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher um tipo de item]</td> 
   <td> <p>Selecione se deseja pesquisar por arquivos, pastas ou ambos.</p> <p>Observação: Não é possível pesquisar pastas em uma unidade [!UICONTROL compartilhada comigo].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um arquivo]

Este módulo de ação obtém os metadados de um arquivo especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obter instruções sobre como conectar seu [!DNL OneDrive] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter (ID do arquivo e caminho do arquivo)]</td> 
   <td>Selecione se deseja identificar o arquivo por ID de arquivo ou pelo Caminho do arquivo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir uma ID de arquivo] / [!UICONTROL Caminho do arquivo]</td> 
   <td> <p>Selecione como deseja inserir a ID do arquivo ou o Caminho do arquivo:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Inserir manualmente]</b> </p> <p>Selecione essa opção se desejar inserir a ID ou o caminho diretamente ou mapeá-lo de um módulo anterior.</p> </li> 
     <li> <p><b>[!UICONTROL Selecionar de uma lista]</b> </p> <p>Selecione essa opção se desejar selecionar de uma lista de arquivos ou caminhos disponíveis. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolha sua [!DNL OneDrive] localização]</td> 
   <td> <p>Selecione o local que deseja pesquisar:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Minha unidade]</b> </p> <p>Selecione se o módulo deve ser habilitado para inserir uma ID de unidade.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sim]</b> </p> <p>Digite a ID da unidade que contém o arquivo que deseja obter.</p> </li> 
       <li> <p><b>[!UICONTROL n.o]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidade do site]</b> </p> <p>Selecione o Site do SharePoint que contém o arquivo que deseja obter. Sites disponíveis são Sites seguidos pelo usuário conectado.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Selecione o grupo cuja unidade contém o arquivo que deseja obter.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da unidade]</td> 
   <td> <p>Selecione ou mapeie a unidade que contém o arquivo que deseja obter. Este campo não estará disponível se você selecionou [!UICONTROL Não] no campo [!UICONTROL Ativar para inserir uma ID de unidade].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo] / [!UICONTROL ID do arquivo] / [!UICONTROL Caminho do arquivo]</td> 
   <td> <p>Se você selecionou [!UICONTROL Inserir manualmente], insira ou mapeie a ID do arquivo ou o caminho do arquivo que deseja obter.</p> <p>Se você selecionou [!UICONTROL Selecionar na lista], selecione o arquivo que deseja obter.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Baixar um arquivo]

Este módulo de ação baixa o arquivo especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obter instruções sobre como conectar seu [!DNL OneDrive] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter (ID do arquivo e caminho do arquivo)]</td> 
   <td>Selecione se deseja identificar o arquivo por ID de arquivo ou pelo Caminho do arquivo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Inserir uma ID de arquivo / Caminho do arquivo</td> 
   <td> <p>Selecione como deseja inserir a ID do arquivo ou o Caminho do arquivo:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Inserir manualmente]</b> </p> <p>Selecione essa opção se desejar inserir a ID ou o caminho diretamente ou mapeá-lo de um módulo anterior.</p> </li> 
     <li> <p><b>[!UICONTROL Selecionar de uma lista]</b> </p> <p>Selecione essa opção se desejar selecionar de uma lista de arquivos ou caminhos disponíveis. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolha sua [!DNL OneDrive] localização]</td> 
   <td> <p>Selecione o local que deseja que contenha o arquivo que deseja baixar:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Minha unidade]</b> </p> <p>Selecione se o módulo deve ser habilitado para inserir uma ID de unidade.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sim]</b> </p> <p>Digite a ID da unidade que contém o arquivo que você deseja baixar.</p> </li> 
       <li> <p><b>[!UICONTROL n.o]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidade do site]</b> </p> <p>Selecione o Site do SharePoint que contém o arquivo que você deseja baixar. Sites disponíveis são Sites seguidos pelo usuário conectado.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Selecione o grupo cuja unidade contém o arquivo que você deseja baixar.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da unidade]</td> 
   <td> <p>Selecione ou mapeie a unidade que contém o arquivo que deseja baixar. Este campo não estará disponível se você selecionou [!UICONTROL Não] no campo [!UICONTROL Ativar para inserir uma ID de unidade].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo] / [!UICONTROL ID do arquivo] / [!UICONTROL Caminho do arquivo]</td>
   <td> <p>Se você selecionou [!UICONTROL Inserir manualmente], insira ou mapeie a ID do arquivo ou o caminho do arquivo que deseja baixar.</p> <p>Se você selecionou [!UICONTROL Selecionar na lista], selecione o arquivo que deseja baixar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Converter em PDF]</td> 
   <td> <p>Ative essa opção para converter o arquivo em um arquivo PDF. Você pode converter dos seguintes tipos de arquivo:</p> 
    <table style="table-layout:auto"> 
     <col> 
     <col> 
     <col> 
     <tbody> 
      <tr> 
       <td> 
        <ul> 
         <li> <p> <p>CSV</p> </p> </li> 
         <li> <p> <p>DOC</p> </p> </li> 
         <li> <p> <p>DOCX</p> </p> </li> 
         <li> <p> <p>ODP</p> </p> </li> 
         <li> <p> <p>ODS</p> </p> </li> 
         <li> <p> <p>ODT</p> </p> </li> 
        </ul> </td> 
       <td> 
        <ul> 
         <li> <p> <p>POT</p> </p> </li> 
         <li> <p> <p>POTM</p> </p> </li> 
         <li> <p> <p>POTX</p> </p> </li> 
         <li> <p> <p>PPS</p> </p> </li> 
         <li> <p> <p>PPSX</p> </p> </li> 
         <li> <p> <p>PPSXM</p> </p> </li> 
        </ul> </td> 
       <td> 
        <ul> 
         <li> <p>PPT</p> </li> 
         <li> <p>PPTM</p> </li> 
         <li> <p>PPTX</p> </li> 
         <li> <p>RTF</p> </li> 
         <li> <p>XLS</p> </li> 
         <li> <p>XLSX</p> </li> 
        </ul> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Carregar um arquivo]

Este módulo de ação carrega um arquivo na pasta especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obter instruções sobre como conectar seu [!DNL OneDrive] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Enter (ID e caminho do local da pasta)</td> 
   <td>Selecione se deseja identificar a pasta de destino por ID ou por um caminho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolha sua [!DNL OneDrive] localização]</td> 
   <td> <p>Selecione o local onde deseja fazer upload de um arquivo:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Minha unidade]</b> </p> <p>Selecione se o módulo deve ser habilitado para inserir uma ID de unidade.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sim]</b> </p> <p>Selecione a unidade que contém o arquivo que deseja obter.</p> </li> 
       <li> <p><b>[!UICONTROL n.o]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidade do site]</b> </p> <p>Selecione o [!DNL SharePoint] Site que contém a pasta onde você deseja carregar um arquivo. Sites disponíveis são Sites seguidos pelo usuário conectado.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Selecione o grupo cuja unidade contém a pasta onde deseja carregar um arquivo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da unidade]</td> 
   <td> <p>Selecione a unidade que contém a pasta onde deseja carregar um arquivo. Este campo não estará disponível se você selecionou [!UICONTROL Não] no campo [!UICONTROL Ativar para inserir uma ID de unidade].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Se o arquivo com o mesmo nome existir]</td> 
   <td>Selecione como proceder se já existir um arquivo com o mesmo nome.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descrição]</td> 
   <td>Adicione uma descrição ao arquivo carregado.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar uma pasta]

Este módulo de ação cria uma nova pasta na unidade especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obter instruções sobre como conectar seu [!DNL OneDrive] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolha sua [!DNL OneDrive] localização]</td> 
   <td> <p>Selecione o local onde deseja criar uma pasta:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Minha unidade]</b> </p> <p>Selecione se o módulo deve ser habilitado para inserir uma ID de unidade.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sim]</b> </p> <p>Selecione a unidade em que deseja criar uma pasta.</p> </li> 
       <li> <p><b>[!UICONTROL n.o]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidade do site]</b> </p> <p>Selecione o [!DNL SharePoint] Site onde deseja criar uma pasta. Sites disponíveis são Sites seguidos pelo usuário conectado.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Selecione o grupo que possui a unidade onde deseja criar uma pasta.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da unidade]</td> 
   <td> <p>Selecione a unidade em que deseja criar uma pasta. Este campo não estará disponível se você selecionou [!UICONTROL Não] no campo [!UICONTROL Ativar para inserir uma ID de unidade].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta]</td> 
   <td>Para que a nova pasta seja uma subpasta, navegue até a pasta na qual deseja que ela seja uma subpasta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Novo nome da pasta]</td> 
   <td> <p>Insira ou mapeie um nome para a nova pasta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Se a pasta com o mesmo nome existir]</td> 
   <td>Selecione como proceder se já existir um arquivo com o mesmo nome.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um link de compartilhamento]

Este módulo de ação retorna um link de compartilhamento para o arquivo especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obter instruções sobre como conectar seu [!DNL OneDrive] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter (ID do arquivo e caminho do arquivo)]</td> 
   <td>Selecione se deseja identificar o arquivo por ID de arquivo ou pelo Caminho do arquivo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir uma ID de arquivo] / [!UICONTROL Caminho do arquivo]</td> 
   <td> <p>Selecione como deseja inserir a ID do arquivo ou o Caminho do arquivo:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Inserir manualmente]</b> </p> <p>Selecione essa opção se desejar inserir a ID ou o caminho diretamente ou mapeá-lo de um módulo anterior.</p> </li> 
     <li> <p><b>[!UICONTROL Selecionar de uma lista]</b> </p> <p>Selecione essa opção se desejar selecionar de uma lista de arquivos ou caminhos disponíveis. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolha sua [!DNL OneDrive] localização]</td> 
   <td> <p>Selecione o local para o qual deseja recuperar um link de compartilhamento:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Minha unidade]</b> </p> <p>Selecione se o módulo deve ser habilitado para inserir uma ID de unidade.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sim]</b> </p> <p>Digite a ID da unidade que contém o arquivo para o qual você deseja recuperar um link de compartilhamento.</p> </li> 
       <li> <p><b>[!UICONTROL n.o]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidade do site]</b> </p> <p>Selecione o Site do SharePoint que contém o arquivo para o qual você deseja recuperar um link de compartilhamento. Sites disponíveis são Sites seguidos pelo usuário conectado.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Selecione o grupo cuja unidade contém o arquivo para o qual você deseja recuperar um link de compartilhamento.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da unidade]</td> 
   <td> <p>Selecione ou mapeie a unidade que contém o arquivo para o qual deseja recuperar um link de compartilhamento. Este campo não estará disponível se você selecionou [!UICONTROL Não] no campo [!UICONTROL Ativar para inserir uma ID de unidade].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo] / [!UICONTROL ID do arquivo] / [!UICONTROL Caminho do arquivo]</td> 
   <td> <p>Se você selecionou [!UICONTROL Inserir manualmente], insira ou mapeie a ID do arquivo ou o caminho do arquivo para o qual deseja recuperar um link de compartilhamento.</p> <p>Se você selecionou [!UICONTROL Selecionar] na lista, selecione o arquivo para o qual deseja recuperar um link de compartilhamento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de permissão]</td> 
   <td> <p>Selecione se deseja que as pessoas com o link possam ler e gravar no arquivo ou somente leitura.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escopo]</td> 
   <td>Selecione se deseja que o arquivo esteja disponível para qualquer pessoa com o link ou somente para os membros da organização que têm o link.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover um arquivo/pasta]

Esse módulo de ação move um arquivo ou pasta para um novo local de pasta

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obter instruções sobre como conectar seu [!DNL OneDrive] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter (ID do arquivo e caminho do arquivo)]</td> 
   <td>Selecione se deseja identificar o arquivo por ID de arquivo ou pelo Caminho do arquivo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir uma ID de arquivo/Caminho do arquivo]</td> 
   <td> <p>Selecione como deseja inserir a ID do arquivo ou o Caminho do arquivo:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Inserir manualmente]</b> </p> <p>Selecione essa opção se desejar inserir a ID ou o caminho diretamente ou mapeá-lo de um módulo anterior.</p> </li> 
     <li> <p><b>[!UICONTROL Selecionar de uma lista]</b> </p> <p>Selecione essa opção se desejar selecionar de uma lista de arquivos ou caminhos disponíveis. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolha sua [!DNL OneDrive] localização]</td> 
   <td> <p>Selecione o local que contém o arquivo ou a pasta que você deseja mover:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Minha unidade]</b> </p> <p>Selecione se o módulo deve ser habilitado para inserir uma ID de unidade.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sim]</b> </p> <p>Digite o ID da unidade que contém o arquivo ou a pasta que você deseja mover.</p> </li> 
       <li> <p><b>[!UICONTROL n.o]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidade do site]</b> </p> <p>Selecione o [!DNL SharePoint] Site que contém o arquivo ou a pasta que você deseja mover. Sites disponíveis são Sites seguidos pelo usuário conectado.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Selecione o grupo cuja unidade contém o arquivo ou a pasta que você deseja mover.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da unidade]</td> 
   <td> <p>Selecione ou mapeie a unidade que contém o arquivo ou a pasta que você deseja mover. Este campo não estará disponível se você selecionou [!UICONTROL Não] no campo [!UICONTROL Ativar para inserir uma ID de unidade].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Selecione [!UICONTROL Arquivo/Pasta]</td> 
   <td>Selecione se deseja mover um arquivo ou uma pasta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL Arquivo] / [!UICONTROL ID do arquivo] / [!UICONTROL Caminho do arquivo]</p> <p role="rowheader">[!UICONTROL Pasta] / [!UICONTROL ID da pasta] / [!UICONTROL Caminho da pasta]</p> </td> 
   <td> <p>Se você selecionou [!UICONTROL Inserir manualmente], insira ou mapeie a ID ou o caminho do arquivo ou pasta que deseja mover.</p> <p>Se você selecionou [!UICONTROL Selecionar] na lista, selecione o arquivo ou a pasta que deseja mover.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir um novo local de pasta]</td> 
   <td> <p>Selecione como deseja inserir o local onde deseja mover o arquivo ou pasta:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Inserir manualmente]</b> </p> <p>Selecione essa opção se desejar inserir a ID ou o caminho diretamente ou mapeá-lo de um módulo anterior.</p> </li> 
     <li> <p><b>[!UICONTROL Selecionar de uma lista]</b> </p> <p>Selecione essa opção se desejar selecionar de uma lista de arquivos ou caminhos disponíveis. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolha sua [!DNL OneDrive] localização]</td> 
   <td> <p>Selecione o local onde deseja mover o arquivo ou pasta:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Minha unidade]</b> </p> <p>Selecione se o módulo deve ser habilitado para inserir uma ID de unidade.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sim]</b> </p> <p>Digite o ID da unidade onde deseja mover o arquivo ou a pasta.</p> </li> 
       <li> <p><b>[!UICONTROL n.o]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidade do site]</b> </p> <p>Selecione o [!DNL SharePoint] Site onde deseja mover o arquivo ou a pasta. Sites disponíveis são Sites seguidos pelo usuário conectado.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Selecione o grupo na unidade em que deseja mover o arquivo ou a pasta.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da unidade]</td> 
   <td> <p>Selecione ou mapeie a unidade que contém a pasta para a qual deseja mover o arquivo ou a pasta. Este campo não estará disponível se você selecionou [!UICONTROL Não] no campo [!UICONTROL Ativar para inserir uma ID de unidade].</p> <p>Se deixar em branco, o arquivo ou pasta só poderá ser movido dentro do mesmo [!DNL OneDrive].</p> <p>Você pode mover arquivos e pastas da [!UICONTROL Minha unidade] para uma [!UICONTROL Unidade do site] ou uma [!UICONTROL Group's Drive]. </p> <p>Você pode mover arquivos de uma [!UICONTROL Site's Drive] somente para a mesma unidade no mesmo site.</p> <p>Você pode mover arquivos de uma [!UICONTROL Group's Drive] somente para a mesma unidade no mesmo grupo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta]</td> 
   <td>Insira ou mapeie a pasta onde deseja mover o arquivo ou a pasta.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiar um arquivo]

Esse módulo de ação copia um arquivo para um novo local de pasta

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obter instruções sobre como conectar seu [!DNL OneDrive] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter (ID do arquivo e caminho do arquivo)]</td> 
   <td>Selecione se deseja identificar o arquivo por ID de arquivo ou pelo Caminho do arquivo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir uma ID de arquivo] / [!UICONTROL Caminho do arquivo]</td> 
   <td> <p>Selecione como deseja inserir a ID do arquivo ou o Caminho do arquivo:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Inserir manualmente]</b> </p> <p>Selecione essa opção se desejar inserir a ID ou o caminho diretamente ou mapeá-lo de um módulo anterior.</p> </li> 
     <li> <p><b>[!UICONTROL Selecionar de uma lista]</b> </p> <p>Selecione essa opção se desejar selecionar de uma lista de arquivos ou caminhos disponíveis. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolha sua [!DNL OneDrive] localização]</td> 
   <td> <p>Selecione o local que contém o arquivo que você deseja copiar:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Minha unidade]</b> </p> <p>Selecione se o módulo deve ser habilitado para inserir uma ID de unidade.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sim]</b> </p> <p>Digite a ID da unidade que contém o arquivo ou a pasta que você deseja copiar.</p> </li> 
       <li> <p><b>[!UICONTROL n.o]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidade do site]</b> </p> <p>Selecione o Site do SharePoint que contém o arquivo que você deseja mover. Sites disponíveis são Sites seguidos pelo usuário conectado.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Selecione o grupo cuja unidade contém o arquivo que você deseja copiar.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da unidade]</td> 
   <td> <p>Selecione ou mapeie a unidade que contém o arquivo que você deseja copiar. Este campo não estará disponível se você selecionou [!UICONTROL Não] no campo [!UICONTROL Ativar para inserir uma ID de unidade].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL Arquivo] / [!UICONTROL ID do arquivo] / [!UICONTROL Caminho do arquivo]</p> </td> 
   <td> <p>Se você selecionou [!UICONTROL Inserir manualmente], insira ou mapeie a ID ou o caminho do arquivo que deseja copiar.</p> <p>Se você selecionou [!UICONTROL Selecionar] na lista, selecione o arquivo que deseja copiar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir um novo local de pasta]</td> 
   <td> <p>Selecione como deseja inserir o local para o qual deseja copiar o arquivo ou para:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Inserir manualmente]</b> </p> <p>Selecione essa opção se desejar inserir a ID ou o caminho diretamente ou mapeá-lo de um módulo anterior.</p> </li> 
     <li> <p><b>[!UICONTROL Selecionar de uma lista]</b> </p> <p>Selecione essa opção se desejar selecionar de uma lista de pastas disponíveis. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Novo local do OneDrive]</td> 
   <td> <p>Selecione o local onde deseja copiar o filtro. Essa opção estará disponível se você optar por selecionar o novo local da pasta em uma lista.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Minha unidade]</b> </p> <p>Selecione se o módulo deve ser habilitado para inserir uma ID de unidade.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sim]</b> </p> <p>Digite a ID da unidade na qual você deseja copiar o arquivo.</p> </li> 
       <li> <p><b>[!UICONTROL n.o]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidade do site]</b> </p> <p>Selecione o [!DNL SharePoint] Site onde deseja copiar o arquivo. Sites disponíveis são Sites seguidos pelo usuário conectado.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Selecione o grupo para a qual você deseja copiar o arquivo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da unidade]</td> 
   <td> <p>Selecione ou mapeie a unidade que contém a pasta para a qual deseja copiar o arquivo. Este campo não estará disponível se você selecionou [!UICONTROL Não] no campo [!UICONTROL Ativar para inserir uma ID de unidade].</p> <p>Se deixar em branco, o arquivo ou pasta só poderá ser copiado dentro do mesmo [!UICONTROL OneDrive].</p> <p>Você pode copiar arquivos e pastas da [!UICONTROL Minha unidade] para uma [!UICONTROL Unidade do site] ou uma [!UICONTROL Group's Drive]. </p> <p>Você pode copiar arquivos de uma [!UICONTROL Site's Drive] somente para a mesma unidade no mesmo site.</p> <p>Você pode copiar arquivos de uma [!UICONTROL Group's Drive] somente para a mesma unidade no mesmo grupo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta]</td> 
   <td>Insira ou mapeie a pasta onde deseja mover a cópia ou pasta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Novo nome do arquivo copiado]</td> 
   <td> <p>Insira ou mapeie um nome para a nova cópia do arquivo. Você pode deixar em branco caso não queira alterar o nome do arquivo original.</p> <p>O nome deve incluir a extensão de arquivo . Exemplo:<code> file.txt</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir um arquivo/pasta]

Esse módulo de ação exclui o arquivo selecionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obter instruções sobre como conectar seu [!DNL OneDrive] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter (ID e caminho do arquivo/pasta)]</td> 
   <td>Selecione se deseja identificar o arquivo por ID de arquivo ou pelo Caminho do arquivo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir um ID de arquivo/pasta /Inserir um caminho de arquivo/pasta]</td> 
   <td> <p>Selecione como deseja inserir a ID do arquivo ou o Caminho do arquivo:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Inserir manualmente]</b> </p> <p>Selecione essa opção se desejar inserir a ID ou o caminho diretamente ou mapeá-lo de um módulo anterior.</p> </li> 
     <li> <p><b>[!UICONTROL Selecionar de uma lista]</b> </p> <p>Selecione essa opção se desejar selecionar de uma lista de arquivos ou caminhos disponíveis. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolha sua [!DNL OneDrive] localização]</td> 
   <td> <p>Selecione o local que deseja pesquisar:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Minha unidade]</b> </p> <p>Selecione se o módulo deve ser habilitado para inserir uma ID de unidade.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sim]</b> </p> <p>Digite a ID da unidade que contém o arquivo ou a pasta que deseja excluir.</p> </li> 
       <li> <p><b>[!UICONTROL n.o]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidade do site]</b> </p> <p>Selecione o [!DNL SharePoint] Site que contém o arquivo ou a pasta que deseja excluir. Sites disponíveis são Sites seguidos pelo usuário conectado.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Selecione o grupo cuja unidade contém o arquivo ou a pasta que deseja excluir.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da unidade]</td> 
   <td> <p>Selecione ou mapeie a unidade que contém o arquivo ou a pasta que deseja excluir. Este campo não estará disponível se você selecionou [!UICONTROL Não] no campo [!UICONTROL Ativar para inserir uma ID de unidade].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Selecione [!UICONTROL Arquivo/Pasta]</td> 
   <td>Selecione se deseja excluir um arquivo ou uma pasta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo] / [!UICONTROL ID do arquivo] / [!UICONTROL Caminho do arquivo]</td>
   <td> <p>Se você selecionou [!UICONTROL Inserir manualmente], insira ou mapeie a ID do arquivo ou o caminho do arquivo que deseja excluir.</p> <p>Se você selecionou [!UICONTROL Selecionar] na lista, selecione o arquivo que deseja excluir.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Outro

#### [!UICONTROL Faça uma chamada de API]

Esse módulo executa uma chamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obter instruções sobre como conectar seu [!DNL OneDrive] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Insira um caminho relativo a <code>https://graph.microsoft.com</code>. Exemplo:<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   td&gt; <p>Selecione o método de solicitação HTTP que você precisa configurar a chamada da API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> <p>O Workfront Fusion adiciona os cabeçalhos de autorização para você.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sequência de consulta]</td> 
   <td> <p>Adicione a query para a chamada de API no formato de um objeto JSON padrão.</p> <p>Por exemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada da API no formato de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>



## Caso não seja possível fazer upload ou atualizar um arquivo

Há vários problemas possíveis quando o upload ou a atualização de um arquivo falha:

* O arquivo carregado é muito grande e excede o limite máximo de tamanho de arquivo para sua [!DNL OneDrive] planeje ou você usou todos os seus [!DNL OneDrive] cota de armazenamento da conta. Para obter mais espaço de armazenamento, exclua arquivos existentes do [!DNL OneDrive] ou atualize seu [!DNL OneDrive] conta.
* O OneDrive não permite carregar dois arquivos com o mesmo nome em uma única pasta. Se a pasta de destino contiver um arquivo com o mesmo nome do arquivo que está sendo carregado, a execução do cenário terminará com um erro. A solução é simplesmente renomear o arquivo que está sendo carregado. Se o objetivo for atualizar um arquivo, use a variável [!UICONTROL Atualizar um arquivo] ação.
* A pasta selecionada anteriormente, para a qual o arquivo está sendo carregado, não existe mais. O cenário é interrompido e será necessário selecionar a pasta de destino novamente.
