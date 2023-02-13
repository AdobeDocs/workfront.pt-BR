---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos Google Docs
description: O Adobe Workfront Fusion [!DNL Google Docs] os módulos permitem monitorar, criar, editar e recuperar documentos em seu [!DNL Google Docs] e [!DNL Google Docs] (para usuários do [!DNL G Suite]).
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: fbe7d628-d833-43ce-83b8-8e4e6a812fd1
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '4042'
ht-degree: 0%

---

# [!DNL Google Docs] módulos

O [!DNL Adobe Workfront Fusion] [!DNL Google Docs] os módulos permitem monitorar, criar, editar e recuperar documentos em seu [!DNL Google Docs] e [!DNL Google Docs] para [!DNL G Suite] usuários).

Para usar [!DNL Google Docs] com [!DNL Adobe Workfront Fusion], é necessário ter um [!DNL Google] conta. Se você não tiver um [!DNL Google] ainda assim, você pode criar uma no [!DNL Google] Página de ajuda da conta.

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

Para usar [!DNL Google Docs] , você deve ter uma conta Google.

## [!DNL Google Docs] módulos e seus campos

Ao configurar [!DNL Google Docs] módulos, [!UICONTROL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Google Docs] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Documento

* [[!UICONTROL Ver documentos]](#watch-documents)
* [[!UICONTROL Listar Documentos]](#list-documents)
* [[!UICONTROL Obter o conteúdo de um documento]](#get-content-of-a-document)
* [[!UICONTROL Criar um documento]](#create-a-document)
* [[!UICONTROL Criar um documento a partir de um modelo]](#create-a-document-from-a-template)
* [[!UICONTROL Inserir um Parágrafo em um Documento]](#insert-a-paragraph-to-a-document)
* [[!UICONTROL Inserir uma imagem em um documento]](#insert-an-image-to-a-document)
* [[!UICONTROL Substituir uma imagem por uma nova imagem]](#replace-an-image-with-a-new-image)
* [[!UICONTROL Substituir texto em um documento]](#replace-text-in-a-document)
* [[!UICONTROL Baixar um documento]](#download-a-document)
* [[!UICONTROL Excluir um documento]](#delete-a-document)

#### [!UICONTROL Ver documentos]

Este módulo de acionador retorna detalhes do documento quando um novo documento é criado ou modificado na pasta selecionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ver documentos]</td> 
   <td> <p style="color: #000000;">Selecione se deseja ver os documentos criados ([!UICONTROL por data de criação]) ou modificados do ([!UICONTROL por data de modificação]).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma unidade]</td> 
   <td> <p>Selecione o tipo de unidade que deseja monitorar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Minha unidade]</strong> </p> <p>Selecione a pasta que deseja visualizar para documentos criados ou modificados.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartilhado Comigo]</strong> </p> <p>Selecione a pasta que deseja visualizar para documentos criados ou modificados.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidade compartilhada]</strong> (disponível para [!DNL G Suite] somente usuários)</p> <p>Selecione se deseja [!UICONTROL Usar acesso de administrador de domínio]. Selecionar [!UICONTROL Sim] emite a solicitação como administrador de domínio e todas as unidades compartilhadas nas quais o solicitante é um administrador são retornadas.</p> <p>Selecione a unidade compartilhada que deseja assistir.</p> <p>Observação: Se você selecionou a variável [!DNL Google Shared Drive] neste campo e você não é uma [!DNL G Suite] usuário, o erro <code>[400] Invalid Value</code> é retornado.</p> </li> 
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
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma unidade]</td> 
   <td> <p>Selecione o tipo de unidade da qual deseja listar documentos.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Minha unidade]</strong> </p> <p>Selecione a pasta da qual deseja listar documentos.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartilhado Comigo]</strong> </p> <p>Selecione a pasta da qual deseja listar documentos.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidade compartilhada]</strong> (disponível para [!DNL G Suite] somente usuários)</p> <p>Selecione se deseja [!UICONTROL Usar acesso de administrador de domínio]. Selecionar [!UICONTROL Sim] emite a solicitação como administrador de domínio e todas as unidades compartilhadas nas quais o solicitante é um administrador são retornadas.</p> <p>Selecione a unidade compartilhada da qual deseja listar documentos.</p> <p>Observação: Se você selecionou a variável [!DNL Google Docs] neste campo e você não é uma [!DNL G Suite] usuário, o erro <code>[400] Invalid Value</code> é retornado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite] </td> 
   <td> <p>Definir o número máximo de documentos [!DNL Workfront Fusion] retorna em um ciclo de execução.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter o conteúdo de um documento]

