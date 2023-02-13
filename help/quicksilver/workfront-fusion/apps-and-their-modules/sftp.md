---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos SFTP
description: O [!DNL Adobe Workfront Fusion SFTP] Os módulos permitem monitorar as alterações de arquivo em uma pasta/subpasta selecionada, fazer upload de novos arquivos para a pasta desejada, modificar ou excluir arquivos existentes que já estão em uma pasta ou alterar permissões de arquivo.
author: Becky
feature: Workfront Fusion
exl-id: aacc61f8-ffc3-48db-9f54-188685c52067
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '1883'
ht-degree: 0%

---

# Módulos SFTP

O [!DNL Adobe Workfront Fusion] SFOs módulos TP permitem monitorar as alterações de arquivo em uma pasta/subpasta selecionada, fazer upload de novos arquivos para a pasta desejada, modificar ou excluir arquivos existentes que já estão em uma pasta ou alterar permissões de arquivo.

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

Para usar o SFTP com [!DNL Workfront Fusion], é necessário ter uma conta SFTP (como [!DNL GoDaddy] hospedagem na web).

## Conectar SFTP ao [!DNL Workfront Fusion] {#connect-sftp-to-workfront-fusion}

Para conectar sua conta SFTP a [!DNL Workfront Fusion] você precisa inserir o host de destino e as credenciais SFTP (nome de usuário e senha ou nome de usuário e chave) no módulo [!UICONTROL Criar uma conexão] caixa de diálogo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome da conexão]</td> 
   <td> <p> Insira o nome da conexão SFTP.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Host]</p> </td> 
   <td> <p>Insira o nome do host do servidor SFTP que você deseja conectar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Port] </td> 
   <td> <p>Insira a porta do servidor SFTP. Por exemplo, 22.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Auth type]</p> </td> 
   <td> <p>Selecione o método de autorização que deseja usar para se conectar ao servidor SFTP.</p> 
    <ul> 
     <li><strong>[!UICONTROL Nome de usuário e senha]</strong>: Insira suas credenciais.</li> 
     <li> <p><strong>[!UICONTROL Nome de usuário e chave]</strong>: Insira seu nome de usuário e a chave privada/certificado</p> <p>Faça upload da chave privada para usar a autorização do lado do cliente ou faça upload do certificado (arquivo P12 ou PFX) se desejar usar o TLS usando o certificado autoassinado. Se estiver usando a autorização de certificado do lado do cliente, você pode inserir o certificado da autoridade de certificação aqui.</p> <p>[!DNL Workfront Fusion] não retém ou armazena dados (arquivos, senhas) fornecidos aqui. O arquivo e a senha são usados apenas para extrair uma chave privada/certificado.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Depois de inserir as informações de conexão, clique em **[!UICONTROL Continuar]** para estabelecer uma conexão.

## [!UICONTROL SFTP] módulos e seus campos

Ao configurar [!UICONTROL SFTP] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!UICONTROL SFTP] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Triggers

#### [!UICONTROL Assistir arquivos em uma pasta]

Retorna arquivos com detalhes quando um arquivo é criado ou alterado em uma pasta especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Para obter instruções sobre como conectar sua conta SFTP a [!DNL Workfront Fusion], consulte <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Conectar SFTP ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Insira ou mapeie a pasta que deseja assistir. Você pode especificar um caminho absoluto, como <code>/home/user/</code>. Ou você pode especificar um caminho relativo apontando para uma pasta específica do usuário conectado, como <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>Tamanho do buffer [B]</td> 
   <td> <p> Insira o tamanho do buffer em bytes. O valor define o tamanho das partes transferidas do servidor. Alguns servidores podem causar problemas ou arquivos corrompidos quando o valor é muito alto.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de arquivos retornados]</td> 
   <td> <p> Defina o número máximo de arquivos que [!DNL Workfront Fusion] funcionará durante um ciclo</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Observação de subpastas em uma pasta]

Retorna pastas com detalhes quando uma pasta é criada ou alterada em uma pasta especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta SFTP a [!DNL Workfront Fusion], consulte <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Conectar SFTP ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Insira ou mapeie a pasta que deseja assistir. Você pode especificar um caminho absoluto, como <code>/home/user/</code>. Ou você pode especificar um caminho relativo apontando para uma pasta específica do usuário conectado, como <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de arquivos retornados]</td> 
   <td> <p> Defina o número máximo de pastas que [!DNL Workfront Fusion] retornará durante um ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ações

