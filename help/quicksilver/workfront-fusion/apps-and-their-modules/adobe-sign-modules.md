---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos Adobe Acrobat Sign
description: Com o [!DNL Adobe Acrobat Sign] módulos, você pode iniciar um [!DNL Adobe Workfront Fusion] com base nos eventos em seu [!DNL Adobe] Conta Acrobat Sign, crie, leia ou atualize contratos e outros registros, pesquise registros usando critérios definidos e carregue documentos.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 01158218-31a6-4c68-a9b7-6a678a8f40c9
source-git-commit: 8bb97b08bb5991fadbf2627f4ebfdaa25ae337ce
workflow-type: tm+mt
source-wordcount: '6579'
ht-degree: 0%

---

# [!DNL Adobe Acrobat Sign] módulos

Com o [!DNL Adobe Acrobat Sign] módulos, você pode iniciar um [!DNL Adobe Workfront Fusion] com base nos eventos em seu [!DNL Adobe Acrobat Sign] contas, criar, ler ou atualizar contratos e outros registros, procurar registros usando critérios definidos e carregar documentos.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Adobe Acrobat Sign] recomendações de uso do conector

O [!DNL Adobe Sign ]O aplicativo automatiza processos de negócios de assinatura eletrônica no [!DNL Fusion] muito mais fácil e poderoso.

Novos usuários para [!DNL Adobe Sign] devem estar muito atentos a algumas das limitações em matéria de atualização dos acordos. Os contratos normalmente não são alterados depois de iniciados. Recomendamos que novos usuários do [!DNL Adobe Sign] concentre-se na criação de novos contratos usando o módulo de criação de contratos. Isso fará com que [!DNL Fusion] automações mais fáceis e funcionam melhor com [!DNL Adobe Sign].

[!DNL Adobe Sign] os acordos precisam de um campo de trabalho. Há algumas opções para fazer isso, mas a mais fácil e comum é fazer o upload de um documento transitório e, em seguida, mapear esse documento para o seu contrato.

![](assets/adobe-sign-recommendations-350x168.png)

## [!DNL Adobe Acrobat Sign] módulos e seus campos

Ao configurar [!DNL Adobe Acrobat Sign] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Adobe Acrobat Sign] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Ações](#actions)
* [Pesquisas](#searches)

### Triggers

<!--
* [Watch for agreements](#watch-for-agreements) 
* [Watch for events](#watch-for-events)
-->

+++ **[!UICONTROL Assista aos contratos]**

Este módulo de acionador inicia um cenário quando um contrato é criado ou atualizado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
<td>Para obter instruções sobre como conectar seu [!DNL Adobe Acrobat Sign] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></td>  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td>Selecione se deseja procurar novos registros, registros atualizados ou ambos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro] </td> 
   <td>Selecione o tipo de registro que deseja que o registro assista.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Localizar texto]</td> 
   <td> <p>Insira os termos que deseja pesquisar. O módulo retorna registros que incluem esses termos como valores de campo.</p> <p>Para obter mais informações sobre como pesquisar campos em [!DNL Adobe Acrobat Sign], consulte "Como funciona a pesquisa de texto" em <a href="https://helpx.adobe.com/sign/using/adobesign-search-users-agreements.html#HowSearchWorks">Pesquisa do Adobe Sign - Como funciona</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de contratos retornados]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Monitoramento de eventos]**

Esse módulo de acionador inicia um cenário quando ocorre um evento selecionado por você.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td>Selecione o webhook que deseja usar ou clique em <b>[!UICONTROL Adicionar]</b> e preencha os seguintes campos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do Webhook]</td> 
   <td> <p>Digite um nome para o webhook</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Adobe Acrobat Sign] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escopos]</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Conta]</p> </li> 
     <li> <p>[!UICONTROL Grupo]</p> </li> 
     <li> <p>[!UICONTROL Usuário]</p> </li> 
     <li> <p>[!UICONTROL Recurso]</p> <p>Se você selecionar [!UICONTROL Recurso], insira o ID do recurso e o tipo de recurso.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nível de recurso]</td> 
   <td> <p>Selecione o tipo de recurso que deseja observar.</p> 
    <ul> 
     <li> <p>[!UICONTROL Contratos]</p> </li> 
     <li> <p>[!UICONTROL Widgets]</p> </li> 
     <li> <p>[!UICONTROL Megasigns]</p> </li> 
     <li> <p>[!UICONTROL Documentos da biblioteca]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eventos de assinatura do Webhook]</td> 
   <td>Selecione o [!DNL Adobe Sign] eventos que você deseja que o módulo assista.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Application display name]</td> 
   <td>O nome de exibição do aplicativo pelo qual o webhook é criado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Application name]</td> 
   <td>O nome de exibição do aplicativo pelo qual o webhook é criado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Emails de notificação de problema]</td> 
   <td> <p>Essa configuração funciona somente para contas de administrador</p> <p>Para cada endereço de email para o qual você deseja enviar emails de notificação de problemas, clique em <b>[!UICONTROL Adicionar]</b> e insira o endereço de email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parâmetros condicionais do Contrato]</td> 
   <td>Se quiser adicionar parâmetros condicionais, selecione <b>[!UICONTROL Sim]</b> no tipo de registro ao qual você deseja adicionar parâmetros, selecione <b>[!UICONTROL Sim]</b> em qualquer parâmetro que você deseja ativar.</td> 
  </tr> 
 </tbody> 
</table>

+++

### Ações

