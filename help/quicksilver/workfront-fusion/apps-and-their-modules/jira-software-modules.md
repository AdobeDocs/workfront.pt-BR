---
title: Módulos do Jira Software
description: Em um [!DNL Adobe Workfront Fusion] cenário, é possível automatizar workflows que usam [!DNL Jira] Software, bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 6437fe98-2c2b-4b49-97e2-f94b23da93fd
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2085'
ht-degree: 1%

---

# [!DNL Jira Software] módulos

Em um [!DNL Adobe Workfront Fusion] cenário, é possível automatizar workflows que usam [!DNL Jira Software], bem como conectá-lo a vários aplicativos e serviços de terceiros.

Se precisar de instruções sobre como criar um cenário, consulte [Criar um cenário no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obter informações sobre módulos, consulte [Módulos no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Pré-requisitos

Para usar [!DNL Jira] módulos que você deve ter [!DNL Jira] conta.

## Conectar [!DNL Jira Software] para [!DNL Workfront Fusion]

Seu método de conexão se baseia no fato de você estar usando [!DNL Jira Cloud] ou [!DNL Jira Server].

* [Conectar [!DNL Jira Cloud] para o Workfront Fusion](#connect-jira-cloud-to-workfront-fusion)
* [Conectar [!DNL Jira Server] para [!DNL Workfront Fusion]](#connect-jira-server-to-workfront-fusion)

### Conectar [!DNL Jira Cloud] para [!DNL Workfront Fusion]

Conectar [!DNL Jira Cloud] para [!DNL Workfront Fusion]

Para conectar [!DNL Jira Software] para [!DNL Workfront Fusion], você deve criar um token de API e inseri-lo junto com seu URL de serviço e Nome de usuário na [!UICONTROL Criar uma conexão] campo em [!DNL Workfront Fusion].

#### Criar um token de API no [!DNL Jira]

1. Ir para [https://id.atlassian.com/manage/api-tokens](https://id.atlassian.com/manage/api-tokens) e faça logon.
1. Clique em **[!UICONTROL Criar token de API]**.
1. Digite um nome para o token, como *Workfront Fusion*.
1. Copie o token usando o **[!UICONTROL Copiar para a área de transferência]** botão.

   >[!IMPORTANT]
   >
   >Você não poderá exibir o token novamente depois de fechar esta caixa de diálogo.
1. Armazene o token gerado em um local seguro.
1. Continuar com [Configure o [!DNL Jira] Token de API em [!DNL Workfront Fusion]](#configure-the-jira-api-token-in-workfront-fusion).

#### Configure o [!DNL Jira] Token de API em [!DNL Workfront Fusion]

1. Entrada [!DNL Workfront Fusion], adicionar um [!DNL Jira] módulo para um cenário para abrir o **[!UICONTROL Criar uma conexão]** caixa.
1. Especifique as seguintes informações:

   * **[!UICONTROL URL do serviço]**
   * **[!UICONTROL Nome do Usuário]**
   * **[!UICONTROL Token de API]:** Este é o token de API que você criou no [Criar um token de API no [!DNL Jira]](#create-an-api-token-in-jira) seção deste artigo.

1. Clique em [!UICONTROL Continuar] para criar a conexão e retornar ao módulo.

### Conectar [!DNL Jira Server] para [!DNL Workfront Fusion]

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Becky: Find out and document how to find these things</p>
-->

Para autorizar uma conexão entre [!DNL Workfront Fusion] e [!DNL Jira Server], você precisa de sua Chave do consumidor, Chave privada e URL do serviço. Talvez seja necessário entrar em contato com [!DNL Jira] administrador para obter essas informações.

* [Gerar chaves públicas e privadas para o [!DNL Jira] conexão](#generate-public-and-private-keys-for-your-jira-connection)
* [Configure o aplicativo cliente como consumidor no [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)
* [Criar uma conexão com o [!DNL Jira] Servidor ou data center Jira em [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### Gerar chaves públicas e privadas para o [!DNL Jira] conexão

Para adquirir uma chave privada para o seu [!DNL Workfront Fusion Jira] conexão, é necessário gerar chaves públicas e privadas.

1. No terminal, execute o seguinte `openssl` comandos.

   * `openssl genrsa -out jira_privatekey.pem 1024`

     Esse comando gera uma chave privada de 1024 bits.

   * `openssl req -newkey rsa:1024 -x509 -key jira_privatekey.pem -out jira_publickey.cer -days 365`

     Este comando cria um certificado X509.

   * `openssl pkcs8 -topk8 -nocrypt -in jira_privatekey.pem -out jira_privatekey.pcks8`

     Este comando extrai a chave privada (formato PKCS8) para o `jira_privatekey.pcks8`
arquivo.

   * `openssl x509 -pubkey -noout -in jira_publickey.cer  > jira_publickey.pem`

     Este comando extrai a chave pública do certificado para a `jira_publickey.pem` arquivo.

     >[!NOTE]
     >
     >Se estiver usando o Windows, talvez seja necessário salvar a chave pública na `jira_publickey.pem` arquivo manualmente:
     >
     >1. No terminal, execute o seguinte comando:
     >   
     >   `openssl x509 -pubkey -noout -in jira_publickey.cer`
     >   
     >1. Copie a saída do terminal (incluindo `-------BEGIN PUBLIC KEY--------` e `-------END PUBLIC KEY--------`
     >   
     >1. Cole a saída do terminal em um arquivo chamado `jira_publickey.pem`.


1. Continue para [Configure o aplicativo cliente como consumidor no [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)

#### Configure o aplicativo cliente como consumidor no [!DNL Jira]

1. Faça logon no [!DNL Jira] instância.
1. No painel de navegação esquerdo, clique em **[!UICONTROL [!DNL Jira]Configurações]** ![](assets/jira-settings-icon.png) > **[!UICONTROL Aplicativos]**> **[!UICONTROL Links de aplicativo]**.
1. No **[!UICONTROL Insira o URL do aplicativo que deseja vincular]** insira

   ```
   https://app.workfrontfusion.com/oauth/cb/workfront-jiraserver-oauth1
   ```

1. Clique em **[!UICONTROL Criar novo link]**. Ignore a mensagem de erro &quot;Nenhuma resposta foi recebida do URL inserido&quot;.
1. No **[!UICONTROL Vincular aplicativos]** insira os valores na janela **[!UICONTROL Chave do consumidor]** e **[!UICONTROL Segredo compartilhado]** campos.

   Você pode escolher os valores desses campos.

1. Copie os valores de **[!UICONTROL Chave do consumidor]** e **[!UICONTROL Segredo compartilhado]** para um local seguro.

   Esses valores serão necessários posteriormente no processo de configuração.

1. Preencha os campos URL da seguinte maneira:

   | Campo | Descrição |
   |---|---|
   | [!UICONTROL URL do token de solicitação] | `<Jira base url>/plugins/servlet/oauth/request-token` |
   | [!UICONTROL URL de autorização] | `<Jira base url>/plugins/servlet/oauth/authorize` |
   | [!UICONTROL URL do token de acesso] | `<Jira base url>/plugins/servlet/oauth/access-token` |

1. Selecione o **[!UICONTROL Criar link de entrada]** caixa de seleção
1. Clique em **[!UICONTROL Continuar]**.
1. No **[!UICONTROL Vincular aplicativos]** preencha os seguintes campos:

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Chave do Consumidor]</p> </td> 
      <td> Cole a chave do consumidor que você copiou para um local seguro.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome do consumidor]</td> 
      <td>Insira um nome de sua escolha. Este nome é para sua própria referência.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Chave pública]</td> 
      <td>Cole a chave pública do seu <code>[!DNL jira_publickey.pem]</code> arquivo.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Continuar]**.
1. Continue para [Criar uma conexão com o [!DNL Jira Server] ou [!DNL Jira Data Center] in [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### Criar uma conexão com o [!DNL Jira Server] ou [!DNL Jira Data Center] in [!DNL Workfront Fusion]

>[!NOTE]
>
>Use o [!DNL Jira Server] aplicativo para conexão [!DNL Jira Server] ou [!DNL Jira Data Center].
1. Em qualquer [!DNL Jira Server] módulo no [!DNL Workfront Fusion], clique em **[!UICONTROL Adicionar]** ao lado da [!UICONTROL conexão] campo.
1. No [!UICONTROL Criar uma conexão] preencha os seguintes campos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nome da Conexão]</p> </td> 
      <td> <p>Insira um nome para a conexão</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Chave do Consumidor]</td> 
      <td>Cole na chave do consumidor que você copiou para um local seguro no <a href="#configure-the-client-app-as-a-consumer-in-jira" class="MCXref xref">Configure o aplicativo cliente como consumidor no [!DNL Jira]</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Private Key]</td> 
      <td>Cole a chave privada no <code>[!DNL jira_privatekey.pcks8]</code> arquivo que você criou em <a href="#generate-public-and-private-keys-for-your-jira-connection" class="MCXref xref">Gerar chaves públicas e privadas para o [!DNL Jira] conexão</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Service URL]</td> 
      <td>Insira seu [!DNL Jira] URL da instância. </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Continuar]** para criar a conexão e voltar ao módulo.

## [!DNL Jira Software] módulos e seus campos

Ao configurar [!DNL Jira Software] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Jira Software] Os campos podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Ações](#actions)
* [Pesquisas](#searches)

### Triggers

#### [!UICONTROL Observar registros]

Este módulo de acionamento inicia um cenário quando um registro é adicionado, atualizado ou excluído.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Selecione o webhook que deseja usar para observar registros. </p> <p>Para adicionar um novo webhook:</p> 
    <ol> 
     <li value="1">Clique em <strong>[!UICONTROL Adicionar]</strong></li> 
     <li value="2">Insira um nome para o webhook.</li> 
     <li value="3"> <p>Selecione a conexão que deseja usar com seu webhook. </p> <p>Para obter instruções sobre como conectar seu [!DNL Jira Software] conta para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] para [!DNL Workfront Fusion]</a> neste artigo.</p> </li> 
     <li value="4"> <p>Selecione o tipo de registro que você deseja que o software assista:</p> 
      <ul> 
       <li>[!UICONTROL Comentário] </li> 
       <li>[!UICONTROL Problema]</li> 
       <li>[!UICONTROL Projeto] </li> 
       <li>[!UICONTROL Sprint]</li> 
      </ul> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [[!UICONTROL Adicionar problema ao sprint]](#add-issue-to-sprint)
* [[!UICONTROL Chamada de API personalizada]](#custom-api-call)
* [[!UICONTROL Criar um registro]](#create-a-record)
* [[!UICONTROL Excluir um registro]](#delete-a-record)
* [[!UICONTROL Baixar um anexo]](#download-an-attachment)
* [[!UICONTROL Ler um registro]](#read-a-record)
* [[!UICONTROL Atualizar um registro]](#update-a-record)

#### [!UICONTROL Adicionar problema ao sprint]

Este módulo de ação adiciona um ou mais problemas a um sprint.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Jira Software] conta para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID Sprint]</td> 
   <td>Insira ou mapeie a ID de velocidade da velocidade à qual você deseja adicionar um problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificação de Problema ou Chaves]</td> 
   <td>Adicione uma ID ou chave de problema para cada problema que você deseja adicionar ao sprint.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar um registro]

Este módulo de ação cria um novo registro no Jira.

O módulo retorna quaisquer campos padrão associados ao registro, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Jira Software] conta para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Registro]</td> 
   <td> <p>Selecione o tipo de registro que deseja que o módulo crie. Quando você seleciona um tipo de registro, outros campos específicos desse tipo de registro aparecem no módulo.</p> 
    <ul> 
     <li>[!UICONTROL Anexo]</li> 
     <li>[!UICONTROL Comentário]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Projeto]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Log de Trabalho]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Chamada de API personalizada]

Esse módulo de ação permite fazer uma chamada autenticada personalizada para o [!DNL Jira Software] API. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pelo outro [!DNL Jira Software] módulos.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Jira Software] conta para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Insira um caminho relativo a<code>&lt;Instance URL>/rest/api/2/ </code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   td&gt; <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formulário de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] O adiciona os cabeçalhos de autorização para você.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadeia de Consulta]</td> 
   <td> <p>Adicione a consulta da chamada à API na forma de um objeto JSON padrão.</p> <p>Por exemplo: <code>{"name":"something-urgent"}</code></p> </td> 
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

