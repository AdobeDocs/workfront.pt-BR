---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de email
description: Em um [!DNL Adobe Workfront Fusion] você pode conectar sua conta de email a vários aplicativos e serviços de terceiros.Isso permite baixar emails via IMAP, enviar emails via SMTP, criar novos rascunhos, mover e copiar emails de uma pasta para outra pasta, marcar emails como lidos ou não lidos e excluir emails.
author: Becky
feature: Workfront Fusion
exl-id: 384ba60a-d79e-4126-a247-6d67b5154ede
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2613'
ht-degree: 0%

---

# Módulos de email

Em um [!DNL Adobe Workfront Fusion] você pode conectar sua conta de email a vários aplicativos e serviços de terceiros.Isso permite baixar emails via IMAP, enviar emails via SMTP, criar novos rascunhos, mover e copiar emails de uma pasta para outra pasta, marcar emails como lidos ou não lidos e excluir emails.

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

## Conecte seu email ao Workfront Fusion {#connect-your-email-to-workfront-fusion}

* [Conectar-se ao Google](#connect-to-google)
* [Conectar-se a outros serviços de email (SMAP)](#connect-to-other-email-services-smap)

### Conectar-se a [!DNL Google]

Use essa opção para criar cenários com módulos de email que exigem uma conexão com seu [!DNL Google] conta. Esta é uma conta com escopos restritos.

Você pode criar uma conexão com o [!DNL Google] conta diretamente de dentro de um módulo de email.

1. Em qualquer módulo de email, clique em **[!UICONTROL Adicionar]** ao lado do [!UICONTROL Conexão] campo.
1. Selecionar **[!DNL Google]** como o tipo de conexão.
1. Digite um nome para a conexão.
1. (Opcional) Insira seu [!UICONTROL [!DNL Google] ID do cliente] e [!UICONTROL Segredo do cliente].
1. Clique em **[!UICONTROL Continuar]** para criar a conexão e retornar ao módulo .

### Conectar-se a outros serviços de email (SMAP)

A conexão SMAP permite acessar sua caixa de correio remotamente e ler ou manipular mensagens em sua caixa de correio. A conexão SMAP é usada pela maioria dos módulos de email.

1. Em qualquer módulo de email, clique em **[!UICONTROL Adicionar]** ao lado do [!UICONTROL Conexão] campo.
1. Selecionar **[!UICONTROL Outros (SMTP)]** como o tipo de conexão.
1. Insira um **[!UICONTROL Nome]** para a conexão.
1. Selecione seu **[!UICONTROL Provedor de email]** na lista. Se o seu provedor de email não estiver na lista, selecione Outro.
1. Insira seu **[!UICONTROL Endereço de email]**, **[!UICONTROL Seu nome completo]**, seu **[!UICONTROL Nome do usuário]** e seu **[!UICONTROL Senha]**.
1. (Condicional) Se o seu provedor não estiver na lista, insira o **[!UICONTROL Servidor SMTP]** e **[!UICONTROL Port]** e especifique se deseja **[!UICONTROL Usar uma conexão segura (TLS)]**. Para localizar essas informações, marque a opção [!UICONTROL Ajuda] para sua caixa de correio. Caso não tenha essas informações disponíveis, entre em contato com seu provedor de serviços de email.
1. Clique em **[!UICONTROL Continuar]** para criar a conexão e retornar ao módulo .

## [!UICONTROL Email] módulos e seus campos

Ao configurar [!UICONTROL Email] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Juntamente com esses campos, campos adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Alguns dos campos de email podem já conter dados, pois você os usou em outro módulo do cenário. Consulte a documentação de ajuda de email se precisar de informações sobre eles.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>A ID de Email Exclusiva conhecida como &#39;[!UICONTROL ID de email (UID)]&#39; é o identificador do email. A ID de email é específica para cada uma das pastas do email.

* [Triggers](#triggers)
* [Ações](#actions)
* [Iteradores](#iterators)

### Triggers

#### [!UICONTROL Assistir aos emails]

Aciona quando um novo email é recebido para processamento de acordo com critérios especificados.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta de email ao [!UICONTROL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conecte seu email ao [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta] </td> 
   <td> <p>Selecione a pasta que contém emails que deseja assistir.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Critérios]</p> </td> 
   <td> <p>Selecione os critérios pelos quais deseja assistir aos emails:</p> 
    <ul> 
     <li>[!UICONTROL Todos os emails]</li> 
     <li>[!UICONTROL Somente Ler Emails]</li> 
     <li>[!UICONTROL Somente Emails Não Lidos]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Endereço de email do remetente] </td> 
   <td> <p>Insira o endereço de email do remetente cujos emails você deseja assistir.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Endereço de email do destinatário]</td> 
   <td> <p> Insira o endereço de email do recipient cujos emails você deseja assistir.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assunto] </td> 
   <td> <p>Insira o assunto do email que deseja assistir.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Frase] </td> 
   <td> <p>Insira quaisquer palavras-chave para observar apenas os emails contendo frases específicas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Marcar mensagem(s) como lida quando obtida]</td> 
   <td> <p>Ative essa opção para marcar o email não lido como lido após recuperar os detalhes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de resultados]</td> 
   <td> <p> O número máximo de emails [!DNL Workfront Fusion] deve retornar durante um ciclo de execução de cenário.</p> </td> 
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
* [[!UICONTROL Obter emails]](#get-emails)
* [[!UICONTROL Enviar-me um e-mail]](#send-me-an-email)

#### [!UICONTROL Enviar um email]

Envia um novo email.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta de email a [!DNL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conecte seu email ao [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salvar mensagem após o envio]</td> 
   <td>Depois que a mensagem de email for enviada, ela será salva na caixa de correio. Ative essa opção se desejar salvar emails enviados usando [!DNL Workfront Fusion] para <i>[!UICONTROL Enviado email]</i> ou outra pasta na caixa de correio. Alguns serviços de email, como [!DNL Gmail], salvar mensagens enviadas automaticamente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL To] </td> 
   <td> <p>Adicione os endereços de email para os quais deseja enviar o email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assunto] </td> 
   <td> <p>Insira ou mapeie a linha de assunto do email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de conteúdo]</p> </td> 
   <td> <p>Selecione o tipo [!UICONTROL content] para o email:</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL Plaintext]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conteúdo] </td> 
   <td> <p>Insira ou mapeie o conteúdo do email no formato HTML usando tags HTML ou no texto simples, dependendo do que você escolheu no campo [!UICONTROL Tipo de conteúdo].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Anexos]</p> </td> 
   <td> <p>Adicionar um anexo:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome do arquivo]</strong> </p> <p>Insira o nome do arquivo. Por exemplo, sample.doc.</p> </li> 
     <li> <p><strong>[!UICONTROL Dados]</strong> </p> <p>Insira o caminho para a pasta para fazer upload do anexo.</p> </li> 
     <li> <p><strong>[!UICONTROL Content-ID]</strong> </p> <p>Insira a [!UICONTROL ID de conteúdo] para inserir o anexo (imagem) no conteúdo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copiar destinatário] </td> 
   <td> <p>Insira ou mapeie um ou mais endereços de email para os quais deseja enviar uma cópia desse email. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recipient de cópia oculta]</td> 
   <td> <p> Insira ou mapeie um ou mais endereços de email para os quais deseja enviar uma cópia desse email sem ter o endereço de email exibido no email.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL De] </td> 
   <td> <p>Insira ou mapeie o endereço de email (e nome, se necessário) que aparece no campo [!UICONTROL De] no email. </p> <p>Importante: Use a sintaxe correta: <code>name@email.com</code> ou <code>"Name" name@email.com</code>.</p> <p>Observação: Normalmente, [!DNL Workfront Fusion] O usa o endereço de email inserido ao criar a conexão como o endereço do remetente. Se você inserir qualquer outro endereço de email, poderá ocorrer um erro ao enviar uma mensagem, pois sua conta pode não ter permissão para enviar emails de um endereço diferente do seu. Por exemplo <code>test@mail.com</code> ou "<code>John Bush" test@email.com</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Remetente]</p> </td> 
   <td> <p>Insira ou mapeie o endereço de email que aparece no campo [!UICONTROL Sender] no email.</p> <p>Dica: Se não tiver certeza se deseja usar esse campo ou o campo De, recomendamos escolher o campo De.</p> <p>Importante: Use a sintaxe correta: <code>name@email.com</code> ou <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Responder para]</td> 
   <td> <p> Se desejar que as respostas a este email sejam enviadas para um endereço diferente do "de", insira o endereço de email para onde deseja que as respostas a esse email sejam enviadas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Em Resposta]</td> 
   <td> <p> Se estiver respondendo a um email específico, insira ou mapeie a ID do email ao qual você está respondendo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Referências] </td> 
   <td> <p>Insira as IDs de mensagem de todas as respostas no thread.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prioridade]</p> </td> 
   <td> <p>Selecione a prioridade do email:</p> 
    <ul> 
     <li>[!UICONTROL Alta]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Baixo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Cabeçalhos]</p> </td> 
   <td> <p>Adicione os cabeçalhos:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Chave]</strong> </p> <p>Adicione a chave. Por exemplo, [!UICONTROL Remetente], [!UICONTROL Data], [!UICONTROL To] e assim por diante.</p> </li> 
     <li> <p><strong>[!UICONTROL Valor]</strong> </p> <p>Insira o valor da chave.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar um rascunho]

