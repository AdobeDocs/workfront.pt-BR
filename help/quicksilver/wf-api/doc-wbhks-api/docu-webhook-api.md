---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: API de Webhooks de documento
description: API de Webhooks de documento
author: Becky
feature: Workfront API
exl-id: 7ac2c6c8-1cb8-49df-8d63-a6b47ad02a13
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '3646'
ht-degree: 3%

---


# API de Webhooks de documento

O Adobe Workfront Document Webhooks define um conjunto de endpoints de API através dos quais a Workfront faz chamadas de API autorizadas para um Provedor de Documentos Externo. Isso permite que qualquer pessoa crie um plug-in middleware para qualquer provedor de armazenamento de documentos.

A experiência do usuário para integrações baseadas em webhook será semelhante à das integrações de documentos existentes, como Google Drive, Box e Dropbox. Por exemplo, um usuário do Workfront poderá executar as seguintes ações:

* Navegar pela estrutura de pastas do provedor de documentos externo
* Pesquisar arquivos
* Vincular arquivos ao Workfront
* Fazer upload de arquivos para o provedor de documentos externo
* Exibir uma miniatura do documento

## Implementação de referência

Para ajudar a iniciar rapidamente o desenvolvimento de uma nova implementação de webhooks, o Workfront fornece uma implementação de referência. O código para isso pode ser encontrado em [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app). Essa implementação é baseada em Java e permite que o Workfront conecte documentos em um sistema de arquivos de rede.

## Registrar uma integração do Webhook

Os administradores do Workfront podem adicionar uma integração personalizada do webhook para sua empresa navegando até Configuração > Documentos > Integrações personalizadas no Workfront. Na página Integração personalizada em Configurar, os administradores podem exibir uma lista de documentos existentes que fazem parte das integrações do Webhook. Nessa página, as integrações podem ser adicionadas, editadas, habilitadas e desativadas. Para adicionar uma integração, clique no botão &quot;Adicionar integração&quot;.

### Campos disponíveis

Ao adicionar uma integração, o administrador inserirá valores para os seguintes campos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome do Campo</th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Nome</td> 
   <td>O nome dessa integração.</td> 
  </tr> 
  <tr> 
   <td>URL base da API</td> 
   <td> <p>A localização da API de retorno de chamada. Ao fazer chamadas para o sistema externo, a Workfront simplesmente anexará o nome do ponto de extremidade a esse endereço. Por exemplo, se o administrador inserisse o URL da API base, " https://www.mycompany.com/api/v1 ", o Workfront usaria o seguinte URL para obter os metadados de um documento: https://www.mycompany.com/api/v1/metadata?id=1234.</p> </td> 
  </tr> 
  <tr> 
   <td>Parâmetros da solicitação</td> 
   <td> <p>Valores opcionais a serem acrescentados à querystring de todas as chamadas para a API. Por exemplo, access_type</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Tipo de autenticação</td> 
   <td>OAuth2 ou ApiKey</td> 
  </tr> 
  <tr> 
   <td>URL de autenticação</td> 
   <td> <p>(Somente OAuth2) O URL completo usado para autenticação de usuário. A Workfront navegará pelos usuários para esse endereço como parte do processo de provisionamento do OAuth. Observação: A Workfront anexará um parâmetro de "estado" à string de consulta. O provedor deve reenviar isso para o Workfront, anexando-o ao URI de redirecionamento do Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>URL token da extremidade final</td> 
   <td> <p>(Somente OAuth2) O URL completo da API usado para recuperar tokens OAuth2. Isso é hospedado pelo provedor do webhook ou provedor de documento externo</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>ID do cliente</td> 
   <td>(Somente OAuth2) A ID do cliente OAuth2 para essa integração</td> 
  </tr> 
  <tr> 
   <td>Segredo do cliente</td> 
   <td> <p>(Somente OAuth2) O Segredo do Cliente OAuth2 para essa integração</p> </td> 
  </tr> 
  <tr> 
   <td>URL de redirecionamento do Workfront</td> 
   <td>  <p>(Somente OAuth2) Este é um campo somente leitura e é gerado pelo Workfront. Esse valor é usado para registrar essa integração no provedor de documentos externos. Observação: Conforme descrito acima para URL de autenticação, o provedor deve anexar o parâmetro "state" e seu valor à sequência de consulta ao executar o redirecionamento.</p></td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td>  <p>(Somente ApiKey) Usado para fazer chamadas de API autorizadas para o provedor webhook. A chave da API emitida pelo provedor do webhook.</p></td> 
  </tr> 
 </tbody> 