Este módulo de ação recupera um documento especificado.

Talvez seja necessário estender suas permissões.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obter conteúdo de um documento]</td> 
   <td> <p>Selecione se deseja mapear a ID do documento do documento ou selecione o documento no menu suspenso manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma unidade]</td> 
   <td> <p>Selecione o tipo de unidade que contém o documento que deseja recuperar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Minha unidade]</strong> </p> <p>Selecione a pasta que contém o documento que deseja recuperar.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartilhado Comigo]</strong> </p> <p>Selecione a pasta que contém o documento que deseja recuperar.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidade compartilhada]</strong> (disponível para [!DNL G Suite] somente usuários)</p> <p>Selecione se deseja [!UICONTROL Usar acesso de administrador de domínio]. Selecionar [!UICONTROL Sim] emite a solicitação como administrador de domínio e todas as unidades compartilhadas nas quais o solicitante é um administrador são retornadas.</p> <p>Selecione a unidade compartilhada que contém o documento que você deseja recuperar.</p> <p>Observação: Se você selecionou a variável [!DNL Google Docs] neste campo e você não é uma [!DNL G Suite] usuário, o erro <code>[400] Invalid Value</code> é retornado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filtro]</p> </td> 
   <td> <p>Selecione o objeto que deseja retornar na saída do módulo.</p> 
    <ul> 
     <li>[!UICONTROL Image] (padrão)</li> 
     <li>[!UICONTROL Desenho]</li> 
     <li>[!UICONTROL Gráfico]</li> 
    </ul> <p>Nota:  <p>Para mais mapeamento desses objetos, use o valor [!UICONTROL Inline Objects Array] na saída deste módulo (em vez de [!UICONTROL inlineObjects]).</p> <p>Os objetos [!UICONTROL Inline Objects Array] são classificados na mesma ordem em que aparecem no documento. Isso facilitará qualquer processamento adicional.</p> </p> </td> 
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
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Insira o nome do documento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conteúdo]</td> 
   <td> <p>Insira o conteúdo do documento. HTML é suportado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma unidade]</td> 
   <td> <p>Selecione o tipo de unidade em que deseja criar um documento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Minha unidade]</strong> </p> <p>Selecione a pasta onde deseja criar um documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartilhado Comigo]</strong> </p> <p>Selecione a pasta onde deseja criar um documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidade compartilhada]</strong> (disponível para [!DNL G Suite] somente usuários)</p> <p>Selecione se deseja [!UICONTROL Usar acesso de administrador de domínio]. Selecionar [!UICONTROL Sim] emite a solicitação como administrador de domínio e todas as unidades compartilhadas nas quais o solicitante é um administrador são retornadas.</p> <p>Selecione a unidade compartilhada na qual deseja criar um documento.</p> <p>Observação: Se você selecionou a variável [!DNL Google Docs] neste campo e você não é uma [!DNL G Suite] usuário, o erro <code>[400] Invalid Value</code> é retornado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir um cabeçalho]</td> 
   <td> <p> Habilite esta opção para inserir o cabeçalho no documento, em seguida, insira ou mapeie o texto do cabeçalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir um rodapé] </td> 
   <td> <p>Habilite esta opção para inserir o rodapé no documento, em seguida, insira ou mapeie o texto do cabeçalho.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar um documento a partir de um modelo]

