---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de email
description: Em um [!DNL Adobe Workfront Fusion] Neste cenário, você pode conectar sua conta de email a vários aplicativos e serviços de terceiros. Isso permite baixar emails via IMAP, enviar emails via SMTP, criar novos rascunhos, mover e copiar emails de uma pasta para outra pasta, marcar emails como lidos ou não lidos e excluir emails.
author: Becky
feature: Workfront Fusion
exl-id: 384ba60a-d79e-4126-a247-6d67b5154ede
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '2626'
ht-degree: 0%

---

# Módulos de email

Em um [!DNL Adobe Workfront Fusion] Neste cenário, você pode conectar sua conta de email a vários aplicativos e serviços de terceiros. Isso permite baixar emails via IMAP, enviar emails via SMTP, criar novos rascunhos, mover e copiar emails de uma pasta para outra pasta, marcar emails como lidos ou não lidos e excluir emails.

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

## Conectar seu email ao Workfront Fusion {#connect-your-email-to-workfront-fusion}

* [Conectar-se ao Google](#connect-to-google)
* [Conectar-se a outros serviços de email (SMAP)](#connect-to-other-email-services-smap)

### Conectar a [!DNL Google]

Use essa opção para criar cenários com módulos de email que exigem uma conexão com o seu [!DNL Google] conta. Esta é uma conta com escopos restritos.

Você pode criar uma conexão com o seu [!DNL Google] diretamente de dentro de um módulo de Email.

1. Em qualquer módulo de Email, clique em **[!UICONTROL Adicionar]** ao lado da [!UICONTROL Conexão] campo.
1. Selecionar **[!DNL Google]** como o tipo de conexão.
1. Insira um nome para a conexão.
1. (Opcional) Insira seu [!UICONTROL [!DNL Google] ID do cliente] e [!UICONTROL Segredo do cliente].
1. Clique em **[!UICONTROL Continuar]** para criar a conexão e voltar ao módulo.

### Conectar-se a outros serviços de email (SMAP)

A conexão SMAP permite que você acesse sua caixa de correio remotamente e leia ou manipule mensagens em sua caixa de correio. A conexão SMAP é usada pela maioria dos módulos de email.

1. Em qualquer módulo de Email, clique em **[!UICONTROL Adicionar]** ao lado da [!UICONTROL Conexão] campo.
1. Selecionar **[!UICONTROL Outros (SMTP)]** como o tipo de conexão.
1. Insira um **[!UICONTROL Nome]** para a conexão.
1. Selecione o **[!UICONTROL Provedor de email]** da lista. Se o seu provedor de email não estiver na lista, selecione Outro.
1. Insira seu **[!UICONTROL Endereço de email]**, **[!UICONTROL Seu nome completo]**, seu **[!UICONTROL Nome do usuário]**, e seu **[!UICONTROL Senha]**.
1. (Condicional) Se seu provedor não estiver na lista, digite seu **[!UICONTROL Servidor SMTP]** e **[!UICONTROL Porta]** e especifique se deseja **[!UICONTROL Usar uma conexão segura (TLS)]**. Para encontrar essas informações, marque a opção [!UICONTROL Ajuda] seção da sua caixa de correio. Se você não tiver essas informações disponíveis, entre em contato com seu provedor de serviços de email.
1. Clique em **[!UICONTROL Continuar]** para criar a conexão e voltar ao módulo.

## [!UICONTROL E-mail] módulos e seus campos

Ao configurar [!UICONTROL E-mail] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Alguns dos campos de email podem já conter dados porque você os usou em outro módulo no cenário. Consulte a documentação de ajuda do email se precisar de informações sobre eles.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>A ID de e-mail exclusiva conhecida como &#39;[!UICONTROL ID de e-mail (UID)]&#39; é o identificador do email. A ID de e-mail é específica para cada uma das pastas de e-mail.

* [Triggers](#triggers)
* [Ações](#actions)
* [Iteradores](#iterators)

### Triggers

#### [!UICONTROL Assistir Emails]

Acionado quando um novo email é recebido para processamento de acordo com critérios especificados.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta de email ao [!UICONTROL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conectar seu email ao [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta] </td> 
   <td> <p>Selecione a pasta que contém os emails que você deseja observar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Critério]</p> </td> 
   <td> <p>Selecione os critérios pelos quais você deseja assistir aos emails:</p> 
    <ul> 
     <li>[!UICONTROL Todos os Emails]</li> 
     <li>[!UICONTROL Ler Emails Somente]</li> 
     <li>[!UICONTROL Somente Emails Não Lidos]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Endereço de Email do Remetente] </td> 
   <td> <p>Insira o endereço de email do remetente cujos emails você deseja assistir.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Endereço de Email do Destinatário]</td> 
   <td> <p> Insira o endereço de email do recipient cujos emails você deseja assistir.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assunto] </td> 
   <td> <p>Digite o assunto do email que você deseja assistir.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Frase] </td> 
   <td> <p>Insira quaisquer palavras-chave para observar apenas os emails que contêm frases específicas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Marcar mensagem(ns) como lida(s) ao buscar]</td> 
   <td> <p>Habilite esta opção para marcar o e-mail não lido como lido após recuperar os detalhes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de resultados]</td> 
   <td> <p> O número máximo de emails [!DNL Workfront Fusion] deve retornar durante um ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [[!UICONTROL Enviar um e-mail]](#send-an-email)
* [[!UICONTROL Criar um rascunho]](#create-a-draft)
* [[!UICONTROL Marcar um email como lido]](#mark-an-email-as-read)
* [[!UICONTROL Marcar um email como não lido]](#mark-an-email-as-unread)
* [[!UICONTROL Mover um email]](#move-an-email)
* [[!UICONTROL Copiar um email]](#copy-an-email)
* [[!UICONTROL Excluir um email]](#delete-an-email)
* [[!UICONTROL Receber Emails]](#get-emails)

#### [!UICONTROL Enviar um e-mail]

Envia um novo email.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta de email ao [!DNL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conectar seu email ao [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salvar Mensagem após Envio]</td> 
   <td>Depois que a mensagem de email for enviada, ela será salva na sua caixa de correio. Ative esta opção se quiser salvar e-mails enviados usando [!DNL Workfront Fusion] para o <i>[!UICONTROL Enviar email]</i> pasta ou outra pasta na sua caixa de correio. Alguns serviços de email, como [!DNL Gmail], salve as mensagens enviadas automaticamente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Para] </td> 
   <td> <p>Adicione os endereços de email para os quais deseja enviar o email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assunto] </td> 
   <td> <p>Insira ou mapeie a linha de assunto do email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de Conteúdo]</p> </td> 
   <td> <p>Selecione o tipo de conteúdo [!UICONTROL] para o email:</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL Texto sem formatação]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conteúdo] </td> 
   <td> <p>Insira ou mapeie o conteúdo do email no formato HTML usando tags HTML ou no texto sem formatação, dependendo do que você escolheu no campo [!UICONTROL Tipo de conteúdo].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Anexos]</p> </td> 
   <td> <p>Adicionar um anexo:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome do arquivo]</strong> </p> <p>Insira o nome do arquivo. Por exemplo, sample.doc.</p> </li> 
     <li> <p><strong>[!UICONTROL Dados]</strong> </p> <p>Insira o caminho para a pasta onde será feito o upload do anexo.</p> </li> 
     <li> <p><strong>[!UICONTROL ID-Conteúdo]</strong> </p> <p>Insira a [!UICONTROL ID de conteúdo] para inserir o anexo (imagem) no conteúdo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copiar Destinatário] </td> 
   <td> <p>Insira ou mapeie um ou mais endereços de email para os quais deseja enviar uma cópia deste email. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destinatário da Cópia Offline]</td> 
   <td> <p> Insira ou mapeie um ou mais endereços de email para os quais deseja enviar uma cópia deste email sem que o endereço de email apareça no email.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL De] </td> 
   <td> <p>Insira ou mapeie o endereço de email (e o nome, se necessário) que aparece no campo [!UICONTROL From] no email. </p> <p>Importante: use a sintaxe correta: <code>name@email.com</code> ou <code>"Name" name@email.com</code>.</p> <p>Observação: normalmente, [!DNL Workfront Fusion] usa o endereço de email que você inseriu ao criar a conexão como o endereço do remetente. Se você inserir qualquer outro endereço de email, poderá ocorrer um erro ao enviar uma mensagem porque sua conta talvez não tenha permissão para enviar emails de um endereço diferente do seu. Por exemplo, <code>test@mail.com</code> ou "<code>John Bush" test@email.com</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Remetente]</p> </td> 
   <td> <p>Insira ou mapeie o endereço de email que aparece no campo [!UICONTROL Remetente] no email.</p> <p>Dica: se você não tiver certeza se deve usar esse campo ou o campo De, recomendamos escolher o campo De.</p> <p>Importante: use a sintaxe correta: <code>name@email.com</code> ou <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Responder para]</td> 
   <td> <p> Se desejar que as respostas a este e-mail sejam enviadas para um endereço diferente do endereço "de", digite o endereço de e-mail para o qual deseja que as respostas a este e-mail sejam enviadas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Em Resposta]</td> 
   <td> <p> Se estiver respondendo a um email específico, insira ou mapeie a ID do email ao qual você está respondendo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Referências] </td> 
   <td> <p>Informe as IDs de mensagem de todas as respostas da thread.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prioridade]</p> </td> 
   <td> <p>Selecione a prioridade do email:</p> 
    <ul> 
     <li>[!UICONTROL Alto]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Baixo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Cabeçalhos]</p> </td> 
   <td> <p>Adicione os cabeçalhos:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Chave]</strong> </p> <p>Adicione a chave. Por exemplo, [!UICONTROL Remetente], [!UICONTROL Data], [!UICONTROL Para], e assim por diante.</p> </li> 
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
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta de email ao [!UICONTROL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conectar seu email ao [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta]</td> 
   <td>Selecione a pasta na qual deseja criar o rascunho de email.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Para] </td> 
   <td> <p>Insira ou mapeie o endereço de email para o qual deseja enviar o email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assunto] </td> 
   <td> <p>Insira ou mapeie a linha de assunto do email.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de Conteúdo]</p> </td> 
   <td> <p>Selecione o tipo de conteúdo do email:</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL Texto sem Formatação]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conteúdo] </td> 
   <td> <p>Insira ou mapeie o conteúdo do email no formato HTML usando tags HTML ou no texto sem formatação, dependendo do que você escolheu no campo [!UICONTROL Tipo de conteúdo].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Anexos]</p> </td> 
   <td> <p>Adicionar um anexo:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome do arquivo]</strong> </p> <p>Insira o nome do arquivo. Por exemplo, sample.doc.</p> </li> 
     <li> <p><strong>[!UICONTROL Dados]</strong> </p> <p>Insira o caminho para a pasta onde será feito o upload do anexo.</p> </li> 
     <li> <p><strong>[!UICONTROL ID-Conteúdo]</strong> </p> <p>Insira a ID de conteúdo para inserir o anexo (imagem) no conteúdo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copiar Destinatário] </td> 
   <td> <p>Insira ou mapeie um ou mais endereços de email para os quais deseja enviar uma cópia deste email. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destinatário da Cópia Offline]</td> 
   <td> <p> Insira ou mapeie um ou mais endereços de email para os quais deseja enviar uma cópia deste email sem que o endereço de email apareça no email.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL De] </td> 
   <td> <p>Insira ou mapeie o endereço de email (e o nome, se necessário) que aparece no campo [!UICONTROL From] no email. </p> <p>Importante: use a sintaxe correta: <code>name@email.com</code> ou <code>"Name" name@email.com</code>.</p> <p>Observação: normalmente, [!DNL Workfront Fusion] usa o endereço de email que você inseriu ao criar a conexão como o endereço do remetente. Se você inserir qualquer outro endereço de email, poderá ocorrer um erro ao enviar uma mensagem porque sua conta talvez não tenha permissão para enviar emails de um endereço diferente do seu. Por exemplo, <code>test@mail.com</code> ou "<code>John Bush" test@email.com</code>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Remetente]</p> </td> 
   <td> <p>Insira ou mapeie o endereço de email que aparece no campo [!UICONTROL Remetente] no email.</p> <p>Dica: se você não tiver certeza se deve usar esse campo ou o campo De, recomendamos escolher o campo De.</p> <p>Importante: use a sintaxe correta: <code>name@email.com</code> ou <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Responder para]</td> 
   <td> <p> Se desejar que respostas a este email sejam enviadas para um endereço diferente do endereço "[!UICONTROL from]", digite o endereço de email para o qual deseja que respostas a este email sejam enviadas.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Em Resposta]</td> 
   <td> <p> Se estiver respondendo a um email específico, insira ou mapeie a ID do email ao qual você está respondendo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Referências] </td> 
   <td> <p>Informe as IDs de mensagem de todas as respostas da thread.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Prioridade]</p> </td> 
   <td> <p>Selecione a prioridade do email:</p> 
    <ul> 
     <li>[!UICONTROL Alto]</li> 
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

