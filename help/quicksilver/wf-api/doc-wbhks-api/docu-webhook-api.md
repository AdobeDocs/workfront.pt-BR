---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: API de webhooks do documento
description: Os Webhooks de documentos do Adobe Workfront definem um conjunto de endpoints de API pelos quais o Workfront faz chamadas de API autorizadas para um Provedor de documentos externo. Isso permite que qualquer pessoa crie um plug-in middleware para qualquer provedor de armazenamento de documentos.
author: Becky
feature: Workfront API
role: Developer
exl-id: 7ac2c6c8-1cb8-49df-8d63-a6b47ad02a13
source-git-commit: 48de4553478fc42d88d81ea953440337f6684e50
workflow-type: tm+mt
source-wordcount: '3649'
ht-degree: 2%

---


# API de webhooks do documento

<!-- Audited: 5/2025 -->

Os Webhooks de documentos do Adobe Workfront definem um conjunto de endpoints de API pelos quais o Workfront faz chamadas de API autorizadas para um Provedor de documentos externo. Isso permite que qualquer pessoa crie um plug-in middleware para qualquer provedor de armazenamento de documentos.

A experiência do usuário para integrações baseadas em webhook será semelhante àquela das integrações de documento existentes, como Google Drive, Box e Dropbox. Por exemplo, um usuário do Workfront poderá executar as seguintes ações:

* Navegar pela estrutura de pastas do provedor de documentos externos
* Pesquisar arquivos
* Vincular arquivos ao Workfront
* Fazer upload de arquivos para o provedor de documentos externos
* Exibir uma miniatura do documento

## Implementação de referência

Para ajudar a iniciar o desenvolvimento de uma nova implementação de webhooks, o Workfront fornece uma implementação de referência. O código para isso pode ser encontrado em [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app). Essa implementação é baseada em Java e permite que o Workfront conecte documentos em um sistema de arquivos de rede.

## Registrar uma integração do Webhook

Os administradores do Workfront podem adicionar uma integração de webhook personalizada para a empresa navegando até Configuração > Documentos > Integrações personalizadas no Workfront. Na página Integração personalizada da Configuração, os administradores podem exibir uma lista de integrações existentes do Webhook. Nessa página, as integrações podem ser adicionadas, editadas, ativadas e desativadas. Para adicionar uma integração, clique no botão Adicionar integração.

### Campos disponíveis

Ao adicionar uma integração, o administrador inserirá valores nos seguintes campos:

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
   <td>URL da API base</td> 
   <td> <p>O local da API de retorno de chamada. Ao fazer chamadas para o sistema externo, o Workfront anexará o nome do ponto de extremidade a esse endereço. Por exemplo, se o administrador inseriu o URL da API de base, " https://www.mycompany.com/api/v1 ", o Workfront usaria o seguinte URL para obter os metadados de um documento: https://www.mycompany.com/api/v1/metadata?id=1234.</p> </td> 
  </tr> 
  <tr> 
   <td>Parâmetros de solicitação</td> 
   <td> <p>Valores opcionais a serem acrescentados à querystring de todas as chamadas para a API. Por exemplo, access_type</p> </td> 
  </tr> 
  <tr> 
   <td>Tipo de autenticação</td> 
   <td>OAuth2 ou ApiKey.</td> 
  </tr> 
  <tr> 
   <td>URL de autenticação</td> 
   <td> <p>(Somente OAuth2) O URL completo usado para autenticação de usuário. O Workfront navegará os usuários para esse endereço como parte do processo de provisionamento do OAuth. <br><br>Observação: o Workfront anexará um parâmetro de "estado" à cadeia de caracteres de consulta. O provedor deve transmitir isso de volta para o Workfront, anexando-o ao URI de redirecionamento do Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>URL token da extremidade final</td> 
   <td> <p>(Somente OAuth2) O URL completo da API usado para recuperar tokens OAuth2. Ele é hospedado pelo provedor de webhook ou pelo provedor de documento externo.</p> </td> 
  </tr> 
  <tr> 
   <td>ID do cliente</td> 
   <td>(Somente OAuth2) A ID do cliente OAuth2 para essa integração.</td> 
  </tr> 
  <tr> 
   <td>Segredo do cliente</td> 
   <td> <p>(Somente OAuth2) O segredo do cliente OAuth2 para essa integração.</p> </td> 
  </tr> 
  <tr> 
   <td>URL de redirecionamento do Workfront</td> 
   <td> <p>(Somente OAuth2) Esse é um campo somente leitura gerado pelo Workfront. Esse valor é usado para registrar essa integração com o provedor de documentos externos. <br><br>Observação: conforme descrito acima para a URL de Autenticação, o provedor deve anexar o parâmetro "state" e seu valor à querystring ao executar o redirecionamento.</p></td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td>  <p>(Somente ApiKey) Usado para fazer chamadas de API autorizadas para o provedor de webhook. A chave da API é emitida pelo provedor do webhook.</p></td> 
  </tr> 
 </tbody> 
