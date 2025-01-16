---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Google Docs
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: fbe7d628-d833-43ce-83b8-8e4e6a812fd1
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '4160'
ht-degree: 0%

---

# [!DNL Google Docs] módulos

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [módulos do Google Docs](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-docs-modules.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

Os módulos do [!DNL Adobe Workfront Fusion] [!DNL Google Docs] permitem que você monitore, crie, edite e recupere documentos no [!DNL Google Docs] e [!DNL Google Docs] (para [!DNL Google Workspace] usuários).

Para usar [!DNL Google Docs] com [!DNL Adobe Workfront Fusion], é necessário ter uma conta [!DNL Google]. Se você ainda não tiver uma conta [!DNL Google], crie uma na página de ajuda da Conta [!DNL Google].

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
   <p>Requisito atual do produto: se você tiver o plano [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], sua organização deve comprar [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] da [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Para usar módulos do [!DNL Google Docs], você deve ter uma conta do Google.

## Informações da API do Google Docs

O conector do Google Docs usa o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL base</td> 
   <td> https://docs.googleapis.com/v1</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Versão da API</td> 
   <td> v1 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tag da API</td> 
   <td>v1.4.13</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Google Docs] módulos e seus campos

Ao configurar módulos do [!DNL Google Docs], o [!UICONTROL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos [!DNL Google Docs] adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Documento

* [[!UICONTROL Assistir Documentos]](#watch-documents)
* [[!UICONTROL Listar Documentos]](#list-documents)
* [[!UICONTROL Obter Conteúdo de um Documento]](#get-content-of-a-document)
* [[!UICONTROL Criar um documento]](#create-a-document)
* [[!UICONTROL Criar um documento a partir de um modelo]](#create-a-document-from-a-template)
* [[!UICONTROL Inserir um Parágrafo em um Documento]](#insert-a-paragraph-to-a-document)
* [[!UICONTROL Inserir uma Imagem em um Documento]](#insert-an-image-to-a-document)
* [[!UICONTROL Substituir uma imagem por uma nova imagem]](#replace-an-image-with-a-new-image)
* [[!UICONTROL Substituir texto em um documento]](#replace-text-in-a-document)
* [[!UICONTROL Baixar um documento]](#download-a-document)
* [[!UICONTROL Excluir um documento]](#delete-a-document)

#### [!UICONTROL Assistir Documentos]

Esse módulo de acionamento retorna detalhes do documento quando um novo documento é criado ou modificado na pasta selecionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Observar Documentos]</td> 
   <td> <p style="color: #000000;">Selecione se deseja observar documentos criados ([!UICONTROL Por Data de Criação]) ou modificados ([!UICONTROL Por Data de Modificação]).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma Unidade]</td> 
   <td> <p>Selecione o tipo de unidade que deseja monitorar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Minha Unidade]</strong> </p> <p>Selecione a pasta que deseja observar para documentos criados ou modificados.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartilhado Comigo]</strong> </p> <p>Selecione a pasta que deseja observar para documentos criados ou modificados.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidade Compartilhada]</strong> (disponível somente para [!DNL Google Workspace] usuários)</p> <p>Selecione se você deseja [!UICONTROL Usar Acesso de Administrador de Domínio]. Selecionar [!UICONTROL Sim] emite a solicitação como administrador de domínio, e todas as unidades compartilhadas nas quais o solicitante é um administrador são retornadas.</p> <p>Selecione a unidade compartilhada que deseja assistir.</p> <p>Observação: se você tiver selecionado a opção [!DNL Google Shared Drive] neste campo e não for um usuário [!DNL Google Workspace], o erro <code>[400] Invalid Value</code> será retornado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite] </td> 
   <td> <p>Defina o número máximo de documentos que o Workfront Fusion retorna em um ciclo de execução.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listar Documentos]

Este módulo de ação recupera uma lista de documentos da pasta selecionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma Unidade]</td> 
   <td> <p>Selecione o tipo de unidade a partir da qual deseja listar documentos.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Minha Unidade]</strong> </p> <p>Selecione a pasta da qual deseja listar documentos.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartilhado Comigo]</strong> </p> <p>Selecione a pasta da qual deseja listar documentos.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidade Compartilhada]</strong> (disponível somente para [!DNL Google Workspace] usuários)</p> <p>Selecione se você deseja [!UICONTROL Usar Acesso de Administrador de Domínio]. Selecionar [!UICONTROL Sim] emite a solicitação como administrador de domínio, e todas as unidades compartilhadas nas quais o solicitante é um administrador são retornadas.</p> <p>Selecione a unidade compartilhada da qual deseja listar documentos.</p> <p>Observação: se você tiver selecionado a opção [!DNL Google Docs] neste campo e não for um usuário [!DNL Google Workspace], o erro <code>[400] Invalid Value</code> será retornado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite] </td> 
   <td> <p>Defina o número máximo de documentos que [!DNL Workfront Fusion] retorna em um ciclo de execução.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter Conteúdo de um Documento]

