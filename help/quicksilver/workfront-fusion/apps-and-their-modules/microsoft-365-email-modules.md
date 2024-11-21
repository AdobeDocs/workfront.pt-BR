---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Email do Microsoft Office 365
description: Em um cenário  [!DNL Adobe Workfront Fusion] , você pode automatizar fluxos de trabalho que usam Email do Microsoft Office 365, bem como conectá-los a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: 29b69e8c-a889-441e-a052-287f1db2052d
source-git-commit: 2e91e9a4c691430f3c98e3cbddb30706ea57f84a
workflow-type: tm+mt
source-wordcount: '2723'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Email] módulos

Em um cenário [!DNL Adobe Workfront Fusion], você pode automatizar fluxos de trabalho que usam o [!UICONTROL Email do Microsoft Office 365], bem como conectá-lo a vários aplicativos e serviços de terceiros.

Para usar o [!UICONTROL Email do Office 365] com [!DNL Adobe Workfront Fusion], é necessário ter uma [!UICONTROL conta do Office 365]. Crie um em www.office.com.

Para obter instruções sobre como conectar sua conta do [!UICONTROL Office 365] ao [!DNL Workfront Fusion], consulte [Criar uma conexão ao [!DNL Adobe Workfront Fusion] - Instruções básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

Após consentir, você será redirecionado de volta para a página de administração do [!UICONTROL Workfront Fusion], na qual poderá continuar criando seu cenário.

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
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Para usar módulos [!DNL Microsoft Office 365 Email], você deve ter uma conta [!DNL Microsoft Office 365 Email].

## Informações da API de email do Microsoft Office 365

O conector de email do Microsoft Office 365 usa o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL base</td> 
   <td> https://graph.microsoft.com/v1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Versão da API</td> 
   <td> v1.0 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tag da API</td> 
   <td>v2.6.5</td> 
  </tr>
 </tbody> 
 </table>



## Conectando o serviço [!DNL Office 365 Email] a [!DNL Workfront Fusion]

Para obter instruções sobre como conectar sua conta do [!DNL Office 365 Email] ao [!UICONTROL Workfront Fusion], consulte [Criar uma conexão com o [!UICONTROL Adobe Workfront Fusion] - Instruções básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Alguns aplicativos do Microsoft usam a mesma conexão, que está vinculada a permissões de usuário individuais. Portanto, ao criar uma conexão, a tela de consentimento de permissões exibe todas as permissões que foram concedidas anteriormente à conexão deste usuário, além de todas as novas permissões necessárias para o aplicativo atual.
>
>Por exemplo, se um usuário tiver permissões de &quot;Tabela de leitura&quot; concedidas por meio do conector do Excel e criar uma conexão no conector do Outlook para ler emails, a tela de consentimento de permissões mostrará a permissão &quot;Tabela de leitura&quot; já concedida e a permissão &quot;Gravar email&quot; recém-necessária.

## [!DNL Microsoft Office 365 Email] módulos e seus campos

Ao configurar módulos do [!DNL Microsoft Office 365 Email], o [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos [!DNL Microsoft Office 365 Email] adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Mensagem](#message)
* [Mensagem de rascunho](#draft-message)
* [Anexo](#attachment)
* [Outro](#other)

### Mensagem

* [[!UICONTROL Criar e Enviar uma Mensagem (herdada)]](#create-and-send-a-message)
* [[!UICONTROL Excluir uma Mensagem]](#delete-a-message)
* [[!UICONTROL Obter uma mensagem]](#get-a-message)
* [[!UICONTROL Mover uma Mensagem]](#move-a-message)
* [[!UICONTROL Pesquisar mensagens]](#search-messages)
* [[!UICONTROL Assistir Mensagens]](#watch-messages)



#### [!UICONTROL Criar e Enviar uma Mensagem (herdada)]

Cria e envia uma mensagem de email.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assunto]</td> 
   <td> <p>Insira ou mapeie a linha de assunto da mensagem.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Tipo de Conteúdo do Corpo]</td> 
   <td>Selecione se o conteúdo do corpo da mensagem é HTML ou Text.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conteúdo do corpo]</td> 
   <td> <p>Insira ou mapeie o texto do corpo da mensagem do email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importância]</td> 
   <td> <p>Selecionar a importância do email</p> 
    <ul> 
     <li>[!UICONTROL Baixo]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Alto]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Para Destinatários]</p> </td> 
   <td> <p>Adicione o endereço de email para o qual deseja enviar as mensagens:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Insira o nome do contato</p> </li> 
     <li> <p><strong>[!UICONTROL Endereço de Email]</strong> </p> <p>Insira o endereço de email do contato.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Adicione os destinatários que você deseja receber uma cópia da mensagem:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Insira o nome do contato</p> </li> 
     <li> <p><strong>[!UICONTROL Endereço de Email]</strong> </p> <p>Insira o endereço de email do contato.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Destinatários Cco]</p> </td> 
   <td> <p>Adicione os recipients que deseja copiar na mensagem, sem permitir que outros recipients vejam seus nomes ou endereços de email:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Insira o nome do contato</p> </li> 
     <li> <p><strong>[!UICONTROL Endereço de Email]</strong> </p> <p>Insira o endereço de email do contato.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Anexos]</p> </td> 
   <td> <p>Adicionar os anexos ao email:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome do Arquivo]</strong> </p> <p>Insira o nome do arquivo. Exemplo: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Dados]</strong> </p> <p>Insira os dados do arquivo no campo ou mapeie a origem do arquivo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos de Mensagens da Internet]</td> 
   <td> <p>Adicione os cabeçalhos de mensagem para o email.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Insira o nome do cabeçalho</p> </li> 
     <li> <p><strong>[!UICONTROL Endereço de Email]</strong> </p> <p>Insira um valor para o cabeçalho.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar e Enviar uma Mensagem]