</table>

 

## Autenticação

Os webhooks de documentos do Workfront oferecem suporte a duas formas diferentes de autenticação: OAuth2 e ApiKey. Em ambos os casos, o Workfront transmite tokens de autenticação no cabeçalho ao fazer uma chamada de API.

### OAuth2

O OAuth2 permite que o Workfront faça chamadas de API autorizadas para um provedor de webhook em nome de um usuário. Antes de fazer isso, o usuário deve conectar sua conta externa de provedor de documentos à Workfront e conceder a Workfront

o acesso à ação em seu nome. Esse processo de handshaking só acontece uma vez para cada usuário. Veja como funciona:

1. O usuário começa a conectar a integração do webhook à sua conta. Atualmente, isso é feito clicando na lista suspensa &quot;Adicionar documento&quot; > &quot;Adicionar serviço&quot; > Nome da integração personalizada.
1. O Workfront navega pelo usuário o URL de autenticação, que pode solicitar que o usuário faça logon no provedor de documento externo. Esta página é hospedada pelo provedor do webhook ou pelo sistema externo de gerenciamento de documentos. Ao fazer isso, o Workfront adiciona um parâmetro &quot;state&quot; ao URL de autenticação. Esse valor deve ser retornado ao Workfront, anexando o mesmo valor ao URI de retorno do Workfront na etapa abaixo.
1. Depois de fazer logon no sistema externo (ou se o usuário já estiver conectado), o usuário é levado a uma página de &quot;Autenticação&quot;, o que explica que a Workfront está solicitando acesso para executar um conjunto de ações em nome do usuário.
1. Se o usuário clicar no botão &quot;Permitir&quot;, o navegador redirecionará para o URI de redirecionamento do Workfront , adicionando &quot;code=`<code>`&quot; para a querystring. De acordo com a especificação do OAuth2, esse token tem duração curta. A querystring também deve ter o seguinte, &quot;state=`<sent_by_workfront>`&quot;.
1. A Workfront processa essa solicitação e faz uma chamada de API para o URL do ponto de extremidade do token com o código de autorização.
1. O URL do Ponto de Extremidade do Token retorna um token de atualização e um token de acesso.
1. A Workfront armazena esses tokens e fornece a integração do webhook para esse usuário.
1. A partir desse ponto, o Workfront poderá fazer chamadas de API autorizadas para o provedor do webhook. Ao fazer essas chamadas, o Workfront enviará o token de acesso no cabeçalho da solicitação HTTP, como mostrado abaixo:

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. Se o token de acesso tiver expirado, o Workfront fará uma chamada para o URL do ponto de extremidade do token para recuperar um novo token de acesso e, em seguida, tentará a chamada da API autorizada novamente com o novo token de acesso.

### ApiKey

Fazer chamadas de API autorizadas para um provedor de webhook usando uma ApiKey é muito mais simples do que o OAuth2. Ao fazer uma chamada de API, o Workfront simplesmente passará a ApiKey e o nome de usuário Workfront no cabeçalho de solicitação HTTP:

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

O provedor Webhook pode usar o nome de usuário para aplicar permissões específicas do usuário. Isso funciona melhor quando ambos os sistemas se conectam ao LDAP usando o Single Sign On (SSO).

### Adicionar cabeçalhos de solicitação (opcional)

Além de usar tokens OAuth2 ou uma ApiKey para autenticação, o Workfront pode enviar um conjunto predefinido de cabeçalhos para o provedor webhook para cada chamada de API. Um administrador do Workfront pode configurar isso ao registrar ou editar uma Integração do Webook, conforme descrito na seção acima. Consulte Registro de uma integração do Webhook .

Por exemplo, isso pode ser usado para Autenticação básica. Para fazer isso, o administrador do Workfront adicionaria as seguintes informações do Cabeçalho da solicitação na caixa de diálogo Integração personalizada :

   Autorização Básica QWxhZGRpbjpvcGVuIHNlc2FtZQ==