</table>

 

## Autenticação

Os webhooks de documento do Workfront são compatíveis com duas formas diferentes de autenticação: OAuth2 e ApiKey. Em ambos os casos, o Workfront transmite tokens de autenticação no cabeçalho ao fazer uma chamada de API.

### OAuth2

O OAuth2 permite que o Workfront faça chamadas de API autorizadas para um provedor de webhook em nome de um usuário. Antes de fazer isso, o usuário deve conectar sua conta de provedor de documentos externos ao Workfront e conceder à Workfront acesso para agir em seu nome. Esse processo de handshaking só ocorre uma vez para cada usuário. Veja como isso funciona:

1. O usuário começa conectando a integração do webhook à conta. Atualmente, isso é feito clicando no menu suspenso Adicionar documento > Adicionar serviço > Nome da integração personalizada.
1. O Workfront navega o usuário para o URL de autenticação, que pode solicitar que o usuário faça logon no provedor de documentos externo. Esta página é hospedada pelo provedor de webhook ou pelo sistema de gerenciamento de documentos externo. Ao fazer isso, o Workfront adiciona um parâmetro de &quot;estado&quot; ao URL de autenticação. Esse valor deve ser passado de volta para o Workfront, anexando o mesmo valor ao URI de retorno do Workfront na etapa abaixo.
1. Depois de fazer logon no sistema externo (ou se o usuário já estiver conectado), o usuário é direcionado a uma página de Autenticação, que explica que a Workfront está solicitando acesso para executar um conjunto de ações em nome do usuário.
1. Se o usuário clicar no botão Permitir, o navegador será redirecionado para o URI de Redirecionamento do Workfront, adicionando &quot;code=`<code>`&quot; à querystring. De acordo com a especificação do OAuth2, esse token tem vida curta. A sequência de consulta também deve ter o seguinte: &quot;state=`<sent_by_workfront>`&quot;.
1. O Workfront processa essa solicitação e faz uma chamada de API para o URL do ponto de extremidade token com o código de autorização.
1. O URL do ponto de extremidade do token retorna um token de atualização e um token de acesso.
1. O Workfront armazena esses tokens e provisiona totalmente a integração de webhook para esse usuário.
1. A partir desse ponto, o Workfront poderá fazer chamadas autorizadas para a API do provedor do webhook. Ao fazer essas chamadas, o Workfront enviará o token de acesso no cabeçalho da solicitação HTTP, conforme mostrado abaixo:

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. Se o token de acesso tiver expirado, a Workfront fará uma chamada para o URL do ponto de extremidade do token para recuperar um novo token de acesso e, em seguida, tentará fazer a chamada de API autorizada novamente com o novo token de acesso.

### ApiKey

Fazer chamadas de API autorizadas para um provedor de webhook usando uma ApiKey é muito mais simples do que o OAuth2. Ao fazer uma chamada de API, o Workfront simplesmente passará o ApiKey e o nome de usuário do Workfront no cabeçalho da solicitação HTTP:

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

O provedor Webhook pode usar o nome de usuário para aplicar permissões específicas do usuário. Isso funciona melhor quando ambos os sistemas se conectam ao LDAP usando Single-Sign-On (SSO).

### Adicionar cabeçalhos de solicitação (opcional)

Além de usar tokens OAuth2 ou uma ApiKey para autenticação, o Workfront pode enviar um conjunto predefinido de cabeçalhos para o provedor do webhook para cada chamada de API. Um administrador do Workfront pode configurar isso ao registrar ou editar uma Integração de webook, conforme descrito na seção acima.