Cria e envia uma mensagem de email.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assunto]</td> 
   <td> <p>Insira ou mapeie a linha de assunto da mensagem.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Tipo de Conteúdo do Corpo]</td> 
   <td>Selecione se o conteúdo do corpo da mensagem é HTML ou Text.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conteúdo do corpo]</td> 
   <td> <p>Insira ou mapeie o texto do corpo da mensagem do email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importância]</td> 
   <td> <p>Selecionar a importância do email</p> 
    <ul> 
     <li>[!UICONTROL Baixo]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Alto]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Para Destinatários]</p> </td> 
   <td> <p>Adicione o endereço de email para o qual deseja enviar as mensagens:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Insira o nome do contato</p> </li> 
     <li> <p><strong>[!UICONTROL Endereço de Email]</strong> </p> <p>Insira o endereço de email do contato.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Adicione os destinatários que você deseja receber uma cópia da mensagem:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Insira o nome do contato</p> </li> 
     <li> <p><strong>[!UICONTROL Endereço de Email]</strong> </p> <p>Insira o endereço de email do contato.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Destinatários Cco]</p> </td> 
   <td> <p>Adicione os recipients que deseja copiar na mensagem, sem permitir que outros recipients vejam seus nomes ou endereços de email:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Insira o nome do contato</p> </li> 
     <li> <p><strong>[!UICONTROL Endereço de Email]</strong> </p> <p>Insira o endereço de email do contato.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Anexos]</p> </td> 
   <td> <p>Adicionar os anexos ao email:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome do Arquivo]</strong> </p> <p>Insira o nome do arquivo. Exemplo: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Dados]</strong> </p> <p>Insira os dados do arquivo no campo ou mapeie a origem do arquivo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos de Mensagens da Internet]</td> 
   <td> <p>Adicione os cabeçalhos de mensagem para o email.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Insira o nome do cabeçalho</p> </li> 
     <li> <p><strong>[!UICONTROL Endereço de Email]</strong> </p> <p>Insira um valor para o cabeçalho.</p> </li> 
    </ul> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL Do endereço de email]</td> 
   <td> <p> Para usar um endereço de email compartilhado, insira o endereço aqui. O usuário cujas credenciais são usadas na conexão usada para este módulo deve ter acesso à pasta compartilhada.<p>Deixe este campo em branco para usar o endereço de email do proprietário da conexão.</p></p> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir uma Mensagem]