onde QWxhZGRpbjpvcGVuIHNlc2FtZQ= é uma string codificada em base 64 de &quot;nome de usuário:senha&quot;. Consulte Autenticação básica . Desde que adicionado, o Workfront passará isso no cabeçalho da solicitação HTTP, além de outros cabeçalhos de solicitação:

```
­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------

apiKey: 12345

username: johndoe@foo.com

Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

## Especificação da API

Abaixo está uma lista de APIs que o provedor do webhook deve implementar para que os webhooks de documento funcionem.

### Obter tokens OAuth2 (somente autenticação OAuth2 necessária)

Retorna o token de atualização OAuth2 e o token de acesso de um usuário autenticado. Isso é chamado uma vez quando o usuário provisionar um Provedor de documentos. As chamadas subsequentes são feitas para obter um token de acesso atualizado.

Solicitação HTTP POST /any/url

O URL é configurável e corresponde ao valor do URL do ponto de extremidade do token na página Configuração da integração personalizada.

**Parâmetros de consulta**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome</th> 
   <th>Obrigatório</th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>grant_type</td> 
   <td>sim</td> 
   <td> <p>Os valores incluem "authorization_code" ou "refresh_token". O valor especificado indica qual dos dois parâmetros será passado para essa chamada de API: ou refresh_token.</p> </td> 
  </tr> 
  <tr> 
   <td>código</td> 
   <td>depende</td> 
   <td> <p>O código de autorização enviado ao Workfront logo após o usuário clicar no botão "Conceder". Isso só é necessário quando o tipo de concessão é "authorization_code". O código de autorização deve ter uma duração curta, geralmente com uma validade inferior ou igual a 10 minutos.</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token</td> 
   <td>depende</td> 
   <td> <p>Isso só é necessário ao fazer chamadas subsequentes para recuperar um novo access_token, visto que o access_token anterior expirou. Ao enviar esse valor, defina o parâmetro grant_type como "refresh_token".</p> </td> 
  </tr> 
  <tr> 
   <td>client_id</td> 
   <td>sim</td> 
   <td>A ID do cliente configurada no Workfront para essa integração personalizada.</td> 
  </tr> 
  <tr> 
   <td>client_secret</td> 
   <td>sim</td> 
   <td> O Segredo do cliente configurado no Workfront para essa integração personalizada.</td> 
  </tr> 
 </tbody> 
</table>

 

**Resposta**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome</th> 
   <th>Tipo </th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>access_token </td> 
   <td>String</td> 
   <td> <p>Um token usado para fazer chamadas de API autorizadas em nome do usuário. Isso deve expirar para evitar chamadas de API não autorizadas.</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token </td> 
   <td>String</td> 
   <td> <p>Um token de longa duração usado para recuperar um novo access_token chamando este método de API.</p> </td> 
  </tr> 
  <tr> 
   <td>expires_in </td> 
   <td>long</td> 
   <td>  <p>(opcional) O tempo (em segundos) antes do access_token expirar, em geral 3.600.</p></td> 
  </tr> 
 </tbody> 
</table>

 

**Exemplo**

```
POST /oauth2/token
grant_type=authorization_code
code=d9ac7asdf6asdf579d7a8
client_id=123456
client_secret=6asdf7a7a9a4af
```


**Resposta**

```
{
"access_token":"ad8af5ad5ads759", 
"refresh_token":"9a0h5d87d808ads", 
"expires_id":"3600" 
}
```

### Obter metadados para ficheiro ou pasta

Retorna metadados para o arquivo ou pasta especificado.

**URL**

GET /metadata?id=[ID do documento ou da pasta]

**Parâmetros de consulta**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome </th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>id</td> 
   <td>  <p>A ID do arquivo ou pasta, conforme referenciado pelo provedor do webhook. Isso é diferente da ID de documento do Workfront. Para obter os metadados do diretório raiz, use o valor '/'.</p><p>Observação: O comprimento máximo da ID é de 255 caracteres.</p></td> 
  </tr> 
 </tbody> 
</table>

 

**Resposta**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome </th> 
   <th>Tipo </th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>title </td> 
   <td>String </td> 
   <td>O nome do documento ou pasta</td> 
  </tr> 
  <tr> 
   <td>tipo </td> 
   <td>String </td> 
   <td>Especifica se este item é um arquivo ou pasta ('arquivo' ou 'pasta')</td> 
  </tr> 
  <tr> 
   <td>id</td> 
   <td>String </td> 
   <td>O ID do arquivo ou pasta.</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>String </td> 
   <td> <p>O caminho do URL usado por um usuário para exibir o documento em uma janela do navegador. O URL pode ser hospedado pelo provedor de documentos ou pelo provedor de armazenamento externo nativo.</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>String </td> 
   <td> <p>O caminho do URL usado por um usuário para baixar o documento em uma janela do navegador. O URL pode ser hospedado pelo provedor de documentos ou pelo provedor de armazenamento externo nativo.</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>String </td> 
   <td>O tipo MIME do arquivo. (opcional)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>String </td> 
   <td>Última vez que este arquivo foi modificado (carimbo de data e hora RFC 3339 formatado)</td> 
  </tr> 
  <tr> 
   <td>size</td> 
   <td>Long</td> 
   <td>  O tamanho do arquivo em bytes. (opcional)</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>Booleano</td> 
   <td>  <p> Indica se este arquivo ou pasta é somente leitura para o usuário autenticado.(opcional)</p><p> </p></td> 
  </tr> 
 </tbody> 
</table>

**Exemplo:** `https://www.acme.com/api/metadata?id=12345`

