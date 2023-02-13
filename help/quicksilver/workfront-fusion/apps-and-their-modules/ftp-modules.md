---
filename: ftp-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos FTP
description: Os módulos FTP permitem monitorar as alterações de arquivo em uma pasta selecionada, fazer upload de novos arquivos para a pasta desejada e modificar ou excluir arquivos existentes que já estão em uma pasta.
author: Becky
exl-id: 360825a4-4580-4039-894e-583e82132ed6
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1295'
ht-degree: 0%

---

# Módulos FTP

Os módulos FTP permitem monitorar as alterações de arquivo em uma pasta selecionada, fazer upload de novos arquivos para a pasta desejada e modificar ou excluir arquivos existentes que já estão em uma pasta.

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

Para usar [Aplicativo Fusion] com [!DNL Workfront Fusion], você deve ter uma conta FTP.

## Criar uma conexão em um módulo FTP {#create-a-connection}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Nome da conexão]</td> 
   <td> <p> Insira o nome da conexão FTP.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Host] </td> 
   <td> <p>Insira o nome do host do servidor FTP. E.g. <code>myftp123.server.com</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Port] </td> 
   <td> <p>Insira o número da porta do servidor FTP. E.g. <code>21</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome do usuário] </td> 
   <td> <p>Insira o nome de usuário da conta FTP.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Senha] </td> 
   <td> <p>Insira a senha da conta FTP.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usar uma conexão segura (TLS)</p> </td> 
   <td> <p>Selecione se deseja usar uma conexão segura.</p> <p style="font-weight: bold;">[!UICONTROL n.o]</p> <p>A conexão não está segura.</p> <p style="font-weight: bold;">[!UICONTROL Criptografia explícita ou criptografia implícita]</p> <p>A conexão é segura usando SSL.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Rejeitar certificados não autorizados]</p> </td> 
   <td> <p>Ative essa opção para verificar o certificado do servidor FTP. Se a verificação falhar, a conexão não será criada. Para ser aprovado na verificação, o certificado deve satisfazer um dos seguintes critérios:</p> 
    <ul> 
     <li>ser assinado por uma raiz <a href="https://en.wikipedia.org/wiki/Certificate_authority">Autoridade de certificação</a></li> 
     <li>ser assinado por uma autoridade de certificação intermediária (consulte, por exemplo, <a href="https://knowledge.digicert.com/solution/SO16297.html">Como as cadeias de certificados funcionam</a> para mais explicações). Nesse caso, todos os Certificados intermediários devem ser instalados no servidor FTP.</li> 
     <li>ser um certificado autoassinado fornecido no campo [!UICONTROL Certificado autoassinado] (veja abaixo)</li> </ul>

Se essa opção estiver desativada, o certificado do servidor FTP não será verificado. Aconselhamos veementemente contra a desativação da opção, pois ela torna a conexão insegura e apresenta um sério risco para a segurança.</td>
</tr> 
  <tr> 
   <td> <p>[!UICONTROL Certificado autoassinado]</p> </td> 
   <td> <p>Clique no botão <b>[!UICONTROL Extract]</b> para abrir a caixa de diálogo de upload.</p> <p>Faça upload do certificado para usar o TLS com seu certificado autoassinado. [!DNL Workfront Fusion] não retém ou armazena dados fornecidos, como arquivos e senhas. Arquivo e senha são usados apenas para extrair o certificado.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Módulos FTP e seus campos