#### [!UICONTROL Excluir um registro]

Esse módulo de ação exclui um registro específico.

Especifique a ID do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Jira Software] conta para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Registro]</td> 
   <td> <p>Selecione o tipo de registro que deseja que o módulo exclua. </p> 
    <ul> 
     <li>[!UICONTROL Anexo]</li> 
     <li>[!UICONTROL Comentário]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Projeto]</li> 
     <li>[!UICONTROL Sprint] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID ou Chave]</td> 
   <td>Insira ou mapeie a ID ou a Chave do registro que deseja excluir.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Baixar um anexo]

Este módulo de ação baixa um anexo específico.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Jira Software] conta para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Insira ou mapeie a ID do anexo que deseja baixar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ler um registro]

Este módulo de ação lê os dados de um único registro no [!DNL Jira Software].

Especifique a ID do registro.

O módulo retorna quaisquer campos padrão associados ao registro, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Jira Software] conta para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Registro]</td> 
   <td> <p>Selecione o tipo de [!DNL Jira] registro que você deseja que o módulo leia.</p> 
    <ul> 
     <li>[!UICONTROL Anexo]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Projeto]</li> 
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
   <td> <p>Insira ou mapeie o único [!DNL Jira Software] ID do registro que você deseja que o módulo leia.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar um registro]

