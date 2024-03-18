---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Adobe Lightroom
description: Com os módulos do Adobe Lightroom, é possível iniciar um cenário do Adobe Workfront Fusion com base em eventos em sua conta do Adobe Lightroom.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
source-git-commit: e99bd69c712a7685512eecc7fccc8211013a259d
workflow-type: tm+mt
source-wordcount: '2244'
ht-degree: 0%

---

# [!DNL Adobe Lightroom] módulos

<!--Add Connection info-->

Em um [!DNL Adobe Workfront Fusion] cenário, é possível automatizar workflows que usam [!DNL Adobe Lightroom], bem como conectá-lo a vários aplicativos e serviços de terceiros.

Se precisar de instruções sobre como criar um cenário, consulte [Criar um cenário](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obter informações sobre módulos, consulte [Módulos no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plano*</td>
      <td>
        <p>[!UICONTROL Pro] ou superior</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] licença*</td>
      <td>
        <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] licença**</td>
      <td >
        <p>[!UICONTROL Workfront Fusion para Automação e Integração do Trabalho]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Produto</td>
      <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td>
    </tr>
    </tr>
  </tbody>
</table>


&#42;Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

&#42;&#42;Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [!DNL [Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Pré-requisitos

Antes de poder usar o [!DNL Adobe Lightroom] deve garantir que os seguintes pré-requisitos sejam atendidos:

* Você deve ter um ativo [!DNL Adobe Lightroom] conta.

## Criar uma conexão com o Adobe Lightroom



## Módulos do Adobe Lightroom e seus campos

Ao configurar [!DNL Adobe Lightroom] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Adobe Lightroom] Os campos podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Outro](#other)
* [Ativos](#assets)
* [Álbuns](#albums)

### Outro

* [Verificação de integridade](#health-check)
* [Recuperar metadados de catálogo do usuário](#retrieve-user-catalog-metadata)

#### Verificação de integridade

Este módulo de ação recupera uma ID de versão do servidor do Lightroom, provando se o serviço do Lightroom está em execução no momento.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Lightroom], consulte <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Lightroom]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Credenciais]</td>
      <td>
        <p>Se quiser fornecer credenciais específicas para garantir que um servidor específico esteja em execução, clique em Adicionar item e insira as credenciais.</p><p>Os cabeçalhos de autorização são adicionados automaticamente.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Recuperar metadados de catálogo do usuário

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Lightroom], consulte <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Lightroom]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Credenciais]</td>
      <td>
        <p>Se quiser fornecer credenciais específicas para garantir que você possa acessar a conta de usuário correta, clique em Adicionar item e insira as credenciais.</p><p>Os cabeçalhos de autorização são adicionados automaticamente.</p>
      </td>
    </tr>
  </tbody>
</table>

### Ativos

* [Criar um arquivo original de ativo](#create-an-asset-external-xmp-develop-setting-file)
* [Criar um ativo](#create-an-asset)
* [Criar um arquivo externo de configuração de desenvolvimento de XMP do ativo](#create-an-asset-external-xmp-develop-setting-file)
* [Gerar representações para um arquivo original](#generate-renditions-for-an-original-file)
* [Obter um ativo de catálogo](#get-a-catalog-asset)
* [Obter a configuração mais recente de desenvolvimento de XMP externo de ativos](#get-the-latest-asset-external-xmp-develop-setting-file)
* [Obter a representação de ativo mais recente](#get-the-latest-asset-rendition)
* [Recuperar ativos](#retrieve-assets)

#### Criar um arquivo original de ativo

Esse módulo de ação cria e faz upload de um arquivo original para um ativo.


<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Lightroom], consulte <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Lightroom]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Catálogo]</td>
      <td>
        <p>Insira ou mapeie a ID do catálogo que contém o ativo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Ativo]</td>
      <td>
        <p>Insira ou mapeie a ID do ativo para o qual você deseja criar e fazer upload de um arquivo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Comprimento do conteúdo em bytes]</td>
      <td>
        <p>Insira ou mapeie o comprimento do conteúdo em bytes.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Intervalo de bytes]</td>
      <td>
        <p>Insira ou mapeie o intervalo de bytes da solicitação, incluindo o primeiro e o último bytes e o comprimento da entidade conforme definido no RFC 2616. Deve ser incluído somente quando os dados são muito grandes para serem carregados em uma única chamada.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo de conteúdo]</td>
      <td>
        <p>Selecione o tipo de conteúdo para o novo arquivo.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Criar um ativo

Esse módulo de ação cria um novo ativo com metadados iniciais e informações de importação.


<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Lightroom], consulte <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Lightroom]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Catálogo]</td>
      <td>
        <p>Insira ou mapeie a ID do catálogo onde o ativo será criado.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Ativo]</td>
      <td>
        <p>Insira ou mapeie a ID do novo ativo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo de ativo]</td>
      <td>
        <p>Selecione se o ativo é uma imagem ou um vídeo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datetime criado pelo usuário]</td>
      <td>
        <p>Inserir ou mapear uma data com o formato <code>YYYY-MM-DDT00:00:00-00:00</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Data e hora atualizado pelo usuário]</td>
      <td>
        <p>Inserir ou mapear uma data com o formato <code>YYYY-MM-DDT00:00:00-00:00</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Data capturada]</td>
      <td>
        <p>Inserir ou mapear uma data com o formato <code>YYYY-MM-DDT00:00:00-00:00</code>.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Criar um arquivo externo de configuração de desenvolvimento de XMP do ativo

