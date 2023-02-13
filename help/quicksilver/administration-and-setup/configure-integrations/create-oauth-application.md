---
title: Crie aplicativos OAuth2 para [!DNL Workfront] integrações
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Como um [!DNL Adobe Workfront] administrador, você pode criar aplicativos OAuth2 para sua instância de [!DNL Workfront], que permitem que outros aplicativos acessem o Workfront. Seus usuários podem conceder permissão a esses outros aplicativos para acessar seus dados do Workfront. Dessa forma, você pode integrar o Workfront com aplicativos de sua escolha, incluindo seus próprios aplicativos internos.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: e13c7dda-8945-47ad-b6d3-4d6a62b368f5
source-git-commit: f7e3182776e6b62103cd755b2fbd5057efc95394
workflow-type: tm+mt
source-wordcount: '1917'
ht-degree: 6%

---

# Crie aplicativos OAuth2 para [!DNL Workfront] integrações

Como um [!DNL Adobe Workfront] administrador, você pode criar aplicativos OAuth2 para sua instância de [!DNL Workfront], que permitem o acesso de outros aplicativos [!DNL Workfront]. Seus usuários podem conceder permissão a esses outros aplicativos para acessar seus [!DNL Workfront] dados. Dessa forma, você pode se integrar aos aplicativos de sua escolha, incluindo seus próprios aplicativos internos.

Ao criar um [!UICONTROL OAuth2] , você gera uma ID do cliente e um Segredo do cliente. Seus usuários podem usar a ID do cliente em chamadas de API para se integrar ao aplicativo criado.

>[!NOTE]
>
>No contexto do OAuth2, &quot;criar um aplicativo&quot; refere-se ao processo de criação desse tipo de link de acesso entre um aplicativo e um servidor, como [!DNL Workfront].

* Para obter instruções sobre como configurar e usar o aplicativo OAuth2 com credenciais de usuário (fluxo do código de autorização), consulte [Configure e use os aplicativos OAuth 2 personalizados de sua organização usando o fluxo do código de autorização](../../wf-api/api/oauth-app-code-token-flow.md).
* Para obter instruções sobre como configurar e usar o aplicativo OAuth2 usando autenticação de servidor (fluxo JWT), consulte [Configure e use os aplicativos OAuth 2 personalizados de sua organização usando o fluxo JWT](../../wf-api/api/oauth-app-jwt-flow.md).
* Para obter instruções sobre como configurar e usar o aplicativo OAuth2 usando PKCE, consulte [Configure e use os aplicativos OAuth 2 personalizados de sua organização usando o fluxo PKCE](../../wf-api/api/oauth-app-pkce-flow.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!UICONTROL Pro] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> Você deve ser um [!DNL Workfront] administrador. </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Visão geral do OAuth2

Imagine que um aplicativo precisa obter algumas informações específicas do [!DNL Workfront]. Um aplicativo que solicita informações é chamado de cliente. Neste exemplo, o nome do cliente é ClientApp. O ClientApp precisa acessar as informações de um usuário específico e, portanto, precisa acessar [!DNL Workfront] como esse usuário. Se o usuário fornecer ao ClientApp o nome de usuário e a senha, o ClientApp poderá acessar todos os dados que o usuário pode acessar. Esse é um risco para a segurança, pois o ClientApp precisa apenas de um pequeno conjunto específico de informações.

Ao criar um aplicativo OAuth2 para ClientApp, você basicamente informa [!DNL Workfront] que o ClientApp tem permissão para acessar [!DNL Workfront], mas somente se o usuário cuja conta ClientApp está acessando conceder permissão para o acesso.

## Criar um aplicativo OAuth2