**Resposta**

```
{
"title":"My Document", 
"kind":"file"
"id":"12345", 
"viewLink":"https://www.acme.com/viewDocument?id=12345", 
"downloadLink":"https://www.acme.com/downloadDocument?id=12345",
"mimeType":"image/png",
"dateModified":"2014­06­05T17:39:45.251Z",
"size": "32554694"
}
```

>[!NOTE]
>
>O tratamento de erros deve ser consistente em todas as chamadas de API. Consulte a seção &quot;Tratamento de erros&quot; abaixo para obter detalhes.

### Obter uma lista de itens numa pasta

Retorna metadados para os arquivos e pastas de uma determinada pasta.

**URL**

GET /files

**Parâmetros de consulta**

| Nome  | Descrição |
|---|---|
| parentId  | A ID da pasta. Para obter os metadados do diretório raiz, use o valor &#39;/&#39;. |

{style="table-layout:auto"}

No momento, a API de Webhooks de documento não suporta paginação.

**Resposta**

JSON contendo uma lista de arquivos e pastas. Os metadados de cada item são os mesmos retornados pelo endpoint /metadata.

**Exemplo:** `https://www.acme.com/api/files?parentId=123456`

**Resposta**

```
[
{
"title":"Folder A",
"kind":"folder",
"id":"2lj23lkj",
"viewLink":"https://www.acme.com/viewDocument?id=2lj23lkj",
"downloadLink":"https://www.acme.com/downloadDocument?id=2lj23lkj",
"mimeType":"",
"dateModified":"2014­06­05T17:39:45.251Z",
"size":"" 
},
{
"title":"My Document",
"kind":"file",
"id":"da8cj234"
"viewLink":"https://www.acme.com/viewDocument?id=da8cj234",
"downloadLink":"https://www.acme.com/downloadDocument?id=da8cj234",
"mimeType":"image/png",
"dateModified":"2014­06­05T17:39:45.251Z",
"size":"32554694"
},
]
```

### Fazer uma pesquisa

Retorna metadados para os arquivos e pastas retornados de uma pesquisa. Isso pode ser implementado como uma pesquisa de texto completo ou como um query de banco de dados regular. O Workfront chama o endpoint /search quando o usuário realiza uma pesquisa a partir do navegador de arquivos externo.

**URL**

GET /search

**Parâmetros de consulta**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome </th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>query</td> 
   <td>O termo de pesquisa ou frase.</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>(opcional) A ID da pasta da qual a pesquisa foi executada. Observação: Este é um espaço reservado para um recurso futuro no Workfront. Atualmente, o workfront não passa esse parâmetro. </p> </td> 
  </tr> 
  </tbody> 
</table>

No momento, a API de Webhooks de documento não suporta paginação.

 

**Resposta**

JSON contendo uma lista de metadados para arquivos e pastas correspondentes ao query. O que constitui uma &quot;correspondência&quot; é determinado pelo provedor do webhook. Idealmente, ele deve fazer uma pesquisa de texto completo. Fazer uma pesquisa baseada em nome de arquivo também funciona.

