---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Frame.io
description: A variável [!DNL Adobe Workfront Fusion Frame].io modules enable you to monitor, create, update, retrieve, or delete assets and comments in your [!DNL Frame.io] conta.
author: Becky
feature: Workfront Fusion
exl-id: 373a86f6-fbba-4914-b08d-a3a035ac0ae4
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '2338'
ht-degree: 0%

---

# [!DNL Frame.io] módulos

A variável [!DNL Adobe Workfront Fusion] [!DNL Frame.io] Os módulos do permitem monitorar, criar, atualizar, recuperar ou excluir ativos e comentários em seu [!DNL Frame.io] conta.

Para obter uma introdução ao vídeo sobre o conector Frame.io, consulte:

* [Frame.io](https://video.tv.adobe.com/v/3427032/){target=_blank}

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

Para usar [!DNL Frame.io] módulos, você deve ter uma [!DNL Frame.io] account

## Conectar [!DNL Frame.io] para [!UICONTROL Adobe Workfront Fusion]

Você pode se conectar a [!DNL Frame.io] usando um token de API ou usando o OAuth 2.0.

[Conectar a [!DNL Frame.io] uso de um token de API](#connect-to-frameio-using-an-api-token)

[Conectar a [!DNL Frame.io] uso do PKCE do OAuth 2.0](#connect-to-frameio-using-oauth-20-pkce)

### Conectar a [!DNL Frame.io] uso de um token de API

Para conectar seu [!DNL Frame.io] conta para [!DNL Workfront Fusion] usando um token de API, você deve criar o token de API em seu [!DNL Frame.io] e insira-a na [!DNL Workfront Fusion] [!DNL Frame.io] [!UICONTROL Criar uma conexão] diálogo.

1. Faça logon no [!DNL Frame.io] conta.
1. Vá para a **[!UICONTROL Tokens]** página no [!DNL Frame.io] Desenvolvedor.
1. Clique em **[!UICONTROL Novo]**.
1. Insira o nome do token, selecione os escopos que deseja usar e clique em **[!UICONTROL Criar]**.
1. Copie o token fornecido.
1. Ir para [!DNL Workfront Fusion] e abra o [!DNL Frame.io] do módulo **[!UICONTROL Criar uma conexão]** diálogo.
1. No **[!UICONTROL Tipo de conexão]** selecione **[!DNL Frame.io]**.
1. Insira o token que você copiou na etapa 5 para o **[!UICONTROL Seu [!DNL Frame.io] Chave de API]** e clique em **[!UICONTROL Continuar]** para estabelecer a conexão.

A conexão foi estabelecida. Você pode prosseguir com a configuração do módulo.

### Conectar a [!DNL Frame.io] uso do PKCE do OAuth 2.0

Você pode criar uma conexão com [!DNL Frame.io] usando o PKCE do OAuth 2.0 com uma ID do cliente opcional. Se quiser incluir uma ID do cliente em sua conexão, crie um aplicativo OAuth 2.0 em [!DNL Frame.io] conta.

* [Conectar a [!DNL Frame.io] usar o PKCE do OAuth 2.0 (sem ID do cliente)](#connect-to-frameio-using-using-oauth-20-pkce-without-client-id)
* [Conectar a [!DNL Frame.io] usar o PKCE do OAuth 2.0 (com ID do cliente)](#connect-to-frameio-using-using-oauth-20-pkce-with-client-id)

#### Conectar a [!DNL Frame.io] usar o PKCE do OAuth 2.0 (sem ID do cliente)

1. Ir para [!DNL Workfront Fusion] e abra o [!DNL Frame.io] do módulo **[!UICONTROL Criar uma conexão]** diálogo.
1. No **[!UICONTROL Tipo de conexão]** selecione **[!UICONTROL [!DNL Frame.io]PKCE do OAuth 2.0]**.
1. Insira um nome para a nova conexão no campo **[!UICONTROL Nome da conexão]** campo.
1. Clique em **[!UICONTROL Continuar]** para estabelecer a conexão.

A conexão foi estabelecida. Você pode prosseguir com a configuração do módulo.

#### Conectar a [!DNL Frame.io] usar o PKCE do OAuth 2.0 (com ID do cliente)

1. Criar um aplicativo OAuth 2.0 no [!DNL Frame.io]. Para obter instruções, consulte [!DNL Frame.io] documentação sobre [!UICONTROL Fluxo de autorização de código OAuth 2.0].

   >[!IMPORTANT]
   >
   >Ao criar o aplicativo OAuth 2.0 no [!DNL Frame.io]:
   >
   >* Insira o seguinte como o URI de redirecionamento:
   >   
   >  Américas / APAC `https://app.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >  EMEA `https://app-eu.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >* Ative a opção PCKE.


1. Copiar o fornecido `client_id`.
1. Ir para [!DNL Workfront Fusion] e abra o [!DNL Frame.io] do módulo **[!UICONTROL Criar uma conexão]** diálogo.
1. No **[!UICONTROL Tipo de conexão]** selecione **[!UICONTROL [!DNL Frame.io]PKCE do OAuth 2.0]**.
1. Insira um nome para a nova conexão no campo **[!UICONTROL Nome da conexão]** campo.
1. Clique em **[!UICONTROL Mostrar configurações avançadas]**.
1. Insira o `client_id` você copiou a etapa 2 para o **[!UICONTROL ID do cliente]** campo.
1. Clique em **[!UICONTROL Continuar]** para estabelecer a conexão.

A conexão foi estabelecida. Você pode prosseguir com a configuração do módulo.

## [!DNL Frame.io] módulos e seus campos

Ao configurar [!DNL Frame.io] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Frame.io] Os campos podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Ativos](#assets)
* [Comentários](#comments)
* [Projetos](#projects)
* [Outro](#other)

### Ativos

* [[!UICONTROL Criar um ativo]](#create-an-asset)
* [[!UICONTROL Excluir um ativo]](#delete-an-asset)
* [[!UICONTROL Obter um ativo]](#get-an-asset)
* [[!UICONTROL Listar ativos]](#list-assets)
* [[!UICONTROL Atualizar um ativo]](#update-an-asset)
* [[!UICONTROL Observar ativo excluído]](#watch-asset-deleted)
* [[!UICONTROL Verificar rótulo de ativo atualizado]](#watch-asset-label-updated)
* [[!UICONTROL Assistir a novo ativo]](#watch-new-asset)

#### [!UICONTROL Criar um ativo]

Este módulo de ação cria um novo ativo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Frame.io], consulte <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] para [!DNL Adobe Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Equipe] </td> 
   <td> <p>Selecione ou mapeie a equipe proprietária do projeto para o qual você deseja criar um ativo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Projeto] </td> 
   <td> <p>Selecione o projeto ou mapeie a ID do projeto para o qual você deseja criar um ativo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Pasta] </td> 
   <td> <p>Selecione a pasta ou mapeie a ID da pasta na qual deseja criar um ativo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo] </td> 
   <td> <p>Selecione se deseja criar uma pasta ou um arquivo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome] </td> 
   <td> <p>Insira o nome do novo arquivo ou pasta.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">File Type </td> 
    <td> <p>Select the type of file you want to upload.</p> </td> 
   </tr>
  --> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">File Size </td> 
    <td> <p>The file size in bytes.</p> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL de Origem] </td> 
   <td> <p>Insira o URL do arquivo que você deseja fazer upload.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descrição] </td> 
   <td> <p>Insira uma breve descrição do ativo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir um ativo]

Esse módulo de ação exclui um ativo especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Frame.io], consulte <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] para [!DNL Adobe Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Equipe] </td> 
   <td> <p>Selecione ou mapeie a equipe que possui o projeto que contém o ativo que você deseja excluir.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Projeto]</td> 
   <td> <p> Selecione o projeto ou que contém o ativo que você deseja excluir.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Pasta] </td> 
   <td> <p>Selecione a pasta que contém o ativo que você deseja excluir</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Ativo] </td> 
   <td> <p>Selecione ou mapeie o ativo que deseja excluir.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um ativo]