Por exemplo, pode ser usado para a Autenticação básica. Para fazer isso, o administrador do Workfront adicionaria as seguintes informações do Cabeçalho da solicitação na caixa de diálogo Integração personalizada:

   Autorização básica QWxhZGRpbjpvcGVuIHNlc2FtZQ==

onde QWxhZGRpbjpvcGVuIHNlc2FtZQ== é uma string codificada na base 64 de &quot;username:password&quot;. Consulte Autenticação básica. Desde que tenha sido adicionado, o Workfront passará isso no cabeçalho da solicitação HTTP, além de outros cabeçalhos de solicitação:

```
­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------

apiKey: 12345

username: johndoe@foo.com

Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

## Especificação da API

Veja abaixo uma lista de APIs que o provedor de webhook deve implementar para que os webhooks de documento funcionem.

### Obter tokens OAuth2 (somente autenticação OAuth2 necessária)

Retorna o token de atualização OAuth2 e o token de acesso para um usuário autenticado. Isso é chamado uma vez quando o usuário provisiona um Provedor de documentos. As chamadas subsequentes são feitas para obter um token de acesso atualizado.

HTTP Request POST /any/url

O URL é configurável e corresponde ao valor do URL do endpoint do token na página de configuração da integração personalizada.

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
   <td>Sim</td> 
   <td> <p>Os valores incluem "authorization_code" ou "refresh_token". O valor especificado indica qual dos dois parâmetros será passado para esta chamada de API: code ou refresh_token.</p> </td> 
  </tr> 
  <tr> 
   <td>código</td> 
   <td>Depende</td> 
   <td> <p>O código de autorização enviado ao Workfront logo após o usuário clicar no botão Conceder. Isso só é necessário quando o tipo de concessão é "authorization_code". O código de autorização deve ter uma vida curta, geralmente expirando em 10 minutos ou menos.</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token</td> 
   <td>Depende</td> 
   <td> <p>Isso só é necessário ao fazer chamadas subsequentes para recuperar um novo access_token, visto que o access_token anterior expirou. Ao enviar esse valor, defina o parâmetro grant_type como "refresh_token".</p> </td> 
  </tr> 
  <tr> 
   <td>client_id</td> 
   <td>Sim</td> 
   <td>A ID do cliente configurada no Workfront para essa integração personalizada.</td> 
  </tr> 
  <tr> 
   <td>client_secret</td> 
   <td>Sim</td> 
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
   <td> <p>Um token de longa duração usado para recuperar um novo access_token chamando esse método de API.</p> </td> 
  </tr> 
  <tr> 
   <td>expires_in </td> 
   <td>long</td> 
   <td>  <p>(Opcional) O tempo (em segundos) antes que o access_token expire, geralmente 3.600.</p></td> 
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

### Obter metadados para arquivo ou pasta

Retorna os metadados do arquivo ou pasta especificada.

**URL**

GET /metadata?id=[ID de documento ou pasta]

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
   <td>  <p>A ID de um arquivo ou pasta, conforme referenciado pelo provedor de webhook. Isso é diferente da ID de documento do Workfront. Para obter os metadados do diretório raiz, use o valor '/'.</p><p>Observação: o tamanho máximo da ID é de 255 caracteres.</p></td> 
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
   <td>título </td> 
   <td>String </td> 
   <td>O nome do documento ou pasta.</td> 
  </tr> 
  <tr> 
   <td>tipo </td> 
   <td>String </td> 
   <td>Especifica se este item é um arquivo ou uma pasta ("arquivo" ou "pasta").</td> 
  </tr> 
  <tr> 
   <td>id</td> 
   <td>String </td> 
   <td>A ID do arquivo ou pasta.</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>String </td> 
   <td> <p>O caminho de URL usado por um usuário para exibir o documento em uma janela do navegador. O URL pode ser hospedado pelo provedor de documentos ou pelo provedor de armazenamento externo nativo.</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>String </td> 
   <td> <p>O caminho de URL usado por um usuário para baixar o documento em uma janela do navegador. O URL pode ser hospedado pelo provedor de documentos ou pelo provedor de armazenamento externo nativo.</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>String </td> 
   <td>(Opcional) O tipo MIME do arquivo.</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>String </td> 
   <td>Última vez que este arquivo foi modificado (carimbo de data/hora RFC 3339 formatado).</td> 
  </tr> 
  <tr> 
   <td>tamanho</td> 
   <td>Long</td> 
   <td>(Opcional) O tamanho do arquivo em bytes.</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>Booleano</td> 
   <td><p> (Opcional) Indica se esse arquivo ou pasta é somente leitura para o usuário autenticado.</p><p> </p></td> 
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
>O tratamento de erros deve ser consistente em todas as chamadas de API. Consulte a seção Tratamento de erros abaixo para obter detalhes.

### Obter uma lista de itens em uma pasta

Retorna metadados dos arquivos e pastas de uma determinada pasta.

**URL**

GET /files

**Parâmetros de consulta**

| Nome  | Descrição |
|---|---|
| parentId  | A ID da pasta. Para obter os metadados do diretório raiz, use o valor &#39;/&#39;. |

{style="table-layout:auto"}

No momento, a API de webhooks de documentos não é compatível com paginação.

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

Retorna metadados dos arquivos e pastas retornados de uma pesquisa. Isso pode ser implementado como uma pesquisa de texto completo ou como uma consulta de banco de dados regular. O Workfront chama o endpoint /search quando o usuário realiza uma pesquisa no navegador de arquivos externos.

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
   <td>O termo ou frase de pesquisa.</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>(Opcional) A ID da pasta da qual a pesquisa foi executada. <br><br>Observação: este é um espaço reservado para um recurso futuro no Workfront. Atualmente, o Workfront não passa esse parâmetro. </p> </td> 
  </tr> 
  </tbody> 
</table>

No momento, a API de webhooks de documentos não é compatível com paginação.

 

**Resposta**

JSON que contém uma lista de metadados para arquivos e pastas que correspondem à consulta. O que constitui uma &quot;correspondência&quot; é determinado pelo provedor de webhook. Idealmente, ele deve fazer uma pesquisa baseada em texto completo ou nome de arquivo.

**Exemplo:** `https://www.acme.com/api/search?query=test-query`