**Exemplo:** `https://www.acme.com/api/search?query=test-query`

**Resposta**

```
[
{ File/Folder Metadata },
{ File/Folder Metadata }
]
```

### Obter o conteúdo de um documento

Retorna os bytes brutos de um documento

**URL**

GET /download

**Parâmetros de consulta**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome </th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>id</p> </td> 
   <td> A ID do documento.</td> 
  </tr> 
 </tbody> 
</table>

 

**Resposta**

Os bytes brutos do documento.

**Exemplo:** `https://www.acme.com/api/download?id=123456`

### Obter uma miniatura de um documento

Retorna os bytes de miniatura brutos de um documento.

**URL**

GET /miniatura

**Parâmetros de consulta**

| Nome  | Descrição |
|---|---|
| id  | A ID do documento. |
| size  |  A largura da miniatura |

{style="table-layout:auto"}

 

**Resposta**

Os bytes de miniatura brutos.

**Exemplo:** `https://www.acme.com/api/thumbnail?id=123456`

### Fazer upload de um arquivo - Parte 1 de 2

O upload de um arquivo para um provedor de armazenamento de documentos é um processo de duas etapas que requer dois endpoints de API separados. O Workfront inicia o processo de upload chamando /uploadInit . Esse ponto de extremidade retorna uma ID de documento que é passada para /upload ao carregar os bytes do documento. Dependendo do sistema de armazenamento de documentos subjacente, pode ser necessário criar um documento de comprimento zero e atualizar posteriormente o conteúdo do documento.

Adicionada à versão 1.1 desta especificação, a ID do documento e a ID da versão do documento podem ser usadas para recuperar informações adicionais do Workfront. Por exemplo, se o sistema de gerenciamento de documentos quiser informações adicionais sobre o documento, o código de implementação do webhook poderá usar a ID do documento para recuperar essas informações usando a API RESTful do Workfront. Como uma boa prática, essas informações podem vir de campos de dados personalizados no documento e estão contendo tarefa, problema ou projeto.

**URL**

POST /uploadInit

**Parâmetros de consulta**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome </th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>parentId </td> 
   <td>A ID da pasta principal, conforme referenciado pelo provedor do webhook.</td> 
  </tr> 
  <tr> 
   <td>filename </td> 
   <td>O nome do documento</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>A ID de documento do Workfront (adicionada na versão 1.1)</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>A ID da versão do documento do Workfront (adicionada na versão 1.1)</td> 
  </tr> 
 </tbody> 
</table>

 

**Resposta**

Os metadados do arquivo, conforme definido pelo endpoint /metadata.

**Exemplo:** `https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&docu mentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b`

**Resposta**

`[file_metadata]` O inclui a nova ID de documento usada pelo provedor de documentos.

### Fazer upload de um arquivo - Parte 2 de 2

Carrega os bytes de um documento para o provedor do webhook.

**URL**

PUT /upload

**Parâmetros de consulta**

| Nome  | Descrição |
|---|---|
| id  |  A ID do documento, que acabou de ser criada. |


 

**Corpo da solicitação**

Os bytes de conteúdo bruto do documento.

**Resposta**

```
{
"result": "success"
}
```

ou

```
{
"result": "fail"
}
```

**Exemplo:** `https://www.acme.com/api/upload?id=1234` *[bytes de documento incluídos no fluxo de atualização]*

**Resposta**

```
{
"result":"success"
}
```

### Obter informações sobre o serviço 

(Data de lançamento - TBD) Retorna informações sobre o serviço, como recursos e recursos. A Workfront usará essas informações para personalizar a interface do usuário no Workfront. Por exemplo, se a implementação do webhook contiver algumas ações personalizadas, o JSON deverá listar essas operações no JSON. Os usuários seriam capazes de invocar essas ações do Workfront.

**URL**

GET /serviceInfo

Parâmetros de consulta

Nenhum. Além disso, as chamadas para esse endpoint não devem exigir autenticação.

**Resposta**

