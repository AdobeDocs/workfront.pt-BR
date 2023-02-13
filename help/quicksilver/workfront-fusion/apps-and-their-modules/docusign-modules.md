---
title: Módulos do DocuSign
description: O [!DNL Adobe Workfront Fusion DocuSign] os módulos permitem monitorar e recuperar o status do envelope, pesquisar e recuperar envelopes ou baixar e enviar um documento para fazer logon [!DNL DocuSign] conta.
author: Becky
draft: Probably
feature: Workfront Fusion, Digital Content and Documents
exl-id: a6ebfe6f-dc3f-41f7-8129-bbc5775cff33
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1911'
ht-degree: 0%

---

# Módulos do DocuSign

O [!DNL Adobe Workfront Fusion] [!DNL DocuSign] os módulos permitem monitorar e recuperar o status do envelope, pesquisar e recuperar envelopes ou baixar e enviar um documento para fazer logon [!DNL DocuSign] conta.

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

Para usar [!DNL DocuSign] módulos, você deve ter um [!DNL DocuSign] conta.

## Connect [!DNL DocuSign] para [!DNL Workfront Fusion] {#connect-docusign-to-workfront-fusion}

Para criar uma conexão para [!DNL DocuSign] módulos:

1. Clique em **[!UICONTROL Adicionar]** ao lado do [!UICONTROL Conexão] ao começar a configurar o primeiro [!DNL DocuSign] módulo.
1. Insira o seguinte:

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nome da conexão]</p> </td> 
      <td>Insira um nome para o novo [!DNL DocuSign] conexão</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo de conta]</td> 
      <td>Selecione se a conta à qual deseja se conectar é uma conta de produção ou uma conta de demonstração.</td> 
     </tr> 
    </tbody> 
   </table>

