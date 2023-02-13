---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Email do Microsoft Office 365
description: Em um [!DNL Adobe Workfront Fusion] você pode automatizar workflows que usam o Microsoft Office 365 Email, bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: 29b69e8c-a889-441e-a052-287f1db2052d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1838'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Email]

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!UICONTROL Email do Microsoft Office 365], bem como conectá-lo a vários aplicativos e serviços de terceiros.

Para usar [!UICONTROL Email do Office 365] com [!DNL Adobe Workfront Fusion], é necessário ter um [!UICONTROL Conta do Office 365]. Você pode criar um em www.office.com.

Para obter instruções sobre como conectar seu [!UICONTROL Office 365] para [!DNL Workfront Fusion], consulte [Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

Após conceder o consentimento, você será redirecionado para a função [!UICONTROL Workfront Fusion] página de administração, onde você pode continuar criando seu cenário.

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

Para usar [!DNL Microsoft Office 365 Email] módulos, você deve ter um [!DNL Microsoft Office 365 Email] conta.

## [!DNL Microsoft Office 365 Email] módulos e seus campos

Ao configurar [!DNL Microsoft Office 365 Email] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Microsoft Office 365 Email] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Mensagem](#message)
* [Mensagem de rascunho](#draft-message)
* [Anexo](#attachment)
* [Outro](#other)

### Mensagem

* [[!UICONTROL Assista às mensagens]](#watch-messages)
* [[!UICONTROL Pesquisar mensagens]](#search-messages)
* [[!UICONTROL Obter uma mensagem]](#get-a-message)
* [[!UICONTROL Criar e enviar uma mensagem]](#create-and-send-a-message)
* [[!UICONTROL Mover uma mensagem]](#move-a-message)
* [[!UICONTROL Excluir uma mensagem]](#delete-a-message)

#### [!UICONTROL Assista às mensagens]

Acionadores quando uma nova mensagem de email é enviada ou recebida.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Mensagens de observação]</p> </td> 
   <td> <p>Selecione as mensagens que deseja assistir:</p> 
    <ul> 
     <li>[!UICONTROL Somente Não Lido]</li> 
     <li>[!UICONTROL Somente leitura]</li> 
     <li>[!UICONTROL Tudo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta de email]</td> 
   <td> <p>Selecione a pasta que contém as mensagens que deseja visualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search]</td> 
   <td>Insira sua consulta de pesquisa. Para obter informações sobre como gravar uma consulta de pesquisa, consulte o [!DNL Microsoft] artigo de suporte <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">Pesquisar email e pessoas em [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite] </td> 
   <td> <p>Insira o número máximo de mensagens [!DNL Workfront Fusion] deve retornar durante um ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Pesquisar mensagens]

Pesquisa mensagens com base em critérios específicos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta de email]</td> 
   <td> <p>Selecione a pasta que contém as mensagens que deseja pesquisar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search]</td> 
   <td>Insira sua consulta de pesquisa. Para obter informações sobre como gravar uma consulta de pesquisa, consulte o [!DNL Microsoft] artigo de suporte <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">Pesquisar email e pessoas em [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pedido por]</td> 
   <td> <p>Selecione como deseja ordenar os resultados:</p> 
    <ul> 
     <li>[!UICONTROL Assunto (crescente ou decrescente)]</li> 
     <li>[!UICONTROL Hora da data de criação (crescente ou decrescente)]</li> 
     <li>[!UICONTROL Hora da última modificação (crescente ou decrescente)]</li> 
     <li>[!UICONTROL Hora da data de recebimento (crescente ou decrescente)]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira o número máximo de mensagens [!DNL Workfront Fusion] deve retornar durante um ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter uma mensagem]

Obtém os metadados de uma mensagem específica

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da mensagem]</td> 
   <td> <p> Selecione ou mapeie a ID da mensagem para a qual deseja recuperar metadados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obter conteúdo MIME]</td> 
   <td>Ative essa opção para recuperar dados sobre o conteúdo MIME da mensagem. O conteúdo da [!UICONTROL MIME] pode incluir imagens, áudio, vídeo ou outros tipos de arquivos.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar e enviar uma mensagem]

Cria e envia uma mensagem de email.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assunto]</td> 
   <td> <p>Insira ou mapeie a linha de assunto da mensagem.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Tipo de conteúdo do corpo]</td> 
   <td>Selecione se o conteúdo do corpo da mensagem é HTML ou Text.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo de conteúdo]</td> 
   <td> <p>Insira ou mapeie o texto do corpo da mensagem do email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importância]</td> 
   <td> <p>Selecione a importância do email</p> 
    <ul> 
     <li>[!UICONTROL Baixo]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Alta]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Para Recipients]</p> </td> 
   <td> <p>Adicione o endereço de email para o qual deseja enviar as mensagens:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Insira o nome do contato</p> </li> 
     <li> <p><strong>[!UICONTROL Endereço de email]</strong> </p> <p>Insira o endereço de email do contato.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Adicione os recipients que você deseja receber uma cópia da mensagem:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Insira o nome do contato</p> </li> 
     <li> <p><strong>[!UICONTROL Endereço de email]</strong> </p> <p>Insira o endereço de email do contato.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Recipients Bcc]</p> </td> 
   <td> <p>Adicione os recipients que deseja copiar na mensagem, sem permitir que outros recipients vejam seus nomes ou endereços de email:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Insira o nome do contato</p> </li> 
     <li> <p><strong>[!UICONTROL Endereço de email]</strong> </p> <p>Insira o endereço de email do contato.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Anexos]</p> </td> 
   <td> <p>Adicione os anexos ao email:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome do arquivo]</strong> </p> <p>Insira o nome do arquivo. Exemplo: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Dados]</strong> </p> <p>Insira os dados do arquivo no campo ou mapeie a fonte do arquivo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos de mensagens da Internet]</td> 
   <td> <p>Adicione os cabeçalhos de mensagem para o email.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Insira o nome do cabeçalho</p> </li> 
     <li> <p><strong>[!UICONTROL Endereço de email]</strong> </p> <p>Insira um valor para o cabeçalho.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover uma mensagem]