Esse módulo de ação cria uma cópia de um documento de modelo existente e substitui qualquer tag. Esse módulo também permite que os usuários substituam imagens por novas imagens por URL.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Criar um documento de um modelo]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL por mapeamento]</strong> <br>Selecione esta opção para mapear o modelo de documento.</li> 
     <li><strong>[!UICONTROL por lista suspensa]</strong> <br>Selecione essa opção para escolher o modelo de documento no menu suspenso.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma unidade]</td> 
   <td> <p>Selecione o tipo de unidade em que seu modelo está localizado. Essa opção estará disponível se você tiver selecionado [!UICONTROL por lista suspensa] no campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Minha unidade]</strong> </p> <p>Selecione a pasta onde seu template está localizado.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartilhado Comigo]</strong> </p> <p>Selecione a pasta onde seu template está localizado.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidade compartilhada]</strong> (disponível para [!DNL G Suite] somente usuários)</p> <p>Selecione se deseja [!UICONTROL Usar acesso de administrador de domínio]. Selecionar [!UICONTROL Sim] emite a solicitação como administrador de domínio e todas as unidades compartilhadas nas quais o solicitante é um administrador são retornadas.</p> <p>Selecione a unidade compartilhada na qual o modelo está localizado.</p> <p>Observação: Se você selecionou a variável [!DNL Google Docs] neste campo e você não é uma [!DNL G Suite] usuário, o erro <code>[400] Invalid Value</code> é retornado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Valores]</p> </td> 
   <td> <p>Insira os valores que serão inseridos em vez das variáveis para o novo documento.</p> 
    <ul> 
     <li><strong>[!UICONTROL Tags]</strong> <br>Insira as tags contidas no template do documento. Não utilizar <code>&#123;&#123;&#125;&#125;</code>. Exemplo: use <code>name</code> em vez de <code>&#123;&#123;name&#125;&#125;</code>.</li> 
     <li><strong>[!UICONTROL Valor substituído]</strong><br>Insira o valor da tag.</li> 
    </ul> <p>Por exemplo, a variável<code> &#123;&#123;name&#125;&#125;</code> no documento de origem será exibida como o campo de nome aqui, onde o valor pode ser inserido, como <code>John</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Substituição de imagens]</p> </td> 
   <td> <p>Insira o link para a [!UICONTROL Image Object ID] e a [!UICONTROL Image URL] que substituirão a imagem atual.</p> <p>Observação: Você pode recuperar as IDs de imagem usando o módulo [!UICONTROL Obter um documento], onde as IDs estão contidas na matriz [!UICONTROL Inline Object Array].</p> <p>Recomendamos que você adicione texto ALT a imagens em seu [!DNL Google] documento. </p> <p>Para adicionar um texto ALT à [!DNL Google Docs] imagem:</p> 
    <ol> 
     <li value="1">Clique com o botão direito na imagem.</li> 
     <li value="2">Selecione a opção [!UICONTROL ALT text] .</li> 
     <li value="3">Insira o [!UICONTROL ALT text] no campo [!UICONTROL Título] e clique em [!UICONTROL OK].</li> 
    </ol> <p>Depois que o texto ALT é adicionado à imagem, o texto ALT é exibido no nome do campo entre parênteses.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Título] </td> 
   <td> <p>Insira o nome do novo documento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma unidade]</td> 
   <td> <p>Selecione o tipo de unidade em que seu modelo está localizado. Essa opção estará disponível se você tiver selecionado [!UICONTROL por lista suspensa] no campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Minha unidade]</strong> </p> <p>Selecione a pasta onde deseja que o documento seja criado.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartilhado Comigo]</strong> </p> <p>Selecione a pasta onde deseja que o documento seja criado.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidade compartilhada]</strong> (disponível para [!DNL G Suite] somente usuários)</p> <p>Selecione se deseja [!UICONTROL Usar acesso de administrador de domínio]. Selecionar [!UICONTROL Sim] emite a solicitação como administrador de domínio e todas as unidades compartilhadas nas quais o solicitante é um administrador são retornadas.</p> <p>Selecione a unidade compartilhada na qual deseja que o documento seja criado.</p> <p>Observação: Se você selecionou a variável [!DNL Google Docs] neste campo e você não é uma [!DNL G Suite] usuário, o erro <code>[400] Invalid Value</code> é retornado.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Inserir um Parágrafo em um Documento]