Ao criar um aplicativo OAuth2, escolha o tipo de aplicativo que melhor atenda às necessidades de sua integração.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de aplicativo</th> 
   <th>Melhor para</th> 
   <th>Método de autenticação</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Aplicativo de máquina para máquina</p> </td> 
   <td> <p>Melhor para CLIs, daemons ou scripts em execução no seu servidor</p> <p>Exemplos:</p> 
    <ul> 
     <li> <p>[!DNL Shell] </p> </li> 
     <li> <p>[!DNL Python]</p> </li> 
    </ul> </td> 
   <td> <p>Autenticação por meio de Token da web JSON com codificação de par de chaves pública/privada.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Aplicativo web de página única</p> </td> 
   <td> <p>Melhor para aplicativos móveis ou de página única da Web</p> <p>Exemplos:</p> 
    <ul> 
     <li> <p>[!DNL Javascript]</p> </li> 
     <li> <p>[!DNL Angular]</p> </li> 
     <li> <p>[!DNL React]</p> </li> 
     <li> <p>[!DNL Vue]</p> </li> 
    </ul> </td> 
   <td> <p>Autenticação por meio do fluxo de código de autorização OAuth 2.0 com chave de prova para troca de código (PKCE).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Aplicativo web</p> </td> 
   <td> <p>O melhor para aplicativos do lado do servidor que lidam com credenciais e tokens no servidor</p> <p>Exemplos:</p> 
    <ul> 
     <li> <p>[!DNL Go]</p> </li> 
     <li> <p>[!DNL Java]</p> </li> 
     <li> <p>[!DNL ASP.Net]</p> </li> 
     <li> <p>[!DNL Node.js]</p> </li> 
     <li> <p>[!DNL PHP]</p> </li> 
    </ul> </td> 
   <td> <p>Autenticação por meio do fluxo de código de autorização OAuth 2.0.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Você pode ter até dez aplicativos OAuth2 por vez.

* [Criar um aplicativo OAuth2 usando autenticação de servidor (fluxo JWT)](#create-an-oauth2-application-using-server-authentication-jwt-flow)
* [Criar um aplicativo OAuth2 usando credenciais do usuário (fluxo do código de autorização)](#create-an-oauth2-application-using-user-credentials-authorization-code-flow)
* [Criar um aplicativo Web de página única OAuth2 usando PKCE](#create-an-oauth2-single-page-web-application-using-pkce)

### Criar um aplicativo OAuth2 usando autenticação de servidor (fluxo JWT) {#create-an-oauth2-application-using-server-authentication-jwt-flow}

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. No painel de navegação esquerdo, clique em **[!UICONTROL Sistema]**, em seguida selecione **[!UICONTROL Aplicativos OAuth]**.
1. Clique em **[!UICONTROL Criar integração de aplicativo]**.
1. Na janela exibida, selecione **[!UICONTROL Autenticação de servidor]**.
1. Insira um nome para o novo aplicativo, como &quot;[!DNL Workfront] para ClientApp.&quot;
1. Clique em **[!UICONTROL Criar]**.
1. Preencha os campos do novo aplicativo.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td> <p>Este campo é gerado automaticamente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Segredo do cliente]</td> 
      <td> <p>Este campo é gerado automaticamente</p> <p><b>IMPORTANTE</b>:  <p>Copie o conteúdo desse campo para outro arquivo seguro antes de fechar esta página. Você não poderá ver esta chave secreta novamente.</p> <p>Se você perder essa chave, exclua-a e crie um novo Segredo do cliente.</p> 
        <ol> 
         <li value="1"> <p>Clique no botão <b>[!UICONTROL Excluir]</b> ícone <img src="assets/delete.png"> para excluir o Segredo do Cliente atual.</p> </li> 
         <li value="2"> <p>Clique em <b>[!UICONTROL Adicionar segredo do cliente]</b> para gerar um novo Segredo do Cliente.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Chaves públicas]</td> 
      <td> <p>Aplicativos de servidor para servidor usam chaves públicas e privadas para autenticação. Siga um destes procedimentos:</p> 
       <ul> 
        <li> <p>Clique em <b>[!UICONTROL Adicionar uma chave pública]</b> e insira a chave pública do outro aplicativo.</p> </li> 
        <li> <p>Clique em <b>[!UICONTROL Gerar um par de chaves público/privado]</b>, em seguida, compartilhe a chave pública com o outro aplicativo.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Esse é o mesmo nome que você deu ao aplicativo. Este campo não pode estar vazio.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrição]</td> 
      <td>Insira uma descrição para a integração.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Salvar]**.

Para obter instruções sobre como configurar e usar o aplicativo OAuth2 com credenciais de usuário (fluxo do código de autorização), consulte [Configure e use os aplicativos OAuth 2 personalizados de sua organização usando o fluxo JWT](../../wf-api/api/oauth-app-jwt-flow.md).