Esse módulo de ação atualiza um registro existente, como um problema ou projeto,.

Especifique a ID do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Jira Software] conta para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Registro]</td> 
   <td> <p>Selecione o tipo de registro que deseja que o módulo atualize. Quando você seleciona um tipo de registro, outros campos específicos desse tipo de registro aparecem no módulo.</p> 
    <ul> 
     <li>[!UICONTROL Comentário]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Projeto]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Problema de transição]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID ou Chave]</td> 
   <td>Insira ou mapeie a ID ou a Chave do registro que deseja atualizar.</td> 
  </tr> 
 </tbody> 
</table>

### Pesquisas

* [[!UICONTROL Listar registros]](#list-records)
* [[!UICONTROL Pesquisar registros]](#search-for-records)

#### [!UICONTROL Listar registros]

Este módulo de pesquisa recupera todos os itens de um tipo específico que correspondam à sua consulta de pesquisa

Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Jira Software] conta para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Registro]</td> 
   <td> <p>Selecione o tipo de registro que deseja que o módulo liste. Quando você seleciona um tipo de registro, outros campos específicos desse tipo de registro aparecem no módulo.</p> 
    <ul> 
     <li>[!UICONTROL Comentário]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Projeto]</li> 
     <li>[!UICONTROL Problema de Sprint]</li> 
     <li>[!UICONTROL Log de Trabalho]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Máximo de Resultados]</p> </td> 
   <td> <p>Insira ou mapeie o número máximo de registros que deseja que o módulo recupere durante cada ciclo de execução de cenário.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Offset</td> 
    <td> Enter or map the ID of the first item you want to retrieve details for. This is a way to paginate the records. If you enter the 5000th item as the offset, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL Pesquisar registros]

Este módulo de pesquisa procura registros em um objeto no [!DNL Jira Software] que correspondam à consulta de pesquisa especificada.

Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Jira Software] conta para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Registro]</td> 
   <td> <p>Selecione o tipo de registro que deseja que o módulo procure. Quando você seleciona um tipo de registro, outros campos específicos desse tipo de registro aparecem no módulo.</p> 
    <ul> 
     <li>[!UICONTROL Problemas]</li> 
     <li> <p>[!UICONTROL Problemas por JQL (Jira Query Language)] </p> <p>Para obter mais informações sobre JQL, consulte <a href="https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14#:~:text=JQLstandsforJiraQuery,projectmanagers%2Candbusinessusers.">JQL</a> no local de ajuda Atlassian. </p> </li> 
     <li>[!UICONTROL Projeto]</li> 
     <li>[!UICONTROL Projeto por problema]</li> 
     <li>[!UICONTROL Usuário]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
