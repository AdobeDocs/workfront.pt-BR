---
filename: ftp-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos FTP
description: Os módulos FTP permitem monitorar as alterações de arquivos em uma pasta selecionada, fazer upload de novos arquivos para a pasta desejada e modificar ou excluir arquivos existentes que já estão em uma pasta.
author: Becky
feature: Workfront Fusion
exl-id: 360825a4-4580-4039-894e-583e82132ed6
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1335'
ht-degree: 0%

---

# Módulos FTP

Os módulos FTP permitem monitorar as alterações de arquivos em uma pasta selecionada, fazer upload de novos arquivos para a pasta desejada e modificar ou excluir arquivos existentes que já estão em uma pasta.

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
   <p>Requisito atual do produto: se você tiver o plano [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], sua organização deve comprar [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Para usar o [Aplicativo Fusion] com o [!DNL Workfront Fusion], é necessário ter uma conta FTP.

## Criar uma conexão em um módulo FTP {#create-a-connection}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Nome da Conexão]</td> 
   <td> <p> Insira o nome da conexão FTP.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Host] </td> 
   <td> <p>Insira o nome de host do servidor FTP. E.g. <code>myftp123.server.com</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Porta] </td> 
   <td> <p>Insira o número da porta do servidor FTP. E.g. <code>21</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome de Usuário] </td> 
   <td> <p>Digite o nome de usuário da sua conta FTP.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Senha] </td> 
   <td> <p>Digite a senha da sua conta FTP.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usar uma conexão segura (TLS)</p> </td> 
   <td> <p>Selecione se deseja usar uma conexão segura.</p> <p style="font-weight: bold;">[!UICONTROL Não]</p> <p>A conexão não é segura.</p> <p style="font-weight: bold;">[!UICONTROL Criptografia explícita ou criptografia implícita]</p> <p>A conexão é protegida por SSL.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Rejeitar certificados não autorizados]</p> </td> 
   <td> <p>Habilite essa opção para verificar o certificado do servidor FTP. Se a verificação falhar, a conexão não será criada. Para ser aprovado na verificação, o certificado deve atender a um dos seguintes critérios:</p> 
    <ul> 
     <li>ser assinado por uma <a href="https://en.wikipedia.org/wiki/Certificate_authority">Autoridade de certificação</a> raiz</li> 
     <li>ser assinado por uma Autoridade de Certificação Intermediária (consulte, por exemplo, <a href="https://knowledge.digicert.com/solution/SO16297.html">Como funcionam as cadeias de certificados</a> para obter mais explicações). Nesse caso, todos os certificados intermediários devem ser instalados no servidor FTP.</li> 
     <li>ser um Certificado Autoassinado fornecido no campo [!UICONTROL Self-signed certificate] (veja abaixo)</li> </ul>

Se essa opção estiver desativada, o certificado do servidor FTP não será verificado. Recomendamos não desativar a opção, pois ela torna a conexão insegura e representa um sério risco de segurança.</td>
</tr> 
  <tr> 
   <td> <p>[!UICONTROL Certificado autoassinado]</p> </td> 
   <td> <p>Clique no botão <b>[!UICONTROL Extract]</b> para abrir a caixa de diálogo de carregamento.</p> <p>Faça upload do certificado para usar o TLS com seu certificado autoassinado. [!DNL Workfront Fusion] não retém nem armazena dados que você fornece, como arquivos e senhas. O arquivo e a senha são usados somente para extrair o certificado.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Módulos FTP e seus campos

* [Triggers](#triggers)
* [Ações](#actions)

### Triggers

#### [!UICONTROL Observar arquivos]

[!UICONTROL Arquivos de observação] é o único módulo de acionador para FTP. Monitora o conteúdo do arquivo da pasta selecionada. O acionador é executado quando um novo arquivo é inserido na pasta especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como estabelecer uma conexão com a conta FTP, consulte <a href="#create-a-connection" class="MCXref xref">[!UICONTROL Criar uma conexão] em um módulo FTP</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Pasta]</p> </td> 
   <td> <p>Selecione a pasta que deseja observar.</p> <p><b>Observação:</b> somente uma pasta por cenário é permitida. Subpastas são ignoradas.</p> <p><b>Dica:</b> para acompanhar várias pastas, crie um cenário independente para cada uma delas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de arquivos retornados] </td> 
   <td> <p>Defina o número máximo de resultados com os quais [!DNL Workfront Fusion] trabalhará durante um ciclo. Se o valor for definido como muito alto, a conexão pode ser interrompida no lado do serviço de terceiros especificado (tempo limite). [!DNL Workfront Fusion] não tem nenhuma influência sobre isso. Recomendamos que você defina um valor mais baixo e defina um valor mais alto para o número máximo de ciclos ou execute o cenário com mais frequência.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [[!UICONTROL Alterar permissões]](#change-permissions)
* [[!UICONTROL Criar uma pasta]](#create-a-folder)
* [[!UICONTROL Excluir um arquivo]](#delete-a-file)
* [[!UICONTROL Excluir uma pasta]](#delete-a-folder)
* [[!UICONTROL Obter um arquivo]](#get-a-file)
* [[!UICONTROL Lista de arquivos em uma pasta]](#list-of-files-in-a-folder)
* [[!UICONTROL Mover um arquivo ou uma pasta]](#move-a-file-or-folder)
* [[!UICONTROL Carregar] um arquivo](#upload-a-file)

#### [!UICONTROL Alterar permissões]

Este módulo de ação altera as configurações de permissão de um arquivo ou pasta.

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL Conexão]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Para obter instruções sobre como estabelecer uma conexão com a conta FTP, consulte <a href="#Create" class="MCXref xref" >[!UICONTROL Criar uma conexão] em um módulo FTP</a> neste artigo.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">[!UICONTROL Alterar configurações de permissão de]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">
               <p>Selecione se deseja alterar as configurações de um arquivo ou pasta.</p>
            </td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL Caminho do arquivo]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Insira ou mapeie o caminho do arquivo para a pasta ou o arquivo.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Permissões]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
               <p>Defina as permissões desejadas para arquivos ou pastas. Use os parâmetros chmod. Por exemplo: <code>777 </code>ou <code>-rwxrwxrwx</code>.</p>
               <p>As permissões devem corresponder ao padrão <code> /(.?([r-][w-][x-]){3})|[0-7]{3,4}/</code>.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL Criar uma pasta]

Este módulo de ação cria uma nova pasta.

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL Conexão]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Para obter instruções sobre como estabelecer uma conexão com a conta FTP, consulte <a href="#Create" class="MCXref xref" >[!UICONTROL Criar uma conexão] em um módulo FTP</a> neste artigo.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">[!UICONTROL Caminho da pasta]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Insira ou mapeie o caminho do arquivo para a nova pasta.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[!UICONTROL Novo nome de pasta]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">
               <p>Insira ou mapeie um nome para a nova pasta.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL Excluir um arquivo]

Exclui um arquivo da pasta especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Para obter instruções sobre como estabelecer uma conexão com a conta FTP, consulte <a href="#Create" class="MCXref xref" >[!UICONTROL Criar uma conexão] em um módulo FTP</a> neste artigo.</td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione a pasta FTP da qual deseja excluir um arquivo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome do arquivo]</td> 
   <td> <p> Insira o nome do arquivo, incluindo a extensão do nome do arquivo. Exemplo: <code>[!DNL image].png</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir uma pasta]