<!--
* [Create a record](#create-a-record) 
* [Create an agreement](#create-an-agreement) 
* [Create related records](#create-related-records) 
* [Custom API Call](#custom-api-call) 
* [List records](#list-records) 
* [Read a record](#read-a-record) 
* [Read related records](#read-related-records) 
* [Update a record](#update-a-record) 
* [Update related record](#update-related-record) 
* [Upload document](#upload-document)
-->

+++ **[!UICONTROL Criar um registro]**

Este módulo de ação cria um novo registro do tipo selecionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obter instruções sobre como conectar seu [!DNL Adobe Acrobat Sign] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão. Por exemplo, <code>{"Content-type":"application/json"}</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione o tipo de registro que deseja criar.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Grupo]</b> </p> </li> 
     <li> <p><b>[!UICONTROL Biblioteca document]</b> </p> </li> 
     <li> <p><b>[!UICONTROL Usuário]</b> </p> </li> 
     <li> <p><b>[!UICONTROL Web form] ([!UICONTROL Widget])</b> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Informações do grupo]</td> 
   <td> <p>Insira ou mapeie o [!UICONTROL Name] e a [!UICONTROL ID] do grupo e indique se esse grupo é o grupo padrão da conta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Library document info]</td> 
   <td> <p>Preencha os seguintes campos:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Arquivos para enviar]</b> </p> <p>Para cada arquivo que deseja adicionar, clique em <b>[!UICONTROL Adicionar item]</b> e preencha os campos.</p> 
      <ul> 
       <li><b>[!UICONTROL ID de documento transitório]</b> <p>Insira a ID do documento transitório</p> </li> 
       <li> <p><b>[!UICONTROL Transferência de arquivo da URL]</b> </p> <p>Preencha os seguintes campos:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Mime-Type]</b> </p> <p>Insira o tipo mime do arquivo original. Os tipos MIME (Multipurpose Internet Mail Extension) são rótulos que permitem ao software identificar diferentes tipos de dados compartilhados na Internet. Os servidores e navegadores da Web usam o tipo MIME para determinar o que deve ser feito com um arquivo. Por exemplo, um arquivo com o tipo MIME <code>text/html</code> será processado em um navegador de forma diferente de um arquivo com o tipo MIME <code>image/jpeg</code>.</p> </li> 
         <li> <p><b>[!UICONTROL Name]</b> </p> <p>Insira um nome para o arquivo.</p> </li> 
         <li> <p><b>[!UICONTROL URL]</b> </p> <p>Insira o URL do arquivo que deseja enviar.</p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL Notarize]</b> </p> <p>Selecione se este documento precisa ser notalizado.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Nome do modelo da biblioteca]</b> </p> <p>Insira ou mapeie o nome do template de biblioteca</p> </li> 
     <li> <p><b>[!UICONTROL Modo de compartilhamento]</b> </p> <p>Especifique quem deve ter acesso ao documento da biblioteca.</p> </li> 
     <li> <p><b>[!UICONTROL Estado do documento da biblioteca]</b> </p> <p>Selecione se o documento está no estado de criação ou ativo.</p> </li> 
     <li> <p><b>[!UICONTROL Tipo de modelo da biblioteca]</b> </p> <p>Para cada tipo de modelo de biblioteca que deseja usar, clique em <b>[!UICONTROL Adicionar item]</b> e selecione o tipo de modelo.</p> </li> 
     <li> <p><b>[!UICONTROL Data do último evento]</b> </p> <p>Insira a última data em que um evento ocorreu no documento da biblioteca.</p> <p>Para obter uma lista de formatos de data e hora compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coação de tipo em [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
     <li> <p><b>[!UICONTROL Status do documento da biblioteca]</b> </p> <p>Selecione o status do documento da biblioteca.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Informações do usuário]</td> 
   <td> <p>Preencha os seguintes campos:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Email]</b> </p> <p>Insira o endereço de email do usuário.</p> </li> 
     <li> <p><b>[!UICONTROL É administrador da conta]</b> </p> <p>Marque essa opção se o usuário criado for um administrador de conta.</p> </li> 
     <li> <p><b>[!UICONTROL ID do usuário]</b> </p> <p>Insira a ID exclusiva do usuário</p> </li> 
     <li> <p><b>[!UICONTROL ID da conta]</b> </p> <p>Insira a ID exclusiva do [!DNL Adobe Acrobat Sign] conta associada a este usuário.</p> </li> 
     <li> <p><b>[!UICONTROL Nome]</b> </p> <p>Insira o nome do usuário.</p> </li> 
     <li> <p><b>[!UICONTROL Sobrenome]</b> </p> <p>Digite o sobrenome do usuário</p> </li> 
     <li> <p><b>[!UICONTROL Company]</b> </p> <p>Insira o nome da empresa do usuário.</p> </li> 
     <li> <p><b>[!UICONTROL Iniciais]</b> </p> <p>Insira as iniciais do usuário.</p> </li> 
     <li> <p><b>[!UICONTROL Locale]</b> </p> <p>Insira a localidade do usuário. Isso determina o idioma da interface do usuário. </p> </li> 
     <li> <p><b>[!UICONTROL Telefone]</b> </p> <p>Digite o número de telefone do usuário</p> </li> 
     <li> <p><b>ID do grupo principal</b> </p> <p>Insira o grupo ao qual o novo usuário é adicionado. Se nada for inserido, o usuário será adicionado ao grupo padrão da conta.</p> </li> 
     <li> <p><b>[!UICONTROL Cargo title]</b> </p> <p>Insira o cargo do usuário.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Informações do formulário web]</td> 
   <td> <p>Preencha os seguintes campos</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Informações do arquivo]</b> </p> <p>Para cada arquivo que deseja adicionar ao formulário web, clique em Add e preencha os seguintes campos:</p> 
      <ul> 
       <li> <p>[!UICONTROL Tipo de arquivo]</p> <p>[!UICONTROL Documento]</p> </li> 
       <li> <p>[!UICONTROL Documento transitório]</p> </li> 
       <li> <p>[!UICONTROL URL file info]</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Nome do formulário web]</b> </p> <p>Insira um nome para o formulário web. Esse nome é usado para identificar o formulário da Web em locais como emails e sites.</p> </li> 
     <li> <p><b>[!UICONTROL Estado do formulário web]</b> </p> <p>Selecione o estado em que o novo formulário web deve ser criado.</p> </li> 
     <li> <p><b>[!UICONTROL Informações do conjunto de participantes do formulário web]</b> </p> 
      <ul> 
       <li> <p><b>[!UICONTROL Informações do membro]</b> </p> <p>Para cada membro que deseja adicionar ao conjunto de participantes, clique em <b>[!UICONTROL Adicionar item]</b>. </p> 
        <ul> 
         <li> <p><b>[!UICONTROL Email]</b> </p> <p>Deixe essa opção em branco.</p> </li> 
         <li> <p><b>[!UICONTROL Opção Segurança]</b> </p> <p>Se quiser adicionar uma opção de segurança para autenticar este usuário, selecione <b>[!UICONTROL Sim]</b>, selecione a opção de segurança e preencha todos os campos necessários.</p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL Função]</b> </p> <p>Selecione a função. Todos os membros deste conjunto de participantes compartilham a função.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Formulário web de participante adicional define informações]</b> </p> 
      <ul> 
       <li> <p><b>[!UICONTROL Informações do membro]</b> </p> <p>Para cada membro que deseja adicionar ao conjunto de participantes, clique em <b>[!UICONTROL Adicionar item]</b>.</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Email]</b> </p> <p>Deixe essa opção em branco.</p> </li> 
         <li> <p><b>[!UICONTROL Opção Segurança]</b> </p> <p>Se quiser adicionar uma opção de segurança para autenticar este usuário, selecione <b>[!UICONTROL Sim]</b>, selecione a opção de segurança e preencha todos os campos necessários.</p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL Função]</b> </p> </li> 
       <li> <p><b>[!UICONTROL ID do participante do formulário web] </b> </p> <p>Insira a ID do participante do formulário web.</p> </li> 
       <li> <p><b>[!UICONTROL Order]</b> </p> <p>Especifique a ordem de quando esse conjunto de participantes deve interagir com o formulário web. Por exemplo, o grupo de participantes que tem o valor de pedido 1 deve ir primeiro, 2 deve ir em seguida e assim por diante. Os números de ordem devem começar com um e não ter lacunas na série. </p> </li> 
       <li> <p><b>[!UICONTROL Provedor de informações do conjunto de participantes]</b> </p> <p>Se o participante for desconhecido, indique se o fornecedor deve fornecer detalhes ao participante e insira uma mensagem com os detalhes necessários para o participante desconhecido.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Informações de falha de autenticação]</b> </p> <p>Se desejar fornecer uma página de erro ou falha para seus usuários, selecione <b>[!UICONTROL Sim]</b>e preencha os seguintes campos:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL URL]</b> </p> <p>Insira o URL da página de erro</p> </li> 
       <li> <p><b>[!UICONTROL Deframe]</b> </p> <p>Ative essa opção se desejar que a página de erro apareça dentro do formulário web</p> </li> 
       <li> <p><b>[!UICONTROL Atraso]</b> </p> <p>Insira o atraso, em segundos, antes que o usuário seja redirecionado para a página de erro.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL CC info]</b> </p> <p>Para cada endereço de email que você deseja receber um email quando o contrato final no formulário web for assinado, clique em <b>[!UICONTROL Adicionar item]</b> e insira o endereço de email.</p> </li> 
     <li> <p><b>[!UICONTROL Informações de conclusão]</b> </p> <p style="font-style: normal;">Se desejar fornecer uma página de sucesso para seus usuários, selecione <b>[!UICONTROL Sim]</b>e preencha os seguintes campos:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL URL]</b> </p> <p>Insira o URL da página de sucesso</p> </li> 
       <li> <p><b>[!UICONTROL Deframe]</b> </p> <p>Ative essa opção se desejar que a página de sucesso apareça dentro do formulário web</p> </li> 
       <li> <p><b>[!UICONTROL Atraso]</b> </p> <p>Insira o atraso, em segundos, antes que o usuário seja redirecionado para a página de sucesso.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL ID do grupo]</b> </p> <p>Insira a ID do grupo ao qual o formulário web pertence. Se nada for inserido, o formulário web pertencerá ao grupo principal do usuário da conta.</p> </li> 
     <li> <p><b>[!UICONTROL Data do último evento]</b> </p> <p>Insira a data em que o último evento ocorreu no formulário web. Usar o formato <code>yyyy-MM-dd'T'HH:mm:ssZ</code>.</p> </li> 
     <li> <p><b>[!UICONTROL Locale]</b> </p> <p>Insira a localidade do usuário. Isso determina o idioma da interface do usuário. </p> </li> 
     <li> <p><b>[!UICONTROL Segurança opção]n</b> </p> <p>Digite a senha usada para proteger o documento. Você deve comunicar essa senha separadamente a qualquer parte relevante.</p> </li> 
     <li> <p><b>[!UICONTROL Informações de compartimentalização]</b> </p> <p>Se sua conta estiver configurada para a compartimentalização de documentos e a opção para habilitar por contrato, você poderá habilitar essa opção para cofre neste contrato.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Criar um contrato]**

