---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Gmail
description: Em um [!DNL Adobe Workfront Fusion] Você pode automatizar fluxos de trabalho que usam o Gmail, bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: 1987156c-e003-4f99-8913-cb47f77efbfc
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1833'
ht-degree: 0%

---

# [!DNL Gmail] módulos

Em um [!DNL Adobe Workfront Fusion] cenário, é possível automatizar workflows que usam [!DNL Gmail], bem como conectá-lo a vários aplicativos e serviços de terceiros.

Se precisar de instruções sobre como criar um cenário, consulte [Criar um cenário no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Para obter informações sobre módulos, consulte [Módulos no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Para usar [!DNL Gmail] módulos, você deve ter uma [!DNL Gmail] conta.

## Conectar [!DNL Gmail] para [!DNL Workfront Fusion] {#connect-gmail-to-workfront-fusion}

* [Conectar [!DNL Gmail] para [!DNL Workfront Fusion] usando o [!DNL G Suite]](#connect-gmail-to-workfront-fusion-usingg-suite)
* [Conectar [!DNL Gmail] para [!DNL Workfront Fusion] usar [!DNL gmail.com] ou [!DNL googlemail].com](#connect-gmail-to-workfront-fusion-using-gmailcom-or-googlemailcom)

### Conectar [!DNL Gmail] para [!DNL Workfront Fusion] usar[!DNL  G Suite] {#connect-gmail-to-workfront-fusion-using-g-suite}

Para obter instruções sobre como conectar seu [!DNL G Suite] conta para [!UICONTROL Workfront Fusion], consulte [Conecte o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) no artigo [Criar um cenário no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Conectar [!DNL Gmail] para [!DNL Workfront Fusion] usar [!DNL gmail.com] ou [!DNL googlemail].com {#connect-gmail-to-workfront-fusion-using-gmail-com-or-googlemail-com}

Se você estiver [!DNL @gmail.com] ou [!DNL @googlemail.com] usuário, você deve criar um cliente OAuth em [o [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) a fim de obter uma [!UICONTROL ID do cliente] e [!UICONTROL Segredo do cliente].

Para obter instruções passo a passo sobre como criar o cliente OAuth e obter um [!UICONTROL ID do cliente] e [!UICONTROL Segredo do cliente], consulte [Conectar o Adobe Workfront Fusion ao Google Services usando um cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## [!DNL Gmail] módulos e seus campos

Ao configurar [!DNL Gmail] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Gmail] Os campos podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Ações](#actions)
* [Iteradores](#iterators)

### Triggers

#### [!UICONTROL Assistir a emails]

Esse módulo de acionamento executa um cenário quando um novo email é recebido para ser processado.

O módulo retorna todos os campos padrão associados ao registro ou aos registros, juntamente com quaisquer campos e valores personalizados que a conexão acesse. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Gmail] conta para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Gmail] para o [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione a pasta de e-mail que deseja observar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de filtro] </td> 
   <td> <p>Selecione o tipo de filtro que deseja usar para assistir a emails</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Filtro simples]</strong> </p> <p>Preencha os campos [!UICONTROL Critérios], [!UICONTROL Endereço de email do remetente], [!UICONTROL Assunto] e [!UICONTROL Frase de Pesquisa]</p> </li> 
     <li> <p> <strong>[!UICONTROL Filtro Gmail]</strong> </p> <p>No campo [!UICONTROL Consulta], insira a consulta que deseja usar para filtrar emails.</p> <p>Para obter mais informações sobre [!DNL Gmail] filtros, consulte <a href="https://support.google.com/mail/answer/7190">Operadores de pesquisa</a> no [!DNL Gmail] documentação.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Critério]</td> 
   <td>Selecione se deseja assistir a emails do [!UICONTROL todos os emails], do [!UICONTROL somente emails lidos] ou do [!UICONTROL somente emails não lidos].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Endereço de email do remetente]</td> 
   <td> <p> Digite um endereço de e-mail para ver apenas os e-mails enviados a partir desse endereço.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assunto]</td> 
   <td>Digite uma sequência de texto para ver somente os emails que tenham essa sequência de texto no assunto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pesquisar frase]</td> 
   <td>Digite uma sequência de texto para ver somente os emails que possuem essa sequência de texto em qualquer lugar do email.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Marcar mensagens de email como lidas quando buscadas]</td> 
   <td> <p> Ative esta opção para marcar os e-mails recuperados como lidos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de resultados]</td> 
   <td> <p> Defina o número máximo de resultados que [!DNL Workfront Fusion] funcionará com durante um ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [[!UICONTROL Enviar um email]](#send-an-email)
* [[!UICONTROL Criar um rascunho]](#create-a-draft)
* [[!UICONTROL Marcar um email como lido]](#mark-an-email-as-read)
* [[!UICONTROL Marcar um email como não lido]](#mark-an-email-as-unread)
* [[!UICONTROL Mover um email]](#move-an-email)
* [[!UICONTROL Copiar um email]](#copy-an-email)
* [[!UICONTROL Excluir um email]](#delete-an-email)
* [[!UICONTROL Modificar rótulos de email]](#modify-email-labels)

#### [!UICONTROL Enviar um email]

Esse módulo de ação envia um novo email.

Especifique o recipient do email.

O módulo retorna a ID do email e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Gmail] conta para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Gmail] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL De]</td> 
   <td> <p>Insira ou mapeie um endereço de email de remetente.</p> <p>Observação: se você inserir um endereço de email incorreto, poderá ocorrer um erro ao enviar uma mensagem porque sua conta talvez não tenha permissão para enviar emails de um endereço diferente do seu.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Para] </td> 
   <td> <p>Clique em <strong>[!UICONTROL Adicionar]</strong>e, em seguida, insira ou mapeie o endereço de email de cada recipient.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assunto] </td> 
   <td> <p>Insira ou mapeie o assunto do email.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Conteúdo] </td> 
   <td> <p>Insira ou mapeie o conteúdo do email (corpo da mensagem). Tags HTML são permitidas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Anexos] </td> 
   <td> <p>Clique em <strong>[!UICONTROL Adicionar]</strong> para adicionar um anexo. Você pode mapear um arquivo dos módulos anteriores.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copiar destinatários]</td> 
   <td> <p> Clique em <strong>[!UICONTROL Adicionar]</strong>e, em seguida, insira ou mapeie o endereço de email de cada destinatário da cópia.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destinatários de cópia oculta]</td> 
   <td> <p> Clique em <strong>[!UICONTROL Adicionar]</strong>e, em seguida, insira ou mapeie o endereço de email de cada destinatário de cópia oculta.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar um rascunho]