1. Continue conforme descrito em [Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas](../../workfront-fusion/connections/connect-to-fusion-general.md#connect).

## [!DNL DocuSign] módulos e seus campos

Ao configurar [!DNL DocuSign] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL DocuSign] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Ações](#actions)

### Triggers

#### [!UICONTROL Assista aos envelopes]

Este módulo de acionador inicia um cenário quando um envelope é enviado, entregue, assinado, concluído ou recusado.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL DocuSign] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crie um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conta] </td> 
   <td> <p>Selecione a conta que contém os registros que deseja visualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de evento]</td> 
   <td> <p> Selecione o tipo de evento que você deseja assistir.</p> 
    <ul> 
     <li>[!UICONTROL Documento concluído]</li> 
     <li>[!UICONTROL Documento recusado]</li> 
     <li>[!UICONTROL Documento enviado]</li> 
     <li>[!UICONTROL Documento assinado]</li> 
     <li>[!UICONTROL Novo documento na caixa de entrada]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Campos de saída]</p> </td> 
   <td> <p>Selecione os campos que deseja incluir na saída do módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Insira ou mapeie o número máximo de registros com os quais deseja que o módulo funcione durante cada ciclo de execução de cenário.</td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [[!UICONTROL Chamada da API personalizada]](#custom-api-call)
* [[!UICONTROL Baixar um documento]](#download-a-document)
* [[!UICONTROL Ler um envelope]](#read-an-envelope)
* [[!UICONTROL Fazer upload de um arquivo para um envelope]](#upload-a-file-to-an-envelope)
* [[!UICONTROL Criar um novo envelope]](#create-a-new-envelope)
* [[!UICONTROL Adicionar Recipient ao Envelope]](#add-recipient-to-envelope)
* [[!UICONTROL Adicionar campo personalizado]](#add-custom-field)
* [[!UICONTROL Modificar campo personalizado]](#modify-custom-field)
* [[!UICONTROL Enviar envelope]](#send-envelope)

#### [!UICONTROL Chamada da API personalizada]

Esse módulo de ação permite executar uma chamada de API personalizada.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL DocuSign] para [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Conta]</td> 
   <td>Insira ou mapeie a conta que deseja usar para acessar o [!DNL DocuSign] API.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>Digite o endereço no servidor da Web com o qual você deseja que o módulo interaja.</p> <p>Você pode digitar um URL relativo, o que significa que não é necessário incluir o protocolo (como <code>http://</code>no início. Isso sugere ao servidor da Web que a interação está ocorrendo no servidor.</p> <p>Por exemplo: <code>[!DNL /api/conversations].create</code></p> <p>Dica: Para obter uma lista de endpoints disponíveis, consulte <a href="https://developers.docusign.com/esign-rest-api/reference">[!DNL DocuSign] Referência da API</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Método]</td> 
   td&gt; <p>Selecione o método de solicitação HTTP que você precisa configurar a chamada da API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão. Isso determina o tipo de conteúdo da solicitação.</p> <p>Por exemplo,<code> {"Content-type":"application/json"}</code></p> <p>Observação: Se você estiver recebendo erros e for difícil determinar sua origem, considere modificar cabeçalhos com base no [!DNL Workfront] documentação. Se a Chamada da API personalizada retornar um Erro de solicitação HTTP 422, tente usar um cabeçalho "Content-Type": "text/plain".</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sequência de consulta]</td> 
   <td> <p>Adicione a query para a chamada de API no formato de um objeto JSON padrão.</p> <p>Por exemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada da API no formato de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limite]</td> 
   <td>Insira ou mapeie o número máximo de resultados a serem trabalhados durante um ciclo de execução.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemplo:** Envelopes de lista
>
>A chamada de API a seguir retorna envelopes da data especificada em [!DNL DocuSign] conta:
>
>**URL**: `/v2.1/accounts/{accountId}/envelopes/`
>
>**Método**: `GET`
>
>**String de consulta**:
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
>Em nosso exemplo, 6 envelopes foram retornados:
>
>![](assets/docusign-example-output-350x677.png)

#### [!UICONTROL Baixar um documento]

Este módulo de ação baixa um único documento.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL DocuSign] para [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conta] </td> 
   <td> <p>Selecione a conta que contém o documento que deseja baixar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do envelope]</td> 
   <td> <p> Insira ou mapeie a ID do envelope que deseja baixar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID do documento]</p> </td> 
   <td> <p>Insira ou mapeie a ID do documento que deseja baixar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Certificado]</td> 
   <td>Selecionar <strong>[!UICONTROL Sim]</strong> se desejar incluir o certificado de assinatura de envelope no download.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Documentos por ID do usuário]</td> 
   <td>Selecionar <strong>[!UICONTROL Sim]</strong> se quiser permitir que os recipients recuperem documentos por ID de usuário. Por exemplo, se um usuário for incluído em duas ordens de roteamento diferentes com visibilidades diferentes, usar essa opção retornará todos os documentos de ambos os roteamentos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encrypt]</td> 
   <td>Selecionar <strong>[!UICONTROL Sim]</strong> se desejar que os bytes de PDF retornados na resposta sejam criptografados para todos os gerentes de chave configurados em sua [!DNL DocuSign] conta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Language]</td> 
   <td>Selecione o idioma.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar alterações]</td> 
   <td>Quando definido como <strong>[!UICONTROL Sim]</strong>, quaisquer campos alterados para o PDF retornado são realçados em amarelo e as assinaturas ou iniciais opcionais são contornadas em vermelho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Marca d'água]</td> 
   <td> <p>Selecionar <strong>[!UICONTROL n.o]</strong> remover a marca d'água dos documentos do PDF.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ler um envelope]

Este módulo de ação lê informações sobre um envelope em [!DNL DocuSign] usando a ID do envelope.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL DocuSign] para [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conta] </td> 
   <td> <p>Selecione a conta que contém o documento do qual deseja ler informações.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do envelope]</td> 
   <td> <p> Insira ou mapeie a ID que contém o documento do qual você deseja ler as informações.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td>Selecione as propriedades que deseja que apareçam na saída do módulo. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Fazer upload de um arquivo para um envelope]

Este módulo carrega um arquivo especificado em um envelope existente no DocuSign.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL DocuSign] para [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conta] </td> 
   <td> <p>Selecione a conta que contém o envelope onde deseja carregar um arquivo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do envelope]</td> 
   <td> <p> Insira ou mapeie a ID do envelope onde deseja fazer upload de um arquivo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td>Selecione um arquivo de origem de um módulo anterior ou insira o nome e os dados do arquivo de origem.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar um novo envelope]

Esse módulo de ação cria um novo envelope a partir de um template. Retorna a ID do novo envelope, bem como o status do novo envelope.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td>

<td> <p>Para obter instruções sobre como conectar sua conta do DocuSign ao Workfront Fusion, consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao Workfront Fusion</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conta] </td>
   <td> <p>Selecione a conta que contém o envelope onde deseja carregar um arquivo.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Modelo]</td>
   <td> <p> Selecione o modelo a partir do qual deseja criar o novo envelope. Os modelos estão disponíveis com base na [!UICONTROL Account] que você selecionou.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">
     [!UICONTROL Após a criação]
   </td> 
   <td> <p>Selecione se deseja salvar o envelope como rascunho ou enviá-lo para assinatura.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Destinatários do modelo]</td>
    <td>Selecione o recipient deste envelope</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Adicionar Recipient ao Envelope]