Move uma mensagem de email para uma pasta selecionada na caixa de correio.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da mensagem]</td> 
   <td> <p> Selecione ou mapeie a ID da mensagem que deseja mover para uma pasta diferente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta de email] </td> 
   <td> <p>Selecione ou mapeie a ID da pasta onde deseja mover a mensagem.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir uma mensagem]

Exclui uma mensagem de email existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da mensagem]</td> 
   <td> <p> Selecione ou mapeie a ID da mensagem que deseja excluir.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Mensagem de rascunho

* [Criar uma mensagem de rascunho](#create-a-draft-message)
* [Enviar uma mensagem de rascunho](#send-a-draft-message)
* [Atualizar uma mensagem](#update-a-message)

#### [!UICONTROL Criar uma mensagem de rascunho]

Cria uma nova mensagem de email.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assunto]</td> 
   <td> <p>Insira a linha de assunto da mensagem.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de conteúdo do corpo]</td> 
   <td>Selecione se o conteúdo do corpo da mensagem é HTML ou Text.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo de conteúdo]</td> 
   <td> <p>Insira o texto do corpo da mensagem do email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importância]</td> 
   <td> <p>Selecione a importância do email</p> 
    <ul> 
     <li>[!UICONTROL Baixo]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Alta]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Para Recipients]</p> </td> 
   <td> <p>Adicione os recipients aos quais deseja enviar as mensagens:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Insira o nome do contato</p> </li> 
     <li> <p><strong>[!UICONTROL Endereço de email]</strong> </p> <p>Insira o endereço de email do contato.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Adicione os destinatários A você deseja receber uma cópia da mensagem:</p> 
    <ul> 
     <li> <p><strong>Nome</strong> </p> <p>Insira o nome do contato</p> </li> 
     <li> <p><strong>Endereço de email</strong> </p> <p>Insira o endereço de email do contato.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Recipients Bcc</p> </td> 
   <td> <p>Adicione os recipients que deseja copiar na mensagem, sem permitir que outros recipients vejam seus nomes ou endereços de email:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Insira o nome do contato</p> </li> 
     <li> <p><strong>[!UICONTROL Endereço de email]</strong> </p> <p>Insira o endereço de email do contato.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Anexos]</p> </td> 
   <td> <p>Adicione os anexos ao email:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome do arquivo]</strong> </p> <p>Insira o nome do arquivo. Exemplo: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Dados]</strong> </p> <p>Insira os dados do arquivo no campo ou mapeie a fonte do arquivo.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Enviar uma mensagem de rascunho]