### Criar um aplicativo OAuth2 usando credenciais do usuário (fluxo do código de autorização) {#create-an-oauth2-application-using-user-credentials-authorization-code-flow}

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).
1. No painel de navegação esquerdo, clique em **[!UICONTROL Sistema]**, em seguida selecione **[!UICONTROL Aplicativos OAuth]**.
1. Clique em **[!UICONTROL Criar integração de aplicativo]**.
1. Na janela exibida, selecione **[!UICONTROL Autenticação do usuário]**.
1. Insira um nome para o novo aplicativo OAuth2, como &quot;[!DNL Workfront] para ClientApp.&quot;
1. Clique em **[!UICONTROL Criar]**.
1. Preencha os campos do novo aplicativo.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td> <p>Este campo é gerado automaticamente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Segredo do cliente]</td> 
      <td> <p>Este campo é gerado automaticamente</p> <p><b>IMPORTANTE</b>:  <p>Copie o conteúdo desse campo para outro arquivo seguro antes de fechar esta página. Você não poderá ver esta chave secreta novamente.</p> <p>Se você perder essa chave, exclua-a e crie um novo Segredo do cliente.</p> 
        <ol> 
         <li value="1"> <p>Clique no botão <b>[!UICONTROL Excluir]</b> ícone <img src="assets/delete.png"> para excluir o Segredo do Cliente atual.</p> </li> 
         <li value="2"> <p>Clique em <b>[!UICONTROL Adicionar segredo do cliente]</b> para gerar um novo Segredo do Cliente.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Redirecionar URLs]</td> 
      <td>Os usuários serão redirecionados para esse caminho após terem sido autenticados com [!DNL Workfront].</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Atualizar rotação de token]</td> 
      <td>Ative esta opção para emitir um novo token de atualização sempre que o token de atualização for usado. Seu aplicativo deve armazenar o novo token de atualização após cada atualização.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Expiração absoluta do token de atualização]</td> 
      <td> <p>Selecione o tempo que deseja que um token de atualização exista antes que ele expire. Quando expirar, os usuários deverão fazer logon na integração novamente. Selecione "[!UICONTROL Sem expiração]" se não quiser que o token de atualização expire.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Expiração do token para atualizar inatividade</td> 
      <td> <p>Selecione o tempo após o qual, se o usuário não tiver estado ativo em seu sistema, o token de atualização expirará. </p> <p>Por exemplo, se a expiração do token de atualização da inatividade for de 6 meses e o usuário não fizer logon por seis meses, o token de atualização expirará mesmo que a expiração absoluta do token de atualização possa ser definida por mais tempo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Logo]</td> 
      <td>Você pode adicionar um logotipo para tornar este aplicativo mais identificável. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Esse é o mesmo nome que você deu ao aplicativo. Este campo não pode estar vazio.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrição]</td> 
      <td>Insira uma descrição para a integração.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL de descrição do aplicativo]</td> 
      <td>Pode ser um link para uma página "Sobre nós" ou uma página com mais informações sobre a integração.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Salvar]**.

Para obter instruções sobre como configurar e usar o aplicativo OAuth2 com credenciais de usuário (fluxo do código de autorização), consulte [Configure e use os aplicativos OAuth 2 personalizados de sua organização usando o fluxo do código de autorização](../../wf-api/api/oauth-app-code-token-flow.md).

### Criar um aplicativo Web de página única OAuth2 usando PKCE {#create-an-oauth2-single-page-web-application-using-pkce}

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).
1. No painel de navegação esquerdo, clique em **[!UICONTROL Sistema]**, em seguida selecione **[!UICONTROL Aplicativos OAuth]**.
1. Clique em **[!UICONTROL Criar integração de aplicativo]**.
1. Na janela exibida, selecione **[!UICONTROL Aplicativo web de página única]**.
1. Insira um nome para o novo [!UICONTROL OAuth2] aplicativo, como &quot;[!DNL Workfront] para ClientApp.&quot;
1. Clique em **[!UICONTROL Criar]**.
1. Preencha os campos do novo aplicativo.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td> <p>Este campo é gerado automaticamente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Redirecionar URLs]</td> 
      <td>Os usuários serão redirecionados para esse caminho após terem sido autenticados com o Workfront.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Atualizar rotação de token]</td> 
      <td>Ative esta opção para emitir um novo token de atualização sempre que o token de atualização for usado. Seu aplicativo deve armazenar o novo token de atualização após cada atualização.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Expiração absoluta do token de atualização]</td> 
      <td> <p>Selecione o tempo que deseja que um token de atualização exista antes que ele expire. Quando expirar, os usuários deverão fazer logon na integração novamente. Selecione "[!UICONTROL Sem expiração]" se não quiser que o token de atualização expire.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Expiração do token de atualização da inatividade]</td> 
      <td> <p>Selecione o tempo após o qual, se o usuário não tiver estado ativo em seu sistema, o token de atualização expirará. </p> <p>Por exemplo, se a expiração do token de atualização da inatividade for de 6 meses e o usuário não fizer logon por seis meses, o token de atualização expirará mesmo que a expiração absoluta do token de atualização possa ser definida por mais tempo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Logo]</td> 
      <td>Você pode adicionar um logotipo para tornar este aplicativo mais identificável. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Esse é o mesmo nome que você deu ao aplicativo. Este campo não pode estar vazio.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrição]</td> 
      <td>Insira uma descrição para a integração.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL de descrição do aplicativo]</td> 
      <td>Pode ser um link para uma página "Sobre nós" ou uma página com mais informações sobre a integração.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Salvar]**.