JSON contendo informações sobre esse serviço

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome</th> 
   <th>Tipo </th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>webhookVersion </td> 
   <td>String </td> 
   <td>A versão do webhook implementada por este serviço. Este é o número de versão listado na parte superior desta especificação.</td> 
  </tr> 
  <tr> 
   <td>version </td> 
   <td>String </td> 
   <td>O número de versão interno deste serviço. Esse número é determinado pelo provedor de serviços do webhook e é usado somente para fins informativos.<br><br></td> 
  </tr> 
  <tr> 
   <td>editor </td> 
   <td>String </td> 
   <td>O nome da empresa que fornece a implementação do webhook.</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>String </td> 
   <td>Uma lista que contém os Endpoints de API implementados por esse serviço. Isso pode ser usado para garantir que a interface do usuário no Workfront reflita os recursos oferecidos pelo provedor do webhook. Cada item na lista deve incluir o nome do ponto de extremidade (como "pesquisa").</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>String</td> 
   <td>  <p>Uma lista contendo as operações personalizadas implementadas por este webhook. Cada item de lista inclui um nome e um nome de exibição. O nome de exibição será exibido na lista suspensa "Ações do documento" no Workfront. Clicar no item na lista suspensa chamará a ação no webhook chamando o endpoint /customAction .</p></td> 
  </tr> 
 </tbody> 
</table>

**Exemplo:** https://www.acme.com/api/serviceInfo

**Devoluções**

```
{
"webhook version": "1.2", "version": "1.0", "publisher": "Acme, LLC", "availableEndpoints": ["files", "metadata", "search", "download"

"thumbnail", "uploadInit", "upload" ], "customActions" [
{
"name": "archive", "displayName": "Archive" }, {

"name": "doSomethingElse", "displayName": "Do Something" }, ] }
```

### Criar uma pasta

(Adicionado na versão 1.2) Cria uma pasta em um determinado diretório.
URL

POST /createFolder

**Parâmetros de consulta**

| Nome  | Descrição |
|---|---|
| parentId  | A ID da pasta na qual a pasta deve ser criada |
| name  | O nome da nova pasta |

{style="table-layout:auto"}

 

**Resposta**

Os metadados da pasta recém-criada, conforme definido pelo endpoint /metadata.

**Exemplo:** `POST https://www.acme.com/api/createFolder`

```
-------------------------------

parentId=1234

name=New Folder ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

devoluções

```
{"title":"New Folder", 
 "kind":"folder""id":"5678",
 "viewLink":"",
 "downloadLink":"",
 "mimeType":"",
 "dateModified":"2014­06­05T17:39:45.251Z" 
 "size": "" 
 }
```

### Excluir um documento ou pasta

(Data de lançamento - TBD) Exclui um documento ou pasta com a ID fornecida no sistema externo. A exclusão de uma pasta também excluirá seu conteúdo.

URL

PUT /delete

**Parâmetros de consulta**

| Nome  | Descrição |
|---|---|
| documentId  | A ID do documento a ser excluída |
| folderId  |  A ID da pasta a ser excluída |

{style="table-layout:auto"}

Resposta Uma string JSON indicando sucesso ou falha, conforme especificado na seção Tratamento de erros abaixo.

**Exemplo:** PUT https://www.acme.com/api/delete id=1234

devoluções

```
{
"status": "success" 
}
```

devoluções

```
{
"status": "failure", "error": "File not found"
}
```


### Renomear um documento ou uma pasta

(Data de lançamento - TBD) Renomeia um documento ou uma pasta com a ID fornecida no sistema externo.

URL

PUT /rename

**Parâmetros de consulta**

| Nome  | Descrição |
|---|---|
| id | O documento ou ID da pasta a ser renomeado |
| name  | O novo nome do documento ou pasta |

{style="table-layout:auto"}

 

Resposta

Uma string JSON indicando sucesso ou falha, conforme especificado na seção Tratamento de erros abaixo.

**Exemplo:**

`PUT https://www.acme.com/api/rename`

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

```
{
"status": "success" 
}returns
{
"status": "failure", error: "Folder cannot be renamed because a folder with that name already exists." 
}
```

### Executar uma ação personalizada

(Data de lançamento - TBD) Esse terminal permitirá que um usuário do Workfront (ou talvez um evento de fluxo de trabalho automatizado) execute uma ação no sistema externo. O endpoint /customAction aceita um parâmetro &quot;name&quot;, que permite ao provedor do webhook implementar várias operações personalizadas.