Esse módulo de ação cria um novo rascunho de email e o adiciona a uma pasta especificada por você.

Você especifica a pasta na qual deseja criar um rascunho.

O módulo retorna a ID do rascunho do email e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Gmail] conta para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Gmail] para o [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione o [!DNL Gmail] pasta na qual você deseja criar um rascunho.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Para] </td> 
   <td> <p>Clique em <strong>[!UICONTROL Adicionar]</strong>e, em seguida, insira ou mapeie o endereço de email de cada recipient.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assunto] </td> 
   <td> <p>Insira ou mapeie o assunto do email.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Conteúdo] </td> 
   <td> <p>Insira ou mapeie o conteúdo do email (corpo da mensagem). Tags HTML são permitidas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Anexos] </td> 
   <td> <p>Clique em <strong>[!UICONTROL Adicionar]</strong> para adicionar um anexo. Você pode mapear um arquivo dos módulos anteriores.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copiar destinatários]</td> 
   <td> <p> Clique em <strong>[!UICONTROL Adicionar]</strong>e, em seguida, insira ou mapeie o endereço de email de cada destinatário da cópia.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destinatários de cópia oculta]</td> 
   <td> <p> Clique em <strong>[!UICONTROL Adicionar]</strong>e, em seguida, insira ou mapeie o endereço de email de cada destinatário de cópia oculta.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Marcar um email como lido]

Este módulo de ação marca um email como lido.

Especifique a ID do email e sua pasta.

O módulo retorna a ID do email e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Gmail] conta para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Gmail] para o [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione o [!DNL Gmail] pasta que contém o email.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID DE E-MAIL (UID)]</td> 
   <td> <p> Insira ou mapeie a ID de email.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Marcar um email como não lido]

Este módulo de ação marca um email ou rascunho de email como não lido.

Especifique a ID do email e sua pasta.

O módulo retorna a ID do email e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Gmail] conta para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Gmail] para o [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione o [!DNL Gmail] pasta que contém o email.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID DE E-MAIL (UID)] </td> 
   <td> <p>Insira ou mapeie a ID de e-mail do e-mail que você deseja marcar como não lido.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover um email]

Esse módulo de ação move um email ou rascunho de email para uma pasta especificada por você.

Você especifica a pasta, a pasta de destino e a ID do email.

O módulo retorna a ID do email e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Gmail] conta para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Gmail] para o [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione o [!DNL Gmail] pasta de origem que contém o email que você deseja mover.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta de destino]</td> 
   <td> <p> Selecione o [!DNL Gmail] pasta de destino para a qual você deseja mover o email.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID DE E-MAIL (UID)]</td> 
   <td> <p> Insira ou mapeie a ID de email do email que você deseja mover.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiar um email]

Esse módulo de ação copia um email ou rascunho de email para uma pasta especificada por você.

Você especifica a pasta, a pasta de destino e a ID do email.

O módulo retorna a ID do email e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Gmail] conta para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Gmail] para o [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta] </td> 
   <td> <p>Selecione o [!DNL Gmail] pasta de origem que contém o email que você deseja copiar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta de destino]</td> 
   <td> <p>Selecione o [!DNL Gmail] pasta de destino para a qual você deseja copiar o email.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID DE E-MAIL (UID)]</td> 
   <td> <p>Insira ou mapeie a ID de e-mail do e-mail que deseja copiar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir um email]

Esse módulo de ação remove um email ou um rascunho de email de uma pasta especificada.

O módulo retorna a ID do email e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Gmail] conta para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Gmail] para o [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL [!DNL Gmail] ID da mensagem]</p> </td> 
   <td> <p>Insira ou mapeie a ID de e-mail do e-mail que deseja excluir.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Permanentemente] </td> 
   <td> <p>Ative esta opção para permitir que o módulo exclua permanentemente o e-mail, em vez de movê-lo para a pasta de lixo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Modificar rótulos de email]

Esse módulo de ação modifica o rótulo em uma mensagem de email especificada.

O módulo retorna a ID do email e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Gmail] conta para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Gmail] para o [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Gmail] ID da mensagem]</td> 
   <td> <p> Insira ou mapeie a ID de e-mail do e-mail que deseja excluir.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Rótulos a serem adicionados]</p> </td> 
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
>[!UICONTROL Rótulo a ser adicionado] e [!UICONTROL Rótulo a ser removido] os campos carregam somente rótulos criados pelo usuário.

### Iteradores

#### [!UICONTROL Iterar anexos]

Você pode iterar anexos de email. Cada anexo é um conjunto separado na saída do módulo. Para obter mais informações, consulte [Módulo Iterador no Adobe Workfront Fusion](../../workfront-fusion/modules/iterator-module.md).

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