Esse módulo de ação anexa ou insere um novo parágrafo a um documento existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Selecionar um documento]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL por mapeamento]</strong> <br>Selecione esta opção para mapear o documento.</li> 
     <li><strong>[!UICONTROL por lista suspensa]</strong> <br> Selecione essa opção para escolher o documento no menu suspenso.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma unidade]</td> 
   <td> <p>Selecione o tipo de unidade na qual o documento ao qual deseja adicionar um parágrafo está localizado. Essa opção estará disponível se você tiver selecionado [!UICONTROL por lista suspensa] no campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Minha unidade]</strong> </p> <p>Selecione a pasta onde o documento que deseja adicionar um parágrafo está localizado e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartilhado Comigo]</strong> </p> <p>Selecione a pasta onde o documento que deseja adicionar um parágrafo está localizado e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidade compartilhada]</strong> (disponível para [!DNL G Suite] somente usuários)</p> <p>Selecione se deseja [!UICONTROL Usar acesso de administrador de domínio]. Selecionar [!UICONTROL Sim] emite a solicitação como administrador de domínio e todas as unidades compartilhadas nas quais o solicitante é um administrador são retornadas.</p> <p>Selecione a unidade compartilhada na qual o documento ao qual você deseja adicionar um parágrafo está localizado e selecione o documento.</p> <p>Observação: Se você selecionou a variável [!DNL Google Docs] neste campo e você não é uma [!DNL G Suite] usuário, o erro <code>[400] Invalid Value</code> é retornado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Inserir um parágrafo]</p> </td> 
   <td> <p>Selecione como deseja que o novo texto seja inserido no documento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Pela especificação da localização]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Por índice]</strong> </p> 
        <ul> 
         <li> <p><strong>[!UICONTROL Índice]</strong> </p> <p>Insira o Número do índice no qual você deseja inserir o texto. Você pode usar o módulo [!UICONTROL Obter um documento] para recuperar o número do índice.</p> <p>Para exibir todos os caracteres (inclusive ocultos) no documento, você pode usar o complemento [!UICONTROL Show]. Você pode encontrar o complemento em [!UICONTROL Complementos] &gt; [!UICONTROL Obter complementos]. Procure por [!UICONTROL Show] e instale o complemento [!UICONTROL Show].</p> </li> 
         <li> <p><strong>[!UICONTROL Texto inserido]</strong> </p> <p>Insira o texto que deseja inserir no documento.</p> </li> 
        </ul> </li> 
       <li> <p><strong>[!UICONTROL Por ID de segmento]</strong> </p> <p>Selecione o cabeçalho e o rodapé para os quais deseja inserir o conteúdo do texto e insira o texto que deseja inserir nos campos correspondentes.</p> <p>Se o cabeçalho ou rodapé já contiver texto, o novo texto será adicionado antes do texto existente.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Ao anexar ao corpo do documento]</strong> </p> <p>Anexa o texto inserido no final do conteúdo do corpo do documento.</p> <p>O estilo do novo parágrafo será copiado do parágrafo no índice de inserção atual, incluindo listas e marcadores.</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL Ao anexar ao final do segmento (Cabeçalho e Rodapé)]</strong> </p> <p>Selecione o cabeçalho e o rodapé para os quais deseja inserir o conteúdo do texto e insira o texto que deseja inserir nos campos correspondentes.</p> <p>Se o cabeçalho ou rodapé já contiver texto, o novo texto será adicionado após o texto existente.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Texto anexado]</td> 
   <td>Inserir ou mapear o texto que deseja anexar ao documento</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Inserir uma imagem em um documento]