Esse módulo de ação suporta dois workflows. O primeiro fluxo de trabalho é carregar o arquivo externo de configurações de desenvolvimento de XMP para o ativo. O segundo fluxo de trabalho é criar um arquivo externo de configurações de desenvolvimento de XMP copiando do arquivo externo de configuração de desenvolvimento xmp de outro ativo.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Lightroom], consulte <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Lightroom]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Comprimento do conteúdo em bytes]</td>
      <td>
        <p>Insira ou mapeie o comprimento do conteúdo em bytes.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Carregar arquivo XMP/develop novo ou copiado]</td>
      <td>
        <p>Selecione se você está fazendo upload de um novo arquivo ou copiando um arquivo de um ativo existente.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Catálogo]</td>
      <td>
        <p>Insira ou mapeie a ID do catálogo que contém o ativo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Ativo]</td>
      <td>
        <p>Insira ou mapeie a ID do ativo para o qual você deseja fazer upload ou copiar um arquivo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Vincular ao arquivo XMP/develop]</td>
      <td>
        <p>Insira ou mapeie um link para o arquivo que deseja fazer upload ou copiar.</p><p>Esse arquivo deve ser JSON ao copiar um arquivo ou XML ao fazer upload de um arquivo.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Gerar representações para um arquivo original

Esse módulo de ação gera representações de forma assíncrona para um arquivo original.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Lightroom], consulte <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Lightroom]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo(s) de representação (separados por ponto-e-vírgula)]</td>
      <td>
        <p>Insira o tipo de representação da representação que deseja criar. Se inserir mais de um tipo, separe-os com um ponto e vírgula (;). <p>Tipos possíveis:</p><ul><li><code>fullsize</code></li><li><code>2560</code></li></ul></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Comprimento do conteúdo em bytes]</td>
      <td>
        <p>Insira ou mapeie o comprimento do conteúdo em bytes.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Catálogo]</td>
      <td>
        <p>Insira ou mapeie a ID do catálogo que contém o ativo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Ativo]</td>
      <td>
        <p>Insira ou mapeie a ID do ativo para o qual você deseja criar uma representação de um arquivo.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Obter um ativo de catálogo

Este módulo de ação recupera informações sobre um único ativo em um catálogo. O catálogo deve ser de propriedade do usuário cujas credenciais estão representadas na conexão usada neste módulo.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Lightroom], consulte <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Lightroom]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Catálogo]</td>
      <td>
        <p>Insira ou mapeie a ID do catálogo que contém o ativo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Ativo]</td>
      <td>
        <p>Insira ou mapeie a ID do ativo para o qual deseja recuperar as informações.</p>
      </td>
    </tr>
  </tbody>
</table>


#### Obter o arquivo de configuração de desenvolvimento de XMP externo de ativo mais recente

Esse módulo de ação recupera o arquivo de configuração XMP externo do ativo mais recente.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Lightroom], consulte <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Lightroom]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Catálogo]</td>
      <td>
        <p>Insira ou mapeie a ID do catálogo que contém o ativo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Ativo]</td>
      <td>
        <p>Insira ou mapeie a ID do ativo associado ao arquivo de configuração de desenvolvimento do XMP.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Obter a representação de ativo mais recente