Este módulo de ação recupera um documento especificado.

Talvez seja necessário estender as permissões.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obter Conteúdo de um Documento]</td> 
   <td> <p>Selecione se deseja mapear a ID do documento ou selecione o documento manualmente no menu suspenso.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma Unidade]</td> 
   <td> <p>Selecione o tipo de unidade que contém o documento que você deseja recuperar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Minha Unidade]</strong> </p> <p>Selecione a pasta que contém o documento que você deseja recuperar.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartilhado Comigo]</strong> </p> <p>Selecione a pasta que contém o documento que você deseja recuperar.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidade Compartilhada]</strong> (disponível somente para [!DNL Google Workspace] usuários)</p> <p>Selecione se você deseja [!UICONTROL Usar Acesso de Administrador de Domínio]. Selecionar [!UICONTROL Sim] emite a solicitação como administrador de domínio, e todas as unidades compartilhadas nas quais o solicitante é um administrador são retornadas.</p> <p>Selecione a unidade compartilhada que contém o documento que você deseja recuperar.</p> <p>Observação: se você tiver selecionado a opção [!DNL Google Docs] neste campo e não for um usuário [!DNL Google Workspace], o erro <code>[400] Invalid Value</code> será retornado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filtro]</p> </td> 
   <td> <p>Selecione o objeto que você deseja retornar na saída do módulo.</p> 
    <ul> 
     <li>[!UICONTROL Imagem] (padrão)</li> 
     <li>[!UICONTROL Desenho]</li> 
     <li>[!UICONTROL Gráfico]</li> 
    </ul> <p>Nota:  <p>Para mapear ainda mais esses objetos, use o valor da [!UICONTROL Inline Objects Array] na saída deste módulo (em vez de [!UICONTROL inlineObjects]).</p> <p>Os objetos [!UICONTROL Inline Objects Array] são classificados na mesma ordem em que aparecem no documento. Isso facilitará qualquer processamento adicional.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar um documento]

Este módulo de ação permite criar um novo documento na pasta selecionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome] </td> 
   <td> <p>Insira o nome do documento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conteúdo]</td> 
   <td> <p>Insira o conteúdo do documento. HTML é compatível.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma Unidade]</td> 
   <td> <p>Selecione o tipo de unidade em que deseja criar um documento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Minha Unidade]</strong> </p> <p>Selecione a pasta onde deseja criar um documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartilhado Comigo]</strong> </p> <p>Selecione a pasta onde deseja criar um documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidade Compartilhada]</strong> (disponível somente para [!DNL Google Workspace] usuários)</p> <p>Selecione se você deseja [!UICONTROL Usar Acesso de Administrador de Domínio]. Selecionar [!UICONTROL Sim] emite a solicitação como administrador de domínio, e todas as unidades compartilhadas nas quais o solicitante é um administrador são retornadas.</p> <p>Selecione a unidade compartilhada onde deseja criar um documento.</p> <p>Observação: se você tiver selecionado a opção [!DNL Google Docs] neste campo e não for um usuário [!DNL Google Workspace], o erro <code>[400] Invalid Value</code> será retornado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir um Cabeçalho]</td> 
   <td> <p> Habilite esta opção para inserir o cabeçalho ao documento e, em seguida, insira ou mapeie o texto do cabeçalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir um Rodapé] </td> 
   <td> <p>Habilite esta opção para inserir o rodapé no documento e, em seguida, insira ou mapeie o texto do cabeçalho.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar um documento a partir de um modelo]