Esse módulo de ação insere uma imagem do URL para o documento.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Selecionar um documento]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL por mapeamento]</strong> <br>Selecione esta opção para mapear o modelo de documento.</li> 
     <li><strong>[!UICONTROL por lista suspensa]</strong> <br> Selecione essa opção para escolher o documento no menu suspenso.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma unidade]</td> 
   <td> <p>Selecione o tipo de unidade em que o documento ao qual deseja adicionar uma imagem está localizado. Essa opção estará disponível se você tiver selecionado [!UICONTROL por lista suspensa] no campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Minha unidade]</strong> </p> <p>Selecione a pasta na qual o documento que deseja adicionar uma imagem está localizado e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartilhado Comigo]</strong> </p> <p>Selecione a pasta na qual o documento que deseja adicionar uma imagem está localizado e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidade compartilhada]</strong> (disponível para [!DNL G Suite] somente usuários)</p> <p>Selecione se deseja [!UICONTROL Usar acesso de administrador de domínio]. Selecionar [!UICONTROL Sim] emite a solicitação como administrador de domínio e todas as unidades compartilhadas nas quais o solicitante é um administrador são retornadas.</p> <p>Selecione a unidade compartilhada na qual o documento ao qual deseja adicionar uma imagem está localizado e selecione o documento.</p> <p>Observação: Se você selecionou a variável [!DNL Google Docs] neste campo e você não é uma [!DNL G Suite] usuário, o erro <code>[400] Invalid Value</code> é retornado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Inserir uma imagem]</p> </td> 
   <td> <p>Selecione como deseja que a nova imagem seja inserida no documento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Pela especificação da localização]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Por índice]</strong> </p> 
        <ul> 
         <li> <p><strong>[!UICONTROL Índice]</strong> </p> <p>Insira o Número do índice no qual você deseja inserir a imagem. Você pode usar o módulo [!UICONTROL Obter um documento] para recuperar [!UICONTROL Número do índice].</p> <p>Para exibir todos os caracteres (inclusive ocultos) no documento, você pode usar o complemento [!UICONTROL Show]. Você pode encontrar o complemento em [!UICONTROL Complementos] &gt; [!UICONTROL Obter complementos]. Procure por [!UICONTROL Show] e instale o complemento [!UICONTROL Show].</p> </li> 
         <li> <p><strong>[!UICONTROL Image URL]</strong> </p> <p>Insira o URL da imagem que deseja inserir no documento.</p> <p>O tamanho máximo da imagem é de 50 MB. Não deve exceder 25 megapixels. Somente o formato PNG, JPEG ou GIF é compatível.</p> </li> 
        </ul> </li> 
       <li> <p><strong>[!UICONTROL Por ID de segmento]</strong> </p> <p>Selecione o cabeçalho e o rodapé para os quais deseja inserir a imagem e insira o URL da imagem nos campos correspondentes.</p> <p>O tamanho máximo da imagem é de 50 MB. A imagem não deve exceder 25 megapixels. Somente o formato PNG, JPEG ou GIF é compatível.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Ao anexar ao corpo do documento]</strong> </p> <p>Anexa uma imagem específica ao final do conteúdo do corpo do documento.</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL Ao anexar ao final do segmento (Cabeçalho e Rodapé)]</strong> </p> <p>Selecione o cabeçalho e o rodapé para os quais deseja inserir uma imagem e insira o URL da imagem que deseja inserir nos campos correspondentes.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Amplitude da altura em pontos/Amplitude da largura em pontos]</p> </td> 
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
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Selecionar um documento]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL por mapeamento]</strong> <br>Selecione esta opção para mapear o modelo de documento.</li> 
     <li><strong>[!UICONTROL por lista suspensa]</strong> <br> Selecione essa opção para escolher o documento no menu suspenso.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma unidade]</td> 
   <td> <p>Selecione o tipo de unidade em que o documento que você deseja substituir uma imagem está localizado. Essa opção estará disponível se você tiver selecionado [!UICONTROL por lista suspensa] no campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Minha unidade]</strong> </p> <p>Selecione a pasta onde está localizado o documento que você deseja substituir uma imagem e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartilhado Comigo]</strong> </p> <p>Selecione a pasta onde está localizado o documento que você deseja substituir uma imagem e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidade compartilhada]</strong> (disponível para [!DNL G Suite] somente usuários)</p> <p>Selecione se deseja [!UICONTROL Usar acesso de administrador de domínio]. Selecionar [!UICONTROL Sim] emite a solicitação como administrador de domínio e todas as unidades compartilhadas nas quais o solicitante é um administrador são retornadas.</p> <p>Selecione a unidade compartilhada na qual o documento que você deseja substituir uma imagem está localizado e selecione o documento.</p> <p>Observação: Se você selecionou a variável [!DNL Google Docs] neste campo e você não é uma [!DNL G Suite] usuário, o erro <code>[400] Invalid Value</code> é retornado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Image URL]</p> </td> 
   <td> <p>Insira ou mapeie o URL da nova imagem que substituirá a imagem existente.</p> <p>As imagens são listadas na ordem em que aparecem no documento. Por exemplo, <code>Body: Image No. 1</code> é a primeira imagem no documento.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Substituir texto em um documento]

