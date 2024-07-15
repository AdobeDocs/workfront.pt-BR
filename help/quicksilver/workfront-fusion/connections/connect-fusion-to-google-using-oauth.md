---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Conectar [!DNL Adobe Workfront Fusion] a [!DNL Google Services] usando um cliente OAuth personalizado
description: Você pode usar o  [!DNL Adobe Workfront Fusion] para se conectar ao [!DNL Google Services] usando um cliente OAuth personalizado. Este procedimento requer uma conta  [!DNL Google]  existente.
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# Conectar [!DNL Adobe Workfront Fusion] a [!DNL Google Services] usando um cliente OAuth personalizado

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td> <p>Novo: [!UICONTROL Padrão]</p><p>Ou</p><p>Atual: [!UICONTROL Trabalho] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licença**</td> 
   <td>
   <p>Atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Herdados: Qualquer um </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Novo:</p> <ul><li>[!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Workfront] Plano: sua organização deve comprar [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plano: [!DNL Workfront Fusion] está incluído.</li></ul>
   <p>Ou</p>
   <p>Atual: sua organização deve comprar o [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Você precisa de uma conta existente do [!DNL Google] para fazer essa conexão.

## Conectar o Fusion aos serviços da Google usando um cliente OAuth personalizado

Para criar essa conexão, você deve criar e configurar um projeto na plataforma Google Cloud e, em seguida, configurar a conexão no Fusion com base nesse projeto.

* [Criar um projeto em [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform)
* [Definir [!UICONTROL configurações de consentimento do OAuth]](#configure-oauth-consent-settings)
* [Criar credenciais do OAuth](#create-oauth-credentials)
* [Conectar a [!DNL Google] em [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion)

>[!NOTE]
>
>Este procedimento destina-se a:
>
>* Uso pessoal ([!DNL `@gmail.com`] e [!DNL `@googlemail.com`] usuários)
>* Uso interno ([!DNL Google Workspace] usuários que preferem usar um cliente OAuth personalizado)

### Criar um projeto em [!DNL Google Cloud Platform]

Para criar um projeto na plataforma [!DNL Google Cloud]:

1. Entre na [[!DNL Google Cloud] Plataforma](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) usando suas credenciais do [!DNL Google].
1. No painel esquerdo, clique em **[!UICONTROL Painel]**.
1. Clique em **[!UICONTROL Criar projeto]** no canto superior direito da tela.
1. Insira o **[!UICONTROL Nome do projeto]** e clique em **[!UICONTROL Criar]**.

1. Clique na guia **[!UICONTROL Habilitar APIs e serviços]** próxima à parte superior da tela.
1. No campo **[!UICONTROL Pesquisar APIs e Serviços]**, na parte superior da tela, digite o nome do serviço que deseja usar (como API [!DNL Gmail] ou API [!DNL Google Drive]).
1. Quando for exibido, clique na API ou no serviço ao qual você deseja se conectar [!DNL Workfront Fusion].
1. Clique em **[!UICONTROL Habilitar]** para habilitar a API selecionada.
1. Repita as etapas 6 a 8 para cada API que deseja ativar.

   >[!NOTE]
   >
   >Você deve habilitar a API [!DNL Google Drive] e também a API de todos os aplicativos [!DNL Google] que deseja usar (como a API [!DNL Google Sheets]).

1. Na tela exibida, clique em **[!UICONTROL Criar credenciais]** no canto superior direito.
1. Prossiga para a seção [Definir configurações de consentimento do OAuth](#configure-oauth-consent-settings) neste artigo.

### Definir configurações de [!UICONTROL consentimento do OAuth]

1. No painel esquerdo, clique em **[!UICONTROL Tela de consentimento do OAuth]**.
1. Selecione **[!UICONTROL Externo]** e clique em **[!UICONTROL Criar]**.

   >[!NOTE]
   >
   >Você não será cobrado ao selecionar essa opção. Para obter mais informações, consulte as informações de [!DNL Google] sobre exceções aos requisitos de verificação.

1. Preencha os campos obrigatórios da seguinte maneira:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nome do aplicativo]</p> </td> 
      <td> <p>Insira o nome do aplicativo que solicita consentimento.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>[!DNL Adobe Workfront Fusion] </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Email de suporte ao usuário]</td> 
      <td>Insira um endereço de email para que os usuários entrem em contato com você caso tenham dúvidas sobre o consentimento deles ao se conectarem a este aplicativo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Endereços de email]</td> 
      <td>Insira um ou mais endereços de email que a Google pode usar para notificá-lo sobre qualquer alteração no seu projeto.</td> 
     </tr> 
    </tbody> 
   </table>

1. Em [!UICONTROL Domínios autorizados], clique em **[!UICONTROL Adicionar domínio]** e digite `workfrontfusion.com`.

1. Clique em **[!UICONTROL Salvar e continuar]**.
1. Clique em **[!UICONTROL Adicionar ou remover escopos]**.
1. No painel direito, ative os seguintes escopos:

<table style="table-layout:auto">
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Serviço/API</th> 
      <th>Escopos necessários</th> 
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

Talvez seja necessário expandir a lista ou ir para a próxima página da lista para ver todos eles.

1. Clique em **[!UICONTROL Atualizar]**.
1. Clique em **[!UICONTROL Salvar e continuar]**.
1. (Opcional) Adicione usuários de teste ao projeto.
1. Clique em **[!UICONTROL Salvar e continuar]**.
1. Examine suas informações para verificar a precisão e clique em **[!UICONTROL Voltar ao painel]**.

   >[!NOTE]
   >
   >Você não precisa enviar sua tela de consentimento e seu aplicativo para verificação por [!DNL Google].

1. Continue em [Criar credenciais do OAuth](#create-oauth-credentials).

### Criar credenciais do OAuth

1. No painel esquerdo, clique em **[!UICONTROL Credenciais]**.

   >[!NOTE]
   >
   >Se esta não for a primeira API ou serviço ([!DNL Gmail] ou [!DNL Google Drive]) habilitado, você não precisará criar novas credenciais.

1. Clique em **[!UICONTROL Criar credenciais]** próximo à parte superior da tela e selecione **[!UICONTROL ID do cliente OAuth]** no menu suspenso.

1. Preencha os campos obrigatórios da seguinte maneira:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo de aplicativo]</td> 
      <td> <p> [!UICONTROL Aplicativo Web]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome]</td> 
      <td>[!DNL Workfront Fusion] </td> 
     </tr> 
    </tbody> 
   </table>

1. Em [!UICONTROL URIs de redirecionamento autorizados], clique em **[!UICONTROL Adicionar URI]** e insira **um** dos seguintes:

   * Para [!DNL Gmail] ou [!DNL Google Drive]: `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * Para outros aplicativos [!DNL Google]: `https://app.workfrontfusion.com/oauth/cb/google`

1. Clique em **[!UICONTROL Criar]**.

   A [!UICONTROL ID do Cliente] e o [!UICONTROL Segredo do Cliente] são exibidos.

1. Copie a [!UICONTROL ID do Cliente] e o [!UICONTROL Segredo do Cliente] para um local seguro. Você os usará para estabelecer uma conexão em [!DNL Workfront Fusion].
1. Continue para [Conectar-se [!DNL Google] em [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion).

### Conectar a [!DNL Google] em [!DNL Workfront Fusion]

O processo de criação de uma conexão com [!DNL Google] difere dependendo se você está usando um módulo de um serviço [!DNL Google] (como [!DNL Google Sheets] ou [!DNL Google Docs]), ou se você está se conectando a [!DNL Google] por meio do módulo de solicitação [!UICONTROL HTTP] >[!UICONTROL Make an OAuth2.0].

* [Conectar-se a [!DNL Google] em um serviço [!DNL Google] ](#connect-to-google-in-a-google-service)
* [Conectar a  [!DNL Google] no módulo [!UICONTROL HTTP] > [!UICONTROL Fazer uma solicitação OAuth2.0]](#connect-to-google-in-the-http--make-an-oauth20-request-module)

#### Conectar a [!DNL Google] em um serviço [!DNL Google]

1. No [!DNL Workfront Fusion], localize o módulo [!DNL Google] para o qual você precisa criar uma conexão.
1. Clique em **[!UICONTROL Criar uma conexão]** e em **[!UICONTROL Mostrar configurações avançadas]**.

1. Insira a [!UICONTROL ID do Cliente] e o [!UICONTROL Segredo do Cliente] recuperados em [[!UICONTROL Criar Credenciais OAuth]](#create-oauth-credentials) nos respectivos campos e clique em **[!UICONTROL Continuar]**.

1. Entre com sua conta [!DNL Google].

   A janela **[!UICONTROL Este aplicativo não foi verificado]** é exibida. Observe que o &quot;aplicativo&quot; mencionado no título da janela é o cliente OAuth criado acima.

1. Clique em **[!UICONTROL Avançado]** e em **[!UICONTROL Ir para [!DNL Workfront Fusion] (não seguro)]** para permitir acesso usando seu cliente OAuth personalizado.

1. Clique em **[!UICONTROL Permitir]** para conceder permissão [!DNL Workfront Fusion].
1. Na janela exibida, clique em **[!UICONTROL Permitir]** novamente para confirmar suas escolhas.

   A conexão com o serviço [!DNL Google] desejado usando um cliente OAuth personalizado foi estabelecida.

#### Conectar-se a [!DNL Google] no módulo [!UICONTROL HTTP] > [!UICONTROL Fazer uma solicitação OAuth2.0] {#connect-to-google-in-the-http--make-an-oauth20-request-module}

Para obter instruções sobre como se conectar a [!DNL Google] no módulo [!UICONTROL HTTP] > [!UICONTROL Fazer uma solicitação OAuth2.0], consulte [Instruções para criar uma conexão com [!DNL Google] no módulo [!UICONTROL HTTP] > [!UICONTROL Fazer uma solicitação OAuth 2.0]](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module) em [[!UICONTROL HTTP] > [!UICONTROL Fazer uma solicitação OAuth 2.0]](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## Possível mensagem de erro:[!UICONTROL [403] Acesso Não Configurado]

Se a mensagem de erro [!UICONTROL `403 Access Not Configured`] for exibida, será necessário habilitar a API correspondente na Google Cloud Platform. Para habilitar a API, siga as etapas da seção [Criar um projeto [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) deste artigo.