**Resposta**

```
[
{ File/Folder Metadata },
{ File/Folder Metadata }
]
```

### Obter o conteúdo de um documento

Retorna os bytes brutos de um documento.

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

Retorna os bytes brutos da miniatura de um documento.

**URL**

GET /miniatura

**Parâmetros de consulta**

| Nome  | Descrição |
|---|---|
| id  | A ID do documento. |
| tamanho  | A largura da miniatura. |

{style="table-layout:auto"}

 

**Resposta**

Os bytes brutos da miniatura.

**Exemplo:** `https://www.acme.com/api/thumbnail?id=123456`

### Carregar um arquivo - Parte 1 de 2

O upload de um arquivo para um provedor de armazenamento de documentos é um processo de duas etapas que requer dois endpoints de API separados. O Workfront inicia o processo de upload chamando /uploadInit. Esse endpoint retorna uma ID de documento, que é passada para /upload ao carregar os bytes do documento. Dependendo do sistema de armazenamento de documentos subjacente, pode ser necessário criar um documento de comprimento zero e, em seguida, atualizar o conteúdo do documento posteriormente.

Adicionado à versão 1.1 desta especificação, o ID do documento e o ID da versão do documento podem ser usados para recuperar informações adicionais do Workfront. Por exemplo, se o sistema de gerenciamento de documentos quiser informações adicionais sobre o documento, o código de implementação do webhook poderá usar a ID do documento para recuperar essas informações usando a API RESTful do Workfront. Como prática recomendada, essas informações podem vir de campos de dados personalizados no documento e sua tarefa, problema ou projeto.

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
   <td>A ID da pasta pai, conforme referenciado pelo provedor do webhook.</td> 
  </tr> 
  <tr> 
   <td>filename </td> 
   <td>O nome do documento.</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>A ID do documento do Workfront (adicionada na versão 1.1).</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>A ID da versão do documento do Workfront (adicionada na versão 1.1).</td> 
  </tr> 
 </tbody> 