Este módulo de ação cria uma cópia de um documento de modelo existente e substitui todas as tags. Esse módulo também permite que os usuários substituam imagens por novas imagens por URL.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Criar um Documento a partir de um Modelo]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Por Mapeamento]</strong> <br>Selecione esta opção para mapear o modelo de documento.</li> 
     <li><strong>[!UICONTROL Por Lista Suspensa]</strong> <br>Selecione esta opção para escolher o modelo de documento no menu suspenso.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma Unidade]</td> 
   <td> <p>Selecione o tipo de unidade onde o modelo está localizado. Esta opção estará disponível se você tiver selecionado [!UICONTROL Por Lista Suspensa] no campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Minha Unidade]</strong> </p> <p>Selecione a pasta onde o modelo está localizado.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartilhado Comigo]</strong> </p> <p>Selecione a pasta onde o modelo está localizado.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidade Compartilhada]</strong> (disponível somente para [!DNL Google Workspace] usuários)</p> <p>Selecione se você deseja [!UICONTROL Usar Acesso de Administrador de Domínio]. Selecionar [!UICONTROL Sim] emite a solicitação como administrador de domínio, e todas as unidades compartilhadas nas quais o solicitante é um administrador são retornadas.</p> <p>Selecione a unidade compartilhada onde o modelo está localizado.</p> <p>Observação: se você tiver selecionado a opção [!DNL Google Docs] neste campo e não for um usuário [!DNL Google Workspace], o erro <code>[400] Invalid Value</code> será retornado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Valores]</p> </td> 
   <td> <p>Insira os valores que serão inseridos em vez das variáveis para o novo documento.</p> 
    <ul> 
     <li><strong>[!UICONTROL Marcas]</strong> <br>Insira as marcas contidas no modelo de documento. Não use <code>&#123;&#123;&#125;&#125;</code>. Exemplo: use <code>name</code> em vez de <code>&#123;&#123;name&#125;&#125;</code>.</li> 
     <li><strong>[!UICONTROL Valor Substituído]</strong><br>Insira o valor da marca.</li> 
    </ul> <p>Por exemplo, a variável <code> &#123;&#123;name&#125;&#125;</code> no documento de origem será exibida como o campo de nome aqui, onde o valor pode ser inserido, como <code>John</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Substituição de Imagens]</p> </td> 
   <td> <p>Insira o link para a [!UICONTROL Image Object ID] e a [!UICONTROL Image URL] que substituirá a imagem atual.</p> <p>Observação: você pode recuperar as IDs de imagem usando o módulo [!UICONTROL Obter um Documento], no qual as IDs estão contidas na matriz [!UICONTROL Inline Object Array].</p> <p>Recomendamos que você adicione texto ALT a imagens em seu documento [!DNL Google]. </p> <p>Para adicionar um texto alternativo à imagem [!DNL Google Docs]:</p> 
    <ol> 
     <li value="1">Clique com o botão direito na imagem.</li> 
     <li value="2">Selecione a opção [!UICONTROL ALT text].</li> 
     <li value="3">Insira o [!UICONTROL ALT text] no campo [!UICONTROL Título] e clique em [!UICONTROL OK].</li> 
    </ol> <p>Depois que o texto ALT é adicionado à imagem, ele é exibido no nome do campo entre parênteses.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Título] </td> 
   <td> <p>Insira o nome do novo documento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma Unidade]</td> 
   <td> <p>Selecione o tipo de unidade onde o modelo está localizado. Esta opção estará disponível se você tiver selecionado [!UICONTROL Por Lista Suspensa] no campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Minha Unidade]</strong> </p> <p>Selecione a pasta onde deseja criar o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartilhado Comigo]</strong> </p> <p>Selecione a pasta onde deseja criar o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidade Compartilhada]</strong> (disponível somente para [!DNL Google Workspace] usuários)</p> <p>Selecione se você deseja [!UICONTROL Usar Acesso de Administrador de Domínio]. Selecionar [!UICONTROL Sim] emite a solicitação como administrador de domínio, e todas as unidades compartilhadas nas quais o solicitante é um administrador são retornadas.</p> <p>Selecione a unidade compartilhada onde deseja criar o documento.</p> <p>Observação: se você tiver selecionado a opção [!DNL Google Docs] neste campo e não for um usuário [!DNL Google Workspace], o erro <code>[400] Invalid Value</code> será retornado.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Inserir um Parágrafo em um Documento]

