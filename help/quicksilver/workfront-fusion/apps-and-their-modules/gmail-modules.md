---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos Gmail
description: Em um [!DNL Adobe Workfront Fusion] você pode automatizar fluxos de trabalho que usam o Gmail, bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: 1987156c-e003-4f99-8913-cb47f77efbfc
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1785'
ht-degree: 0%

---

# [!DNL Gmail] módulos

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL Gmail], bem como conectá-lo a vários aplicativos e serviços de terceiros.

Se precisar de instruções para criar um cenário, consulte [Crie um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Para obter informações sobre módulos, consulte [Módulos em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Para usar [!DNL Gmail] módulos, você deve ter um [!DNL Gmail] conta.

## Connect [!DNL Gmail] para [!DNL Workfront Fusion] {#connect-gmail-to-workfront-fusion}

* [Connect [!DNL Gmail] para [!DNL Workfront Fusion] usando o [!DNL G Suite]](#connect-gmail-to-workfront-fusion-usingg-suite)
* [Connect [!DNL Gmail] para [!DNL Workfront Fusion] usar [!DNL gmail.com] ou [!DNL googlemail].com](#connect-gmail-to-workfront-fusion-using-gmailcom-or-googlemailcom)

### Connect [!DNL Gmail] para [!DNL Workfront Fusion] usar[!DNL  G Suite] {#connect-gmail-to-workfront-fusion-using-g-suite}

Para obter instruções sobre como conectar seu [!DNL G Suite] para [!UICONTROL Workfront Fusion], consulte [Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) no artigo [Crie um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Connect [!DNL Gmail] para [!DNL Workfront Fusion] usar [!DNL gmail.com] ou [!DNL googlemail].com {#connect-gmail-to-workfront-fusion-using-gmail-com-or-googlemail-com}

Se você [!DNL @gmail.com] ou [!DNL @googlemail.com] usuário, você deve criar um cliente OAuth em [o [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) para obter um [!UICONTROL ID do cliente] e [!UICONTROL Segredo do cliente].

Para obter instruções passo a passo sobre como criar o cliente OAuth e obter um [!UICONTROL ID do cliente] e [!UICONTROL Segredo do cliente], consulte [Conecte o Adobe Workfront Fusion ao Google Services usando um cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## [!DNL Gmail] módulos e seus campos

Ao configurar [!DNL Gmail] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Gmail] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Ações](#actions)
* [Iteradores](#iterators)

### Triggers

#### [!UICONTROL Assistir a emails]

Esse módulo de acionador executa um cenário quando um novo email é recebido para ser processado.

O módulo retorna todos os campos padrão associados ao registro ou registros, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Gmail] para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] para [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione a pasta de email que deseja visualizar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de filtro] </td> 
   <td> <p>Selecione o tipo de filtro que deseja usar para assistir aos emails</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Filtro simples]</strong> </p> <p>Preencha os campos [!UICONTROL Critérios], [!UICONTROL Endereço de email do remetente], [!UICONTROL Assunto] e [!UICONTROL Frase de pesquisa]</p> </li> 
     <li> <p> <strong>[!UICONTROL Filtro Gmail]</strong> </p> <p>No campo [!UICONTROL Query] , insira a consulta que deseja usar para filtrar emails.</p> <p>Para obter mais informações sobre [!DNL Gmail] filtros, consulte <a href="https://support.google.com/mail/answer/7190">Operadores de pesquisa</a> no [!DNL Gmail] documentação.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Critérios]</td> 
   <td>Selecione se você deseja assistir a emails do [!UICONTROL todo o email], do [!UICONTROL somente leitura] ou do [!UICONTROL somente não lidos].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Endereço de email do remetente]</td> 
   <td> <p> Insira um endereço de email para assistir somente emails enviados desse endereço.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assunto]</td> 
   <td>Insira uma string de texto para observar apenas emails que tenham essa string de texto no assunto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Frase de pesquisa]</td> 
   <td>Insira uma string de texto para observar somente emails que tenham essa string de texto em qualquer lugar do email.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Marcar mensagens de email como lidas quando buscadas]</td> 
   <td> <p> Ative essa opção para marcar os emails recuperados como lidos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de resultados]</td> 
   <td> <p> Defina o número máximo de resultados que [!DNL Workfront Fusion] funcionará durante um ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [[!UICONTROL Enviar um email]](#send-an-email)
* [[!UICONTROL Criar um rascunho]](#create-a-draft)
* [[!UICONTROL Marcar um email como lido]](#mark-an-email-as-read)
* [[!UICONTROL Marcar email como não lido]](#mark-an-email-as-unread)
* [[!UICONTROL Mover um email]](#move-an-email)
* [[!UICONTROL Copiar um email]](#copy-an-email)
* [[!UICONTROL Excluir um email]](#delete-an-email)
* [[!UICONTROL Modificar rótulos de email]](#modify-email-labels)

#### [!UICONTROL Enviar um email]

Este módulo de ação envia um novo email.

Especifique o recipient do email.

O módulo retorna a ID do email e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Gmail] para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL De]</td> 
   <td> <p>Insira ou mapeie um endereço de email do remetente.</p> <p>Observação: Se você digitar um endereço de email incorreto, pode ocorrer um erro ao enviar uma mensagem porque sua conta pode não ter permissão para enviar emails de um endereço diferente do seu.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL To] </td> 
   <td> <p>Clique em <strong>[!UICONTROL Adicionar]</strong>, em seguida, insira ou mapeie o endereço de email de cada recipient.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assunto] </td> 
   <td> <p>Insira ou mapeie o assunto do email.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Conteúdo] </td> 
   <td> <p>Insira ou mapeie o conteúdo do email (corpo da mensagem). Tags de HTML são permitidas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Anexos] </td> 
   <td> <p>Clique em <strong>[!UICONTROL Adicionar]</strong> para adicionar um anexo. Você pode mapear um arquivo dos módulos anteriores.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copiar destinatários]</td> 
   <td> <p> Clique em <strong>[!UICONTROL Adicionar]</strong>, em seguida, insira ou mapeie o endereço de email de cada destinatário de cópia.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destinatários de cópia oculta]</td> 
   <td> <p> Clique em <strong>[!UICONTROL Adicionar]</strong>, em seguida, insira ou mapeie o endereço de email de cada destinatário de cópia oculta.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar um rascunho]