O provedor webhook registra ações personalizadas no Workfront, ao incluir as ações na resposta /serviceInfo em customActions. O Workfront carrega essa lista ao configurar ou atualizar o provedor do webhook em Configurar > Documentos > Integrações personalizadas.\
![](assets/mceclip0-350x262.png)

Os usuários podem acionar a ação personalizada selecionando a seção &quot;Ações do documento&quot;\
![](assets/mceclip1-350x95.png)

**URL**

GET /customAction

**Parâmetros de consulta**

<table style="table-layout:auto">
 <col>
 <col>
 <thead>
  <tr>
   <th>Nome </th>
   <th>Descrição</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td><p>name</p></td>
   <td><p>O identificador que especifica o tipo de ação a ser executada. Esse valor corresponde a um dos valores customAction listados retornados pelo endpoint /serviceInfo.</p></td>
  </tr>
  <tr>
   <td>documentId </td>
   <td>A ID do documento da frente de trabalho para a qual a ação está sendo executada.</td>
  </tr>
  <tr>
   <td>documentVersionId </td>
   <td> A ID da versão do documento da frente de trabalho para a qual a ação está sendo executada.</td>
  </tr>
 </tbody>
</table>

 

**Resposta**

Uma string JSON indicando sucesso ou falha, conforme especificado na seção Tratamento de erros abaixo. Em caso de falha (ou seja, status = &quot;falha&quot;), o Workfront exibirá a mensagem de erro fornecida ao usuário.

**Exemplo:** https://sample.com/webhooks/customName?name=archive&amp;documentId=5502082c003a4f30 ddec2fb2b739cb7c&amp;documentVersionId=54b598a700e2342d6971597a5df1a8d3

response

```
{
"status": "success" 
}
```


## Tratamento de erros

Problemas podem surgir ao processar solicitações de API. Isso deve ser feito de maneira consistente em todos os pontos de extremidade da API. Quando ocorre um erro, o provedor do webhook faz o seguinte:

* Inclua um código de erro no cabeçalho de resposta. Os códigos de erro incluem:

   * 403 - Proibido. Indica que os tokens de solicitação estão ausentes ou são inválidos ou que as credenciais associadas aos tokens não têm acesso ao recurso especificado. Para provedores de webhook baseados em OAuth, a Workfront tentará recuperar novos tokens de acesso.
   * 404 - Não encontrado. Indica que o arquivo ou pasta especificado não existe.
   * 500 - Erro interno do servidor. Qualquer outro tipo de erro.

* Descreva o erro no corpo da resposta usando o seguinte formato:


```
{
"status": "error"
"error": "Sample error message" 
}
```


## Teste

Para verificar se a implementação do webhook do documento funciona corretamente, execute os seguintes testes. Esses são testes manuais que passam pela interface da Web do Workfront e acessam indiretamente os endpoints de sua implementação do webhook.

### Pré-requisitos

Para executar esses testes, você precisará do seguinte:

* Uma conta Workfront com o Gerenciamento Avançado de Documentos (ADM) ativado
* Um usuário do Workfront para esta conta com direitos de administrador do sistema
* Uma instância do Webhook de documento, que são pontos de extremidade HTTP, pode ser acessada pelo Workfront

Esses testes também pressupõem que você já tenha registrado a instância do Webhook do documento no Workfront em Configurar > Documentos > Integrações personalizadas.

### Teste 1: Provisionar o serviço do Webhook de documentos para um usuário

Testa o URL de autenticação e o URL do ponto de extremidade do token para provedores do Webhook baseados em OAuth.

1. No Workfront, vá para a página principal de Documentos clicando no link Documents na barra de navegação superior.
1. Clique na lista suspensa Adicionar documentos e selecione o serviço Webhook de documentos em Adicionar serviço.
1. (Somente serviços OAuth) Após concluir a etapa anterior, você verá a página de autenticação OAuth2 do seu serviço ser carregada em uma janela pop-up. (Observação: você pode ser solicitado a fazer logon em seu serviço primeiro.) Na página de autenticação, conceda à Workfront acesso à conta do usuário clicando no botão Confiar ou Permitir .
1. Verifique se o serviço foi adicionado à lista suspensa Adicionar documentos . Se não o vir inicialmente, tente atualizar seu navegador.

### Teste 2: Vincule um documento aos Testes do Workfront aos seguintes endpoints: /files, /metadata