Exclui uma mensagem de email existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Do endereço de email]</td> 
   <td> <p> Para usar um endereço de email compartilhado, insira o endereço aqui. O usuário cujas credenciais são usadas na conexão usada para este módulo deve ter acesso à pasta compartilhada.<p>Deixe este campo em branco para usar o endereço de email do proprietário da conexão.</p></p> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL ID da Mensagem]</td> 
   <td> <p> Selecione ou mapeie a ID da mensagem que deseja excluir.</p> </td> 
  </tr> 
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
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Do endereço de email]</td> 
   <td> <p> Para usar um endereço de email compartilhado, insira o endereço aqui. O usuário cujas credenciais são usadas na conexão usada para este módulo deve ter acesso à pasta compartilhada.<p>Deixe este campo em branco para usar o endereço de email do proprietário da conexão.</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Mensagem]</td> 
   <td> <p> Selecione ou mapeie a ID da mensagem para a qual deseja recuperar metadados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obter conteúdo MIME]</td> 
   <td>Habilite esta opção para recuperar dados sobre o conteúdo MIME da mensagem. O conteúdo [!UICONTROL MIME] pode incluir imagens, áudio, vídeo ou outros tipos de arquivos.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover uma Mensagem]

Move uma mensagem de email para uma pasta selecionada na caixa de correio.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Mensagem]</td> 
   <td> <p> Selecione ou mapeie a ID da mensagem que deseja mover para uma pasta diferente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta de Email] </td> 
   <td> <p>Selecione ou mapeie a ID da pasta para onde deseja mover a mensagem.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Pesquisar mensagens]

Procura mensagens com base em critérios específicos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL Do endereço de email]</td> 
   <td> <p> Para usar um endereço de email compartilhado, insira o endereço aqui. O usuário cujas credenciais são usadas na conexão usada para este módulo deve ter acesso à pasta compartilhada.<p>Deixe este campo em branco para usar o endereço de email do proprietário da conexão.</p></p> </td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Pasta de Email]</td> 
   <td> <p>Selecione a pasta que contém as mensagens que você deseja pesquisar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pesquisar]</td> 
   <td>Insira sua consulta de pesquisa. Para obter informações sobre como gravar uma consulta de pesquisa, consulte o artigo de suporte do [!DNL Microsoft] <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">Pesquisar Emails e Pessoas no [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordenar por]</td> 
   <td> <p>Selecione como deseja ordenar os resultados:</p> 
    <ul> 
     <li>[!UICONTROL Assunto (Crescente ou Decrescente)]</li> 
     <li>[!UICONTROL Data Hora de Criação (Crescente ou Decrescente)]</li> 
     <li>[!UICONTROL Data e hora da última modificação (crescente ou decrescente)]</li> 
     <li>[!UICONTROL Data Hora de Recebimento (Crescente ou Decrescente)]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira o número máximo de mensagens que [!DNL Workfront Fusion] deve retornar durante um ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Assistir Mensagens]