Este módulo de ação anexa ou insere um novo parágrafo a um documento existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Selecionar um Documento]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Por Mapeamento]</strong> <br>Selecione esta opção para mapear o documento.</li> 
     <li><strong>[!UICONTROL Por Lista Suspensa]</strong> <br> Selecione esta opção para escolher o documento no menu suspenso.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma Unidade]</td> 
   <td> <p>Selecione o tipo de unidade em que o documento ao qual você deseja adicionar um parágrafo está localizado. Esta opção estará disponível se você tiver selecionado [!UICONTROL Por Lista Suspensa] no campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Minha Unidade]</strong> </p> <p>Selecione a pasta onde está localizado o documento ao qual deseja adicionar um parágrafo e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartilhado Comigo]</strong> </p> <p>Selecione a pasta onde está localizado o documento ao qual deseja adicionar um parágrafo e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidade Compartilhada]</strong> (disponível somente para [!DNL Google Workspace] usuários)</p> <p>Selecione se você deseja [!UICONTROL Usar Acesso de Administrador de Domínio]. Selecionar [!UICONTROL Sim] emite a solicitação como administrador de domínio, e todas as unidades compartilhadas nas quais o solicitante é um administrador são retornadas.</p> <p>Selecione a unidade compartilhada onde o documento ao qual deseja adicionar um parágrafo está localizado e selecione o documento.</p> <p>Observação: se você tiver selecionado a opção [!DNL Google Docs] neste campo e não for um usuário [!DNL Google Workspace], o erro <code>[400] Invalid Value</code> será retornado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Inserir um Parágrafo]</p> </td> 
   <td> <p>Selecione como deseja inserir o novo texto no documento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Por especificação de local]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL por índice]</strong> </p> 
        <ul> 
         <li> <p><strong>[!UICONTROL Índice]</strong> </p> <p>Insira o número do índice onde deseja inserir o texto. Você pode usar o módulo [!UICONTROL Obter um Documento] para recuperar o número do Índice.</p> <p>Para exibir todos os caracteres (inclusive ocultos) no documento, é possível usar o complemento [!UICONTROL Mostrar]. Você pode encontrar o complemento em [!UICONTROL Complementos] &gt; [!UICONTROL Obter complementos]. Procure por [!UICONTROL Show] e instale o complemento [!UICONTROL Show].</p> </li> 
         <li> <p><strong>[!UICONTROL Texto inserido]</strong> </p> <p>Insira o texto que deseja inserir no documento.</p> </li> 
        </ul> </li> 
       <li> <p><strong>[!UICONTROL por ID de segmento]</strong> </p> <p>Selecione o cabeçalho e o rodapé nos quais deseja inserir o conteúdo do texto e insira o texto que deseja inserir nos campos correspondentes.</p> <p>Se o cabeçalho ou rodapé já contiver texto, o novo texto será adicionado antes do texto existente.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Anexando ao corpo do documento]</strong> </p> <p>Adiciona o texto inserido ao final do conteúdo do corpo do documento.</p> <p>O estilo do novo parágrafo será copiado do parágrafo no índice de inserção atual, incluindo listas e marcadores.</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL Acrescentando ao final do segmento (Cabeçalho e Rodapé)]</strong> </p> <p>Selecione o cabeçalho e o rodapé nos quais deseja inserir o conteúdo do texto e insira o texto que deseja inserir nos campos correspondentes.</p> <p>Se o cabeçalho ou rodapé já contiver texto, o novo texto será adicionado após o texto existente.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Texto Anexado]</td> 
   <td>Insira ou mapeie o texto que deseja anexar ao documento</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Inserir uma Imagem em um Documento]