</table>

 

**Resposta**

Os metadados do arquivo, conforme definido pelo endpoint /metadata.

**Exemplo:** `https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&docu mentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b`

**Resposta**

`[file_metadata]` inclui a nova ID de documento usada pelo provedor de documentos.

### Carregar um arquivo - Parte 2 de 2

Carrega os bytes de um documento para o provedor de webhook.

**URL**

PUT /upload

**Parâmetros de consulta**

| Nome  | Descrição |
|---|---|
| id  |  A ID do documento que acabou de ser criada. |


 

**Solicitar corpo**

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

**Exemplo:** `https://www.acme.com/api/upload?id=1234` *[bytes de documentos incluídos no fluxo de atualização]*

**Resposta**

```
{
"result":"success"
}
```

### Obter informações sobre o serviço 

(Data de lançamento - A ser definido) Retorna informações sobre o serviço, como recursos e funcionalidades. O Workfront usará essas informações para personalizar a interface do usuário no Workfront. Por exemplo, se a implementação de webhook contiver algumas ações personalizadas, o JSON deverá listar essas operações no JSON. Os usuários poderão então invocar essas ações a partir do Workfront.

**URL**

GET /serviceInfo

Parâmetros de consulta

Nenhum. Além disso, as chamadas para esse endpoint não devem exigir autenticação.

**Resposta**

JSON que contém informações sobre este serviço.

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
   <td>A versão de webhook implementada por este serviço. Esse é o número da versão listado na parte superior desta especificação.</td> 
  </tr> 
  <tr> 
   <td>version </td> 
   <td>String </td> 
   <td>O número da versão interna deste serviço. Esse número é determinado pelo provedor de serviços de webhook e é usado apenas para fins informativos.<br><br></td> 
  </tr> 
  <tr> 
   <td>editor </td> 
   <td>String </td> 
   <td>O nome da empresa que fornece a implementação do webhook.</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>String </td> 
   <td>Uma lista contendo os endpoints de API implementados por este serviço. Isso pode ser usado para garantir que a interface do usuário no Workfront reflita os recursos oferecidos pelo provedor de webhook. Cada item na lista deve incluir o nome do endpoint (como "pesquisa").</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>String</td> 
   <td>  <p>Uma lista contendo as operações personalizadas implementadas por este webhook. Cada item da lista inclui um nome e um nome de exibição. O nome de exibição aparecerá no menu suspenso Ações do documento no Workfront. Clicar no item no menu suspenso chamará a ação no webhook, chamando o ponto de extremidade /customAction.</p></td> 
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
| parentId  | A ID da pasta na qual a pasta deve ser criada. |
| name  | O nome da nova pasta. |

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

### Excluir um documento ou uma pasta

(Data de lançamento - A ser definida) Exclui um documento ou pasta com a ID fornecida no sistema externo. A exclusão de uma pasta também excluirá seu conteúdo.

URL

PUT /delete

**Parâmetros de consulta**

| Nome  | Descrição |
|---|---|
| documentId  | A ID do documento a ser excluído. |
| folderId  | A ID da pasta a ser excluída. |

{style="table-layout:auto"}

Resposta Uma string JSON que indica sucesso ou falha, conforme especificado na seção Tratamento de erros abaixo.

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

(Data de lançamento - A ser definida) Renomeia um documento ou pasta com a ID fornecida no sistema externo.

URL

PUT /rename

**Parâmetros de consulta**

| Nome  | Descrição |
|---|---|
| id | A ID do documento ou da pasta a ser renomeada. |
| name  | O novo nome do documento ou pasta. |

{style="table-layout:auto"}

 

Resposta

Uma string JSON que indica sucesso ou falha, conforme especificado na seção Tratamento de erros abaixo.

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

(Data de lançamento - A ser definida) Esse endpoint permitirá que um usuário do Workfront (ou talvez um evento de fluxo de trabalho automatizado) execute uma ação no sistema externo. O ponto de extremidade /customAction aceita um parâmetro &quot;name&quot;, que permite que o provedor de webhook implemente várias operações personalizadas.