Marca um email ou rascunho em uma pasta selecionada como lido ao configurar o [!UICONTROL Ler] sinalizador.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta de email ao [!UICONTROL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conectar seu email ao [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta]</td> 
   <td>Selecione a pasta do email que deseja marcar como lido. Exemplo: Principal.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID DE E-MAIL (UID)]</p> </td> 
   <td> <p>Insira a UID de e-mail do e-mail que deseja marcar como lido.</p> <p>É possível obter a UID do email usando o módulo [!UICONTROL Email] &gt;[!UICONTROL Assistir Email] ou o módulo [!UICONTROL Pesquisar Email].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Marcar um email como não lido]

Marca um email ou rascunho em uma pasta selecionada como não lido ao configurar o sinalizador Não lido.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta de email ao [!UICONTROL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conectar seu email ao [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta]</td> 
   <td>Selecione a pasta do email que deseja marcar como não lido. Exemplo: Principal.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID DE E-MAIL (UID)]</p> </td> 
   <td> <p>Insira a UID de e-mail do e-mail que você deseja marcar como não lido.</p> <p>É possível obter a UID do email usando o módulo [!UICONTROL Email] &gt;[!UICONTROL Assistir Email] ou o módulo [!UICONTROL Pesquisar Email].</p> </td> 
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
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta de email ao [!UICONTROL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conectar seu email ao [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta de Origem]</td> 
   <td>Selecione a pasta que contém o email a partir da qual deseja mover o email. Exemplo: Principal.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta de Destino]</td> 
   <td> <p> Selecione a pasta à qual deseja adicionar o email. Exemplo: Trabalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID DE E-MAIL (UID)]</p> </td> 
   <td> <p>Insira a UID de email do email que você deseja mover para a pasta de destino.</p> <p>É possível obter a UID do email usando o módulo [!UICONTROL Email] &gt;[!UICONTROL Assistir Email] ou o módulo [!UICONTROL Pesquisar Email].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiar um email]