Esse módulo de ação cria um contrato, o envia para assinatura e retorna a ID do contrato.

>[!NOTE]
>
>Recomendamos fazer upload do documento para assinar como um documento transitório e, em seguida, mapeá-lo para a [!UICONTROL Arquivo para enviar] no campo [!UICONTROL Criar um contrato] módulo. Para obter um exemplo, consulte &quot;Carregar documento&quot; neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
<td>Para obter instruções sobre como conectar seu [!DNL Adobe Acrobat Sign] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></td>  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão. Por exemplo, <code>{"Content-type":"application/json"}</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivos para enviar]</td> 
   <td> <p>Para cada item que você deseja incluir no contrato, clique em <b>[!UICONTROL Adicionar item]</b> e preencha os seguintes campos:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Tipo de arquivo]</b> </p> 
      <ul> 
       <li> <p><b>[!UICONTROL Documento]</b> </p> <p>Preencha os seguintes campos:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Data de criação]</b> </p> <p>Inserir ou mapear a data em que o documento foi criado no formato <code>yyyy-MM-dd'T'HH:mm:ssZ</code>. Por exemplo, <code>2016-02-25T18:46:19Z</code> representa a hora UTC.</p> </li> 
         <li> <p><b>[!UICONTROL ID]</b> </p> <p>Insira ou mapeie a ID do documento.</p> </li> 
         <li> <p><b>[!UICONTROL Rótulo]</b> </p> <p>Insira ou mapeie um rótulo exclusivo para o arquivo. No caso de fluxo de trabalho personalizado, esse mapeará um arquivo para o elemento de arquivo correspondente na definição do fluxo de trabalho. Isso deve ser especificado no caso de solicitação de criação de contrato de fluxo de trabalho personalizado.</p> </li> 
         <li> <p><b>[!UICONTROL Número de páginas]</b> </p> <p>Insira ou mapeie o número de páginas no documento.</p> </li> 
         <li> <p><b>[!UICONTROL Mime-Type]</b> </p> <p>Insira ou mapeie o tipo mime do arquivo original. Os tipos MIME (Multipurpose Internet Mail Extension) são rótulos que permitem ao software identificar diferentes tipos de dados compartilhados na Internet. Os servidores e navegadores da Web usam o tipo MIME para determinar o que deve ser feito com um arquivo. Por exemplo, um arquivo com o tipo MIME <code>text/html</code> será processado em um navegador de forma diferente de um arquivo com o tipo MIME <code>image/jpeg</code>.</p> </li> 
         <li> <p><b>[!UICONTROL Name]</b> </p> <p>Insira ou mapeie um nome para o documento.<br></p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL ID do documento da biblioteca]</b> </p> <p>Insira a ID do documento da biblioteca</p> </li> 
       <li> <p><b>[!UICONTROL ID de documento transitório]</b> </p> <p>Insira a ID do documento transitório</p> </li> 
       <li> <p><b>[!UICONTROL Transferência de arquivo da URL]</b> </p> <p>Preencha os seguintes campos:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Mime-Type]</b> </p> <p>Insira o tipo mime do arquivo original. Os tipos MIME (Multipurpose Internet Mail Extension) são rótulos que permitem ao software identificar diferentes tipos de dados compartilhados na Internet. Os servidores e navegadores da Web usam o tipo MIME para determinar o que deve ser feito com um arquivo. Por exemplo, um arquivo com o tipo MIME <code>text/html</code> será processado em um navegador de forma diferente de um arquivo com o tipo MIME <code>image/jpeg</code>.</p> </li> 
         <li> <p><b>[!UICONTROL Name]</b> </p> <p>Insira um nome para o arquivo.</p> </li> 
         <li> <p><b>[!UICONTROL URL]</b> </p> <p>Insira o URL do arquivo que deseja enviar.</p> </li> 
        </ul> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Rótulo]</b> </p> <p>Insira um rótulo para o arquivo.</p> </li> 
     <li> <p><b>[!UICONTROL Notarize]</b> </p> <p>Habilite esta opção para indicar que o arquivo deve ser notalizado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do contrato]</td> 
   <td>Informe um nome para o novo contrato. Esse nome é usado para identificar o contrato em locais como emails e sites.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Participante define informações]</td> 
   <td> <p>Para cada conjunto de participantes que deseja adicionar, clique em <b>[!UICONTROL Adicionar item]</b> e preencha os seguintes campos.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Membros]</b> </p> <p>Para cada pessoa que deseja adicionar ao conjunto de participantes, clique em <b>[!UICONTROL Adicionar item]</b> e insira o endereço de email da pessoa.</p> </li> 
     <li> <p><b>[!UICONTROL Order]</b> </p> <p>Especifique a ordem de quando este conjunto de participantes deverá assinar o contrato. Por exemplo, o grupo de participantes que tem o valor de ordem 1 deve assinar primeiro, 2 deve assinar depois e assim por diante. Os números de ordem devem começar com um e não ter lacunas na série. </p> </li> 
     <li> <p><b>[!UICONTROL Função]</b> </p> <p>Selecione uma função para este conjunto de participantes. Todos os participantes no conjunto recebem essa função.</p> </li> 
     <li> <p><b>[!UICONTROL ID]</b> </p> <p>Insira ou mapeie a ID desse conjunto de participantes.</p> </li> 
     <li> <p><b>[!UICONTROL Rótulo]</b> </p> <p>Insira ou mapeie um rótulo exclusivo para o conjunto de participantes. Para fluxos de trabalho personalizados, o rótulo especificado no conjunto de participação deve mapeá-lo para a etapa de participação no fluxo de trabalho personalizado.</p> </li> 
     <li> <p><b>[!UICONTROL Name]</b> </p> <p>Digite um nome para o conjunto de participantes. Esse nome deve ser exclusivo no contrato.</p> </li> 
     <li> <p><b>[!UICONTROL Mensagem privada]</b> </p> <p>Insira ou mapeie uma mensagem para este conjunto de participantes. Todos os participantes no conjunto receberão esta mensagem.</p> </li> 
     <li> <p><b>[!UICONTROL Páginas visíveis]</b> </p> <p>Se a visibilidade limitada do documento estiver ativada para este contrato, especifique quais arquivos estarão visíveis para este conjunto de participantes. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de assinatura]</td> 
   <td> <p>Selecione o tipo de assinatura que o contrato requer.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL E-sign]</b> </p> <p>O acordo deve ser assinado eletronicamente.</p> </li> 
     <li> <p><b>[!UICONTROL Gravado]</b> </p> <p>O contrato deve ser assinado manualmente e o contrato assinado deve ser digitalizado e carregado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Estado]</td> 
   <td> <p>Selecione um estado para este contrato.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Criação]</b> </p> <p>Ainda é possível editar ou adicionar campos a este contrato.</p> </li> 
     <li> <p><b>[!UICONTROL Rascunho]</b> </p> <p>Você pode criar este contrato incrementalmente antes de enviá-lo.</p> </li> 
     <li> <p><b>[!UICONTROL Em Andamento]</b> </p> <p>Este contrato será enviado imediatamente.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CCs]</td> 
   <td> <p>Você pode enviar este contrato para partes interessadas que não precisam assinar, como participantes. Eles recebem um email no início do processo de assinatura e outro quando a assinatura final é recebida. Eles também recebem uma PDF do contrato. </p> <p>Para cada pessoa que você deseja CC sobre este contrato, clique em <b>[!UICONTROL Adicionar item]</b> e preencha os seguintes campos:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Email]</b> </p> <p>Insira ou mapeie o endereço de email que deseja CC no contrato.</p> </li> 
     <li> <p><b>[!UICONTROL Rótulo]</b> </p> <p>Insira ou mapeie um rótulo para este endereço de email, como visto na descrição do workflow</p> </li> 
     <li> <p><b>[!UICONTROL Páginas visíveis]</b> </p> </li> 
     <li> <p>Se a visibilidade limitada do documento estiver ativada para este contrato, especifique quais arquivos estarão visíveis para este conjunto de participantes. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Opção Email]</td> 
   <td> <p>Para cada tipo de email, selecione se esse tipo de email é enviado para todos os participantes ou nenhum.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Finalizar emails]</b> </p> <p>Envie um email quando este contrato for concluído, cancelado, expirado ou rejeitado.</p> </li> 
     <li> <p><b>[!UICONTROL Emails in-flight]</b> </p> <p>Enviado um email quando este contrato é delegado ou substituído.</p> </li> 
     <li> <p><b>[!UICONTROL Envio de emails de iniciação do Contrato]</b> </p> <p>Envie um email quando este contrato for criado ou quando uma ação nele for solicitada.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID Externa]</td> 
   <td> <p>Insira ou mapeie uma ID para este contrato. Você pode especificar isso quando o contrato for criado e usá-lo para localizar o contrato em módulos ou consultas posteriores.</p> <p>Observação: O valor da ID externa é visível para todos os participantes por meio da API, portanto, não deve ser usado para conter um token sensível.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mesclar informações do campo]</td> 
   <td> <p>Para cada campo no contrato para o qual você deseja colocar um valor padrão, clique em <b>[!UICONTROL Adicionar item]</b> e insira o valor padrão e o nome do campo.</p> <p>Os valores serão apresentados aos signatários para campos editáveis Para campos somente leitura, os valores fornecidos não serão editáveis durante o processo de assinatura.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Informações notórias]</td> 
   <td> <p>Preencha os seguintes campos:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Compromisso]</b> </p> <p>Insira ou mapeie a hora e a data propostas para o compromisso para notificar este contrato.</p> </li> 
     <li> <p><b>[!UICONTROL Nota]</b> </p> <p>Insira ou mapeie as observações que deseja incluir sobre a sessão notária.</p> </li> 
     <li> <p><b>[!UICONTROL Pagamento]</b> </p> <p>Selecione se o notário é pago pelo assinante ou pelo remetente do contrato.</p> </li> 
     <li> <p><b>[!UICONTROL Tipo de notário]</b> </p> <p>Selecione o tipo de notário</p> 
      <ul> 
       <li> <p>[!UICONTROL Provedor notary]</p> <p>O notário é fornecido pelo notário.</p> </li> 
       <li> <p>[!UICONTROL BYON notary]</p> <p>O notário é fornecido pelo cliente.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Opção de sinal de postagem]</td> 
   <td> <p>Selecione se deseja que os signatários sejam direcionados a uma página de sucesso após a assinatura do contrato. Se você selecionar <b>[!UICONTROL Sim]</b>, preencha os seguintes campos:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Redirect delay]</b> </p> <p>Insira ou mapeie um número que representa o número de segundos antes do assinante ser redirecionado para a página de sucesso. Se esse valor for maior que 0, o usuário primeiro verá o padrão [!DNL Adobe Sign] mensagem de sucesso e depois de um atraso será redirecionado para a página de sucesso.</p> </li> 
     <li> <p><b>[!UICONTROL Redirecionar URL]</b> </p> <p>Insira ou mapeie um URL acessível publicamente para o qual o usuário será enviado após concluir com sucesso o processo de assinatura.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Opção Segurança]</td> 
   <td> <p>Insira ou mapeie a senha secundária que será usada para proteger o documento PDF. </p> <p>Importante: [!DNL Adobe Sign] O nunca compartilhará essa senha, portanto, você deve comunicá-la separadamente a qualquer parte relevante.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Informações de compartimentalização]</td> 
   <td>Se sua conta estiver configurada para a compartimentalização de documentos e a opção para habilitar por contrato, você poderá habilitar essa opção para cofre neste contrato.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Criar registros relacionados]**