Cria e adiciona um novo rascunho a uma pasta selecionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta de email ao [!UICONTROL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conecte seu email ao [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta]</td> 
   <td>Selecione a pasta na qual deseja criar o email de rascunho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL To] </td> 
   <td> <p>Insira ou mapeie o endereço de email para o qual deseja enviar o email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assunto] </td> 
   <td> <p>Insira ou mapeie a linha de assunto do email.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de conteúdo]</p> </td> 
   <td> <p>Selecione o tipo de conteúdo do email:</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL Texto simples]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conteúdo] </td> 
   <td> <p>Insira ou mapeie o conteúdo do email no formato HTML usando tags HTML ou no texto simples, dependendo do que você escolheu no campo [!UICONTROL Tipo de conteúdo].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Anexos]</p> </td> 
   <td> <p>Adicionar um anexo:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome do arquivo]</strong> </p> <p>Insira o nome do arquivo. Por exemplo, sample.doc.</p> </li> 
     <li> <p><strong>[!UICONTROL Dados]</strong> </p> <p>Insira o caminho para a pasta para fazer upload do anexo.</p> </li> 
     <li> <p><strong>[!UICONTROL Content-ID]</strong> </p> <p>Insira a ID de conteúdo para inserir o anexo (imagem) no conteúdo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copiar destinatário] </td> 
   <td> <p>Insira ou mapeie um ou mais endereços de email para os quais deseja enviar uma cópia desse email. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recipient de cópia oculta]</td> 
   <td> <p> Insira ou mapeie um ou mais endereços de email para os quais deseja enviar uma cópia desse email sem ter o endereço de email exibido no email.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL De] </td> 
   <td> <p>Insira ou mapeie o endereço de email (e nome, se necessário) que aparece no campo [!UICONTROL De] no email. </p> <p>Importante: Use a sintaxe correta: <code>name@email.com</code> ou <code>"Name" name@email.com</code>.</p> <p>Observação: Normalmente, [!DNL Workfront Fusion] O usa o endereço de email inserido ao criar a conexão como o endereço do remetente. Se você inserir qualquer outro endereço de email, poderá ocorrer um erro ao enviar uma mensagem, pois sua conta pode não ter permissão para enviar emails de um endereço diferente do seu. Por exemplo <code>test@mail.com</code> ou "<code>John Bush" test@email.com</code>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Remetente]</p> </td> 
   <td> <p>Insira ou mapeie o endereço de email que aparece no campo [!UICONTROL Sender] no email.</p> <p>Dica: Se não tiver certeza se deseja usar esse campo ou o campo De, recomendamos escolher o campo De.</p> <p>Importante: Use a sintaxe correta: <code>name@email.com</code> ou <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Responder para]</td> 
   <td> <p> Se desejar que as respostas a este email sejam enviadas para um endereço diferente do endereço "[!UICONTROL from]", insira o endereço de email para onde deseja que as respostas a esse email sejam enviadas.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Em Resposta]</td> 
   <td> <p> Se estiver respondendo a um email específico, insira ou mapeie a ID do email ao qual você está respondendo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Referências] </td> 
   <td> <p>Insira as IDs de mensagem de todas as respostas no thread.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Prioridade]</p> </td> 
   <td> <p>Selecione a prioridade do email:</p> 
    <ul> 
     <li>[!UICONTROL Alta]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Baixo]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Cabeçalhos]</p> </td> 
   <td> <p>Adicione os cabeçalhos:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Chave]</strong> </p> <p>Adicione a chave. Por exemplo, Remetente, Data, Para e assim por diante.</p> </li> 
     <li> <p><strong>[!UICONTROL Valor]</strong> </p> <p>Insira o valor da chave.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Marcar um email como lido]