Esse módulo de ação insere uma imagem do URL no documento.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Selecionar um Documento]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Por Mapeamento]</strong> <br>Selecione esta opção para mapear o modelo de documento.</li> 
     <li><strong>[!UICONTROL Por Lista Suspensa]</strong> <br> Selecione esta opção para escolher o documento no menu suspenso.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma Unidade]</td> 
   <td> <p>Selecione o tipo de unidade em que o documento ao qual você deseja adicionar uma imagem está localizado. Esta opção estará disponível se você tiver selecionado [!UICONTROL Por Lista Suspensa] no campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Minha Unidade]</strong> </p> <p>Selecione a pasta onde está localizado o documento ao qual deseja adicionar uma imagem e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartilhado Comigo]</strong> </p> <p>Selecione a pasta onde está localizado o documento ao qual deseja adicionar uma imagem e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidade Compartilhada]</strong> (disponível somente para [!DNL Google Workspace] usuários)</p> <p>Selecione se você deseja [!UICONTROL Usar Acesso de Administrador de Domínio]. Selecionar [!UICONTROL Sim] emite a solicitação como administrador de domínio, e todas as unidades compartilhadas nas quais o solicitante é um administrador são retornadas.</p> <p>Selecione a unidade compartilhada onde o documento ao qual você deseja adicionar uma imagem está localizado e selecione o documento.</p> <p>Observação: se você tiver selecionado a opção [!DNL Google Docs] neste campo e não for um usuário [!DNL Google Workspace], o erro <code>[400] Invalid Value</code> será retornado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Inserir uma Imagem]</p> </td> 
   <td> <p>Selecione como você deseja que a nova imagem seja inserida no documento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Por especificação de local]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL por índice]</strong> </p> 
        <ul> 
         <li> <p><strong>[!UICONTROL Índice]</strong> </p> <p>Insira o número do índice no qual você deseja inserir sua imagem. Você pode usar o módulo [!UICONTROL Obter um Documento] para recuperar o [!UICONTROL Número de índice].</p> <p>Para exibir todos os caracteres (inclusive ocultos) no documento, é possível usar o complemento [!UICONTROL Mostrar]. Você pode encontrar o complemento em [!UICONTROL Complementos] &gt; [!UICONTROL Obter complementos]. Procure por [!UICONTROL Show] e instale o complemento [!UICONTROL Show].</p> </li> 
         <li> <p><strong>[!UICONTROL URL da Imagem]</strong> </p> <p>Insira a URL da imagem que deseja inserir no documento.</p> <p>O tamanho máximo da imagem é 50 MB. Não deve exceder 25 megapixels. Somente o formato PNG, JPEG ou GIF é compatível.</p> </li> 
        </ul> </li> 
       <li> <p><strong>[!UICONTROL por ID de segmento]</strong> </p> <p>Selecione o cabeçalho e o rodapé nos quais deseja inserir a imagem e insira o URL da imagem nos campos correspondentes.</p> <p>O tamanho máximo da imagem é 50 MB. A imagem não deve exceder 25 megapixels. Somente os formatos PNG, JPEG ou GIF são suportados.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Anexando ao corpo do documento]</strong> </p> <p>Adiciona uma imagem específica ao final do conteúdo do corpo do documento.</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL Acrescentando ao final do segmento (Cabeçalho e Rodapé)]</strong> </p> <p>Selecione o cabeçalho e o rodapé nos quais deseja inserir uma imagem e insira o URL da imagem que deseja inserir nos campos correspondentes.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Magnitude de Altura em Pontos/Magnitude de Largura em Pontos]</p> </td> 
   <td> <p>Defina o tamanho da imagem inserida. A proporção será mantida.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Substituir uma imagem por uma nova imagem]

Esse módulo de ação substitui uma imagem existente. A proporção da imagem original será mantida.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Selecionar um Documento]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Por Mapeamento]</strong> <br>Selecione esta opção para mapear o modelo de documento.</li> 
     <li><strong>[!UICONTROL Por Lista Suspensa]</strong> <br> Selecione esta opção para escolher o documento no menu suspenso.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma Unidade]</td> 
   <td> <p>Selecione o tipo de unidade em que o documento que você deseja substituir uma imagem está localizado. Esta opção estará disponível se você tiver selecionado [!UICONTROL Por Lista Suspensa] no campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Minha Unidade]</strong> </p> <p>Selecione a pasta onde está localizado o documento que você deseja substituir uma imagem e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartilhado Comigo]</strong> </p> <p>Selecione a pasta onde está localizado o documento que você deseja substituir uma imagem e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidade Compartilhada]</strong> (disponível somente para [!DNL Google Workspace] usuários)</p> <p>Selecione se você deseja [!UICONTROL Usar Acesso de Administrador de Domínio]. Selecionar [!UICONTROL Sim] emite a solicitação como administrador de domínio, e todas as unidades compartilhadas nas quais o solicitante é um administrador são retornadas.</p> <p>Selecione a unidade compartilhada onde o documento que você deseja substituir uma imagem está localizado e selecione o documento.</p> <p>Observação: se você tiver selecionado a opção [!DNL Google Docs] neste campo e não for um usuário [!DNL Google Workspace], o erro <code>[400] Invalid Value</code> será retornado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL da imagem]</p> </td> 
   <td> <p>Insira ou mapeie o URL da nova imagem que substituirá a imagem existente.</p> <p>As imagens são listadas na ordem em que aparecem no documento. Por exemplo, <code>Body: Image No. 1</code> é a primeira imagem no documento.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Substituir texto em um documento]

