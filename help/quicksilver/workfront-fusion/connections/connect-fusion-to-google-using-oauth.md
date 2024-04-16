---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Conectar [!DNL Adobe Workfront Fusion] para [!DNL Google Services] uso de um cliente OAuth personalizado
description: Você pode usar [!DNL Adobe Workfront Fusion] para se conectar a [!DNL Google Services] usar um cliente OAuth personalizado. Este procedimento requer um procedimento existente [!DNL Google] conta.
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: 7d2b4a9940cb21de1b8b5f2955f53b3d88040e44
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# Conectar [!DNL Adobe Workfront Fusion] para [!DNL Google Services] uso de um cliente OAuth personalizado

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
   <p>Atual: Não [!DNL Workfront Fusion] requisito de licença.</p>
   <p>Ou</p>
   <p>Herdados: Qualquer um </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Novo:</p> <ul><li>[!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Workfront] Plano: sua organização deve comprar [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plano: [!DNL Workfront Fusion] está incluído.</li></ul>
   <p>Ou</p>
   <p>Atual: sua organização deve comprar [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Você precisa de um existente [!DNL Google] para fazer essa conexão.

## Conectar o Fusion aos serviços da Google usando um cliente OAuth personalizado

Para criar essa conexão, você deve criar e configurar um projeto na plataforma Google Cloud e, em seguida, configurar a conexão no Fusion com base nesse projeto.

* [Criar um projeto em [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform)
* [Configurar [!UICONTROL Consentimento OAuth] configurações](#configure-oauth-consent-settings)
* [Criar credenciais do OAuth](#create-oauth-credentials)
* [Conectar a [!DNL Google] in [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion)

>[!NOTE]
>
>Este procedimento destina-se a:
>
>* Uso pessoal ([!DNL `@gmail.com`] e [!DNL `@googlemail.com`] usuários)
>* Uso interno ([!DNL G Suite] usuários que preferem usar um cliente OAuth personalizado)

### Criar um projeto em [!DNL Google Cloud Platform]

Para criar um projeto em [!DNL Google Cloud] Plataforma:

1. Fazer logon em [[!DNL Google Cloud] Platform](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) usar seu [!DNL Google] credenciais.
1. No painel esquerdo, clique em **[!UICONTROL Painel]**.
1. Clique em **[!UICONTROL Criar projeto]** no canto superior direito da tela.
1. Insira o **[!UICONTROL Nome do projeto]** e, em seguida, clique em **[!UICONTROL Criar]**.

1. Clique em **[!UICONTROL Habilitar APIs e serviços]** perto da parte superior da tela.
1. No **[!UICONTROL Pesquisar APIs e serviços]** na parte superior da tela, digite o nome do serviço que deseja usar (como [!DNL Gmail] API ou [!DNL Google Drive] API).
1. Quando for exibido, clique na API ou no serviço ao qual deseja se conectar [!DNL Workfront Fusion].
1. Clique em **[!UICONTROL Ativar]** para habilitar a API selecionada.
1. Repita as etapas 6 a 8 para cada API que deseja ativar.

   >[!NOTE]
   >
   >Você deve ativar [!DNL Google Drive] API, bem como a API de todas as [!DNL Google] aplicativos que deseja usar (como [!DNL Google Sheets] API).

1. Na tela exibida, clique em **[!UICONTROL Criar credenciais]** no canto superior direito.
1. Continue até a seção [Definir configurações de consentimento do OAuth](#configure-oauth-consent-settings) neste artigo.

### Configurar [!UICONTROL Consentimento OAuth] configurações

1. No painel esquerdo, clique em **[!UICONTROL Tela de consentimento do OAuth]**.
1. Selecionar **[!UICONTROL Externo]** e, em seguida, clique em **[!UICONTROL Criar]**.

   >[!NOTE]
   >
   >Você não será cobrado ao selecionar essa opção. Para obter mais informações, consulte [!DNL Google]Informações do sobre exceções aos requisitos de verificação.

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
   >Você não precisa enviar sua tela de consentimento e o pedido para verificação até [!DNL Google].

1. Continue para [Criar credenciais do OAuth](#create-oauth-credentials).

### Criar credenciais do OAuth

1. No painel esquerdo, clique em **[!UICONTROL Credenciais]**.

   >[!NOTE]
   >
   >Se essa não for a primeira API ou serviço ([!DNL Gmail] ou [!DNL Google Drive]) você ativou, não é necessário criar novas credenciais.

1. Clique em **[!UICONTROL Criar credenciais]** próximo à parte superior da tela, selecione **[!UICONTROL ID do cliente OAuth]** no menu suspenso.

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

1. Em [!UICONTROL URIs de redirecionamento autorizados], clique em **[!UICONTROL Adicionar URI]** e insira **um** do seguinte:

   * Para [!DNL Gmail] ou [!DNL Google Drive]: `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * Para outras [!DNL Google] aplicativos: `https://app.workfrontfusion.com/oauth/cb/google`

1. Clique em **[!UICONTROL Criar]**.

   A variável [!UICONTROL ID do cliente] e [!UICONTROL Segredo do cliente] exibição.

1. Copie o [!UICONTROL ID do cliente] e [!UICONTROL Segredo do cliente] para um local seguro. Você os usará para fazer uma conexão no [!DNL Workfront Fusion].
1. Continue para [Conectar a [!DNL Google] in [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion).

### Conectar a [!DNL Google] in [!DNL Workfront Fusion]

O processo de criação de uma conexão com o [!DNL Google] diferente dependendo se você está usando um módulo de um [!DNL Google] serviço(como [!DNL Google Sheets] ou [!DNL Google Docs]), ou se você estiver se conectando a [!DNL Google] por meio da [!UICONTROL HTTP] >[!UICONTROL Criar um OAuth2.0] módulo de solicitação.

* [Conectar a [!DNL Google] em um [!DNL Google] serviço](#connect-to-google-in-a-google-service)
* [Conectar a [!DNL Google] no [!UICONTROL HTTP] > [!UICONTROL Fazer uma solicitação do OAuth2.0] módulo](#connect-to-google-in-the-http--make-an-oauth20-request-module)

#### Conectar a [!DNL Google] em um [!DNL Google] serviço

1. Entrada [!DNL Workfront Fusion], localize o [!DNL Google] que você precisa criar uma conexão para.
1. Clique em **[!UICONTROL Criar uma conexão]** e, em seguida, clique em **[!UICONTROL Mostrar configurações avançadas]**.

1. Insira o [!UICONTROL ID do cliente] e [!UICONTROL Segredo do cliente] você recuperou em [[!UICONTROL Criar credenciais do OAuth]](#create-oauth-credentials) nos respectivos campos, depois clique em **[!UICONTROL Continuar]**.

1. Entre com seu [!DNL Google] conta.

   A variável **[!UICONTROL Este aplicativo não foi verificado]** é exibida. Observe que o &quot;aplicativo&quot; mencionado no título da janela é o cliente OAuth criado acima.

1. Clique em **[!UICONTROL Avançado]** e, em seguida, clique em **[!UICONTROL Ir para [!DNL Workfront Fusion] (não seguro)]** para permitir o acesso usando seu cliente OAuth personalizado.

1. Clique em **[!UICONTROL Permitir]** a conceder [!DNL Workfront Fusion] permissão.
1. Na janela exibida, clique em **[!UICONTROL Permitir]** novamente para confirmar suas escolhas.

   A conexão com o servidor [!DNL Google] serviço usando um cliente OAuth personalizado é estabelecido.

#### Conectar a [!DNL Google] no [!UICONTROL HTTP] > [!UICONTROL Fazer uma solicitação do OAuth2.0] módulo {#connect-to-google-in-the-http--make-an-oauth20-request-module}

Para obter instruções sobre como se conectar ao [!DNL Google] no [!UICONTROL HTTP] > [!UICONTROL Fazer uma solicitação do OAuth2.0] módulo, consulte [Instruções para criar uma conexão com o [!DNL Google] no [!UICONTROL HTTP] > [!UICONTROL Fazer uma solicitação do OAuth 2.0] módulo](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module) in [[!UICONTROL HTTP] > [!UICONTROL Fazer uma solicitação do OAuth 2.0] módulo](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## Possível mensagem de erro:[!UICONTROL [403] Acesso não configurado]

Se a variável [!UICONTROL `403 Access Not Configured`] for exibida, será necessário habilitar a API correspondente na Google Cloud Platform. Para habilitar a API, siga as etapas na seção [Criar um projeto em [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) neste artigo.