Copia um email ou um rascunho para uma pasta selecionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta de email ao [!UICONTROL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conectar seu email ao [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta de Origem]</td> 
   <td>Selecione a pasta da qual deseja copiar o email. Exemplo: Principal.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta de Destino]</td> 
   <td> <p> Selecione a pasta para a qual deseja copiar o email. Exemplo: Trabalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID DE E-MAIL (UID)]</p> </td> 
   <td> <p>Insira a UID de email do email que você deseja copiar para a pasta de destino.</p> <p>É possível obter a UID do email usando o módulo [!UICONTROL Email] &gt;[!UICONTROL Assistir Email] ou o módulo [!UICONTROL Pesquisar Email].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir um email]

Remove um email ou um rascunho da pasta selecionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta de email ao [!UICONTROL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conectar seu email ao [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta]</td> 
   <td>Selecione a pasta do email que deseja excluir. Exemplo: Principal.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID DE E-MAIL (UID)]</p> </td> 
   <td> <p>Insira a UID de e-mail do e-mail que deseja excluir.</p> <p>É possível obter a UID do email usando o módulo [!UICONTROL Email] &gt;[!UICONTROL Assistir Email] ou o módulo [!UICONTROL Pesquisar Email].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eliminar]</td> 
   <td> <p>Habilite esta opção para permitir que o módulo remova permanentemente todas as mensagens sinalizadas como [!UICONTROL Excluído] na caixa de correio atualmente aberta.</p> <p>Observação: em [!DNL Gmail], esse comportamento é conduzido pela configuração na seção [!UICONTROL Configurações] &gt;[!UICONTROL Encaminhando POP/IMAP no acesso IMAP].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Receber Emails]