O provedor de webhook registra ações personalizadas com o Workfront incluindo as ações na resposta /serviceInfo em customActions. O Workfront carrega essa lista ao configurar ou atualizar o provedor de webhook em Configurar > Documentos > Integrações personalizadas.\
![Executar uma ação personalizada](assets/mceclip0-350x262.png)

Os usuários podem acionar a ação personalizada selecionando a seção em Ações do documento.\
![Acionar ações personalizadas](assets/mceclip1-350x95.png)

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
   <td><p>O identificador que especifica o tipo de ação a ser executada. Esse valor corresponde a um dos valores de customAction listados retornados pelo ponto de extremidade /serviceInfo.</p></td>
  </tr>
  <tr>
   <td>documentId </td>
   <td>A ID do documento do Workfront para a qual a ação está sendo executada.</td>
  </tr>
  <tr>
   <td>documentVersionId </td>
   <td>O ID da versão do documento do Workfront para o qual a ação está sendo executada.</td>
  </tr>
 </tbody>
</table>

 

**Resposta**

Uma string JSON que indica sucesso ou falha, conforme especificado na seção Tratamento de erros abaixo. Na falha (ou seja, status = &quot;failure&quot;), o Workfront exibirá a mensagem de erro fornecida para o usuário.

**Exemplo:** https://sample.com/webhooks/customName?name=archive&amp;documentId=5502082c003a4f30 ddec2fb2b739cb7c&amp;documentVersionId=54b598a700e2342d6971597a5df1a8d3

resposta

```
{
"status": "success" 
}
```


## Tratamento de erros

Problemas podem surgir ao processar solicitações de API. Isso deve ser tratado de forma consistente em todos os endpoints da API. Quando ocorre um erro, o provedor do webhook faz o seguinte:

* Incluir um código de erro no cabeçalho da resposta. Os códigos de erro incluem:

   * 403 - Proibido. Indica que os tokens de solicitação estão ausentes ou são inválidos, ou que as credenciais associadas aos tokens não têm acesso ao recurso especificado. Para provedores de webhook baseados em OAuth, o Workfront tentará recuperar novos tokens de acesso.
   * 404 - Não encontrado. Indica que o arquivo ou pasta especificada não existe.
   * 500 - Erro interno do servidor. Qualquer outro tipo de erro.

* Descreva o erro no corpo da resposta usando o seguinte formato:


```
{
"status": "error"
"error": "Sample error message" 
}
```


## Testando

Para verificar se a implementação do webhook do seu documento funciona corretamente, execute os testes a seguir. Esses são testes manuais que passam pela interface da Web do Workfront e atingem indiretamente os endpoints da implementação do webhook.

### Pré-requisitos

Para executar esses testes, você precisará do seguinte:

* Uma conta do Workfront com o Gerenciamento avançado de documentos (ADM) habilitado.
* Um usuário do Workfront para esta conta com direitos de administrador do sistema.
* Uma instância do Webhook de documentos, cujos pontos de extremidade HTTP são acessíveis para o Workfront.

Esses testes também pressupõem que você já tenha registrado a instância do Webhook do documento no Workfront em Configuração > Documentos > Integrações personalizadas.

### Teste 1: provisionar o serviço Webhook do documento para um usuário

Testa o URL de autenticação e o URL do ponto de extremidade do token para provedores de Webhook baseados em OAuth.

1. No Workfront, vá para a página principal Documentos clicando no link Documentos na barra de navegação superior.
1. Clique na lista suspensa Adicionar documentos e selecione o serviço Webhook de documentos em Adicionar serviço.
1. (Somente serviços OAuth) Depois de concluir a etapa anterior, você verá o carregamento da página de autenticação OAuth2 do serviço em uma janela pop-up. (Observação: você pode ser solicitado a fazer logon no serviço primeiro.) Na página de autenticação, conceda acesso à conta do usuário pelo Workfront clicando no botão Confiar ou Permitir.
1. Verifique se o serviço foi adicionado à lista suspensa Adicionar documentos. Caso não o veja inicialmente, tente atualizar o navegador.

### Teste 2: vincular um documento no Workfront Testa os seguintes endpoints: /files, /metadata