Esse módulo de ação substitui o texto em um documento.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Selecionar um documento]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL por mapeamento]</strong> <br>Selecione esta opção para mapear o modelo de documento.</li> 
     <li><strong>[!UICONTROL por lista suspensa]</strong> <br> Selecione essa opção para escolher o documento no menu suspenso.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma unidade]</td> 
   <td> <p>Selecione o tipo de unidade na qual o documento ao qual deseja adicionar texto está localizado. Essa opção estará disponível se você tiver selecionado [!UICONTROL por lista suspensa] no campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Minha unidade]</strong> </p> <p>Selecione a pasta na qual o documento que deseja adicionar texto está localizado e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartilhado Comigo]</strong> </p> <p>Selecione a pasta na qual o documento que deseja adicionar texto está localizado e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidade compartilhada]</strong> (disponível para [!DNL G Suite] somente usuários)</p> <p>Selecione se deseja [!UICONTROL Usar acesso de administrador de domínio]. Selecionar [!UICONTROL Sim] emite a solicitação como administrador de domínio e todas as unidades compartilhadas nas quais o solicitante é um administrador são retornadas.</p> <p>Selecione a unidade compartilhada na qual o documento ao qual deseja adicionar texto está localizado e selecione o documento.</p> <p>Observação: Se você selecionou a variável [!DNL Google Docs] neste campo e você não é uma [!DNL G Suite] usuário, o erro <code>[400] Invalid Value</code> é retornado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Substituir um texto]</p> </td> 
   <td> <p>Adicione cada texto que você deseja substituir.</p> 
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
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma unidade]</td> 
   <td> <p>Selecione o tipo de unidade onde o documento que deseja baixar está localizado.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Minha unidade]</strong> </p> <p>Selecione a pasta onde o documento que deseja baixar está localizado e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartilhado Comigo]</strong> </p> <p>Selecione a pasta onde o documento que deseja baixar está localizado e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidade compartilhada]</strong> (disponível para [!DNL G Suite] somente usuários)</p> <p>Selecione se deseja [!UICONTROL Usar acesso de administrador de domínio]. Selecionar [!UICONTROL Sim] emite a solicitação como administrador de domínio e todas as unidades compartilhadas nas quais o solicitante é um administrador são retornadas.</p> <p>Selecione a unidade compartilhada na qual o documento que você deseja baixar está localizado e selecione o documento.</p> <p>Observação: Se você selecionou a variável [!DNL Google Docs] neste campo e você não é uma [!DNL G Suite] usuário, o erro <code>[400] Invalid Value</code> é retornado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo] </p> </td> 
   <td> <p>Selecione o formato de arquivo de destino do documento baixado.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir um documento]