Esse módulo de ação cria registros vinculados a um módulo selecionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Adobe Acrobat Sign] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] adiciona cabeçalhos de autorização automaticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Selecione o tipo de registro do registro original ao qual deseja associar os registros criados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Agreement]/[!UICONTROL Library document]/[!UICONTROL User]/[!UICONTROL Widget ID]</td> 
   <td>Insira ou mapeie a ID do objeto ao qual você deseja associar o registro criado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campo relacionado do contrato]</td> 
   <td> <p>Selecione o tipo de campo relacionado que deseja criar</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Campos de formulário]</b> </p> <p>Insira a ID do modelo que contém os campos que você deseja criar</p> </li> 
     <li> <p><b>[!UICONTROL Lembretes]</b> </p> <p>Preencha os seguintes campos:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL ID do participante do destinatário]</b> </p> <p>Para cada participante que você deseja receber um lembrete, clique em [!UICONTROL Adicionar item] e insira a ID do participante.</p> </li> 
       <li> <p><b>[!UICONTROL Status]</b> </p> <p>Para novos registros, o status deve ser [!UICONTROL Ativo].</p> </li> 
       <li> <p><b>[!UICONTROL Primeiro atraso de lembrete]</b> </p> <p>Insira o atraso em horas antes de enviar o primeiro lembrete. O valor mínimo permitido é de 1 hora e o valor máximo não pode ser maior que a diferença na criação do acordo e no tempo de expiração do acordo em horas. Se esse atraso não for definido, o primeiro lembrete será baseado na frequência.</p> </li> 
       <li> <p><b>[!UICONTROL Frequência do lembrete]</b> </p> <p>Defina a frequência na qual deseja que o lembrete seja enviado. Se a frequência não for fornecida, o lembrete será enviado uma vez.</p> </li> 
       <li> <p><b>[!UICONTROL Última data de envio]</b> </p> <p>Este campo é definido pelo sistema.</p> </li> 
       <li> <p><b>[!UICONTROL Próxima data de envio]</b> </p> <p>Este campo deve estar em branco ou definido como [!UICONTROL UMA VEZ].</p> </li> 
       <li> <p><b>[!UICONTROL Nota]</b> </p> <p>Insira uma nota a ser incluída com o lembrete. Isso é útil para informar ao participante por que sua participação é necessária.</p> </li> 
       <li> <p><b>[!UICONTROL Iniciar contador de lembretes de]</b> </p> <p>Selecione se o lembrete é enviado com base em quando o contrato é criado em quando ele fica disponível.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Relatório de identidade do assinante]</b> </p> <p>Digite a senha usada para proteger o documento PDF.</p> </li> 
     <li> <p><b>[!UICONTROL Exibições]</b> </p> <p>Insira os seguintes campos</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Name]</b> </p> <p>Selecione o nome da exibição que deseja criar.</p> </li> 
       <li> <p><b>[!UICONTROL Usuário de logon automático]</b> </p> <p>Selecionar <b>[!UICONTROL Sim]</b> para fazer logon automático no URL retornado.</p> </li> 
       <li> <p><b>[!UICONTROL Quadro pai]</b> </p> <p>Insira ou mapeie uma lista separada por vírgulas de URLs de domínio pai, onde os URLs retornados podem ser enquadrados. Se deixado em branco, a variável [!DNL Adobe Acrobat Sign] as páginas não são visualizadas no iframe.</p> </li> 
       <li> <p><b>[!UICONTROL Locale]</b> </p> <p>Insira o idioma no qual você deseja criar a exibição. </p> </li> 
       <li> <p><b>[!UICONTROL Sem sinalizador de cromo]</b> </p> <p>Selecionar <b>[!UICONTROL Sim]</b> para mostrar a página incorporada sem um cabeçalho ou rodapé de navegação.</p> </li> 
       <li> <p><b>[!UICONTROL Pode editar arquivos]</b> </p> <p>Selecionar <b>[!UICONTROL Sim]</b> se desejar que a seção de upload do arquivo seja editada adicionando ou removendo arquivos. Este não é um mecanismo de controle de acesso. O padrão é [!UICONTROL Sim].</p> </li> 
       <li> <p><b>[!UICONTROL Biblioteca document]</b> </p> <p>Selecionar <b>[!UICONTROL Sim]</b> se quiser que os links do documento da biblioteca fiquem visíveis. O padrão é [!UICONTROL Sim].</p> </li> 
       <li> <p><b>[!UICONTROL Arquivo local]</b> </p> <p>Selecionar <b>[!UICONTROL Sim]</b> se desejar que o botão local de upload do arquivo seja exibido. O padrão é [!UICONTROL Sim].</p> </li> 
       <li> <p><b>[!UICONTROL Web connectors]</b> </p> <p>Selecionar <b>[!UICONTROL Sim]</b> se desejar que os links anexem documentos de fontes da Web sejam exibidos. O padrão é Sim.</p> </li> 
       <li> <p><b>[!UICONTROL É pré-visualização selecionada]</b> </p> <p>Selecionar <b>[!UICONTROL Sim]</b> para definir a página Compor no modo Criação.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Compartilhamento de membros]</b> </p> <p>Para cada membro com o qual você deseja compartilhar o contrato, clique em <b>[!UICONTROL Adicionar item]</b> e insira o endereço de email do membro e uma mensagem para esse membro.</p> </li> 
     <li> <p>[!UICONTROL Delegar conjunto de participantes]</p> 
      <ul> 
       <li> <p><b>[!UICONTROL ID do conjunto de participantes]</b> </p> <p>Inserir a ID do conjunto de participantes</p> </li> 
       <li> <p><b>[!UICONTROL Informações do membro]</b> </p> <p>Para cada membro que deseja adicionar, clique em [!UICONTROL Adicionar item] e insira o endereço de email e as informações de telefone do membro.</p> </li> 
       <li> <p><b>[!UICONTROL Mensagem privada]</b> </p> <p>Insira uma mensagem. Todos os membros do conjunto de participantes receberão esta mensagem.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Library view info]</td> 
   <td> <p>Preencha os seguintes campos:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Name]</b> </p> <p>Insira um nome para o template da biblioteca. Esse nome é usado em emails e sites.</p> </li> 
     <li> <p><b>[!UICONTROL Usuário de logon automático]</b> </p> <p>Selecionar <b>[!UICONTROL Sim]</b> para fazer logon automático no URL retornado.</p> </li> 
     <li> <p><b>[!UICONTROL Quadro pai]</b> </p> <p>Insira ou mapeie uma lista separada por vírgulas de URLs de domínio pai, onde os URLs retornados podem ser enquadrados. Se deixado em branco, a variável [!DNL Adobe Acrobat Sign] as páginas não são visualizadas no iframe.</p> </li> 
     <li> <p><b>[!UICONTROL Locale]</b> </p> <p>Insira o idioma no qual você deseja criar a exibição. </p> </li> 
     <li> <p><b>[!UICONTROL Sem sinalizador de cromo]</b> </p> <p>Selecionar <b>[!UICONTROL Sim]</b> para mostrar a página incorporada sem um cabeçalho ou rodapé de navegação.</p> </li> 
     <li> <p><b>[!UICONTROL Enviar configuração de exibição]</b> </p> <p>Selecionar <b>[!UICONTROL Sim]</b> se quiser configurar a visualização do [!UICONTROL Enviar], preencha os seguintes campos.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Nome do contrato]</b> </p> <p>Insira ou mapeie o nome do contrato para o documento da biblioteca na página de composição.</p> </li> 
       <li> <p><b>[!UICONTROL Pode editar arquivos]</b> </p> <p>Selecionar <b>[!UICONTROL Sim]</b> se desejar que a seção de upload do arquivo seja editada adicionando ou removendo arquivos. Este não é um mecanismo de controle de acesso. O padrão é [!UICONTROL Sim].</p> </li> 
       <li> <p><b>[!UICONTROL Arquivo local]</b> </p> <p>Selecionar <b>[!UICONTROL Sim]</b> se quiser que os links do documento da biblioteca fiquem visíveis. O padrão é [!UICONTROL Sim].</p> </li> 
       <li> <p><b>[!UICONTROL Web connectors]</b> </p> <p>Selecionar <b>[!UICONTROL Sim]</b> se desejar que os links anexem documentos de fontes da Web sejam exibidos. O padrão é [!UICONTROL Sim].</p> </li> 
       <li> <p><b>Está selecionada a visualização</b> </p> <p>Selecionar <b>[!UICONTROL Sim]</b> para definir a página Compor no modo Criação.</p> </li> 
      </ul> <p> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Informações de exibição do usuário]</td> 
   <td> <p>Preencha os seguintes campos</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Name]</b> </p> <p>Selecione o nome da exibição de usuário solicitada.</p> </li> 
     <li> <p><b>[!UICONTROL Usuário de logon automático]</b> </p> <p>Selecionar <b>[!UICONTROL Sim]</b> para fazer logon automático no usuário. Selecionar <b>[!UICONTROL n.o]</b> para exigir credenciais. O padrão é [!UICONTROL Não].</p> </li> 
     <li> <p><b>[!UICONTROL Quadro pai]</b> </p> <p>Insira ou mapeie uma lista separada por vírgulas de URLs de domínio pai, onde os URLs retornados podem ser enquadrados. Se deixado em branco, a variável [!DNL Adobe Acrobat Sign] as páginas não são visualizadas no iframe.</p> </li> 
     <li> <p><b>Sem sinalizador de cromo</b> </p> <p>Selecionar <b>[!UICONTROL Sim]</b> para mostrar a página incorporada sem um cabeçalho ou rodapé de navegação.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos relacionados ao widget]</td> 
   <td> <p>Selecione o registro relacionado que deseja criar.</p> 
    <ul> 
     <li> <p>[!UICONTROL Exibições]</p> <p>Preencha os campos a seguir.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Name]</b> </p> <p>Selecione o nome da exibição de formulário web solicitada</p> </li> 
       <li> <p><b>[!UICONTROL Usuário de logon automático]</b> </p> <p>Selecionar <b>[!UICONTROL Sim]</b> para fazer logon automático no usuário. Selecionar <b>[!UICONTROL n.o]</b> para exigir credenciais. O padrão é [!UICONTROL Não].</p> </li> 
       <li> <p><b>[!UICONTROL Quadro pai]</b> </p> <p>Insira ou mapeie uma lista separada por vírgulas de URLs de domínio pai, onde os URLs retornados podem ser enquadrados. Se deixado em branco, a variável [!DNL Adobe Acrobat Sign] as páginas não são visualizadas no iframe.</p> </li> 
       <li> <p><b>[!UICONTROL Locale]</b> </p> <p>Insira o idioma no qual você deseja criar a exibição. </p> </li> 
       <li> <p><b>[!UICONTROL Sem sinalizador de cromo]</b> </p> <p>Selecionar <b>[!UICONTROL Sim]</b> para mostrar a página incorporada sem um cabeçalho ou rodapé de navegação.</p> </li> 
       <li> <p>[!UICONTROL Configuração de visualização de assinatura personalizada]</p> <p>Se quiser configurar uma exibição de assinatura personalizada, selecione <b>[!UICONTROL Sim]</b> e preencha os seguintes campos:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Email]</b> </p> <p>Insira o endereço de email da pessoa que recebe o formulário web recém-criado</p> </li> 
         <li> <p><b>[!UICONTROL Comentário]</b> </p> <p>Insira um comentário descrevendo como o chamador da API estabeleceu a identidade do assinante. Essas informações aparecem no [!DNL Adobe Acrobat Sign] trilha de auditoria.</p> </li> 
         <li> <p><b>[!UICONTROL Expiração]</b> </p> <p>Insira uma data de expiração para a personalização desse formulário web. </p> <p>Para obter uma lista de formatos de data e hora compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Coação de tipo em [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
         <li> <p><b>[!UICONTROL Reutilizável]</b> </p> <p>Selecionar <b>[!UICONTROL Sim]</b> se desejar que o assinante desejado possa assinar o formulário mais de uma vez.</p> </li> 
        </ul> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Compartilhamento de membros]</b> </p> <p>Para cada membro com o qual você deseja compartilhar o contrato, clique em <b>[!UICONTROL Adicionar item]</b> e insira o endereço de email do membro e uma mensagem para esse membro.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Chamada da API personalizada]**