Este módulo de ação recupera a representação de ativo mais recente do tipo especificado.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Lightroom], consulte <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Lightroom]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Catálogo]</td>
      <td>
        <p>Insira ou mapeie a ID do catálogo que contém o ativo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Ativo]</td>
      <td>
        <p>Insira ou mapeie a ID do ativo associado ao arquivo de configuração de desenvolvimento do XMP.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo de representação]</td>
      <td>
        <p>Selecione o tipo de representação que deseja recuperar.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Recuperar ativos

Este módulo de ação recupera ativos de propriedade do usuário cujas credenciais estão representadas na conexão usada neste módulo.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Lightroom], consulte <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Lightroom]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Catálogo]</td>
      <td>
        <p>Insira ou mapeie a ID do catálogo que contém o ativo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Iniciando carimbo de data/hora]</td>
      <td>
        <p>Insira ou mapeie um carimbo de data e hora. O módulo retorna registros que foram atualizados após esse carimbo de data e hora.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Retornar ativos capturados antes]</td>
      <td>
        <p>Inserir uma data com o formato <code>YYYY-MM-DDT00:00:00</code>. O módulo retorna resultados capturados antes dessa data.</p><p> Este campo não pode ser usado com o campo <code>Return assets captured after</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Número máximo de ativos retornados]</td>
      <td>
        <p>Defina o número máximo de ativos que [!DNL Workfront Fusion] retornará durante um ciclo de execução. Este número deve ser menor ou igual a 100.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL valor de hash SHA256 do arquivo original]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ocultar ativos que estão dentro de pilhas?"]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Valores de subtipo de ativo]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL IDs de Ativo]</td>
      <td>
        <p>Insira ou mapeie até 100 IDs de ativos, separadas por vírgulas.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipos de ativos a serem excluídos]</td>
      <td>
        <p>Selecione se deseja excluir ativos completos ou incompletos. Para incluir todos os ativos, deixe este campo em branco.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Agrupar valores]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Nomear valores]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Status Favorito]</td>
      <td>
        <p></p>
      </td>
    </tr>
    </tr>
  </tbody>
</table>

### Álbuns

* [Adicionar ativos a um álbum](#add-assets-to-an-album)
* [Criar um álbum](#create-an-album)
* [Excluir um álbum](#delete-an-album)
* [Obter um álbum](#get-an-album)
* [Listar os ativos de um álbum](#list-assets-of-an-album)
* [Recuperar álbuns](#retrieve-albums)
* [Atualizar um álbum](#update-album)

#### Adicionar ativos a um álbum

Este módulo de ação adiciona um ou mais ativos ao álbum especificado. Você pode adicionar até 50 ativos em um ciclo de execução.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Lightroom], consulte <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Lightroom]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Catálogo]</td>
      <td>
        <p>Insira ou mapeie a ID do catálogo que contém o álbum ao qual você deseja adicionar ativos.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Álbum]</td>
      <td>
        <p>Insira ou mapeie a ID do álbum ao qual você deseja adicionar ativos.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ativos]</td>
      <td>
        <p>Para cada ativo que deseja adicionar ao álbum, clique em <b>Adicionar item</b> e insira os seguintes campos.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Ativo]</td>
      <td>
        <p>Insira ou mapeie a ID do ativo que você deseja adicionar ao álbum</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Este ativo é uma capa de álbum?]</td>
      <td>
        <p>Selecione se deseja que esse ativo seja exibido como a imagem que representa o álbum.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Ordem]</td>
      <td>
        <p></p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Metadados]</td>
      <td>
        <p>Insira ou mapeie quaisquer metadados que deseja incluir com o ativo. Deve ser uma única cadeia de texto com um comprimento máximo de 1 a 24 caracteres.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL ID Remota]</td>
      <td>
        <p>Insira um identificador para o ativo.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Criar um álbum