Esse módulo de ação cria um novo rascunho de email e o adiciona a uma pasta especificada.

Especifique a pasta onde deseja criar um rascunho.

O módulo retorna a ID do rascunho de email e de quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Gmail] para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] para [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione o [!DNL Gmail] pasta na qual deseja criar um rascunho.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL To] </td> 
   <td> <p>Clique em <strong>[!UICONTROL Adicionar]</strong>, em seguida, insira ou mapeie o endereço de email de cada recipient.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assunto] </td> 
   <td> <p>Insira ou mapeie o assunto do email.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Conteúdo] </td> 
   <td> <p>Insira ou mapeie o conteúdo do email (corpo da mensagem). Tags de HTML são permitidas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Anexos] </td> 
   <td> <p>Clique em <strong>[!UICONTROL Adicionar]</strong> para adicionar um anexo. Você pode mapear um arquivo dos módulos anteriores.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copiar destinatários]</td> 
   <td> <p> Clique em <strong>[!UICONTROL Adicionar]</strong>, em seguida, insira ou mapeie o endereço de email de cada destinatário de cópia.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destinatários de cópia oculta]</td> 
   <td> <p> Clique em <strong>[!UICONTROL Adicionar]</strong>, em seguida, insira ou mapeie o endereço de email de cada destinatário de cópia oculta.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Marcar um email como lido]

Este módulo de ação marca um email como lido.

Especifique a ID do email e sua pasta.

O módulo retorna a ID do email e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Gmail] para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] para [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione o [!DNL Gmail] pasta que contém o email.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de email (UID)]</td> 
   <td> <p> Insira ou mapeie a ID do email.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Marcar email como não lido]

Este módulo de ação marca um email ou rascunho de email como não lido.

Especifique a ID do email e sua pasta.

O módulo retorna a ID do email e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Gmail] para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] para [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione o [!DNL Gmail] pasta que contém o email.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de email (UID)] </td> 
   <td> <p>Insira ou mapeie a ID de email do email que você deseja marcar como não lido.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover um email]

Esse módulo de ação move um email ou rascunho de email para uma pasta especificada.

Especifique a pasta, a pasta de destino e a ID do email.

O módulo retorna a ID do email e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Gmail] para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] para [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione o [!DNL Gmail] pasta de origem que contém o email que deseja mover.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta de destino]</td> 
   <td> <p> Selecione o [!DNL Gmail] pasta de destino para a qual deseja mover o email.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de email (UID)]</td> 
   <td> <p> Insira ou mapeie a ID de email do email que deseja mover.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiar um email]

Esse módulo de ação copia um email ou rascunho de email para uma pasta especificada.

Especifique a pasta, a pasta de destino e a ID do email.

O módulo retorna a ID do email e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Gmail] para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] para [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione o [!DNL Gmail] pasta de origem que contém o email que você deseja copiar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta de destino]</td> 
   <td> <p>Selecione o [!DNL Gmail] pasta de destino para a qual deseja copiar o email.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de email (UID)]</td> 
   <td> <p>Insira ou mapeie a ID de email do email que deseja copiar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir um email]

Esse módulo de ação remove um email ou rascunho de email de uma pasta especificada.

O módulo retorna a ID do email e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Gmail] para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] para [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL [!DNL Gmail] ID da mensagem]</p> </td> 
   <td> <p>Insira ou mapeie a ID de email do email que deseja excluir.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Permanentemente] </td> 
   <td> <p>Ative essa opção para permitir que o módulo exclua permanentemente o email, em vez de movê-lo para a pasta de lixo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Modificar rótulos de email]

Esse módulo de ação modifica o rótulo de uma mensagem de email especificada.

O módulo retorna a ID do email e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Gmail] para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] para [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Gmail] ID da mensagem]</td> 
   <td> <p> Insira ou mapeie a ID de email do email que deseja excluir.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Rótulos para adicionar]</p> </td> 
   <td> <p>Selecione ou mapeie o rótulo que deseja adicionar à mensagem de email selecionada.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rótulos a serem removidos]</td> 
   <td> <p> Selecione ou mapeie o rótulo que deseja remover da mensagem de email selecionada.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>[!UICONTROL Rótulo para adicionar] e [!UICONTROL Rótulo a ser removido] campos carregam somente rótulos criados pelo usuário.

### Iteradores

#### [!UICONTROL Iterar anexos]

Você pode iterar anexos de email. Cada anexo é um pacote separado na saída do módulo. Para obter mais informações, consulte [Módulo iterador no Adobe Workfront Fusion](../../workfront-fusion/modules/iterator-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Módulo de origem] </td> 
   <td> <p>Selecione o módulo do qual deseja iterar anexos. </p> </td> 
  </tr> 
 </tbody> 
</table>