Acionado quando uma nova mensagem de email é enviada ou recebida.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Observar Mensagens]</p> </td> 
   <td> <p>Selecione as mensagens que deseja assistir:</p> 
    <ul> 
     <li>[!UICONTROL Somente Não Lido]</li> 
     <li>[!UICONTROL Somente leitura]</li> 
     <li>[!UICONTROL Tudo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta de Email]</td> 
   <td> <p>Selecione a pasta que contém as mensagens que você deseja observar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pesquisar]</td> 
   <td>Insira sua consulta de pesquisa. Para obter informações sobre como gravar uma consulta de pesquisa, consulte o artigo de suporte do [!DNL Microsoft] <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">Pesquisar Emails e Pessoas no [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite] </td> 
   <td> <p>Insira o número máximo de mensagens que [!DNL Workfront Fusion] deve retornar durante um ciclo de execução de cenário.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assunto]</td> 
   <td> <p>Insira a linha de assunto da mensagem.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Conteúdo do Corpo]</td> 
   <td>Selecione se o conteúdo do corpo da mensagem é HTML ou Text.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conteúdo do corpo]</td> 
   <td> <p>Insira o texto do corpo da mensagem de email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importância]</td> 
   <td> <p>Selecionar a importância do email</p> 
    <ul> 
     <li>[!UICONTROL Baixo]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Alto]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Para Destinatários]</p> </td> 
   <td> <p>Adicione os recipients para os quais deseja enviar as mensagens:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Insira o nome do contato</p> </li> 
     <li> <p><strong>[!UICONTROL Endereço de Email]</strong> </p> <p>Insira o endereço de email do contato.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Adicionar os recipients A mensagem que você deseja receber:</p> 
    <ul> 
     <li> <p><strong>Nome</strong> </p> <p>Insira o nome do contato</p> </li> 
     <li> <p><strong>Endereço de email</strong> </p> <p>Insira o endereço de email do contato.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Destinatários com Cco</p> </td> 
   <td> <p>Adicione os recipients que deseja copiar na mensagem, sem permitir que outros recipients vejam seus nomes ou endereços de email:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Insira o nome do contato</p> </li> 
     <li> <p><strong>[!UICONTROL Endereço de Email]</strong> </p> <p>Insira o endereço de email do contato.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Anexos]</p> </td> 
   <td> <p>Adicionar os anexos ao email:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome do Arquivo]</strong> </p> <p>Insira o nome do arquivo. Exemplo: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Dados]</strong> </p> <p>Insira os dados do arquivo no campo ou mapeie a origem do arquivo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Do endereço de email]</td> 
   <td> <p> Para usar um endereço de email compartilhado, insira o endereço aqui. O usuário cujas credenciais são usadas na conexão usada para este módulo deve ter acesso à pasta compartilhada.<p>Deixe este campo em branco para usar o endereço de email do proprietário da conexão.</p></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Enviar uma mensagem de rascunho]

Envia uma mensagem de email que está atualmente no rascunho.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Do endereço de email]</td> 
   <td> <p> Para usar um endereço de email compartilhado, insira o endereço aqui. O usuário cujas credenciais são usadas na conexão usada para este módulo deve ter acesso à pasta compartilhada.<p>Deixe este campo em branco para usar o endereço de email do proprietário da conexão.</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Mensagem de Rascunho]</td> 
   <td> <p> Selecione ou mapeie a ID da mensagem do rascunho que deseja enviar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar uma Mensagem]

Atualiza uma mensagem existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Do endereço de email]</td> 
   <td> <p> Para usar um endereço de email compartilhado, insira o endereço aqui. O usuário cujas credenciais são usadas na conexão usada para este módulo deve ter acesso à pasta compartilhada.<p>Deixe este campo em branco para usar o endereço de email do proprietário da conexão.</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir uma ID de mensagem]</td> 
   <td> <p>Selecione como deseja identificar a mensagem a ser atualizada:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir Manualmente]</strong> </p> <p>Insira ou mapeie a ID da mensagem.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar na lista]</strong> </p> <p>Selecione a pasta que contém a mensagem que você deseja atualizar e selecione a mensagem</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assunto]</td> 
   <td> <p>Insira a linha de assunto da mensagem.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conteúdo do corpo]</td> 
   <td> <p>Insira o texto do corpo da mensagem de email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importância]</td> 
   <td> <p>Selecionar a importância do email</p> 
    <ul> 
     <li>[!UICONTROL Baixo]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Alto]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Para Destinatários]</p> </td> 
   <td> <p>Adicione o endereço de email para o qual deseja enviar as mensagens:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Insira o nome do contato</p> </li> 
     <li> <p><strong>[!UICONTROL Endereço de Email]</strong> </p> <p>Insira o endereço de email do contato.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Adicionar os recipients A mensagem que você deseja receber:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Insira o nome do contato</p> </li> 
     <li> <p><strong>[!UICONTROL Endereço de Email]</strong> </p> <p>Insira o endereço de email do contato.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Destinatários Cco]</p> </td> 
   <td> <p>Adicione os recipients que deseja copiar na mensagem, sem permitir que outros recipients vejam seus nomes ou endereços de email:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Insira o nome do contato</p> </li> 
     <li> <p><strong>[!UICONTROL Endereço de Email]</strong> </p> <p>Insira o endereço de email do contato.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Anexos]</p> </td> 
   <td> <p>Adicionar os anexos ao email:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome do Arquivo]</strong> </p> <p>Insira o nome do arquivo. Exemplo: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Dados]</strong> </p> <p>Insira os dados do arquivo no campo ou mapeie a origem do arquivo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Marcá-lo como Lido]</td> 
   <td>Habilite esta opção para marcar a mensagem atualizada como lida.</td> 
  </tr> 
 </tbody> 