Marca um email ou um rascunho em uma pasta selecionada como lido ao definir a variável [!UICONTROL Ler] sinalizador.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta de email ao [!UICONTROL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conecte seu email ao [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta]</td> 
   <td>Selecione a pasta do email que deseja marcar como lido. Exemplo: Primário.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de email (UID)]</p> </td> 
   <td> <p>Insira o UID do email que você deseja marcar como lido.</p> <p>Você pode obter a UID do email usando o módulo [!UICONTROL Email] &gt;[!UICONTROL Watch Email] ou o módulo [!UICONTROL Search Email].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Marcar email como não lido]

Marca um email ou um rascunho em uma pasta selecionada como não lido ao configurar o sinalizador Não lido .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta de email ao [!UICONTROL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conecte seu email ao [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta]</td> 
   <td>Selecione a pasta do email que deseja marcar como não lido. Exemplo: Primário.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de email (UID)]</p> </td> 
   <td> <p>Insira o UID do email que você deseja marcar como não lido.</p> <p>Você pode obter a UID do email usando o módulo [!UICONTROL Email] &gt;[!UICONTROL Watch Email] ou o módulo [!UICONTROL Search Email].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover um email]

Move um email ou rascunho escolhido para uma pasta selecionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta de email ao [!UICONTROL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conecte seu email ao [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta de origem]</td> 
   <td>Selecione a pasta que contém o email da qual deseja mover o email. Exemplo: Primário.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta de destino]</td> 
   <td> <p> Selecione a pasta à qual deseja adicionar o email. Exemplo: Trabalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de email (UID)]</p> </td> 
   <td> <p>Insira o UID de email do email que você deseja mover para a pasta de destino.</p> <p>Você pode obter a UID do email usando o módulo [!UICONTROL Email] &gt;[!UICONTROL Watch Email] ou o módulo [!UICONTROL Search Email].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiar um email]

