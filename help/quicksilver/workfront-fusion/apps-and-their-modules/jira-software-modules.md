---
title: Módulos de software Jira
description: Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL Jira] Software, além de conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 6437fe98-2c2b-4b49-97e2-f94b23da93fd
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2039'
ht-degree: 1%

---

# [!DNL Jira Software] módulos

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL Jira Software], bem como conectá-lo a vários aplicativos e serviços de terceiros.

Se precisar de instruções para criar um cenário, consulte [Crie um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obter informações sobre módulos, consulte [Módulos em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

<!-- Bob Fix this compared to original -->

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
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Pré-requisitos

Para usar [!DNL Jira] os módulos devem ter um [!DNL Jira] conta.

## Connect [!DNL Jira Software] para [!DNL Workfront Fusion]

Seu método de conexão se baseia no uso de [!DNL Jira Cloud] ou [!DNL Jira Server].

* [Connect [!DNL Jira Cloud] para o Workfront Fusion](#connect-jira-cloud-to-workfront-fusion)
* [Connect [!DNL Jira Server] para [!DNL Workfront Fusion]](#connect-jira-server-to-workfront-fusion)

### Connect [!DNL Jira Cloud] para [!DNL Workfront Fusion]

Connect [!DNL Jira Cloud] para [!DNL Workfront Fusion]

Para ligar [!DNL Jira Software] para [!DNL Workfront Fusion], você deve criar um token de API e inseri-lo junto com seu URL de serviço e nome de usuário no [!UICONTROL Criar uma conexão] em [!DNL Workfront Fusion].

#### Criar um token de API em [!DNL Jira]

1. Ir para [https://id.atlassian.com/manage/api-tokens](https://id.atlassian.com/manage/api-tokens) e faça logon.
1. Clique em **[!UICONTROL Criar token de API]**.
1. Digite um nome para o token, como *Workfront Fusion*.
1. Copie o token usando o **[!UICONTROL Copiar para a área de transferência]** botão.

   >[!IMPORTANT]
   >
   >Não é possível exibir o token novamente após fechar esta caixa de diálogo.
1. Armazene o token gerado em um local seguro.
1. Continue com [Configure o [!DNL Jira] Token de API em [!DNL Workfront Fusion]](#configure-the-jira-api-token-in-workfront-fusion).

#### Configure o [!DNL Jira] Token de API em [!DNL Workfront Fusion]

1. Em [!DNL Workfront Fusion], adicione um [!DNL Jira] para um cenário para abrir o **[!UICONTROL Criar uma conexão]** caixa.
1. Especifique as seguintes informações:

   * **[!UICONTROL URL de serviço]**
   * **[!UICONTROL Nome do Usuário]**
   * **[!UICONTROL Token de API]:** Esse é o token de API criado no [Criar um token de API em [!DNL Jira]](#create-an-api-token-in-jira) seção deste artigo.

1. Clique em [!UICONTROL Continuar] para criar a conexão e retornar ao módulo.

### Connect [!DNL Jira Server] para [!DNL Workfront Fusion]

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Becky: Find out and document how to find these things</p>
-->

Para autorizar uma conexão entre [!DNL Workfront Fusion] e [!DNL Jira Server], é necessário ter sua Chave do consumidor, Chave privada e URL de serviço. Talvez seja necessário entrar em contato com a [!DNL Jira] para obter essas informações.

* [Gere chaves públicas e privadas para seu [!DNL Jira] conexão](#generate-public-and-private-keys-for-your-jira-connection)
* [Configure o aplicativo do cliente como consumidor no [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)
* [Criar uma conexão com [!DNL Jira] Servidor ou data center Jira em [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### Gere chaves públicas e privadas para seu [!DNL Jira] conexão

Para adquirir uma chave privada para seu [!DNL Workfront Fusion Jira] , é necessário gerar chaves públicas e privadas.

1. No terminal, execute o seguinte `openssl` comandos.

   * `openssl genrsa -out jira_privatekey.pem 1024`

      Esse comando gera uma chave privada de 1024 bits.

   * `openssl req -newkey rsa:1024 -x509 -key jira_privatekey.pem -out jira_publickey.cer -days 365`

      Esse comando cria um certificado X509.

   * `openssl pkcs8 -topk8 -nocrypt -in jira_privatekey.pem -out jira_privatekey.pcks8`

      Este comando extrai a chave privada (formato PKCS8) para o `jira_privatekey.pcks8`
arquivo.

   * `openssl x509 -pubkey -noout -in jira_publickey.cer  > jira_publickey.pem`

      Este comando extrai a chave pública do certificado para a `jira_publickey.pem` arquivo.

      >[!NOTE]
      >
      >Se você estiver usando o Windows, talvez seja necessário salvar a chave pública no `jira_publickey.pem` arquivo manualmente:
      >
      >1. No terminal, execute o seguinte comando:
      >   
      >   `openssl x509 -pubkey -noout -in jira_publickey.cer`
      >   
      >1. Copie a saída do terminal (incluindo `-------BEGIN PUBLIC KEY--------` e `-------END PUBLIC KEY--------`
      >   
      >1. Cole a saída do terminal em um arquivo chamado `jira_publickey.pem`.



1. Continue para [Configure o aplicativo do cliente como consumidor no [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)

#### Configure o aplicativo do cliente como consumidor no [!DNL Jira]

1. Faça logon no [!DNL Jira] instância.
1. No painel de navegação esquerdo, clique em **[!UICONTROL [!DNL Jira]Configurações]** ![](assets/jira-settings-icon.png) > **[!UICONTROL Aplicativos]**> **[!UICONTROL Links de aplicativo]**.
1. No **[!UICONTROL Insira o URL do aplicativo que deseja vincular]** , insira

   ```
   https://app.workfrontfusion.com/oauth/cb/workfront-jiraserver-oauth1
   ```

1. Clique em **[!UICONTROL Criar novo link]**. Ignore a mensagem de erro &quot;Nenhuma resposta foi recebida do URL digitado&quot;.
1. No **[!UICONTROL Vincular aplicativos]** digite valores na janela **[!UICONTROL Chave do consumidor]** e **[!UICONTROL Segredo compartilhado]** campos.

   Você pode escolher os valores para esses campos.

1. Copie os valores do **[!UICONTROL Chave do consumidor]** e **[!UICONTROL Segredo compartilhado]** para um local seguro.

   Esses valores serão necessários posteriormente no processo de configuração.

1. Preencha os campos do URL da seguinte maneira:

   | Campo | Descrição |
   |---|---|
   | [!UICONTROL URL do token de solicitação] | `<Jira base url>/plugins/servlet/oauth/request-token` |
   | [!UICONTROL URL de autorização] | `<Jira base url>/plugins/servlet/oauth/authorize` |
   | [!UICONTROL URL do token de acesso] | `<Jira base url>/plugins/servlet/oauth/access-token` |

1. Selecione o **[!UICONTROL Criar link de entrada]** caixa de seleção.
1. Clique em **[!UICONTROL Continuar]**.
1. No **[!UICONTROL Vincular aplicativos]** , preencha os seguintes campos:

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Chave do consumidor]</p> </td> 
      <td> Cole na chave do consumidor que você copiou para um local seguro.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome do consumidor]</td> 
      <td>Insira um nome de sua escolha. Este nome é para sua própria referência.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Chave pública]</td> 
      <td>Cole a chave pública do <code>[!DNL jira_publickey.pem]</code> arquivo.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Continuar]**.
1. Continue para [Criar uma conexão com [!DNL Jira Server] ou [!DNL Jira Data Center] em [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### Criar uma conexão com [!DNL Jira Server] ou [!DNL Jira Data Center] em [!DNL Workfront Fusion]

>[!NOTE]
>
>Use o [!DNL Jira Server] aplicativo ao qual se conectar [!DNL Jira Server] ou [!DNL Jira Data Center].
1. Em qualquer [!DNL Jira Server] módulo em [!DNL Workfront Fusion], clique em **[!UICONTROL Adicionar]** ao lado do [!UICONTROL conexão] campo.
1. No [!UICONTROL Criar uma conexão] , preencha os seguintes campos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nome da conexão]</p> </td> 
      <td> <p>Digite um nome para a conexão</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Chave do consumidor]</td> 
      <td>Cole na chave do consumidor que você copiou para um local seguro em <a href="#configure-the-client-app-as-a-consumer-in-jira" class="MCXref xref">Configure o aplicativo do cliente como consumidor no [!DNL Jira]</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Private Key]</td> 
      <td>Cole na chave privada do <code>[!DNL jira_privatekey.pcks8]</code> arquivo criado em <a href="#generate-public-and-private-keys-for-your-jira-connection" class="MCXref xref">Gere chaves públicas e privadas para seu [!DNL Jira] conexão</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Service URL]</td> 
      <td>Insira seu [!DNL Jira] URL da instância. </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Continuar]** para criar a conexão e retornar ao módulo .

## [!DNL Jira Software] módulos e seus campos

Ao configurar [!DNL Jira Software] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Jira Software] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Ações](#actions)
* [Pesquisas](#searches)

### Triggers

#### [!UICONTROL Observar registros]

Esse módulo de acionador inicia um cenário quando um registro é adicionado, atualizado ou excluído.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Selecione o webhook que deseja usar para monitorar os registros. </p> <p>Para adicionar um novo webhook:</p> 
    <ol> 
     <li value="1">Clique em <strong>[!UICONTROL Adicionar]</strong></li> 
     <li value="2">Insira um nome para o webhook.</li> 
     <li value="3"> <p>Selecione a conexão que deseja usar para o seu webhook. </p> <p>Para obter instruções sobre como conectar seu [!DNL Jira Software] para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] para [!DNL Workfront Fusion]</a> neste artigo.</p> </li> 
     <li value="4"> <p>Selecione o tipo de registro que o software deve observar:</p> 
      <ul> 
       <li>[!UICONTROL Comentário] </li> 
       <li>[!UICONTROL Problema]</li> 
       <li>[!UICONTROL Project] </li> 
       <li>[!UICONTROL Sprint]</li> 
      </ul> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [[!UICONTROL Adicionar problema à impressão]](#add-issue-to-sprint)
* [[!UICONTROL Chamada da API personalizada]](#custom-api-call)
* [[!UICONTROL Criar um registro]](#create-a-record)
* [[!UICONTROL Excluir um registro]](#delete-a-record)
* [[!UICONTROL Baixar um anexo]](#download-an-attachment)
* [[!UICONTROL Ler um registro]](#read-a-record)
* [[!UICONTROL Atualizar um registro]](#update-a-record)

#### [!UICONTROL Adicionar problema à impressão]

Esse módulo de ação adiciona um ou mais problemas a uma etapa.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Jira Software] para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sprint ID]</td> 
   <td>Insira ou mapeie a ID do Sprint da fonte à qual deseja adicionar um problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do problema ou chaves]</td> 
   <td>Adicione uma ID de problema ou chave para cada problema que você deseja adicionar à impressão.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar um registro]

Esse módulo de ação cria um novo registro em Jira.

O módulo retorna quaisquer campos padrão associados ao registro, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Jira Software] para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione o tipo de registro que deseja que o módulo crie. Quando você seleciona um tipo de registro, outros campos específicos desse tipo de registro são exibidos no módulo .</p> 
    <ul> 
     <li>[!UICONTROL Anexo]</li> 
     <li>[!UICONTROL Comentário]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Chamada da API personalizada]

Esse módulo de ação permite que você faça uma chamada autenticada personalizada para o [!DNL Jira Software] API. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pela outra [!DNL Jira Software] módulos.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Jira Software] para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Insira um caminho relativo a<code>&lt;Instance URL>/rest/api/2/ </code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   td&gt; <p>Selecione o método de solicitação HTTP que você precisa configurar a chamada da API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] adiciona os cabeçalhos de autorização para você.</p> </td> 
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

#### [!UICONTROL Excluir um registro]

Esse módulo de ação exclui um registro específico.

Especifique a ID do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Jira Software] para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione o tipo de registro que deseja que o módulo exclua. </p> 
    <ul> 
     <li>[!UICONTROL Anexo]</li> 
     <li>[!UICONTROL Comentário]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID ou chave]</td> 
   <td>Insira ou mapeie a ID ou Chave do registro que deseja excluir.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Baixar um anexo]

Este módulo de ação baixa um anexo específico.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Jira Software] para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Insira ou mapeie a ID do anexo que deseja baixar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ler um registro]