Retorna emails que correspondem aos critérios especificados.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta de email ao [!UICONTROL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conectar seu email ao [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta] </td> 
   <td> <p>Selecione a pasta que contém os emails que deseja recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Marcar mensagem(ns) como lida(s) ao buscar] </td> 
   <td> <p>Ative esta opção se quiser marcar o e-mail não lido como lido após recuperar os detalhes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Critério]</p> </td> 
   <td> <p>Selecione os critérios dos emails que deseja recuperar:</p> 
    <ul> 
     <li>[!UICONTROL Todos os Emails]</li> 
     <li>[!UICONTROL Ler Emails Somente]</li> 
     <li>[!UICONTROL Somente Emails Não Lidos]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Endereço de Email do Remetente] </td> 
   <td> <p>Insira ou mapeie o endereço de email do remetente cujos emails você deseja recuperar.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Endereço de Email do Destinatário]</td> 
   <td> <p> Insira ou mapeie o endereço de email do recipient cujos emails você deseja recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Da data] </td> 
   <td> <p>Insira ou mapeie a data para recuperar os emails processados na data especificada ou após essa data.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Antes da data]</td> 
   <td> <p> Insira ou mapeie a data para recuperar os emails processados na data especificada ou antes dela.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assunto] </td> 
   <td> <p>Insira ou mapeie o assunto do email que você deseja recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Frase] </td> 
   <td> <p>Insira ou mapeie quaisquer palavras-chave para recuperar apenas os emails que contêm frases específicas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID DE E-MAIL (UID)]</td> 
   <td> <p> Insira a ID de email (UID) do email cujos detalhes você deseja recuperar.</p> <p>É possível obter a UID do email usando [!DNL Workfront Fusion]Módulo do [!UICONTROL Watch Email] ou do [!UICONTROL Search Email].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de resultados]</td> 
   <td> <p> O número máximo de emails [!DNL Workfront Fusion] deve retornar durante um ciclo de execução de cenário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Continuar a execução da rota mesmo se o módulo não retornar resultados]</td> 
   <td> <p> Selecione se deseja continuar a executar o módulo mesmo se não houver resultados retornados.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Iteradores

#### [!UICONTROL Anexos iterados]

Repete os anexos recebidos um por um.

O módulo iterador de email permite gerenciar anexos de email separadamente. Por exemplo, você pode configurar o para observar emails e iterar os emails com anexos e receber alertas.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Módulo de origem]</td> 
   <td> <p>Selecione o módulo que gera o email com os anexos através dos quais você deseja iterar.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais informações sobre iteradores, consulte [Módulo Iterador em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
