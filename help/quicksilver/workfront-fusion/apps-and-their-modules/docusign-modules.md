---
title: Módulos do DocuSign
description: Os  [!DNL Adobe Workfront Fusion DocuSign] módulos permitem que você monitore e recupere o status do envelope, pesquise e recupere envelopes, ou baixe e envie um documento para entrar em sua  [!DNL DocuSign] conta.
author: Becky
draft: Probably
feature: Workfront Fusion, Digital Content and Documents
exl-id: a6ebfe6f-dc3f-41f7-8129-bbc5775cff33
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '1946'
ht-degree: 0%

---

# Módulos do DocuSign

Os módulos do [!DNL Adobe Workfront Fusion] [!DNL DocuSign] permitem que você monitore e recupere o status dos envelopes, pesquise e recupere envelopes, ou baixe e envie um documento para entrar em sua conta do [!DNL DocuSign].

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

## Pré-requisitos

Para usar módulos [!DNL DocuSign], você deve ter uma conta [!DNL DocuSign].

## Conectar [!DNL DocuSign] a [!DNL Workfront Fusion] {#connect-docusign-to-workfront-fusion}

Para criar uma conexão para seus módulos do [!DNL DocuSign]:

1. Clique em **[!UICONTROL Adicionar]** ao lado da caixa [!UICONTROL Conexão] ao começar a configurar o primeiro módulo [!DNL DocuSign].
1. Insira o seguinte:

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nome da Conexão]</p> </td> 
      <td>Digite um nome para a nova conexão [!DNL DocuSign]</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo de conta]</td> 
      <td>Selecione se a conta à qual deseja se conectar é uma conta de produção ou uma conta de demonstração.</td> 
     </tr> 
    </tbody> 
   </table>

1. Continue conforme descrito em [Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas](../../workfront-fusion/connections/connect-to-fusion-general.md#connect).

## [!DNL DocuSign] módulos e seus campos

Ao configurar módulos do [!DNL DocuSign], o [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos [!DNL DocuSign] adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Ações](#actions)

### Triggers

#### [!UICONTROL Assistir a envelopes]

Esse módulo de acionamento inicia um cenário quando um envelope é enviado, entregue, assinado, concluído ou recusado.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL DocuSign] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conta] </td> 
   <td> <p>Selecione a conta que contém os registros que você deseja observar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de evento]</td> 
   <td> <p> Selecione o tipo de evento que deseja assistir.</p> 
    <ul> 
     <li>[!UICONTROL Documento concluído]</li> 
     <li>[!UICONTROL Documento recusado]</li> 
     <li>[!UICONTROL Documento enviado]</li> 
     <li>[!UICONTROL Documento assinado]</li> 
     <li>[!UICONTROL Novo documento na Caixa de Entrada]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Campos de saída]</p> </td> 
   <td> <p>Selecione os campos que deseja incluir na saída do módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Insira ou mapeie o número máximo de registros com os quais você deseja que o módulo funcione durante cada ciclo de execução de cenário.</td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [[!UICONTROL Chamada de API personalizada]](#custom-api-call)
* [[!UICONTROL Baixar um documento]](#download-a-document)
* [[!UICONTROL Ler um envelope]](#read-an-envelope)
* [[!UICONTROL Carregar um arquivo em um envelope]](#upload-a-file-to-an-envelope)
* [[!UICONTROL Criar um novo envelope]](#create-a-new-envelope)
* [[!UICONTROL Adicionar Destinatário ao Envelope]](#add-recipient-to-envelope)
* [[!UICONTROL Adicionar campo personalizado]](#add-custom-field)
* [[!UICONTROL Modificar campo personalizado]](#modify-custom-field)
* [[!UICONTROL Enviar envelope]](#send-envelope)

#### [!UICONTROL Chamada de API personalizada]

Esse módulo de ação permite executar uma chamada de API personalizada.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL DocuSign] ao [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Conectar [!DNL DocuSign] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Conta]</td> 
   <td>Insira ou mapeie a conta que deseja usar para acessar a API [!DNL DocuSign].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>Digite o endereço no servidor Web com o qual você deseja que o módulo interaja.</p> <p>Você pode digitar uma URL relativa, o que significa que não é necessário incluir o protocolo (como <code>http://</code>) no início. Isso sugere ao servidor Web que a interação está ocorrendo no servidor.</p> <p>Por exemplo: <code>[!DNL /api/conversations].create</code></p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Método]</td> 
   <td> <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formulário de um objeto JSON padrão. Isso determina o tipo de conteúdo da solicitação.</p> <p>Por exemplo,<code> {"Content-type":"application/json"}</code></p> <p>Observação: se você estiver recebendo erros e for difícil determinar sua origem, considere modificar cabeçalhos com base na documentação [!DNL Workfront]. Se sua chamada de API personalizada retornar um erro de solicitação HTTP 422, tente usar um cabeçalho "Content-Type":"text/plain".</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cadeia de Consulta]</td> 
   <td> <p>Adicione a consulta da chamada à API na forma de um objeto JSON padrão.</p> <p>Por exemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada à API na forma de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar instruções condicionais como <code>if</code> em seu JSON, coloque as aspas fora da instrução condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limite]</td> 
   <td>Insira ou mapeie o número máximo de resultados com os quais trabalhar durante um ciclo de execução.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemplo:** Envelopes de Lista
>
>A chamada de API a seguir retorna envelopes a partir da data especificada em sua conta [!DNL DocuSign]:
>
>**URL**: `/v2.1/accounts/{accountId}/envelopes/`
>
>**Método**: `GET`
>
>**Cadeia de Caracteres de Consulta**:
>
>* **Chave**: `from_date`
>
>* **Valor**: `YYYY-MM-DD`
>
>Especifica quando a solicitação começa a verificar alterações de status para envelopes na conta.
>
>![](assets/example-docusign-setup-350x770.png)
>
>O resultado pode ser encontrado na Saída do módulo em Pacote > Corpo > envelopes.
>
>No nosso exemplo, 6 envelopes foram retornados:
>
>![](assets/docusign-example-output-350x677.png)

#### [!UICONTROL Baixar um documento]

Este módulo de ação baixa um único documento.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL DocuSign] ao [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Conectar [!DNL DocuSign] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conta] </td> 
   <td> <p>Selecione a conta que contém o documento que você deseja baixar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Envelope]</td> 
   <td> <p> Insira ou mapeie a ID do envelope que deseja baixar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de Documento]</p> </td> 
   <td> <p>Insira ou mapeie a ID do documento que deseja baixar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Certificado]</td> 
   <td>Selecione <strong>[!UICONTROL Sim]</strong> se desejar incluir o certificado de assinatura de envelope no download.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Documentos por ID de Usuário]</td> 
   <td>Selecione <strong>[!UICONTROL Yes]</strong> se você deseja permitir que os destinatários recuperem documentos por ID de Usuário. Por exemplo, se um usuário estiver incluído em duas ordens de roteiro diferentes com visibilidades diferentes, o uso dessa opção retornará todos os documentos de ambos os roteiros.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Criptografar]</td> 
   <td>Selecione <strong>[!UICONTROL Sim]</strong> se desejar que os bytes de PDF retornados na resposta sejam criptografados para todos os gerenciadores de chaves configurados na sua conta [!DNL DocuSign].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Idioma]</td> 
   <td>Selecione o idioma.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar Alterações]</td> 
   <td>Quando definido como <strong>[!UICONTROL Yes]</strong>, os campos alterados para o PDF retornado serão realçados em amarelo e as assinaturas ou iniciais opcionais serão contornadas em vermelho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Marca D'Água]</td> 
   <td> <p>Selecione <strong>[!UICONTROL No]</strong> para remover a marca d'água dos documentos PDF.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ler um envelope]