Envia uma mensagem de email que está atualmente em rascunho.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da mensagem de rascunho]</td> 
   <td> <p> Selecione ou mapeie a ID da mensagem do rascunho que deseja enviar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar uma mensagem]

Atualiza uma mensagem existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir uma ID de mensagem]</td> 
   <td> <p>Selecione como deseja identificar a mensagem a ser atualizada:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a ID da mensagem.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione a pasta que contém a mensagem que deseja atualizar e selecione a mensagem</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assunto]</td> 
   <td> <p>Insira a linha de assunto da mensagem.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo de conteúdo]</td> 
   <td> <p>Insira o texto do corpo da mensagem do email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importância]</td> 
   <td> <p>Selecione a importância do email</p> 
    <ul> 
     <li>[!UICONTROL Baixo]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Alta]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Para Recipients]</p> </td> 
   <td> <p>Adicione o endereço de email para o qual deseja enviar as mensagens:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Insira o nome do contato</p> </li> 
     <li> <p><strong>[!UICONTROL Endereço de email]</strong> </p> <p>Insira o endereço de email do contato.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Adicione os destinatários A você deseja receber uma cópia da mensagem:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Insira o nome do contato</p> </li> 
     <li> <p><strong>[!UICONTROL Endereço de email]</strong> </p> <p>Insira o endereço de email do contato.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Recipients Bcc]</p> </td> 
   <td> <p>Adicione os recipients que deseja copiar na mensagem, sem permitir que outros recipients vejam seus nomes ou endereços de email:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Insira o nome do contato</p> </li> 
     <li> <p><strong>[!UICONTROL Endereço de email]</strong> </p> <p>Insira o endereço de email do contato.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Anexos]</p> </td> 
   <td> <p>Adicione os anexos ao email:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome do arquivo]</strong> </p> <p>Insira o nome do arquivo. Exemplo: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Dados]</strong> </p> <p>Insira os dados do arquivo no campo ou mapeie a fonte do arquivo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Marcar como Lido]</td> 
   <td>Habilite esta opção para marcar a mensagem atualizada como lida.</td> 
  </tr> 
 </tbody> 
</table>

### Anexo

* [[!UICONTROL Listar anexos]](#list-attachments)
* [[!UICONTROL Baixar um anexo]](#download-an-attachment)

#### [!UICONTROL Listar anexos]

Esse módulo recupera uma lista de anexos pertencentes à mensagem especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da mensagem]</td> 
   <td> <p> Selecione ou mapeie a ID da mensagem da qual deseja recuperar anexos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de anexos que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Baixar um anexo]

Este módulo baixa o anexo especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da mensagem]</td> 
   <td> <p> Selecione ou mapeie a ID da mensagem que contém o anexo que deseja baixar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do anexo]</td> 
   <td> <p>Insira ou mapeie a ID do anexo que deseja baixar.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Outro

* [[!UICONTROL Faça uma chamada de API]](#make-an-api-call)
* [[!UICONTROL Adicionar um anexo]](#add-an-attachment)

#### [!UICONTROL Faça uma chamada de API]

Esse módulo permite executar uma chamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Insira um caminho relativo a <code>https://graph.microsoft.com</code>. Exemplo:<code> /v1.0/me/messages</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   td&gt; <p>Selecione o método de solicitação HTTP que você precisa configurar a chamada da API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão. Por exemplo, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] adiciona os cabeçalhos de autorização para você.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sequência de consulta]</td> 
   <td> <p> Adicione a query para a chamada de API no formato de um objeto JSON padrão.</p> </td> 
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

#### [!UICONTROL Adicionar um anexo]

Esse módulo adiciona um anexo grande a uma mensagem.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da mensagem]</td> 
   <td> <p> Selecione ou mapeie a ID da mensagem à qual deseja adicionar um anexo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td> <p>Selecione um arquivo de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> </td> 
  </tr> 
 </tbody> 
</table>