Este módulo de ação recupera detalhes do ativo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Frame.io], consulte <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] para [!DNL Adobe Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Equipe] </td> 
   <td> <p>Selecione ou mapeie a equipe proprietária do projeto que contém o ativo sobre o qual você deseja recuperar detalhes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Projeto]</td> 
   <td> <p> Selecione o projeto que contém o ativo do qual deseja recuperar detalhes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Pasta] </td> 
   <td> <p>Selecione a pasta que contém o ativo do qual deseja recuperar detalhes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Ativo] </td> 
   <td> <p>Selecione o ativo ou mapeie a ID do ativo sobre o qual deseja recuperar detalhes.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listar ativos]

Este módulo de pesquisa recupera todos os ativos na pasta do projeto especificado.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Frame.io], consulte <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] para [!DNL Adobe Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Equipe] </td> 
   <td> <p>Selecione ou mapeie a equipe proprietária do projeto que contém a pasta da qual você deseja recuperar ativos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Projeto]</td> 
   <td> <p> Selecione o projeto que contém a pasta da qual deseja recuperar ativos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Pasta] </td> 
   <td> <p>Selecione a pasta da qual deseja listar ativos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite] </td> 
   <td> <p>Definir o número máximo de ativos [!DNL Workfront Fusion] retornará durante um ciclo de execução.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### `[!UICONTROL Update an Asset]`