Este módulo de ação lê informações sobre um envelope em [!DNL DocuSign] usando a ID de envelope.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL DocuSign] ao [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Conectar [!DNL DocuSign] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conta] </td> 
   <td> <p>Selecione a conta que contém o documento do qual deseja ler informações.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Envelope]</td> 
   <td> <p> Insira ou mapeie a ID que contém o documento do qual você deseja ler as informações.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td>Selecione as propriedades que você deseja que apareçam na saída do módulo. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Carregar um arquivo em um envelope]

Este módulo carrega um arquivo especificado em um envelope existente no DocuSign.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL DocuSign] ao [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Conectar [!DNL DocuSign] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conta] </td> 
   <td> <p>Selecione a conta que contém o envelope no qual você deseja carregar um arquivo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Envelope]</td> 
   <td> <p> Insira ou mapeie a ID do envelope no qual deseja fazer upload de um arquivo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL arquivo Source]</td> 
   <td>Selecione um arquivo de origem de um módulo anterior ou insira o nome e os dados do arquivo de origem.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar um novo envelope]

Este módulo de ação cria um novo envelope a partir de um modelo. Ele retorna a ID do novo envelope, bem como o status do novo envelope.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexão] </td>

<td> <p>Para obter instruções sobre como conectar sua conta do DocuSign ao Workfront Fusion, consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao Workfront Fusion</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conta] </td>
   <td> <p>Selecione a conta que contém o envelope no qual você deseja carregar um arquivo.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Modelo]</td>
   <td> <p> Selecione o modelo a partir do qual deseja criar o novo envelope. Os modelos estão disponíveis com base na [!UICONTROL Account] selecionada.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">
     [!UICONTROL Após criação]
   </td> 
   <td> <p>Selecione se deseja salvar o envelope como rascunho ou enviá-lo para assinatura.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Destinatários do modelo]</td>
    <td>Selecionar o destinatário deste envelope</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Adicionar Destinatário ao Envelope]