## Configurar e usar o aplicativo OAuth2 criado

A configuração e o uso adicionais do aplicativo OAuth2 criado exigem conhecimento técnico, incluindo chamadas de API.

* Para obter instruções sobre como configurar e usar o aplicativo OAuth2 com credenciais de usuário (fluxo do código de autorização), consulte [Configure e use os aplicativos OAuth 2 personalizados de sua organização usando o fluxo do código de autorização](../../wf-api/api/oauth-app-code-token-flow.md).
* Para obter instruções sobre como configurar e usar o aplicativo OAuth2 usando autenticação de servidor (fluxo JWT), consulte [Configure e use os aplicativos OAuth 2 personalizados de sua organização usando o fluxo JWT](../../wf-api/api/oauth-app-jwt-flow.md).
* Para obter instruções sobre como configurar e usar o aplicativo OAuth2 usando PKCE, consulte [Configure e use os aplicativos OAuth 2 personalizados de sua organização usando o fluxo PKCE](../../wf-api/api/oauth-app-pkce-flow.md).

## Processos OAuth2 para fluxo de código de autorização

>[!NOTE]
>
>Seus usuários acessam o [!UICONTROL OAuth2] por meio da API. Esta seção descreve a funcionalidade em termos gerais e é fornecida apenas para informações.
>
>Para obter instruções específicas sobre como usar o aplicativo OAuth2, incluindo chamadas de API específicas, consulte [Configure e use os aplicativos OAuth 2 personalizados de sua organização usando o fluxo do código de autorização](../../wf-api/api/oauth-app-code-token-flow.md).

### Autorização com um código de autorização e token de acesso {#authorizing-with-an-authorization-code-and-access-token}

1. O ClientApp precisa de algumas informações do [!DNL Workfront], portanto, envia uma solicitação para a [!DNL Workfront] API `/authorize` endpoint . A solicitação inclui a variável [!UICONTROL response_type] `code`, que indica que o pedido deve retornar um código de autorização.
1. Isso aciona [!DNL Workfront] para enviar um prompt de autenticação ao usuário. O usuário pode inserir suas credenciais no prompt, que fornece [!DNL Workfront] permissão para se comunicar com o ClientApp. Se o usuário já estiver conectado [!DNL Workfront], esta etapa pode ser ignorada.
1. O [!DNL Workfront] A API envia um código de autorização para o ClientApp.
1. O ClientApp envia as seguintes informações em uma solicitação para o [!DNL Workfront] API `/token`   endpoint:

   * O código de autorização enviado para o ClientApp na etapa 3. Isso identifica a instância específica da permissão do usuário.
   * O Segredo do cliente que foi gerado quando você configurou o aplicativo OAuth2 do ClientApp em [!DNL Workfront]. Isso permite [!DNL Workfront] para saber que a solicitação vem do ClientApp.

1. Se o código de autorização e o segredo do cliente estiverem corretos, [!DNL Workfront] envia um token de acesso para o ClientApp. Este token de acesso é enviado diretamente de [!DNL Workfront] para o ClientApp e não pode ser visualizado, copiado ou usado por qualquer outro usuário ou aplicativo cliente.
1. O ClientApp envia o token de acesso para o [!DNL Workfront] juntamente com o pedido específico de informações.
1. Como o token de acesso está correto, [!DNL Workfront] envia as informações para o ClientApp.

#### Atualização de tokens de acesso

Para fins de segurança, os tokens de acesso expiram após um curto período de tempo. Para obter novos tokens de acesso sem precisar inserir credenciais todas as vezes, [!DNL OAuth2] O usa tokens de atualização. Os tokens de atualização são armazenados pelo cliente.

O processo para adquirir um token de atualização é o mesmo do procedimento discutido na seção [Autorização com um código de autorização e token de acesso](#authorizing-with-an-authorization-code-and-access-token). O pedido de código de autorização inclui o âmbito `offline_access`, que indica que a solicitação deve retornar um token de solicitação junto com o código de autorização.