#### [!UICONTROL Listar o conteúdo de uma pasta]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Para obter instruções sobre como conectar sua conta SFTP a [!DNL Workfront Fusion], consulte <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Conectar SFTP ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show] </td> 
   <td> <p>Selecione se deseja recuperar arquivos, pastas ou ambos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Insira ou mapeie a pasta que contém os arquivos ou pastas que deseja listar. Você pode especificar um caminho absoluto, como <code>/home/user/</code>. Ou você pode especificar um caminho relativo apontando para uma pasta específica do usuário conectado, como <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>Insira ou mapeie o termo de pesquisa. Por exemplo, se você deseja pesquisar por arquivos com a extensão de arquivo .txt, insira <code>.txt</code>.Também é possível inserir ou mapear o nome do arquivo que deseja pesquisar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Classificar por]</td> 
   <td> <p> Selecione se deseja classificar os resultados por nome de arquivo, tamanho, data de último acesso ou data da última modificação.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordem de classificação] </td> 
   <td> <p>Selecione se o resultado deve ser retornado em ordem crescente ou decrescente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Continuar a execução da rota mesmo se o módulo não retornar nenhum resultado]</p> </td> 
   <td>Ative essa opção para garantir que esse módulo não interrompa o cenário se não retornar resultados.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de resultados retornados]</td> 
   <td> <p> Defina o número máximo de resultados que [!DNL Workfront Fusion] retornará durante um ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter arquivos]

Esse módulo lista arquivos de uma pasta especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Para obter instruções sobre como conectar sua conta SFTP a [!DNL Workfront Fusion], consulte <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Conectar SFTP ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tamanho do buffer [B]]</td> 
   <td> <p> Insira o tamanho do buffer em bytes. O valor define o tamanho das partes transferidas do servidor. Alguns servidores podem causar problemas ou arquivos corrompidos quando o valor é muito alto.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Insira ou mapeie a pasta que contém os arquivos ou pastas que deseja listar. Você pode especificar um caminho absoluto, como <code>/home/user/</code>. Ou você pode especificar um caminho relativo apontando para uma pasta específica do usuário conectado, como <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>Insira ou mapeie o termo de pesquisa. Por exemplo, se você deseja pesquisar por arquivos com a extensão de arquivo .txt, insira <code>.txt</code>.Também é possível inserir ou mapear o nome do arquivo que deseja pesquisar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Classificar por]</td> 
   <td> <p> Selecione se deseja classificar os resultados pelo nome do arquivo, tamanho, data de último acesso ou data da última modificação.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordem de classificação]</td> 
   <td> <p> Selecione se o resultado deve ser retornado em ordem crescente ou decrescente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Continuar a execução da rota mesmo se o módulo não retornar nenhum resultado]</p> </td> 
   <td>Ative essa opção para garantir que esse módulo não interrompa o cenário se não retornar resultados.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de resultados retornados]</td> 
   <td> <p> Defina o número máximo de arquivos que [!DNL Workfront Fusion] retornará durante um ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um arquivo]

Esse módulo recupera detalhes do arquivo, incluindo os dados de um arquivo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Para obter instruções sobre como conectar sua conta SFTP a [!DNL Workfront Fusion], consulte <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Conectar SFTP ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tamanho do buffer [B]]</td> 
   <td> <p> Insira o tamanho do buffer em bytes. O valor define o tamanho das partes transferidas do servidor. Alguns servidores podem causar problemas ou arquivos corrompidos quando o valor é muito alto.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Caminho do arquivo] </td> 
   <td> <p>Insira o caminho para o arquivo. Você pode especificar um caminho absoluto, como <code>/home/user/file.txt</code>. Ou você pode especificar um caminho relativo apontando para uma pasta específica do usuário conectado, como <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Fazer upload de um arquivo]

Esse módulo permite fazer upload de um arquivo para o servidor SFTP.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Para obter instruções sobre como conectar sua conta SFTP a [!DNL Workfront Fusion], consulte <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Conectar SFTP ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Especifique uma pasta existente como o local de armazenamento do arquivo. Você pode especificar um caminho absoluto, como <code>/home/user/</code>. Ou você pode especificar um caminho relativo apontando para uma pasta específica do usuário conectado, como <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arquivo de origem]</td> 
   <td> <p> Mapeie o arquivo de origem de um módulo anterior, como [!UICONTROL Dropbox] &gt; [!UICONTROL Obter arquivo]. Você também pode inserir ou mapear o nome do arquivo e os dados do arquivo.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Permissões]</p> </td> 
   <td> <p>Defina as permissões desejadas para o arquivo ou pasta. Use parâmetros de chmod. Por exemplo: <code>777 </code>ou <code>-rwxrwxrwx</code>.</p> <p>Para obter mais detalhes sobre o chmod, consulte o <a href="https://ss64.com/bash/chmod.html">documentação do chmod</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Renomear um arquivo]