Este módulo de ação adiciona um ou mais destinatários a um envelope existente. Se o envelope já tiver sido enviado, o recipient receberá um email. Este módulo não é válido para envelopes que já foram concluídos.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Conexão] </td>
   <td> <p>Para obter instruções sobre como conectar sua conta do DocuSign ao Workfront Fusion, consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar o aplicativo ou serviço Web do módulo ao Workfront Fusion</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Conta] </td>
   <td> <p>Selecione a conta que contém o envelope no qual deseja adicionar recipients.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL ID de Envelope]</td>
    <td>Selecione ou mapeie a ID do envelope ao qual deseja adicionar o recipient.</td>
  </tr> 
  <tr data-mc-conditions="">
    <td role="rowheader">[!UICONTROL Tipo de destinatário]</td>
   <td> <p> Selecione o tipo de destinatário que deseja adicionar ao envelope.</p> 
    <ul> 
     <li> <p>[!UICONTROL Agent]</p> </li> 
     <li> <p>[!UICONTROL Cópia carbono]</p> </li> 
     <li> <p>[!UICONTROL Entrega certificada]</p> </li> 
     <li> <p>[!UICONTROL Assinante presencial]</p> </li> 
     <li> <p>[!UICONTROL Intermediário]</p> </li> 
     <li> <p>[!UICONTROL Signatário]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Email]</td>
   <td> <p>Insira ou mapeie o endereço de email do destinatário que deseja adicionar ao envelope.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Nome]</td>
   <td>Insira ou mapeie o nome do destinatário que deseja adicionar ao envelope.</td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Ordem de roteamento]</td>
   <td> <p>Insira ou mapeie o número do roteamento do recipient. O número do banco determina a ordem na qual os destinatários recebem e assinam seus documentos.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL corpo do email]</td>
   <td>Insira ou mapeie o corpo (conteúdo) do email que é enviado ao destinatário.</td> 
  </tr> 
  <tr>
    <td role="rowheader">[!UICONTROL Assunto do email]</td>
   <td>Insira ou mapeie o assunto do email enviado ao recipient.</td> 
  </tr> 
    <td role="rowheader">[!UICONTROL Mensagem privada]</td>
   <td> <li> <p>Somente o recipient selecionado vê a mensagem privada, bem como a mensagem geral. A mensagem privada é limitada a 1000 caracteres.</p> </li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Autenticação]</td> 
   <td> <p>Selecione o método de autenticação que deseja usar para confirmar a identidade do recipient.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nenhum]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Código de acesso]</strong> </p> <p>Insira ou mapeie o código de acesso.</p> </li> 
     <li> <p><strong>[!UICONTROL Telefone]</strong> </p> <p>Insira ou mapeie o número de telefone</p> </li> 
     <li> <p><strong>[!UICONTROL SMS]</strong> </p> <p>Insira ou mapeie o número de telefone</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Adicionar campo personalizado]

Este módulo de ação adiciona um campo personalizado ao documento

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL DocuSign] ao [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Conectar [!DNL DocuSign] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conta] </td> 
   <td> <p>Selecione a conta que contém o documento ao qual você deseja adicionar um campo personalizado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Envelope]</td> 
   <td> <p> Insira ou mapeie a ID do envelope que contém o documento ao qual você deseja adicionar um campo personalizado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do campo]</td> 
   <td>Insira ou mapeie um nome para o novo campo que deseja adicionar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Necessário]</td> 
   <td>Ative essa opção se desejar que o campo adicionado seja um campo obrigatório.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar campo]</td> 
   <td>Ative essa opção se desejar que o campo fique visível.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valor]</td> 
   <td>Insira ou mapeie o valor (conteúdo) do campo adicionado. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Modificar campo personalizado]

Esse módulo de ação modifica um campo personalizado usando o nome do campo.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL DocuSign] ao [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Conectar [!DNL DocuSign] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conta] </td> 
   <td> <p>Selecione a conta que contém o documento no qual você deseja modificar um campo personalizado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Envelope]</td> 
   <td> <p> Insira ou mapeie a ID do envelope que contém o documento no qual você deseja modificar um campo personalizado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Campo]</td> 
   <td>Insira ou mapeie a ID do campo que você deseja modificar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do campo]</td> 
   <td>Insira ou mapeie o nome do campo que você deseja modificar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Necessário]</td> 
   <td>Habilite essa opção se desejar que o campo modificado seja obrigatório.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar campo]</td> 
   <td>Ative essa opção se desejar que o campo fique visível.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valor]</td> 
   <td>Insira ou mapeie o valor (conteúdo) do campo modificado. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Enviar envelope]

Esse módulo de ação envia um envelope de rascunho para seus recipients.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL DocuSign] ao [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Conectar [!DNL DocuSign] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conta] </td> 
   <td> <p>Selecione a conta que contém o envelope de rascunho que você deseja enviar aos recipients.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Envelope]</td> 
   <td> <p> Insira ou mapeie a ID do envelope de rascunho que você deseja enviar aos recipients.</p> </td> 
  </tr> 
 </tbody> 
</table>