Este módulo de ação lê dados de um único registro em [!DNL Jira Software].

Especifique a ID do registro.

O módulo retorna quaisquer campos padrão associados ao registro, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Jira Software] para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione o tipo de [!DNL Jira] gravar que deseja que o módulo leia.</p> 
    <ul> 
     <li>[!UICONTROL Anexo]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Usuário]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td>Selecione as saídas que deseja receber. As opções de saída estão disponíveis com base no tipo de registro selecionado no campo "[!UICONTROL Tipo de registro]".</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>Insira ou mapeie a [!DNL Jira Software] ID do registro que você deseja que o módulo leia.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar um registro]

Esse módulo de ação atualiza um registro existente, como um problema ou projeto.

Especifique a ID do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Jira Software] para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione o tipo de registro que deseja que o módulo atualize. Quando você seleciona um tipo de registro, outros campos específicos desse tipo de registro são exibidos no módulo .</p> 
    <ul> 
     <li>[!UICONTROL Comentário]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Problema de transição]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID ou chave]</td> 
   <td>Insira ou mapeie a ID ou Chave do registro que deseja atualizar.</td> 
  </tr> 
 </tbody> 
</table>

### Pesquisas

* [[!UICONTROL Listar registros]](#list-records)
* [[!UICONTROL Procurar registros]](#search-for-records)

#### [!UICONTROL Listar registros]

Este módulo de pesquisa recupera todos os itens de um tipo específico que correspondem à consulta de pesquisa

Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Jira Software] para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione o tipo de registro que deseja que o módulo liste. Quando você seleciona um tipo de registro, outros campos específicos desse tipo de registro são exibidos no módulo .</p> 
    <ul> 
     <li>[!UICONTROL Comentário]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Problema da primavera]</li> 
     <li>[!UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Resultados máximos]</p> </td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo recupere durante cada ciclo de execução de cenário.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Offset</td> 
    <td> Enter or map the ID of the first item you want to retrieve details for. This is a way to paginate the records. If you enter the 5000th item as the offset, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL Procurar registros]

Este módulo de pesquisa procura registros em um objeto em [!DNL Jira Software] que correspondem à consulta de pesquisa especificada.

Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Jira Software] para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione o tipo de registro que deseja que o módulo procure. Quando você seleciona um tipo de registro, outros campos específicos desse tipo de registro são exibidos no módulo .</p> 
    <ul> 
     <li>[!UICONTROL Problemas]</li> 
     <li> <p>[!UICONTROL Problemas por JQL (Jira Query Language)] </p> <p>Para obter mais informações sobre JQL, consulte <a href="https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14#:~:text=JQLstandsforJiraQuery,projectmanagers%2Candbusinessusers.">JQL</a> no site de ajuda do Atlassian. </p> </li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Projeto por edição]</li> 
     <li>[!UICONTROL Usuário]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