Este módulo de ação substitui o texto em um documento.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Selecionar um Documento]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Por Mapeamento]</strong> <br>Selecione esta opção para mapear o modelo de documento.</li> 
     <li><strong>[!UICONTROL Por Lista Suspensa]</strong> <br> Selecione esta opção para escolher o documento no menu suspenso.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma Unidade]</td> 
   <td> <p>Selecione o tipo de unidade em que o documento ao qual você deseja adicionar texto está localizado. Esta opção estará disponível se você tiver selecionado [!UICONTROL Por Lista Suspensa] no campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Minha Unidade]</strong> </p> <p>Selecione a pasta onde está localizado o documento ao qual deseja adicionar texto e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartilhado Comigo]</strong> </p> <p>Selecione a pasta onde está localizado o documento ao qual deseja adicionar texto e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidade Compartilhada]</strong> (disponível somente para [!DNL Google Workspace] usuários)</p> <p>Selecione se você deseja [!UICONTROL Usar Acesso de Administrador de Domínio]. Selecionar [!UICONTROL Sim] emite a solicitação como administrador de domínio, e todas as unidades compartilhadas nas quais o solicitante é um administrador são retornadas.</p> <p>Selecione a unidade compartilhada na qual o documento ao qual você deseja adicionar texto está localizado e selecione o documento.</p> <p>Observação: se você tiver selecionado a opção [!DNL Google Docs] neste campo e não for um usuário [!DNL Google Workspace], o erro <code>[400] Invalid Value</code> será retornado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Substituir um Texto]</p> </td> 
   <td> <p>Adicione cada texto que deseja substituir.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Texto antigo a ser substituído]</strong> </p> <p>Insira o texto que deseja substituir.</p> </li> 
     <li> <p><strong>[!UICONTROL Novo texto a ser inserido]</strong> </p> <p>Insira o novo texto.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Baixar um documento]

Este módulo de ação converte e baixa o documento selecionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma Unidade]</td> 
   <td> <p>Selecione o tipo de unidade onde o documento que você deseja baixar está localizado.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Minha Unidade]</strong> </p> <p>Selecione a pasta onde o documento que você deseja baixar está localizado e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartilhado Comigo]</strong> </p> <p>Selecione a pasta onde o documento que você deseja baixar está localizado e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidade Compartilhada]</strong> (disponível somente para [!DNL Google Workspace] usuários)</p> <p>Selecione se você deseja [!UICONTROL Usar Acesso de Administrador de Domínio]. Selecionar [!UICONTROL Sim] emite a solicitação como administrador de domínio, e todas as unidades compartilhadas nas quais o solicitante é um administrador são retornadas.</p> <p>Selecione a unidade compartilhada onde o documento que você deseja baixar está localizado e selecione o documento.</p> <p>Observação: se você tiver selecionado a opção [!DNL Google Docs] neste campo e não for um usuário [!DNL Google Workspace], o erro <code>[400] Invalid Value</code> será retornado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo] </p> </td> 
   <td> <p>Selecione o formato de arquivo de destino do documento baixado.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir um documento]