Esse módulo permite executar uma chamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Adobe Acrobat Sign] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Insira um caminho relativo a <code>https://api.[region].adobesign.com/api/rest/v6/</code></p> <p>Observação: Para obter a lista de endpoints disponíveis, consulte [!DNL Adobe Sign] Referência da API.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   <td> <p>Selecione o método de solicitação HTTP que você precisa configurar a chamada da API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] adiciona cabeçalhos de autorização automaticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sequência de consulta] </td> 
   <td> <p>Insira a sequência de consulta da solicitação.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada da API no formato de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fazer upload de um documento transitório]</td> 
   <td> <p>Para carregar um documento transitório, insira o arquivo de origem do documento que deseja fazer upload.</p> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Listar registros]**

Este módulo de ação lista todos os registros do tipo selecionado ao qual a conta tem acesso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Adobe Acrobat Sign] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] adiciona cabeçalhos de autorização automaticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Selecione o tipo de registro para o qual você deseja recuperar registros relacionados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Locale]</td> 
   <td> <p>Insira a localidade do usuário. Isso determina o idioma da interface do usuário. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID Externa]</td> 
   <td>Insira ou mapeie a ID externa (uma ID atribuída fora de [!DNL Adobe Acrobat Sign]) para os contratos que você deseja retornar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do grupo]</td> 
   <td>Insira a ID do grupo associado aos registros que deseja listar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar oculto (registros)]</td> 
   <td>Ative essa opção se desejar incluir registros ocultos nos resultados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cursor] / [!UICONTROL Iniciar índice]</td> 
   <td> <p>Insira o número do primeiro registro que o módulo deve retornar. </p> <p>Observação: Este campo é combinado com o campo [!UICONTROL Número máximo de registros retornados] para paginação. Por exemplo, se o [!UICONTROL Número máximo de eventos retornados] for 100 e o [!UICONTROL Start index] for 101, o módulo retornará registros 101-200 ou a segunda página de resultados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de registros retornados]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros para o módulo [action] durante cada ciclo de execução de cenário.</p> <p>Observação: Este campo é combinado com o campo [!UICONTROL Cursor] ou o campo [!UICONTROL Start Index] para paginação. Por exemplo, se o [!UICONTROL Número máximo de eventos retornados] for 100 e o [!UICONTROL Start index] for 101, o módulo retornará registros 101-200 ou a segunda página de resultados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URLs de domínio pai]</td> 
   <td> <p>Insira ou mapeie uma lista separada por vírgulas de URLs de domínio pai, onde os URLs retornados podem ser enquadrados. Se deixado em branco, a variável [!DNL Adobe Acrobat Sign] as páginas não são visualizadas no iframe.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Ler um registro]**