1. No Workfront, vá para a página principal de Documentos clicando no link Documents na barra de navegação superior.
1. Selecione o serviço Webhook do documento em Adicionar documentos.
1. No modal , navegue pela estrutura de pastas.
1. Verifique se você consegue navegar na estrutura de pastas corretamente.
1. Selecionar e vincular um documento ao Workfront

### Teste 3: Navegue até um documento no sistema de gerenciamento de conteúdo

Testa os seguintes endpoints: /metadata (especificamente o viewLink)

1. Vincular um documento ao Workfront
1. Selecione o documento e clique no link Open .
1. Verifique se o documento abre em uma nova guia.

### Teste 4: Navegue até um documento no sistema de gerenciamento de conteúdo (com logon)

Testa os seguintes endpoints: /metadata (especificamente o viewLink)

1. Verifique se você está desconectado do sistema de gerenciamento de conteúdo.
1. Vincule um documento ao Workfront.
1. Selecione o documento e clique no link Open .
1. Verifique se a tela de logon do sistema de gerenciamento de conteúdo é carregada em uma nova guia.
1. Faça logon e verifique se você foi levado para o documento

### Teste 5: Baixe o documento do sistema de gerenciamento de conteúdo

Testa os seguintes endpoints: /metadata (especificamente o downloadLink)

1. Vincule um documento ao Workfront.
1. Selecione o documento e clique no link Download .
1. Verifique se o download começa.

### Teste 6: Pesquisar conteúdo

Testa os seguintes endpoints: /search

1. No Workfront, vá para a página principal de Documentos clicando no link Documents na barra de navegação superior.
1. Selecione o serviço Webhook do documento em Adicionar documentos.
1. No modal , faça uma pesquisa.
1. Verifique se os resultados da pesquisa estão corretos.

### Teste 7: Enviar documento do Workfront para o sistema de gerenciamento de conteúdo

Testa os seguintes endpoints: /files, /uploadInit, /upload

1. No Workfront, vá para a página principal de Documentos clicando no link Documents na barra de navegação superior.
1. Carregar um documento no Workfront a partir do seu computador
1. Vá para a página de detalhes do documento
1. Na lista suspensa Ações do documento , selecione o serviço Webhook do documento em Enviar para...
1. Vá para a pasta de destino desejada e clique no botão Save .
1. Verifique se o documento foi carregado no local correto no sistema de gerenciamento de conteúdo.

### Teste 8: Exibir miniaturas no Workfront

Testa os seguintes endpoints: /miniatura

1. Vincule um documento ao Workfront.
1. Selecione o documento na lista.
1. Verifique se a miniatura aparece no painel direito.

### Teste 9: Obter os bytes de conteúdo

Testa os seguintes endpoints: /download

1. Vincule um documento ao Workfront.
1. Vá para a página de detalhes do documento.
1. Envie o documento para o Workfront selecionando Ações do documento > Enviar para... > Workfront. Isso criará uma nova versão de documento no Workfront.
1. Baixe o documento do Workfront clicando no link Download .

### Teste 10: Atualizar token de acesso (somente provedores do Webhook OAuth2)

Testa os seguintes endpoints: URL do ponto de extremidade do token

1. Provisionar o serviço do Webhook de documentos para um usuário
1. Invalidar o token de acesso do usuário ao aguardar o tempo limite de 1 ou 2) invalidá-lo manualmente no sistema externo.
1. Atualize o token de acesso no Workfront. Você pode fazer isso, por exemplo, vinculando um documento ao Workfront. Você saberá que o token de acesso foi atualizado com êxito se conseguir navegar e vincular um documento.

>[!NOTE]
>
>Atualmente, o Enviar para... não está disponível para documentos vinculados. Isso será adicionado pelo Workfront. Você pode testar o endpoint /download acessando o endpoint manualmente usando um cliente REST, como o Postman. Como alternativa, o endpoint /download pode ser testado gerando uma prova digital. Para ativar a prova digital, entre em contato com a Workfront.

## Versões

* Versão 1.0 (Data de lançamento - maio de 2015)

   * Especificação inicial

* Versão 1.1 (Data de lançamento - junho de 2015)

   * Atualizado /uploadInit - Adição de documentId e documentVersionId

* Versão 1.2 (Data de lançamento - outubro de 2015)

   * Adição de /createFolder