Esse módulo de ação permite atualizar o nome, a descrição ou os campos personalizados de um ativo existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Frame.io], consulte <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] para [!DNL Adobe Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Equipe] </td> 
   <td> <p>Selecione ou mapeie a equipe proprietária do projeto para o qual você deseja atualizar um ativo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Projeto] </td> 
   <td> <p>Selecione o projeto ou mapeie a ID do projeto para o qual você deseja atualizar um ativo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Pasta] </td> 
   <td> <p>Selecione a pasta ou mapeie a ID da pasta na qual deseja atualizar um ativo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome] </td> 
   <td> <p>Insira o nome do arquivo atualizado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descrição] </td> 
   <td> <p>Insira uma breve descrição do ativo atualizado.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Observar ativo excluído]

Este módulo de acionamento inicia um cenário quando um ativo é excluído.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do Webhook]</td> 
   <td> <p> Insira o nome do webhook, por exemplo, Ativo excluído.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Frame.io], consulte <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] para [!DNL Adobe Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Equipe] </td> 
   <td> <p>Selecione a equipe para a qual este webhook foi criado.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Verificar rótulo de ativo atualizado]

Esse módulo de acionamento inicia um cenário quando o status de um ativo é definido, alterado ou removido.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do Webhook]</td> 
   <td> <p> Insira o nome do webhook, por exemplo, Status do ativo atualizado.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Frame.io], consulte <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] para [!DNL Adobe Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Equipe] </td> 
   <td> <p>Selecione a equipe para a qual este webhook foi criado.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Assistir a novo ativo]

Esse módulo de acionador inicia um cenário quando um novo ativo é criado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do Webhook]</td> 
   <td> <p> Insira o nome do webhook, por exemplo, Asset created.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Frame.io], consulte <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] para [!DNL Adobe Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Equipe] </td> 
   <td> <p>Selecione a equipe para a qual este webhook foi criado.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Comentários

* [[!UICONTROL Criar um comentário]](#create-a-comment)
* [[!UICONTROL Excluir um comentário]](#delete-a-comment)
* [[!UICONTROL Obter um comentário]](#get-a-comment)
* [[!UICONTROL Listar comentários]](#list-comments)
* [[!UICONTROL Atualizar um comentário]](#update-a-comment)
* [[!UICONTROL Assista ao comentário atualizado]](#watch-comment-updated)
* [[!UICONTROL Assistir ao novo comentário]](#watch-new-comment)

#### [!UICONTROL Criar um comentário]

Esse módulo de ação adiciona um novo comentário ou resposta ao ativo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Frame.io], consulte <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] para [!DNL Adobe Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo] </td> 
   <td> <p>Selecione se deseja criar um comentário ou responder a um comentário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Equipe] </td> 
   <td> <p>Selecione ou mapeie a equipe proprietária do projeto que contém o ativo ao qual você deseja adicionar um comentário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Projeto] </td> 
   <td> <p>Selecione o projeto ou mapeie a ID do projeto que contém o ativo ao qual você deseja adicionar um comentário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Pasta] </td> 
   <td> <p>Selecione a pasta ou mapeie a ID da pasta que contém o ativo ao qual você deseja adicionar um comentário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Ativo] </td> 
   <td> <p>Selecione ou mapeie o ativo ao qual deseja adicionar um comentário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Comentário] </td> 
   <td> <p>Selecione ou mapeie o comentário ao qual deseja adicionar uma resposta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Texto]</td> 
   <td> <p> Insira o conteúdo do texto do comentário ou da resposta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carimbo de Data/Hora] </td> 
   <td> <p>Insira o número do quadro no vídeo ao qual o comentário deve ser vinculado.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir um comentário]

Este módulo de ação exclui um comentário existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Frame.io], consulte <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] para [!DNL Adobe Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Equipe]</td> 
   <td> <p> Selecione ou mapeie a equipe proprietária do projeto que contém o ativo do qual você deseja excluir um comentário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Projeto]</td> 
   <td> <p> Selecione o projeto ou mapeie a ID do projeto que contém o ativo do qual você deseja excluir um comentário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Pasta]</td> 
   <td> <p> Selecione a pasta que contém o ativo do qual você deseja excluir um comentário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Ativo] </td> 
   <td> <p>Selecione o ativo que contém o comentário que deseja excluir.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Comentário] </td> 
   <td> <p>Selecione o comentário que deseja excluir.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um comentário]