Esse módulo de ação recupera informações de um único registro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Adobe Acrobat Sign] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] adiciona cabeçalhos de autorização automaticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Selecione o tipo de registro para o qual você deseja recuperar registros relacionados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do registro]</td> 
   <td>Insira ou mapeie a ID do registro que deseja recuperar.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Ler registros relacionados]**

Leia informações adicionais relacionadas a um único registro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Adobe Acrobat Sign] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] adiciona cabeçalhos de autorização automaticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Selecione o tipo de registro para o qual você deseja recuperar registros relacionados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do registro] (Exemplo: [!UICONTROL Account ID])</td> 
   <td>Insira ou mapeie a ID do registro para o qual deseja recuperar registros relacionados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outros campos]</td> 
   <td>Insira informações em campos específicos com base no tipo de registro e campos relacionados.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Atualizar um registro]**

Este módulo de ação atualiza um único registro em [!DNL Adobe Acrobat Sign].

>[!IMPORTANT]
>
>* Como prática recomendada, se estiver a antecipar alterações substanciais a um acordo, recomendamos a criação de um novo acordo em vez de atualizar o acordo existente.
>* Algumas atualizações exibem campos obrigatórios do recurso. Ao configurar sua atualização, preencha todos os campos obrigatórios. Os campos obrigatórios estão em negrito em [!DNL Workfront Fusion] módulos.
>




