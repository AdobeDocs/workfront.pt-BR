---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Connect [!DNL Adobe Workfront Fusion] para [!DNL Google Services] usando um cliente OAuth personalizado
description: Você pode usar [!DNL Adobe Workfront Fusion] para se conectar a [!DNL Google Services] usando um cliente OAuth personalizado. Este procedimento requer um [!DNL Google] conta.
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 0%

---

# Connect [!DNL Adobe Workfront Fusion] para [!DNL Google Services] usando um cliente OAuth personalizado

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

Você precisa de um [!DNL Google] para fazer essa conexão.

## Crie um projeto em [!DNL Google Cloud Platform]

O seguinte procedimento destina-se:

* Uso pessoal ([!DNL @gmail.com] e [!DNL @googlemail.com] users)
* Uso interno ([!DNL G Suite] usuários que preferem usar um cliente OAuth personalizado)

Para criar um projeto em [!DNL Google Cloud] Plataforma:

1. Fazer logon em [[!DNL Google Cloud] Plataforma](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) usar seu [!DNL Google] credenciais.
1. No painel esquerdo, clique em **[!UICONTROL Painel]**.
1. Clique em **[!UICONTROL Criar projeto]** no canto superior direito da tela.
1. Insira o **[!UICONTROL Nome do projeto]**, depois clique em **[!UICONTROL Criar]**.

1. Clique no botão **[!UICONTROL Ativar APIs e serviços]** próximo à parte superior da tela.
1. No **[!UICONTROL Pesquisar por APIs e serviços]** na parte superior da tela, digite o nome do serviço que deseja usar (como [!DNL Gmail] API ou [!DNL Google Drive] API).
1. Quando for exibido, clique na API ou no serviço ao qual deseja se conectar [!DNL Workfront Fusion].
1. Clique em **[!UICONTROL Habilitar]** para ativar a API selecionada.
1. Repita as etapas de 6 a 8 para cada API que desejar ativar.

   >[!NOTE]
   >
   >Você deve ativar [!DNL Google Drive] API, bem como a API de todos [!DNL Google] aplicativos que você deseja usar (como [!DNL Google Sheets] API).

1. Na tela que aparece, clique em **[!UICONTROL Criar credenciais]** no canto superior direito.
1. Prossiga para a seção [Definir configurações de consentimento do OAuth](#configure-oauth-consent-settings) neste artigo.

## Configurar [!UICONTROL Consentimento OAuth] configurações

1. No painel esquerdo, clique em **[!UICONTROL Tela de consentimento OAuth]**.
1. Selecionar **[!UICONTROL Externo]**, depois clique em **[!UICONTROL Criar]**.

   >[!NOTE]
   >
   >Você não será cobrado ao selecionar essa opção. Para obter mais informações, consulte [!DNL Google]Informações da Comissão sobre as exceções aos requisitos de verificação.

1. Preencha os campos obrigatórios da seguinte maneira:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nome do aplicativo]</p> </td> 
      <td> <p>Insira o nome do aplicativo solicitando consentimento.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>[!DNL Adobe Workfront Fusion] </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Email de suporte ao usuário]</td> 
      <td>Digite um endereço de email para que os usuários possam contatá-lo com perguntas sobre o consentimento deles ao se conectar a este aplicativo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Endereços de email]</td> 
      <td>Insira um ou mais endereços de email que a Google pode usar para notificá-lo sobre qualquer alteração no projeto.</td> 
     </tr> 
    </tbody> 
   </table>

1. Em [!UICONTROL Domínios autorizados], clique em **[!UICONTROL Adicionar domínio]** e insira `workfrontfusion.com`.

1. Clique em **[!UICONTROL Salvar e continuar]**.
1. Clique em **[!UICONTROL Adicionar ou remover escopos]**.
1. No painel direito, ative os seguintes escopos:

<table style="table-layout:auto">
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Serviço/API</th> 
      <th>Escopos obrigatórios</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p>[!DNL Gmail]</p> </td> 
      <td> <p>https://mail.google.com/</p> <p>https://www.googleapis.com/auth/gmail.labels</p> <p>https://www.googleapis.com/auth/gmail.send</p> <p>https://www.googleapis.com/auth/gmail.readonly</p> <p>https://www.googleapis.com/auth/gmail.compose</p> <p>https://www.googleapis.com/auth/gmail.insert</p> <p>https://www.googleapis.com/auth/gmail.modify</p> <p>https://www.googleapis.com/auth/gmail.metadata</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!DNL Google Drive]</p> </td> 
      <td> <p>https://www.googleapis.com/auth/drive</p> <p>https://www.googleapis.com/auth/drive.readonly</p> </td> 
     </tr> 
    </tbody> 
   </table>

Talvez seja necessário expandir a lista ou ir para a próxima página da lista para ver todos.