</table>

### Anexo

* [[!UICONTROL Baixar um Anexo]](#download-an-attachment)
* [[!UICONTROL Listar anexos]](#list-attachments)

#### [!UICONTROL Baixar um Anexo]

Este módulo baixa o anexo especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Do endereço de email]</td> 
   <td> <p> Para usar um endereço de email compartilhado, insira o endereço aqui. O usuário cujas credenciais são usadas na conexão usada para este módulo deve ter acesso à pasta compartilhada.<p>Deixe este campo em branco para usar o endereço de email do proprietário da conexão.</p></p> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL ID da Mensagem]</td> 
   <td> <p> Selecione ou mapeie a ID da mensagem que contém o anexo que você deseja baixar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Anexo]</td> 
   <td> <p>Insira ou mapeie a ID do anexo que deseja baixar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listar anexos]

Este módulo recupera uma lista de anexos pertencentes à mensagem especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Do endereço de email]</td> 
   <td> <p> Para usar um endereço de email compartilhado, insira o endereço aqui. O usuário cujas credenciais são usadas na conexão usada para este módulo deve ter acesso à pasta compartilhada.<p>Deixe este campo em branco para usar o endereço de email do proprietário da conexão.</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Mensagem]</td> 
   <td> <p> Selecione ou mapeie a ID da mensagem da qual deseja recuperar anexos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de anexos que você deseja que o módulo retorne durante cada ciclo de execução do cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Outro

* [[!UICONTROL Adicionar Anexo]](#add-an-attachment)
  <!--Create and send a message-->
* [[!UICONTROL Fazer uma chamada de API]](#make-an-api-call)

#### [!UICONTROL Adicionar Anexo]

Este módulo adiciona um grande anexo a uma mensagem.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Do endereço de email]</td> 
   <td> <p> Para usar um endereço de email compartilhado, insira o endereço aqui. O usuário cujas credenciais são usadas na conexão usada para este módulo deve ter acesso à pasta compartilhada.<p>Deixe este campo em branco para usar o endereço de email do proprietário da conexão.</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Mensagem]</td> 
   <td> <p> Selecione ou mapeie a ID da mensagem à qual deseja adicionar um anexo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL arquivo Source]</td> 
   <td> <p>Selecione um arquivo de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Fazer uma chamada de API]

Este módulo permite executar uma chamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Insira um caminho relativo para <code>https://graph.microsoft.com</code>. Exemplo:<code> /v1.0/me/messages</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   td&gt; <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação na forma de um objeto JSON padrão. Por exemplo, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] adiciona os cabeçalhos de autorização para você.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadeia de Consulta]</td> 
   <td> <p> Adicione a consulta da chamada à API na forma de um objeto JSON padrão.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada à API na forma de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar instruções condicionais como <code>if</code> em seu JSON, coloque as aspas fora da instrução condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