Este módulo de ação recupera detalhes do comentário especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Frame.io], consulte <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] para [!DNL Adobe Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Equipe] </td> 
   <td> <p>Selecione ou mapeie a equipe proprietária do projeto que contém a pasta da qual você deseja recuperar ativos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Projeto] </td> 
   <td> <p>Selecione o projeto que contém a pasta da qual deseja recuperar ativos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Pasta] </td> 
   <td> <p>Selecione a pasta da qual deseja listar ativos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Ativo] </td> 
   <td> <p>Selecione o ativo que contém o comentário que você deseja recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Comentário] </td> 
   <td> <p>Selecione o comentário sobre o qual deseja recuperar detalhes.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listar comentários]

Este módulo de pesquisa recupera todos os comentários do ativo especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Frame.io], consulte <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] para [!DNL Adobe Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Equipe] </td> 
   <td> <p>Selecione ou mapeie a equipe proprietária do projeto que contém a pasta da qual você deseja recuperar comentários.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Projeto] </td> 
   <td> <p>Selecione o projeto que contém a pasta da qual deseja recuperar comentários.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Pasta] </td> 
   <td> <p>Selecione a pasta que contém o ativo do qual deseja listar comentários.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Ativo] </td> 
   <td> <p>Selecione o ativo para o qual deseja listar comentários.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite] </td> 
   <td> <p>Definir o número máximo de comentários [!DNL Workfront Fusion] retornará durante um ciclo de execução.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar um comentário]

Este módulo de ação edita um comentário existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Frame.io], consulte <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] para [!DNL Adobe Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Equipe] </td> 
   <td> <p>Selecione ou mapeie a equipe proprietária do projeto que contém o ativo no qual você deseja atualizar um comentário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Projeto] </td> 
   <td> <p>Selecione o projeto \ que contém o ativo no qual você deseja atualizar um comentário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Pasta] </td> 
   <td> <p>Selecione a pasta que contém o ativo sobre o qual deseja atualizar um comentário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Ativo] </td> 
   <td> <p>Selecione o ativo no qual deseja atualizar um comentário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Comentário] </td> 
   <td> <p>Selecione o comentário que deseja atualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Texto]</td> 
   <td> <p> Insira o conteúdo do texto do comentário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carimbo de Data/Hora] </td> 
   <td> <p>Insira o número do quadro no vídeo ao qual o comentário está vinculado.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Assista ao comentário atualizado]

Este módulo de acionamento inicia um cenário quando um comentário é editado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do Webhook] </td> 
   <td> <p>Insira o nome do webhook, por exemplo, Comment Edited.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Frame.io], consulte <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] para [!DNL Adobe Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Equipe] </td> 
   <td> <p>Selecione a equipe para a qual este webhook foi criado.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Assistir ao novo comentário]

Este módulo de acionamento inicia um cenário quando um novo comentário ou resposta é criado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do Webhook] </td> 
   <td> <p>Insira o nome do webhook, por exemplo Novo comentário.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Frame.io], consulte <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] para [!DNL Adobe Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Equipe] </td> 
   <td> <p>Selecione a equipe para a qual este webhook foi criado.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Projetos

#### [!UICONTROL Listar Projetos]

Este módulo de pesquisa recupera todos os projetos da equipe especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Frame.io], consulte <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] para [!DNL Adobe Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Equipe] </td> 
   <td> <p>Selecione ou mapeie a equipe para a qual deseja recuperar projetos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite] </td> 
   <td> <p>Definir o número máximo de projetos [!DNL Workfront Fusion] retornará durante um ciclo de execução.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Outro

#### [!UICONTROL Fazer uma chamada de API]

Este módulo permite executar uma chamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Frame.io], consulte <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] para [!DNL Adobe Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Insira um caminho relativo a <code>https://api.frame.io</code>. Exemplo: <code> /v2/teams</code></p> <p>Observação: para obter a lista de endpoints disponíveis, consulte o [!DNL Frame.io] Referência da API.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   <td> <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formulário de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] O adiciona cabeçalhos de autorização automaticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadeia de Consulta] </td> 
   <td> <p>Insira a string de consulta da solicitação. Para cada parâmetro que você deseja incluir na cadeia de caracteres de consulta, clique em <b>[!UICONTROL Adicionar item]</b> e insira o nome do campo e o valor desejado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada à API na forma de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Exemplo:** A chamada de API a seguir retorna todas as equipes e seus detalhes na [!DNL Frame.io] conta:

URL: `/v2/teams`

Método: `GET`

![](assets/api-call-example.png)

O resultado pode ser encontrado na Saída do módulo em Pacote > Corpo.

Em nosso exemplo, os detalhes de 1 equipe foram retornados:

![](assets/api-call-output.png)