<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Adobe Acrobat Sign] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] adiciona cabeçalhos de autorização automaticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do registro] </td> 
   <td>Insira ou mapeie a ID do registro que deseja atualizar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Selecione o tipo de registro que deseja atualizar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outros campos]</td> 
   <td> <p>Insira informações em campos específicos com base no tipo de registro e campos relacionados.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Agreement]</b> </p> <p>Como prática recomendada, se estiver a antecipar alterações substanciais a um acordo, recomendamos a criação de um novo acordo em vez de atualizar o acordo existente.</p> </li> 
     <li> <p><b>[!UICONTROL Biblioteca document]</b> </p> <p>Selecione os campos que deseja atualizar e preencha os campos selecionados:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Status]</b> </p> <p>Selecione o novo status para o documento da biblioteca.</p> </li> 
       <li> <p><b>[!UICONTROL Name]</b> </p> <p>Insira ou mapeie o nome do template de biblioteca</p> </li> 
       <li> <p><b>[!UICONTROL Modo de compartilhamento]</b> </p> <p>Especifique quem deve ter acesso ao documento da biblioteca.</p> </li> 
       <li> <p><b>[!UICONTROL Tipo de modelo da biblioteca]</b> </p> <p>Para cada tipo de modelo de biblioteca que deseja usar, clique em <b>[!UICONTROL Adicionar item]</b> e selecione o tipo de modelo.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Usuário]</b> </p> <p>Selecione os campos que deseja atualizar e preencha os campos selecionados:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Nome]</b> </p> <p>Insira o nome do usuário.</p> </li> 
       <li> <p><b>[!UICONTROL Sobrenome]</b> </p> <p>Digite o sobrenome do usuário</p> </li> 
       <li> <p><b>[!UICONTROL Company]</b> </p> <p>Insira o nome da empresa do usuário.</p> </li> 
       <li> <p><b>[!UICONTROL Telefone]</b> </p> <p>Digite o número de telefone do usuário</p> </li> 
       <li> <p><b>[!UICONTROL ID do grupo principal]</b> </p> <p>Insira o grupo ao qual o novo usuário é adicionado. Se nada for inserido, o usuário será adicionado ao grupo padrão da conta.</p> </li> 
       <li> <p><b>[!UICONTROL Cargo title]</b> </p> <p>Insira o cargo do usuário.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Web form] ([!UICONTROL widget])</b> </p> <p>Insira informações em campos específicos com base no tipo de registro e campos relacionados.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Atualizar registro relacionado]**

Esse módulo de ação atualiza registros relacionados a um objeto específico.

>[!IMPORTANT]
>
>* Como prática recomendada, se estiver a antecipar alterações substanciais a um acordo, recomendamos a criação de um novo acordo em vez de atualizar o acordo existente.
>* Algumas atualizações exibem campos obrigatórios do recurso. Ao configurar sua atualização, preencha todos os campos obrigatórios. Os campos obrigatórios estão em negrito em [!DNL Workfront Fusion] módulos.
>




<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Adobe Acrobat Sign] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] adiciona cabeçalhos de autorização automaticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Selecione o tipo de registro do registro ao qual os campos relacionados estão associados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Agreement]/[!UICONTROL Library document]/[!UICONTROL User]/[!UICONTROL Widget ID]</td> 
   <td>Insira ou mapeie a ID do objeto ao qual você deseja associar o registro criado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outros campos]</td> 
   <td> <p>Insira informações em campos específicos com base no tipo de registro e campos relacionados.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Agreement]</b> </p> <p>Como prática recomendada, se estiver a antecipar alterações substanciais a um acordo, recomendamos a criação de um novo acordo em vez de atualizar o acordo existente.</p> </li> 
     <li> <p><b>[!UICONTROL Biblioteca document]</b> </p> <p>Selecione os campos que deseja atualizar e preencha os campos selecionados:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Estado]</b> </p> <p>Selecione o novo status para o documento da biblioteca.</p> </li> 
       <li> <p><b>[!UICONTROL Nota]</b> </p> <p>Insira ou mapeie o texto da nota.</p> </li> 
       <li> <p><b>[!UICONTROL Visibility]</b> </p> <p>Selecione se o documento da biblioteca é exibido ou oculto.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Usuário]</b> </p> <p>Selecione os campos que deseja atualizar e preencha os campos selecionados:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Lista de informações do grupo]</b> </p> <p>Preencha os seguintes campos</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Status]</b> </p> <p>Selecione o novo status para o usuário.</p> </li> 
         <li> <p><b>[!UICONTROL ID]</b> </p> <p>Insira a ID exclusiva do grupo</p> </li> 
         <li> <p><b>[!UICONTROL É administrador de grupo]</b> </p> <p>Selecionar <b>[!UICONTROL Sim]</b> para tornar este usuário um administrador de grupo.</p> </li> 
         <li> <p><b>É o grupo principal</b> </p> <p>Selecionar <b>[!UICONTROL Sim]</b> para atualizar este grupo para o grupo principal do usuário.</p> </li> 
         <li> <p><b>[!UICONTROL Data de criação]</b> </p> <p>Insira a data em que o grupo foi criado.</p> <p>Para obter uma lista de formatos de data e hora compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Estilo de coerção no [!UICONTROL Adobe Workfront Fusion]</a>.</p> </li> 
         <li> <p><b>[!UICONTROL Name]</b> </p> <p>Insira ou mapeie o nome do grupo.</p> </li> 
         <li> <p><b>[!UICONTROL Biblioteca criação de documentos visível]</b> </p> <p>Essas configurações determinam se o usuário pode criar documentos da biblioteca</p> 
          <ul> 
           <li> <p>[!UICONTROL Valor]</p> <p>Permitir</p> </li> 
           <li> <p>[!UICONTROL Herdado]</p> <p>Herdar configuração de grupo do grupo ou da conta</p> </li> 
          </ul> </li> 
         <li> <p><b>[!UICONTROL Enviar restrito a workflows]</b> </p> <p>Essas configurações determinam se o usuário pode criar contratos somente usando workflows.</p> 
          <ul> 
           <li> <p>[!UICONTROL Valor]</p> <p>Permitir</p> </li> 
           <li> <p>[!UICONTROL Herdado]</p> <p>Herdar configuração de grupo do grupo ou da conta</p> </li> 
          </ul> </li> 
         <li> <p><b>[!UICONTROL Usuário pode enviar]</b> </p> 
          <ul> 
           <li> <p>[!UICONTROL Valor]</p> <p>Permitir</p> </li> 
           <li> <p>[!UICONTROL Herdado]</p> <p>Herdar configuração de grupo do grupo ou da conta</p> </li> 
          </ul> </li> 
        </ul> </li> 
      </ul> 
      <ul> 
       <li> <p><b>[!UICONTROL Estado]</b> </p> <p>Selecione o novo estado do usuário e insira um comentário sobre por que você deseja ativar ou desativar o usuário.</p> </li> 
       <li> <p><b>[!UICONTROL Locale]</b> </p> <p>Insira a localidade do usuário. Isso determina o idioma da interface do usuário. </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Web form] ([!UICONTROL widget])</b> </p> <p>Insira informações em campos específicos com base no tipo de registro e campos relacionados.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Carregar documento]**