* [Triggers](#triggers)
* [Ações](#actions)

### Triggers

#### [!UICONTROL Assistir arquivos]

[!UICONTROL Assistir arquivos] é o único módulo de acionador para FTP. Ele monitora o conteúdo do arquivo da pasta selecionada. O acionador é executado quando um novo arquivo é inserido na pasta especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como estabelecer uma conexão com a conta FTP, consulte <a href="#create-a-connection" class="MCXref xref">[!UICONTROL Criar uma conexão] em um módulo FTP</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Pasta]</p> </td> 
   <td> <p>Selecione a pasta que deseja visualizar.</p> <p><b>Observação:</b> Somente uma pasta por cenário é permitida. As subpastas são ignoradas.</p> <p><b>Dica:</b> Para rastrear várias pastas, crie um cenário independente para cada uma delas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de arquivos retornados] </td> 
   <td> <p>Defina o número máximo de resultados que [!DNL Workfront Fusion] funcionará durante um ciclo. Se o valor estiver definido como muito alto, a conexão pode ser interrompida no lado do serviço de terceiros fornecido (tempo limite). [!DNL Workfront Fusion] não tem influência sobre isso. Recomendamos que você defina um valor menor e defina um valor maior para o número máximo de ciclos ou execute o cenário com mais frequência.</p> </td> 
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
* [[!UICONTROL Mover um arquivo ou pasta]](#move-a-file-or-folder)
* [[!UICONTROL Upload] um arquivo](#upload-a-file)

#### [!UICONTROL Alterar permissões]

Este módulo de ação altera as configurações de permissão de um arquivo ou pasta.

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL Connection]</td>
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
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Insira ou mapeie o caminho do arquivo para a pasta ou arquivo.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Permissões]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
               <p>Defina as permissões de arquivo ou pasta desejadas. Use os parâmetros de chmod. Por exemplo: <code>777 </code>ou <code>-rwxrwxrwx</code>.</p>
               <p>As permissões devem corresponder ao padrão <code> /(.?([r-][w-][x-]){3})|[0-7]{3,4}/</code>.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL Criar uma pasta]

Esse módulo de ação cria uma nova pasta.

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Para obter instruções sobre como estabelecer uma conexão com a conta FTP, consulte <a href="#Create" class="MCXref xref" >[!UICONTROL Criar uma conexão] em um módulo FTP</a> neste artigo.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">[!UICONTROL Caminho da pasta]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Insira ou mapeie o caminho do arquivo para a nova pasta.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[!UICONTROL Novo nome da pasta]</td>
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
   <td>[!UICONTROL Connection] </td> 
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
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">[!UICONTROL Connection]</td>
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

Recupera um arquivo do servidor FTP que pode ser processado posteriormente, por exemplo, carregado para a [!DNL Dropbox].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como estabelecer uma conexão com a conta FTP, consulte <a href="#creating-the-ftp-connection" class="MCXref xref">Criação da conexão FTP</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Caminho do arquivo]</td> 
   <td> <p> Insira o caminho do arquivo que deseja obter.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lista de arquivos em uma pasta]

Recupera informações do arquivo e/ou da pasta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como estabelecer uma conexão com a conta FTP, consulte <a href="#creating-the-ftp-connection" class="MCXref xref">Criação da conexão FTP</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione a pasta FTP na qual deseja pesquisar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show] </td> 
   <td> <p>Selecione se deseja recuperar informações sobre arquivos ou pastas, ou ambos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>Insira o termo de pesquisa. Se nenhum termo de pesquisa for inserido, todos os arquivos e pastas da pasta especificada serão recuperados.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de arquivos retornados]</td> 
   <td> <p> Defina o número máximo de arquivos recuperados por este módulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover um arquivo ou pasta]

Esse módulo de ação move um arquivo ou pasta para um local diferente.

<table style="width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
   <col style="width: 301px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <tbody>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Para obter instruções sobre como estabelecer uma conexão com a conta FTP, consulte <a href="#Create" class="MCXref xref" >[!UICONTROL Criar uma conexão] em um módulo FTP</a> neste artigo.</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">[!UICONTROL Caminho do arquivo antigo]</td>
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

Carrega um arquivo no servidor FTP.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Para obter instruções sobre como estabelecer uma conexão com a conta FTP, consulte <a href="#creating-the-ftp-connection" class="MCXref xref">Criação da conexão FTP</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione a pasta FTP para a qual deseja fazer upload do arquivo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arquivo de origem] </td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Anexar a um arquivo já existente]</td> 
   <td> <p>Se essa opção estiver habilitada e o arquivo já existir no servidor FTP, o conteúdo do arquivo será anexado ao arquivo existente. Se essa opção não estiver ativada, o conteúdo do arquivo será substituído.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Criar pastas se não existirem] </td> 
   <td> <p>Se essa opção estiver ativada e a pasta inserida no campo Pasta não existir no servidor FTP, o módulo criará a pasta</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solução de problemas {#troubleshooting}

Se estiver tendo problemas com o aplicativo FTP durante a criação da conexão ou durante a operação de um módulo, tente usar um dos clientes FTP populares e tente executar a mesma ação (por exemplo, crie uma conexão ou liste arquivos em uma pasta). com o cliente FTP. Se você estiver enfrentando os mesmos problemas também com o cliente FTP, o motivo pode ser uma configuração incorreta do servidor FTP.