1. Clique em **[!UICONTROL Atualizar]**.
1. Clique em **[!UICONTROL Salvar e continuar]**.
1. (Opcional) Adicione quaisquer usuários de teste ao projeto.
1. Clique em **[!UICONTROL Salvar e continuar]**.
1. Examine suas informações para obter precisão e clique em **[!UICONTROL Voltar ao painel]**.

   >[!NOTE]
   >
   >Não é necessário enviar a tela de consentimento e o aplicativo para verificação por [!DNL Google].

1. Continue para [Criar credenciais do OAuth](#create-oauth-credentials).

## Criar credenciais do OAuth

1. No painel esquerdo, clique em **[!UICONTROL Credenciais]**.

   >[!NOTE]
   >
   >Se essa não for a primeira API ou serviço ([!DNL Gmail] ou [!DNL Google Drive]) estiver habilitado, não será necessário criar novas credenciais.

1. Clique em **[!UICONTROL Criar credenciais]** próximo à parte superior da tela, selecione **[!UICONTROL ID de cliente OAuth]** no menu suspenso.

1. Preencha os campos obrigatórios da seguinte maneira:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Application type]</td> 
      <td> <p> [!UICONTROL Web application]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>[!DNL Workfront Fusion] </td> 
     </tr> 
    </tbody> 
   </table>

1. Em [!UICONTROL URIs de redirecionamento autorizados], clique em **[!UICONTROL Adicionar URI]** e insira **one** do seguinte:

   * Para [!DNL Gmail] ou [!DNL Google Drive]: `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * Para outros [!DNL Google] aplicativos: `https://app.workfrontfusion.com/oauth/cb/google`

1. Clique em **[!UICONTROL Criar]**.

   O [!UICONTROL ID do cliente] e [!UICONTROL Segredo do cliente] exibir.

1. Copie o [!UICONTROL ID do cliente] e [!UICONTROL Segredo do cliente] para um local seguro. Você os usará para fazer uma conexão no [!DNL Workfront Fusion].
1. Continue para [Conectar-se a [!DNL Google] em [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion).

## Conectar-se a [!DNL Google] em [!DNL Workfront Fusion]

O processo de criação de uma conexão com o [!DNL Google] varia dependendo se você está usando um módulo de um [!DNL Google] (como [!DNL Google Sheets] ou [!DNL Google Docs]) ou se estiver se conectando a [!DNL Google] através da [!UICONTROL HTTP] >[!UICONTROL Faça um OAuth2.0] módulo de solicitação.

* [Conectar-se a [!DNL Google] em [!DNL Google] service](#connect-to-google-in-a-google-service)
* [Conectar-se a [!DNL Google] no [!UICONTROL HTTP] > [!UICONTROL Faça uma solicitação do OAuth2.0] módulo](#connect-to-google-in-the-http--make-an-oauth20-request-module)

### Conectar-se a [!DNL Google] em [!DNL Google] service

1. Em [!DNL Workfront Fusion], localize o [!DNL Google] módulo para o qual você precisa criar uma conexão.
1. Clique em **[!UICONTROL Criar uma conexão]**, depois clique em **[!UICONTROL Mostrar configurações avançadas]**.

1. Insira o [!UICONTROL ID do cliente] e [!UICONTROL Segredo do cliente] você recuperou em [[!UICONTROL Criar credenciais do OAuth]](#create-oauth-credentials) nos respectivos campos, em seguida, clique em **[!UICONTROL Continuar]**.

1. Faça logon com seu [!DNL Google] conta.

   O **[!UICONTROL Este aplicativo não foi verificado]** será exibida. Observe que o &quot;aplicativo&quot; mencionado no título da janela é o cliente OAuth que você criou acima.

1. Clique em **[!UICONTROL Avançado]**, depois clique em **[!UICONTROL Ir para [!DNL Workfront Fusion] (não seguro)]** para permitir acesso usando seu cliente OAuth personalizado.

1. Clique em **[!UICONTROL Permitir]** para conceder [!DNL Workfront Fusion] permissão.
1. Na janela exibida, clique em **[!UICONTROL Permitir]** novamente para confirmar suas opções.

   A conexão com o [!DNL Google] O serviço que usa um cliente OAuth personalizado é estabelecido.

### Conectar-se a [!DNL Google] no [!UICONTROL HTTP] > [!UICONTROL Faça uma solicitação do OAuth2.0] módulo {#connect-to-google-in-the-http--make-an-oauth20-request-module}

Para obter instruções sobre como conectar-se a [!DNL Google] no [!UICONTROL HTTP] > [!UICONTROL Faça uma solicitação do OAuth2.0] módulo, consulte [Instruções para criação de uma conexão com o [!DNL Google] no [!UICONTROL HTTP] > [!UICONTROL Fazer uma solicitação do OAuth 2.0] módulo](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instruct) em [[!UICONTROL HTTP] > [!UICONTROL Fazer uma solicitação do OAuth 2.0] módulo](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## Possível mensagem de erro:[!UICONTROL [403] Acesso não configurado]

Se a variável [!UICONTROL [403] Acesso não configurado] for exibida, é necessário ativar a API correspondente na Google Cloud Platform. Para ativar a API, siga as etapas na seção [Crie um projeto em [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) neste artigo.