Faça upload de um documento transitório. Um documento transitório fica disponível por 7 dias após ser carregado.

>[!NOTE]
>
>Recomendamos fazer upload do documento para assinar como um documento transitório, em seguida, mapeá-lo para o campo File to send no módulo Create an agreement .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Adobe Acrobat Sign] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] adiciona cabeçalhos de autorização automaticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do registro]</td> 
   <td>Insira ou mapeie a ID do registro que deseja atualizar</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL tipo MIME]</td> 
   <td>Insira o tipo mime do arquivo original. Os tipos MIME (Multipurpose Internet Mail Extension) são rótulos que permitem ao software identificar diferentes tipos de dados compartilhados na Internet. Os servidores e navegadores da Web usam o tipo MIME para determinar o que deve ser feito com um arquivo. Por exemplo, um arquivo com o tipo MIME <code>text/html</code> será processado em um navegador de forma diferente de um arquivo com o tipo MIME <code>image/jpeg</code>.</td> 
  </tr> 
 </tbody> 
</table>

**Exemplo:** Nesse fluxo de trabalho, o documento para assinar (baixado anteriormente do Workfront) é carregado como um documento transitório.

![](assets/sign-example-1-350x308.png)

O [!UICONTROL Carregar documento] O módulo fornece um [!DNL Adobe Acrobat Sign] ID que pode ser referenciada em módulos posteriores. Quando o contrato é criado, a ID do documento carregado é incluída no [!UICONTROL Arquivos para enviar] campo.

![](assets/sign-example-2-350x356.png)

+++

### Pesquisas

+++ **[!UICONTROL Pesquisar contratos]**

Este módulo de pesquisa procura por contratos baseados em critérios fornecidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Adobe Acrobat Sign] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro de texto]</td> 
   <td> <p>Procure por texto nos metadados do contrato. </p> 
    <ul> 
     <li> <p><b>[!UICONTROL Localizar texto]</b> </p> <p>Insira o texto que deseja localizar nos metadados do contrato. Cada palavra é tratada como um item de texto separado. </p> </li> 
     <li> <p><b>[!UICONTROL Localizar texto em]</b> </p> <p>Selecione os campos de metadados nos quais deseja localizar o texto. Se você não selecionar nada, os módulos pesquisarão todos os metadados.</p> </li> 
    </ul> <p>O módulo retorna qualquer contrato que contenha qualquer texto inserido em qualquer um dos campos selecionados. Exemplo: inserir "campanha da primavera" e selecionar as opções Título e Nota retorna quaisquer acordos com as palavras "Primavera" ou "Campanha" no Título ou na Nota.</p> <p>Para obter mais informações sobre como pesquisar campos em [!DNL Adobe Acrobat Sign], consulte "Como funciona a pesquisa de texto" em <a href="https://helpx.adobe.com/sign/using/adobesign-search-users-agreements.html#HowSearchWorks">[!DNL Adobe Sign] Pesquisar - Como funciona</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data de criação]</td> 
   <td>Selecione datas. O módulo retorna somente registros em que a data criada corresponde a esse critério.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data de expiração]</td> 
   <td>Selecione datas. O módulo retorna somente registros em que a data de expiração corresponde a esse critério.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL Data de modificação]</p> </td> 
   <td>Selecione datas. O módulo retorna somente registros em que a data modificada corresponde a esse critério.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID Externa]</td> 
   <td> <p> A ID externa é uma ID atribuída ao remetente para o contrato que pode ser de qualquer forma, mas geralmente na forma de "&lt;groupid&gt;:&lt;id&gt;".</p> <p>Para cada ID externa que deseja adicionar, clique em <b>[!UICONTROL Adicionar]</b> e insira ou mapeie a ID externa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do grupo]</td> 
   <td> <p>ID de grupo é um identificador atribuído quando o grupo foi criado.</p> <p>Para cada ID externa que deseja adicionar, clique em <b>[!UICONTROL Adicionar]</b> e insira ou mapeie a ID externa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de ativo]</td> 
   <td> <p>Essa é a ID atribuída ao contrato específico. </p> <p>Para cada ID externa que deseja adicionar, clique em <b>[!UICONTROL Adicionar]</b> e insira ou mapeie a ID externa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID pai]</td> 
   <td> <p>Esta é a ID atribuída ao objeto principal do contrato. </p> <p>Para cada ID externa que deseja adicionar, clique em <b>[!UICONTROL Adicionar]</b> e insira ou mapeie a ID externa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email do participante]</td> 
   <td> <p>O endereço de email de um participante. </p> <p>Para cada ID externa que deseja adicionar, clique em <b>[!UICONTROL Adicionar]</b> e insira ou mapeie a ID externa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Função]</td> 
   <td>Selecione as funções que deseja que os resultados retornados incluam.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Classificar por]</td> 
   <td>Se desejar que o módulo classifique os resultados, selecione o campo no qual deseja classificar os resultados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Classificar ordem]r</td> 
   <td>Se desejar que o módulo classifique os resultados, selecione se deseja classificar crescente ou decrescente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status]</td> 
   <td>Selecione os status que você deseja que os resultados retornados incluam.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo]</td> 
   <td>Selecione os tipos de contrato que você deseja que os resultados retornados incluam.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subtipos]</td> 
   <td>Selecione os subtipos de contrato que você deseja que os resultados retornados incluam. Somente os contratos de modelo de biblioteca incluem subtipos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do usuário]</td> 
   <td> <p>A ID de usuário com a qual o contrato é compartilhado.</p> <p>Para cada ID de usuário que deseja adicionar, clique em <b>[!UICONTROL Adicionar]</b> e insira ou mapeie a ID do usuário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Visibility]</td> 
   <td>Selecione o nível de visibilidade que deseja que os resultados retornados incluam.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Iniciar índice]</td> 
   <td> <p>Informe a posição do primeiro resultado que você deseja retornar. Combine isso com o máximo de [!UICONTROL resultados retornados] para paginar resultados</p> <p>Exemplo: se você retornar 100 resultados por vez, insira 100 para retornar os resultados 100-200.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de resultados retornados]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros para o módulo [action] durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++