Esse módulo de ação exclui um documento.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma unidade]</td> 
   <td> <p>Selecione o tipo de unidade onde o documento que deseja excluir está localizado.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Minha unidade]</strong> </p> <p>Selecione a pasta onde o documento que deseja excluir está localizado e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartilhado Comigo]</strong> </p> <p>Selecione a pasta onde o documento que deseja excluir está localizado e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidade compartilhada]</strong> (disponível para [!DNL G Suite] somente usuários)</p> <p>Selecione se deseja [!UICONTROL Usar acesso de administrador de domínio]. Selecionar [!UICONTROL Sim] emite a solicitação como administrador de domínio e todas as unidades compartilhadas nas quais o solicitante é um administrador são retornadas.</p> <p>Selecione a unidade compartilhada na qual o documento que deseja excluir está localizado e selecione o documento.</p> <p>Observação: Se você selecionou a variável [!DNL Google Docs] neste campo e você não é uma [!DNL G Suite] usuário, o erro <code>[400] Invalid Value</code> é retornado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Unidade compartilhada]</td> 
   <td> <p>Selecione a unidade que contém o documento que você deseja baixar e selecione um documento. Essa opção estará disponível se você tiver selecionado [!DNL Google Docs] no campo [!UICONTROL Escolher uma unidade] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do documento]</td> 
   <td> <p> Selecione ou mapeie o documento em que deseja substituir uma ou mais imagens.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Outro

* [[!UICONTROL Faça uma chamada de API]](#make-an-api-call)
* [[!UICONTROL Tornar todos os links em um documento clicáveis]](#make-all-links-in-a-document-clickable)

#### [!UICONTROL Faça uma chamada de API]

Esse módulo de ação permite executar uma chamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Insira um caminho relativo a <code>https://docs.googleapis.com/</code>. Exemplo: <code>/v1/documents/{presentationID}</code>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Selecione o método de solicitação HTTP que você precisa configurar a chamada da API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão. Por exemplo, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] adiciona os cabeçalhos de autorização para você.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sequência de consulta]</td> 
   <td> <p> Insira a sequência de consulta da solicitação.</p> </td> 
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

**Exemplo:** A chamada à API a seguir recupera os detalhes do documento especificado em sua documentação da Google:

**URL:**

/v1/documents/1ujkf-GDgB0TQSYPrxbCSK4Uso54tHVMqHZEVZZxB6aY

**Método:**

[!UICONTROL GET]

![](assets/api-call-example.png)

Detalhes do documento recuperado podem ser encontrados na Saída do módulo em [!UICONTROL Pacote] > [!UICONTROL Corpo].

![](assets/api-output.png)

#### [!UICONTROL Tornar todos os links em um documento clicáveis]

Esse módulo de ação encontra todos os links no documento e os torna clicáveis.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Criar todos os links em um documento]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL por mapeamento]</strong> <br>Selecione esta opção para mapear o modelo de documento.</li> 
     <li><strong>[!UICONTROL por lista suspensa]</strong> <br> Selecione essa opção para escolher o documento no menu suspenso.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma unidade]</td> 
   <td> <p>Selecione o tipo de unidade em que o documento em que você deseja tornar os links clicáveis está localizado. Essa opção estará disponível se você tiver selecionado [!UICONTROL por lista suspensa] no campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Minha unidade]</strong> </p> <p>Selecione a pasta na qual o documento na qual você deseja tornar os links clicáveis está localizado e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartilhado Comigo]</strong> </p> <p>Selecione a pasta na qual o documento na qual você deseja tornar os links clicáveis está localizado e selecione o documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidade compartilhada]</strong> (disponível para [!DNL G Suite] somente usuários)</p> <p>Selecione se deseja [!UICONTROL Usar acesso de administrador de domínio]. Selecionar [!UICONTROL Sim] emite a solicitação como administrador de domínio e todas as unidades compartilhadas nas quais o solicitante é um administrador são retornadas.</p> <p>Selecione a unidade compartilhada na qual o documento no qual você deseja tornar os links clicáveis está localizado e selecione o documento.</p> <p>Observação: Se você selecionou a variável [!DNL Google Docs] neste campo e você não é uma [!DNL G Suite] usuário, o erro <code>[400] Invalid Value</code> é retornado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Unidade compartilhada]</td> 
   <td> <p>Selecione a unidade que contém o documento no qual você deseja atualizar os links e, em seguida, selecione um documento. Essa opção estará disponível se você tiver selecionado [!DNL Google Docs] no campo [!UICONTROL Escolher uma unidade].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do documento]</td> 
   <td> <p> Selecione ou mapeie o documento no qual deseja atualizar os links.</p> </td> 
  </tr> 
 </tbody> 
</table>