Copia um email ou rascunho em uma pasta selecionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta de email ao [!UICONTROL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conecte seu email ao [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta de origem]</td> 
   <td>Selecione a pasta da qual deseja copiar o email. Exemplo: Primário.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta de destino]</td> 
   <td> <p> Selecione a pasta para a qual deseja copiar o email. Exemplo: Trabalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de email (UID)]</p> </td> 
   <td> <p>Insira o UID de email do email que você deseja copiar para a pasta de destino.</p> <p>Você pode obter a UID do email usando o módulo [!UICONTROL Email] &gt;[!UICONTROL Watch Email] ou o módulo [!UICONTROL Search Email].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir um email]

Remove um email ou rascunho da pasta selecionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta de email ao [!UICONTROL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conecte seu email ao [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta]</td> 
   <td>Selecione a pasta do email que deseja excluir. Exemplo: Primário.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de email (UID)]</p> </td> 
   <td> <p>Insira o UID do email que deseja excluir.</p> <p>Você pode obter a UID do email usando o módulo [!UICONTROL Email] &gt;[!UICONTROL Watch Email] ou o módulo [!UICONTROL Search Email].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expunge]</td> 
   <td> <p>Habilite esta opção para permitir que o módulo remova permanentemente todas as mensagens sinalizadas como [!UICONTROL Excluído] na caixa de correio aberta no momento.</p> <p>Observação: Em [!DNL Gmail], esse comportamento é impulsionado pela configuração na seção [!UICONTROL Configurações] &gt;[!UICONTROL Encaminhamento POP/IMAP no acesso IMAP].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter emails]

