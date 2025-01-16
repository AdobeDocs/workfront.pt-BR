---
title: Módulos do Jira Software
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 6437fe98-2c2b-4b49-97e2-f94b23da93fd
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '2165'
ht-degree: 1%

---

# [!DNL Jira Software] módulos

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Módulos do Jira Software](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

Em um cenário [!DNL Adobe Workfront Fusion], você pode automatizar fluxos de trabalho que usam [!DNL Jira Software], bem como conectá-los a vários aplicativos e serviços de terceiros.

Se você precisar de instruções sobre como criar um cenário, consulte [Criar um cenário [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

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

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Pré-requisitos

Para usar módulos do [!DNL Jira] é necessário ter uma conta do [!DNL Jira].

## Informações da API Jira

O conector Jira usa o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"></td> 
   <td> Jira Cloud</td> 
   <td> Servidor Jira</td> 
  </tr> 
  <tr> 
   <td role="rowheader">apiVersion</td> 
   <td> 2</td> 
   <td> 2</td> 
  </tr> 
  <tr> 
   <td role="rowheader">apiVersionAgile</td> 
   <td> 1,0 </td> 
   <td> 1,0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tag da API</td> 
   <td>1.7.29</td> 
   <td>1.0.19</td> 
  </tr>
 </tbody> 
 </table>

## Conectar [!DNL Jira Software] a [!DNL Workfront Fusion]

O método de conexão é baseado no uso do [!DNL Jira Cloud] ou do [!DNL Jira Server].

* [Conectar [!DNL Jira Cloud] ao Workfront Fusion](#connect-jira-cloud-to-workfront-fusion)
* [Conectar [!DNL Jira Server] a [!DNL Workfront Fusion]](#connect-jira-server-to-workfront-fusion)

### Conectar [!DNL Jira Cloud] a [!DNL Workfront Fusion]

Conectar [!DNL Jira Cloud] a [!DNL Workfront Fusion]

Para conectar [!DNL Jira Software] a [!DNL Workfront Fusion], você deve criar um token de API e inseri-lo junto com a URL de Serviço e o Nome de Usuário no campo [!UICONTROL Criar uma conexão] em [!DNL Workfront Fusion].

#### Criar um token de API em [!DNL Jira]

1. Vá para [https://id.atlassian.com/manage/api-tokens](https://id.atlassian.com/manage/api-tokens) e faça logon.
1. Clique em **[!UICONTROL Criar token de API]**.
1. Digite um nome para o token, como *Workfront Fusion*.
1. Copie o token usando o botão **[!UICONTROL Copiar para a área de transferência]**.

   >[!IMPORTANT]
   >
   >Você não poderá exibir o token novamente depois de fechar esta caixa de diálogo.
1. Armazene o token gerado em um local seguro.
1. Continuar com [Configurar o token de API [!DNL Jira] em [!DNL Workfront Fusion]](#configure-the-jira-api-token-in-workfront-fusion).

#### Configurar o token de API [!DNL Jira] em [!DNL Workfront Fusion]

1. Em [!DNL Workfront Fusion], adicione um módulo [!DNL Jira] a um cenário para abrir a caixa **[!UICONTROL Criar uma conexão]**.
1. Especifique as seguintes informações:

   * **[!UICONTROL URL do Serviço]:** Esta é a URL base que você usa para acessar sua conta Jira. Exemplo: `yourorganization.atlassian.net`
   * **[!UICONTROL Nome de usuário]**
   * **[!UICONTROL Token de API]:** Este é o token de API criado na seção [Criar um token de API [!DNL Jira]](#create-an-api-token-in-jira) deste artigo.

1. Clique em [!UICONTROL Continuar] para criar a conexão e retornar ao módulo.

### Conectar [!DNL Jira Server] a [!DNL Workfront Fusion]

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Becky: Find out and document how to find these things</p>
-->

Para autorizar uma conexão entre [!DNL Workfront Fusion] e [!DNL Jira Server], você precisa de sua Chave do Consumidor, Chave Privada e URL do Serviço. Talvez seja necessário contatar o administrador do [!DNL Jira] para obter essas informações.

* [Gerar chaves Públicas e Privadas para sua  [!DNL Jira] conexão](#generate-public-and-private-keys-for-your-jira-connection)
* [Configurar o aplicativo cliente como consumidor no  [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)
* [Criar uma conexão com o [!DNL Jira] Servidor ou o Jira Data Center em [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### Gerar chaves públicas e privadas para sua conexão [!DNL Jira]

Para adquirir uma chave privada para sua conexão [!DNL Workfront Fusion Jira], você precisa gerar chaves públicas e privadas.

1. No terminal, execute os seguintes comandos `openssl`.

   * `openssl genrsa -out jira_privatekey.pem 1024`

     Esse comando gera uma chave privada de 1024 bits.

   * `openssl req -newkey rsa:1024 -x509 -key jira_privatekey.pem -out jira_publickey.cer -days 365`

     Este comando cria um certificado X509.

   * `openssl pkcs8 -topk8 -nocrypt -in jira_privatekey.pem -out jira_privatekey.pcks8`

     Este comando extrai a chave privada (formato PKCS8) para o `jira_privatekey.pcks8`
arquivo.

   * `openssl x509 -pubkey -noout -in jira_publickey.cer  > jira_publickey.pem`

     Este comando extrai a chave pública do certificado para o arquivo `jira_publickey.pem`.

     >[!NOTE]
     >
     >Se você estiver usando o Windows, talvez precise salvar manualmente a chave pública no arquivo `jira_publickey.pem`:
     >
     >1. No terminal, execute o seguinte comando:
     >   
     >   `openssl x509 -pubkey -noout -in jira_publickey.cer`
     >   
     >1. Copiar a saída do terminal (incluindo `-------BEGIN PUBLIC KEY--------` e `-------END PUBLIC KEY--------`
     >   
     >1. Cole a saída do terminal em um arquivo chamado `jira_publickey.pem`.


1. Prossiga para [Configurar o aplicativo cliente como consumidor em [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)

#### Configure o aplicativo cliente como um consumidor no [!DNL Jira]

1. Faça logon na instância do [!DNL Jira].
1. No painel de navegação esquerdo, clique em **[!UICONTROL [!DNL Jira]Configurações]** ![](assets/jira-settings-icon.png) > **[!UICONTROL Aplicativos]**> **[!UICONTROL Links de aplicativos]**.
1. No campo **[!UICONTROL Insira a URL do aplicativo que deseja vincular]**, digite

   ```
   https://app.workfrontfusion.com/oauth/cb/workfront-jiraserver-oauth1
   ```

1. Clique em **[!UICONTROL Criar novo link]**. Ignore a mensagem de erro &quot;Nenhuma resposta foi recebida do URL inserido&quot;.
1. Na janela **[!UICONTROL Vincular aplicativos]**, insira valores nos campos **[!UICONTROL Chave do consumidor]** e **[!UICONTROL Segredo compartilhado]**.

   Você pode escolher os valores desses campos.

1. Copie os valores dos campos **[!UICONTROL Chave do consumidor]** e **[!UICONTROL Segredo compartilhado]** para um local seguro.

   Esses valores serão necessários posteriormente no processo de configuração.

1. Preencha os campos URL da seguinte maneira:

   | Campo | Descrição |
   |---|---|
   | [!UICONTROL URL do token de solicitação] | `<Jira base url>/plugins/servlet/oauth/request-token` |
   | [!UICONTROL URL de autorização] | `<Jira base url>/plugins/servlet/oauth/authorize` |
   | [!UICONTROL URL do token de acesso] | `<Jira base url>/plugins/servlet/oauth/access-token` |

1. Marque a caixa de seleção **[!UICONTROL Criar link de entrada]**.
1. Clique em **[!UICONTROL Continuar]**.
1. Na janela **[!UICONTROL Vincular aplicativos]**, preencha os seguintes campos:

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
      <td>Cole a chave pública do arquivo <code>[!DNL jira_publickey.pem]</code>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Continuar]**.
1. Continue para [Criar uma conexão com [!DNL Jira Server] ou [!DNL Jira Data Center] em [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### Criar uma conexão com [!DNL Jira Server] ou [!DNL Jira Data Center] em [!DNL Workfront Fusion]

>[!NOTE]
>
>Use o aplicativo [!DNL Jira Server] para se conectar a [!DNL Jira Server] ou [!DNL Jira Data Center].

1. Em qualquer módulo [!DNL Jira Server] em [!DNL Workfront Fusion], clique em **[!UICONTROL Adicionar]** ao lado do campo [!UICONTROL conexão].
1. No painel [!UICONTROL Criar uma conexão], preencha os seguintes campos:

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
      <td>Cole a chave do consumidor que você copiou em um local seguro no <a href="#configure-the-client-app-as-a-consumer-in-jira" class="MCXref xref">Configure o aplicativo cliente como um consumidor no [!DNL Jira]</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Private Key]</td> 
      <td>Cole a chave privada do arquivo <code>[!DNL jira_privatekey.pcks8]</code> criado em <a href="#generate-public-and-private-keys-for-your-jira-connection" class="MCXref xref">Gerar chaves públicas e privadas para sua conexão [!DNL Jira]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Service URL]</td> 
      <td>Insira a URL da instância do [!DNL Jira]. Exemplo: <code>yourorganization.atlassian.net</code></td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Continuar]** para criar a conexão e voltar para o módulo.

## [!DNL Jira Software] módulos e seus campos

Ao configurar módulos do [!DNL Jira Software], o [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos [!DNL Jira Software] adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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
     <li value="3"> <p>Selecione a conexão que deseja usar com seu webhook. </p> <p>Para obter instruções sobre como conectar sua conta do [!DNL Jira Software] ao [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </li> 
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
* [[!UICONTROL Criar um Registro]](#create-a-record)
* [[!UICONTROL Chamada de API personalizada]](#custom-api-call)
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
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Jira Software] ao [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
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

#### [!UICONTROL Criar um Registro]

Este módulo de ação cria um novo registro no Jira.

O módulo retorna quaisquer campos padrão associados ao registro, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Jira Software] ao [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
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

Este módulo de ação permite fazer uma chamada autenticada personalizada para a API [!DNL Jira Software]. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pelos outros módulos do [!DNL Jira Software].

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Jira Software] ao [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
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
   <td> <p>Adicione o conteúdo do corpo para a chamada à API na forma de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar instruções condicionais como <code>if</code> em seu JSON, coloque as aspas fora da instrução condicional.</p> 
     <img src="assets/quotes-in-json-350x120.png">  </td> 
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
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Jira Software] ao [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
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
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Jira Software] ao [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
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

O módulo retorna quaisquer campos padrão associados ao registro, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Jira Software] ao [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Registro]</td> 
   <td> <p>Selecione o tipo de registro [!DNL Jira] que deseja que o módulo leia.</p> 
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
   <td> <p>Insira ou mapeie a ID [!DNL Jira Software] exclusiva do registro que você deseja que o módulo leia.</p> </td> 
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
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Jira Software] ao [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
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
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Jira Software] ao [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
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
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo recupere durante cada ciclo de execução de cenário.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Offset</td> 
    <td> Enter or map the ID of the first item you want to retrieve details for. This is a way to paginate the records. If you enter the 5000th item as the offset, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL Pesquisar registros]

Este módulo de pesquisa procura registros em um objeto em [!DNL Jira Software] que correspondam à consulta de pesquisa especificada.

Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Jira Software] ao [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Registro]</td> 
   <td> <p>Selecione o tipo de registro que deseja que o módulo procure. Quando você seleciona um tipo de registro, outros campos específicos desse tipo de registro aparecem no módulo.</p> 
    <ul> 
     <li>[!UICONTROL Problemas]</li> 
     <li> <p>[!UICONTROL Problemas por JQL (Jira Query Language)] </p> <p>Para obter mais informações sobre JQL, consulte <a href="https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14#:~:text=JQLstandsforJiraQuery,projectmanagers%2Candbusinessusers.">JQL</a> no site de ajuda da Atlassian. </p> </li> 
     <li>[!UICONTROL Projeto]</li> 
     <li>[!UICONTROL Projeto por problema]</li> 
     <li>[!UICONTROL Usuário]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