Este módulo de ação exclui permanentemente a pasta especificada.

<table style="width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
   <col style="width: 301px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <tbody>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">[!UICONTROL Conexão]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Para obter instruções sobre como estabelecer uma conexão com a conta FTP, consulte <a href="#Create" class="MCXref xref" >[!UICONTROL Criar uma conexão] em um módulo FTP</a> neste artigo.</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">[!UICONTROL Pasta]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">
               <p>Selecione a pasta FTP da qual deseja excluir um arquivo.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL Obter um arquivo]

Recupera um arquivo do servidor FTP que pode ser processado, por exemplo, carregado para o [!DNL Dropbox].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como estabelecer uma conexão com a conta FTP, consulte <a href="#creating-the-ftp-connection" class="MCXref xref">Criando a conexão FTP</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Caminho do arquivo]</td> 
   <td> <p> Insira o caminho do arquivo que deseja obter.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lista de arquivos em uma pasta]

Recupera informações de arquivos e/ou pastas.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como estabelecer uma conexão com a conta FTP, consulte <a href="#creating-the-ftp-connection" class="MCXref xref">Criando a conexão FTP</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione a pasta FTP na qual deseja pesquisar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mostrar] </td> 
   <td> <p>Selecione se deseja recuperar informações sobre arquivos ou pastas, ou ambos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pesquisar] </td> 
   <td> <p>Insira o termo de pesquisa. Se nenhum termo de pesquisa for inserido, todos os arquivos e pastas da pasta especificada serão recuperados.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de arquivos retornados]</td> 
   <td> <p> Defina o número máximo de arquivos recuperados por esse módulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover um arquivo ou uma pasta]

Este módulo de ação move um arquivo ou pasta para um local diferente.

<table style="width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
   <col style="width: 301px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <tbody>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">[!UICONTROL Conexão]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Para obter instruções sobre como estabelecer uma conexão com a conta FTP, consulte <a href="#Create" class="MCXref xref" >[!UICONTROL Criar uma conexão] em um módulo FTP</a> neste artigo.</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">[!UICONTROL Caminho de arquivo antigo]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">
               <p>Insira o caminho do qual deseja mover o arquivo. Exemplo: <code>/folder1/document.txt</code>.</p>
            </td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="font-weight: bold;">[!UICONTROL Novo caminho de arquivo]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">
               <p>Insira o caminho para o qual deseja mover o arquivo. Exemplo: <code>/folder2/document.txt</code>.</p>
            </td>
         </tr>
   </tbody>
</table>


#### [!UICONTROL Carregar um arquivo]

Faz upload de um arquivo para o servidor FTP.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td>Para obter instruções sobre como estabelecer uma conexão com a conta FTP, consulte <a href="#creating-the-ftp-connection" class="MCXref xref">Criando a conexão FTP</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione a pasta FTP na qual deseja fazer upload do arquivo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL arquivo Source] </td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Anexar a um arquivo já existente]</td> 
   <td> <p>Se essa opção estiver ativada e o arquivo já existir no servidor FTP, o conteúdo do arquivo será anexado ao arquivo existente. Se essa opção não estiver habilitada, o conteúdo do arquivo será substituído.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Criar pastas se não existir] </td> 
   <td> <p>Se essa opção estiver ativada e a pasta inserida no campo Pasta não existir no servidor FTP, o módulo criará a pasta</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solução de problemas {#troubleshooting}

Se tiver problemas com o aplicativo FTP durante a criação da conexão ou durante a operação de um módulo, tente usar um dos clientes FTP populares e tente executar a mesma ação (por exemplo, criar uma conexão ou listar arquivos em uma pasta). com o cliente FTP. Se você estiver tendo os mesmos problemas com o cliente FTP, o motivo pode ser uma configuração incorreta do servidor FTP.