Este módulo de ação exclui um documento.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma Unidade]</td> 
   <td> <p>Selecione o tipo de unidade onde o documento que você deseja excluir está localizado.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Minha Unidade]</strong> </p> <p>Selecione a pasta onde o documento que você deseja excluir está localizado e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartilhado Comigo]</strong> </p> <p>Selecione a pasta onde o documento que você deseja excluir está localizado e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidade Compartilhada]</strong> (disponível somente para [!DNL Google Workspace] usuários)</p> <p>Selecione se você deseja [!UICONTROL Usar Acesso de Administrador de Domínio]. Selecionar [!UICONTROL Sim] emite a solicitação como administrador de domínio, e todas as unidades compartilhadas nas quais o solicitante é um administrador são retornadas.</p> <p>Selecione a unidade compartilhada onde o documento que você deseja excluir está localizado e selecione o documento.</p> <p>Observação: se você tiver selecionado a opção [!DNL Google Docs] neste campo e não for um usuário [!DNL Google Workspace], o erro <code>[400] Invalid Value</code> será retornado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Unidade Compartilhada]</td> 
   <td> <p>Selecione a unidade que contém o documento a ser baixado e selecione um documento. Esta opção estará disponível se você tiver selecionado [!DNL Google Docs] no campo [!UICONTROL Escolher uma Unidade].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Documento]</td> 
   <td> <p> Selecione ou mapeie o documento no qual deseja substituir uma ou mais imagens.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Outro

* [[!UICONTROL Fazer uma chamada de API]](#make-an-api-call)
* [[!UICONTROL Tornar todos os links em um documento clicáveis]](#make-all-links-in-a-document-clickable)

#### [!UICONTROL Fazer uma chamada de API]

Esse módulo de ação permite executar uma chamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Insira um caminho relativo para <code>https://docs.googleapis.com/</code>. Exemplo: <code>/v1/documents/{presentationID}</code>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação na forma de um objeto JSON padrão. Por exemplo, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] adiciona os cabeçalhos de autorização para você.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadeia de Consulta]</td> 
   <td> <p> Insira a string de consulta da solicitação.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada à API na forma de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar instruções condicionais como <code>if</code> em seu JSON, coloque as aspas fora da instrução condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Exemplo:** a chamada de API a seguir recupera os detalhes do documento especificado em sua Google Docs:

**URL:**

/v1/documents/1ujkf-GDgB0TQSYPrxbCSK4Uso54tHVMqHZEVZZxB6aY

**Método:**

[!UICONTROL GET]

![](assets/api-call-example.png)

Detalhes do documento recuperado podem ser encontrados na Saída do módulo em [!UICONTROL Pacote] > [!UICONTROL Corpo].

![](assets/api-output.png)

#### [!UICONTROL Tornar todos os links em um documento clicáveis]

Este módulo de ação encontra todos os links no documento e os torna clicáveis.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Criar Todos os Links em um Documento]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Por Mapeamento]</strong> <br>Selecione esta opção para mapear o modelo de documento.</li> 
     <li><strong>[!UICONTROL Por Lista Suspensa]</strong> <br> Selecione esta opção para escolher o documento no menu suspenso.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma Unidade]</td> 
   <td> <p>Selecione o tipo de unidade em que o documento no qual você deseja tornar os links clicáveis está localizado. Esta opção estará disponível se você tiver selecionado [!UICONTROL Por Lista Suspensa] no campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Minha Unidade]</strong> </p> <p>Selecione a pasta onde está localizado o documento no qual você deseja tornar os links clicáveis e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartilhado Comigo]</strong> </p> <p>Selecione a pasta onde está localizado o documento no qual você deseja tornar os links clicáveis e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidade Compartilhada]</strong> (disponível somente para [!DNL Google Workspace] usuários)</p> <p>Selecione se você deseja [!UICONTROL Usar Acesso de Administrador de Domínio]. Selecionar [!UICONTROL Sim] emite a solicitação como administrador de domínio, e todas as unidades compartilhadas nas quais o solicitante é um administrador são retornadas.</p> <p>Selecione a unidade compartilhada onde está localizado o documento no qual você deseja tornar os links clicáveis e selecione o documento.</p> <p>Observação: se você tiver selecionado a opção [!DNL Google Docs] neste campo e não for um usuário [!DNL Google Workspace], o erro <code>[400] Invalid Value</code> será retornado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Unidade Compartilhada]</td> 
   <td> <p>Selecione a unidade que contém o documento no qual você deseja atualizar os links e selecione um documento. Esta opção estará disponível se você tiver selecionado [!DNL Google Docs] no campo [!UICONTROL Escolher uma Unidade].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Documento]</td> 
   <td> <p> Selecione ou mapeie o documento no qual deseja atualizar os links.</p> </td> 
  </tr> 
 </tbody> 
</table>