Renomeia um arquivo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Para obter instruções sobre como conectar sua conta SFTP a [!DNL Workfront Fusion], consulte <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Conectar SFTP ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Caminho do arquivo]</td> 
   <td> <p> Insira o caminho para o arquivo que deseja renomear. Você pode especificar um caminho absoluto, como <code>/home/user/file.txt</code>. Ou você pode especificar um caminho relativo apontando para uma pasta específica do usuário conectado, como <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Novo nome de arquivo]</td> 
   <td> <p> Insira o novo nome do arquivo, incluindo a extensão de arquivo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover um arquivo]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Para obter instruções sobre como conectar sua conta SFTP a [!DNL Workfront Fusion], consulte <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Conectar SFTP ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Caminho do arquivo]</td> 
   <td> <p> Insira o caminho para o arquivo que deseja mover. Você pode especificar um caminho absoluto, como <code>/home/user/file.txt</code>. Ou você pode especificar um caminho relativo apontando para uma pasta específica do usuário conectado, como <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nova pasta]</td> 
   <td> <p> Insira o caminho para o novo local do arquivo. Você pode especificar um caminho absoluto, como <code>/home/user/</code>. Ou você pode especificar um caminho relativo apontando para uma pasta específica do usuário conectado, como <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir um arquivo]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Para obter instruções sobre como conectar sua conta SFTP a [!DNL Workfront Fusion], consulte <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Conectar SFTP ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Caminho do arquivo]</td> 
   <td> <p> Insira o caminho para o arquivo que deseja excluir. Você pode especificar um caminho absoluto, como <code>/home/user/file.txt</code>. Ou você pode especificar um caminho relativo apontando para uma pasta específica do usuário conectado, como <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar permissões de arquivo]

Permite alterar as permissões do arquivo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Para obter instruções sobre como conectar sua conta SFTP a [!DNL Workfront Fusion], consulte <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Conectar SFTP ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Caminho do arquivo]</td> 
   <td> <p> Insira o caminho para o arquivo que deseja mover. Você pode especificar um caminho absoluto, como <code>/home/user/file.txt</code>. Ou você pode especificar um caminho relativo apontando para uma pasta específica do usuário conectado, como <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Permissões]</p> </td> 
   <td> <p>Defina as permissões de arquivo desejadas. Use os parâmetros de chmod. Por exemplo, <code>777 </code>ou <code>-rwxrwxrwx</code>.</p> <p>Deve corresponder ao padrão <code> /(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>Para obter mais detalhes sobre o chmod, consulte o <a href="https://ss64.com/bash/chmod.html">documentação do chmod</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar pasta]

Cria uma nova pasta no local especificado.

>[!NOTE]
>
>Se a pasta já existir, o módulo emitirá um erro. Para continuar o fluxo sem interrupções, anexe uma rota do manipulador de erros ao módulo para capturar o erro e usar o [!UICONTROL Retomar] diretiva para continuar o fluxo. Para obter informações sobre como anexar uma rota do manipulador de erros, consulte [Tratamento de erros em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md). Para obter informações sobre a rota do manipulador de erros, consulte [Diretivas relativas ao tratamento de erros [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Para obter instruções sobre como conectar sua conta SFTP a [!DNL Workfront Fusion], consulte <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Conectar SFTP ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Especifique uma pasta existente como o local de armazenamento para a nova pasta. Você pode especificar um caminho absoluto, como <code>/home/user/file.txt</code>. Ou você pode especificar um caminho relativo apontando para uma pasta específica do usuário conectado, como <code>./</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome da pasta]</td> 
   <td> <p> Insira o nome da pasta.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Permissões]</p> </td> 
   <td> <p>Defina as permissões de pasta desejadas. Use parâmetros de chmod. Por exemplo, <code>777 </code>ou <code>-rwxrwxrwx</code>.</p> <p>Deve corresponder ao padrão <code>/(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>Para obter mais detalhes sobre o chmod, consulte o <a href="https://ss64.com/bash/chmod.html">Página do Homem de Moda</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir uma pasta]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Para obter instruções sobre como conectar sua conta SFTP a [!DNL Workfront Fusion], consulte <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Conectar SFTP ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Folder Path]</td> 
   <td> <p> Especifique o caminho para a pasta que deseja excluir. Você pode especificar um caminho absoluto, como <code>/home/user/</code>. Ou você pode especificar um caminho relativo apontando para uma pasta específica do usuário conectado, como <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