Este módulo de ação cria um novo álbum no Lightroom.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Lightroom], consulte <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Lightroom]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Catálogo]</td>
      <td>
        <p>Insira ou mapeie a ID do catálogo em que deseja criar um álbum.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Álbum]</td>
      <td>
        <p>Insira ou mapeie uma ID para o novo álbum.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Subtipo]</td>
      <td>
        <p>Selecione o subtipo do álbum.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Chave de API]</td>
      <td>
        <p>Insira a chave da API do serviço que está criando o álbum.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Datetime criado pelo usuário]</td>
      <td>
        <p>Inserir ou mapear uma data com o formato <code>YYYY-MM-DDT00:00:00-00:00Z</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Data e hora atualizado pelo usuário]</td>
      <td>
        <p>Inserir ou mapear uma data com o formato <code>YYYY-MM-DDT00:00:00-00:00Z</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Album name]</td>
      <td>
        <p>Insira ou mapeie um nome para o novo álbum.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Capa]</td>
      <td>
        <p>Insira ou mapeie a ID de um ativo para usar como capa deste álbum.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL ID Remota]</td>
      <td>
        <p>Insira um identificador para o ativo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Data de criação]</td>
      <td>
        <p>Inserir ou mapear uma data com o formato <code>YYYY-MM-DDT00:00:00-00:00Z</code>.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Data de atualização]</td>
      <td>
        <p>Inserir ou mapear uma data com o formato <code>YYYY-MM-DDT00:00:00-00:00Z</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL O álbum foi excluído?]</td>
      <td>
        <p>Ative essa opção se o conteúdo externo afiliado tiver sido excluído.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL do local para editar conteúdo afiliado]</td>
      <td>
        <p>Se houver um URL no qual os usuários possam editar o conteúdo desse álbum, insira o URL aqui.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL do local para exibir conteúdo afiliado]</td>
      <td>
        <p>Se houver um URL no qual os usuários possam visualizar o conteúdo desse álbum, insira o URL aqui.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Excluir um álbum

Este módulo de ação exclui um álbum.

O álbum excluído deve ter sido criado pelo mesmo aplicativo cliente que o está excluindo agora e deve ser do subtipo `project` ou `project_set`.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Lightroom], consulte <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Lightroom]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Catálogo]</td>
      <td>
        <p>Insira ou mapeie a ID do catálogo que contém o álbum que você deseja excluir.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Álbum]</td>
      <td>
        <p>Insira ou mapeie a ID do álbum que você deseja excluir.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Excluir álbuns filhos?]</td>
      <td>
        <p>Selecione se deseja excluir os álbuns filhos do álbum excluído.</p>
      </td>
    </tr>
  </tbody>
</table>

### Obter um álbum

Este módulo de ação recupera o álbum especificado

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Lightroom], consulte <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Lightroom]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Catálogo]</td>
      <td>
        <p>Insira ou mapeie a ID do catálogo que contém o álbum que você deseja recuperar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Álbum]</td>
      <td>
        <p>Insira ou mapeie a ID do álbum que você deseja recuperar.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Listar os ativos de um álbum

Este módulo de ação recupera uma lista de ativos no álbum especificado.



#### Recuperar álbuns

Este módulo de ação recupera uma lista de álbuns no catálogo especificado.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Lightroom], consulte <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Lightroom]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Catálogo]</td>
      <td>
        <p>Insira ou mapeie a ID do catálogo que contém os álbuns que você deseja recuperar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Subtipos]</td>
      <td>
        <p>Insira ou mapeie a ID do álbum que você deseja recuperar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Nome do álbum para preceder os resultados atuais]</td>
      <td>
        <p>Se estiver paginando os resultados, digite ou mapeie o nome do último álbum na página anterior.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Número máximo de álbuns retornados]</td>
      <td>
        <p>Defina o número máximo de ativos que [!DNL Workfront Fusion] retornará durante um ciclo de execução. O valor padrão para este campo é 100. Este módulo poderá retornar mais álbuns que este limite se vários álbuns no limite tiverem o mesmo <code>name_after</code> valor.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Atualizar álbum

Este módulo de ação atualiza o álbum especificado.

O álbum atualizado deve ter sido criado pelo mesmo aplicativo cliente que o está atualizando e deve ser do subtipo `project` ou `project_set`.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Lightroom], consulte <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Lightroom]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Catálogo]</td>
      <td>
        <p>Insira ou mapeie a ID do catálogo que contém o álbum que você deseja atualizar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Álbum]</td>
      <td>
        <p>Insira ou mapeie a ID do álbum que você deseja atualizar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Outros campos</td>
      <td>
      <td>Para obter descrições de outros campos neste módulo, consulte <a href="#create-an-album" class="MCXref xref" >Criar um álbum</a> neste artigo.</td>
      </td>
    </tr>
  </tbody>
</table>