Este módulo de ação adiciona um ou mais recipients a um envelope existente. Se o envelope já tiver sido enviado, o recipient receberá um email. Este módulo não é válido para envelopes que já foram concluídos.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Connection] </td>
   <td> <p>Para obter instruções sobre como conectar sua conta do DocuSign ao Workfront Fusion, consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte o aplicativo ou o serviço da Web do módulo ao Workfront Fusion</a> no artigo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Conta] </td>
   <td> <p>Selecione a conta que contém o envelope à qual deseja adicionar recipients.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL ID do envelope]</td>
    <td>Selecione ou mapeie a ID do envelope onde deseja adicionar o recipient.</td>
  </tr> 
  <tr data-mc-conditions="">
    <td role="rowheader">[!UICONTROL Tipo de destinatário]</td>
   <td> <p> Selecione o tipo de recipient que deseja adicionar ao envelope.</p> 
    <ul> 
     <li> <p>[!UICONTROL Agent]</p> </li> 
     <li> <p>[!UICONTROL Cópia de carbono]</p> </li> 
     <li> <p>[!UICONTROL Certified delivery]</p> </li> 
     <li> <p>[!UICONTROL Assinante pessoalmente]</p> </li> 
     <li> <p>[!UICONTROL Intermediário]</p> </li> 
     <li> <p>[!UICONTROL Assinante]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Email]</td>
   <td> <p>Insira ou mapeie o endereço de email do recipient que deseja adicionar ao envelope.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Name]</td>
   <td>Insira ou mapeie o nome do recipient que deseja adicionar ao envelope.</td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Ordem de roteamento]</td>
   <td> <p>Insira ou mapeie o número do roteamento para o recipient. O número de roteamento determina a ordem em que os recipients recebem e assinam seus documentos.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Corpo do email]</td>
   <td>Insira ou mapeie o corpo (conteúdo) do email para o recipient.</td> 
  </tr> 
  <tr>
    <td role="rowheader">[!UICONTROL Assunto do email]</td>
   <td>Insira ou mapeie o assunto do email enviado para o recipient.</td> 
  </tr> 
    <td role="rowheader">[!UICONTROL Mensagem privada]</td>
   <td> <li> <p>Somente o recipient selecionado vê a mensagem privada, bem como a mensagem geral. A mensagem privada é limitada a 1000 caracteres.</p> </li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Autenticação]</td> 
   <td> <p>Selecione o método de autenticação que deseja usar para confirmar a identidade do recipient.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nenhum]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Access code]</strong> </p> <p>Insira ou mapeie o código de acesso.</p> </li> 
     <li> <p><strong>[!UICONTROL Telefone]</strong> </p> <p>Digite ou mapeie o número de telefone</p> </li> 
     <li> <p><strong>[!UICONTROL SMS]</strong> </p> <p>Digite ou mapeie o número de telefone</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Adicionar campo personalizado]

Esse módulo de ação adiciona um campo personalizado ao documento

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL DocuSign] para [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conta] </td> 
   <td> <p>Selecione a conta que contém o documento à qual deseja adicionar um campo personalizado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do envelope]</td> 
   <td> <p> Insira ou mapeie a ID do envelope que contém o documento ao qual você deseja adicionar um campo personalizado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do campo]</td> 
   <td>Insira ou mapeie um nome para o novo campo que deseja adicionar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obrigatório]</td> 
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

Este módulo de ação modifica um campo personalizado usando o nome do campo.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL DocuSign] para [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conta] </td> 
   <td> <p>Selecione a conta que contém o documento onde deseja modificar um campo personalizado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do envelope]</td> 
   <td> <p> Insira ou mapeie a ID do envelope que contém o documento no qual você deseja modificar um campo personalizado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do campo]</td> 
   <td>Insira ou mapeie a ID do campo que deseja modificar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do campo]</td> 
   <td>Insira ou mapeie o nome do campo que deseja modificar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obrigatório]</td> 
   <td>Ative essa opção se desejar que o campo modificado seja um campo obrigatório.</td> 
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

Este módulo de ação envia um envelope de rascunho para seus recipients.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL DocuSign] para [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conta] </td> 
   <td> <p>Selecione a conta que contém o envelope de rascunho que você deseja enviar para seus recipients.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do envelope]</td> 
   <td> <p> Insira ou mapeie a ID do envelope de rascunho que você deseja enviar para seus recipients.</p> </td> 
  </tr> 
 </tbody> 
</table>