Retorna emails que correspondem aos critérios especificados.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta de email ao [!UICONTROL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conecte seu email ao [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta] </td> 
   <td> <p>Selecione a pasta que contém os emails que deseja recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Marcar mensagem(s) como lida quando obtida] </td> 
   <td> <p>Ative essa opção se desejar marcar o email não lido como lido após recuperar os detalhes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Critérios]</p> </td> 
   <td> <p>Selecione os critérios dos emails que deseja recuperar:</p> 
    <ul> 
     <li>[!UICONTROL Todos os emails]</li> 
     <li>[!UICONTROL Somente Ler Emails]</li> 
     <li>[!UICONTROL Somente Emails Não Lidos]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Endereço de email do remetente] </td> 
   <td> <p>Insira ou mapeie o endereço de email do remetente cujos emails deseja recuperar.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Endereço de email do destinatário]</td> 
   <td> <p> Insira ou mapeie o endereço de email do recipient cujos emails deseja recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Da data] </td> 
   <td> <p>Insira ou mapeie a data para recuperar os emails processados na ou após a data especificada.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Antes da data]</td> 
   <td> <p> Insira ou mapeie a data para recuperar os emails processados na ou antes da data especificada.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assunto] </td> 
   <td> <p>Insira ou mapeie o assunto do email que deseja recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Frase] </td> 
   <td> <p>Insira ou mapeie quaisquer palavras-chave para recuperar apenas os emails contendo frases específicas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de email (UID)]</td> 
   <td> <p> Insira a ID de email (UID) do email cujos detalhes você deseja recuperar.</p> <p>Você pode obter a UID do email usando [!DNL Workfront Fusion]Módulo s[!UICONTROL Watch Email] ou módulo [!UICONTROL Search Email].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de resultados]</td> 
   <td> <p> O número máximo de emails [!DNL Workfront Fusion] deve retornar durante um ciclo de execução de cenário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Continuar a execução da rota mesmo se o módulo não retornar nenhum resultado]</td> 
   <td> <p> Selecione se deseja continuar a executar o módulo mesmo que não haja resultados retornados.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Enviar-me um e-mail]

Envia um novo email para seu endereço de email.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assunto] </td> 
   <td> <p>Insira ou mapeie a linha de assunto do email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conteúdo] </td> 
   <td> <p>Insira o corpo do email.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Iteradores

#### [!UICONTROL Iterar Anexos]

Itera anexos recebidos um por um.

O módulo iterador de email permite gerenciar anexos de email separadamente. Por exemplo, você pode configurar para assistir a emails para iterar os emails com anexos e receber alertas.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Módulo de origem]</td> 
   <td> <p>Selecione o módulo que gera o email com os anexos que você deseja iterar.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais informações sobre iteradores, consulte [Módulo iterador em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