1. No Workfront, vá para a página principal Documentos clicando no link Documentos na barra de navegação superior.
1. Selecione o serviço Webhook de documentos em Adicionar documentos.
1. Na modal, navegue pela estrutura de pastas.
1. Verifique se você pode navegar pela estrutura de pastas corretamente.
1. Selecione e vincule um documento ao Workfront.

### Teste 3: Navegar até um documento no sistema de gerenciamento de conteúdo

Testa os seguintes pontos de extremidade: /metadata (especificamente o viewLink).

1. Vincule um documento ao Workfront.
1. Selecione o documento e clique no link Abrir.
1. Verifique se o documento abre em uma nova guia.

### Teste 4: Navegar até um documento no sistema de gerenciamento de conteúdo (com logon)

Testa os seguintes pontos de extremidade: /metadata (especificamente o viewLink).

1. Verifique se você está desconectado do sistema de gerenciamento de conteúdo.
1. Vincule um documento ao Workfront.
1. Selecione o documento e clique no link Abrir.
1. Verifique se a tela de logon do sistema de gerenciamento de conteúdo é carregada em uma nova guia.
1. Faça logon e verifique se você está direcionado ao documento.

### Teste 5: baixar o documento do sistema de gerenciamento de conteúdo

Testa os seguintes pontos de extremidade: /metadata (especificamente o downloadLink).

1. Vincule um documento ao Workfront.
1. Selecione o documento e clique no link Download.
1. Verifique se o download foi iniciado.

### Teste 6: pesquisar conteúdo

Testa os seguintes pontos de extremidade: /search

1. No Workfront, vá para a página principal Documentos clicando no link Documentos na barra de navegação superior.
1. Selecione o serviço Webhook de documentos em Adicionar documentos.
1. No modal, execute uma pesquisa.
1. Verifique se os resultados da pesquisa estão corretos.

### Teste 7: enviar documento do Workfront para o sistema de gerenciamento de conteúdo

Testa os seguintes pontos de extremidade: /files, /uploadInit, /upload

1. No Workfront, vá para a página principal Documentos clicando no link Documentos na barra de navegação superior.
1. Carregue um documento do seu computador para o Workfront.
1. Vá para a página de detalhes do documento.
1. Na lista suspensa Ações do documento, selecione o serviço Webhook do documento em Enviar para...
1. Vá para a pasta de destino desejada e clique no botão Save.
1. Verifique se o documento foi carregado no local correto no sistema de gerenciamento de conteúdo.

### Teste 8: exibir miniaturas no Workfront

Testa os seguintes pontos de extremidade: /thumbnail

1. Vincule um documento ao Workfront.
1. Selecione o documento na lista.
1. Verifique se a miniatura aparece no painel direito.

### Teste 9: obter os bytes de conteúdo

Testa os seguintes pontos de extremidade: /download

1. Vincule um documento ao Workfront.
1. Vá para a página de detalhes do documento.
1. Envie o documento para o Workfront selecionando Ações do documento > Enviar para... > Workfront. Isso criará uma nova versão do documento no Workfront.
1. Baixe o documento do Workfront clicando no link Download.

### Teste 10: atualizar token de acesso (somente provedores de Webhook OAuth2)

Testa os seguintes endpoints: URL do endpoint do token

1. Provisione um serviço de Webhook de documentos para um usuário.
1. Invalide o token de acesso do usuário aguardando o tempo limite ou invalidando-o manualmente no sistema externo.
1. Atualize o token de acesso no Workfront. Você pode fazer isso, por exemplo, vinculando um documento ao Workfront. Você saberá que o token de acesso foi atualizado com êxito se conseguir navegar e vincular um documento.

>[!NOTE]
>
>Atualmente, Enviar para... não está disponível para documentos vinculados. Isso será adicionado pelo Workfront. Você pode testar o terminal /download acessando o terminal manualmente usando um cliente REST, como o Postman. Como alternativa, o endpoint /download pode ser testado gerando uma prova digital. Para ativar a prova digital, entre em contato com a Workfront.

## Versões

* Versão 1.0 (Data de lançamento - maio de 2015)

   * Especificação inicial

* Versão 1.1 (Data de lançamento - junho de 2015)

   * Atualização de /uploadInit - documentId e documentVersionId adicionados

* Versão 1.2 (Data de lançamento - outubro de 2015)

   * Adição de /createFolder

