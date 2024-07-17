---
title: Criar aplicativos OAuth2 para  [!DNL Workfront] integrações
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Como administrador do  [!DNL Adobe Workfront] , você pode criar aplicativos OAuth2 para sua instância do  [!DNL Workfront], que permitem que outros aplicativos acessem o Workfront. Seus usuários podem conceder permissão a esses outros aplicativos para acessar os dados do Workfront. Dessa forma, você pode integrar o Workfront com os aplicativos de sua escolha, incluindo seus próprios aplicativos internos.
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: e13c7dda-8945-47ad-b6d3-4d6a62b368f5
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '1956'
ht-degree: 6%

---

# Criar aplicativos OAuth2 para integrações de [!DNL Workfront]

Como administrador [!DNL Adobe Workfront], você pode criar aplicativos OAuth2 para sua instância do [!DNL Workfront], que permitem que outros aplicativos acessem [!DNL Workfront]. Seus usuários podem conceder permissão a esses outros aplicativos para acessar os dados do [!DNL Workfront]. Dessa forma, é possível integrar   com aplicativos de sua escolha, incluindo aplicativos internos.

Ao criar um aplicativo [!UICONTROL OAuth2], você gera uma ID do cliente e um Segredo do cliente. Seus usuários podem usar a ID do cliente em chamadas de API para integrar com o aplicativo criado.

>[!NOTE]
>
>No contexto de OAuth2, &quot;criação de um aplicativo&quot; refere-se ao processo de criação desse tipo de link de acesso entre um aplicativo e um servidor, como [!DNL Workfront].

* Para obter instruções sobre como configurar e usar o aplicativo OAuth2 com credenciais de usuário (fluxo de código de autorização), consulte [Configurar e usar os aplicativos OAuth 2 personalizados da sua organização usando o fluxo de código de autorização](../../wf-api/api/oauth-app-code-token-flow.md).
* Para obter instruções sobre como configurar e usar o aplicativo OAuth2 usando a autenticação de servidor (fluxo JWT), consulte [Configurar e usar os aplicativos OAuth 2 personalizados da sua organização usando o fluxo JWT](../../wf-api/api/oauth-app-jwt-flow.md).
* Para obter instruções sobre como configurar e usar o aplicativo OAuth2 usando o PKCE, consulte [Configurar e usar os aplicativos OAuth 2 personalizados de sua organização usando o fluxo de PKCE](../../wf-api/api/oauth-app-pkce-flow.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td><p>Novo: [!UICONTROL Padrão]</p>
   Ou
   <p>Atual:[!UICONTROL Plano]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> Você deve ser um administrador [!DNL Workfront]. </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

+++

## Visão geral do OAuth2

Imagine que um aplicativo deve obter algumas informações específicas de [!DNL Workfront]. Um aplicativo que solicita informações é chamado de cliente. Para este exemplo, o nome do cliente é ClientApp. O ClientApp precisa acessar as informações de um usuário específico e, portanto, deve acessar [!DNL Workfront] como esse usuário. Se o usuário fornecer ao ClientApp o nome de usuário e a senha, ele poderá acessar todos os dados que o usuário puder acessar. Esse é um risco de segurança, pois o ClientApp precisa apenas de um conjunto pequeno e específico de informações.

Ao criar um aplicativo OAuth2 para ClientApp, você basicamente diz a [!DNL Workfront] que o ClientApp tem permissão para acessar [!DNL Workfront], mas somente se o usuário cuja conta o ClientApp está acessando conceder permissão para o acesso.

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
   <td> <p>Melhor para CLIs, daemons ou scripts em execução no servidor</p> <p>Exemplos:</p> 
    <ul> 
     <li> <p>[!DNL Shell] </p> </li> 
     <li> <p>[!DNL Python]</p> </li> 
    </ul> </td> 
   <td> <p>Autenticação por meio de Token da web JSON com codificação de par de chaves pública/privada.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Aplicativo web de página única</p> </td> 
   <td> <p>Melhor para aplicativos web móveis ou de página única</p> <p>Exemplos:</p> 
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
   <td> <p>Melhor para aplicativos do lado do servidor que lidam com credenciais e tokens no servidor</p> <p>Exemplos:</p> 
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
>Você pode ter até dez aplicativos OAuth2 ao mesmo tempo.

* [Criar um aplicativo OAuth2 usando autenticação de servidor (fluxo JWT)](#create-an-oauth2-application-using-server-authentication-jwt-flow)
* [Criar um aplicativo OAuth2 usando credenciais do usuário (Fluxo de código de autorização)](#create-an-oauth2-application-using-user-credentials-authorization-code-flow)
* [Criar um aplicativo web de página única OAuth2 usando PKCE](#create-an-oauth2-single-page-web-application-using-pkce)

### Criar um aplicativo OAuth2 usando autenticação de servidor (fluxo JWT) {#create-an-oauth2-application-using-server-authentication-jwt-flow}

{{step-1-to-setup}}

1. No painel de navegação esquerdo, clique em **[!UICONTROL Sistema]** e selecione **[!UICONTROL Aplicativos OAuth2]**.
1. Clique em **[!UICONTROL Criar integração de aplicativo]**.
A caixa **Novo aplicativo OAuth2** é exibida.
1. Na caixa **Novo aplicativo OAuth2**, selecione **[!UICONTROL Computador para Aplicativo de Computador]**.
1. Digite um nome para o novo aplicativo, como &quot;[!DNL Workfront] para ClientApp.&quot;
1. Clique em **[!UICONTROL Criar]**.
1. Preencha os campos do novo aplicativo.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID do Cliente]</td> 
      <td> <p>Este campo é gerado automaticamente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Segredo do cliente]</td> 
      <td> <p>Este campo é gerado automaticamente</p> <p><b>IMPORTANTE</b>:  <p>Copie o conteúdo desse campo para outro arquivo seguro antes de fechar esta página. Você não poderá ver essa chave secreta novamente.</p> <p>Se você perder essa chave, exclua-a e crie um Segredo do cliente.</p> 
        <ol> 
         <li value="1"> <p>Clique no ícone <img src="assets/delete.png"> <b>[!UICONTROL Excluir]</b> para excluir o Segredo do Cliente atual.</p> </li> 
         <li value="2"> <p>Clique em <b>[!UICONTROL Adicionar segredo do cliente]</b> para gerar um novo Segredo do Cliente.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Chaves Públicas]</td> 
      <td> <p>Os aplicativos de servidor para servidor usam chaves públicas e privadas para autenticação. Siga um destes procedimentos:</p> 
       <ul> 
        <li> <p>Clique em <b>[!UICONTROL Adicionar uma chave pública]</b> e insira a chave pública do outro aplicativo.</p> </li> 
        <li> <p>Clique em <b>[!UICONTROL Gerar um par de chaves públicas/privadas]</b> e compartilhe a chave pública com o outro aplicativo.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome]</td> 
      <td>Este é o mesmo nome que você deu ao aplicativo. Este campo não pode estar vazio.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrição]</td> 
      <td>Insira uma descrição para a integração.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Salvar]**.

Para obter instruções sobre como configurar e usar o aplicativo OAuth2 com credenciais de usuário (fluxo de código de autorização), consulte [Configurar e usar os aplicativos OAuth 2 personalizados da sua organização usando o fluxo JWT](../../wf-api/api/oauth-app-jwt-flow.md).

### Criar um aplicativo OAuth2 usando credenciais do usuário (Fluxo de código de autorização) {#create-an-oauth2-application-using-user-credentials-authorization-code-flow}

{{step-1-to-setup}}

1. No painel de navegação esquerdo, clique em **[!UICONTROL Sistema]** e selecione **[!UICONTROL Aplicativos OAuth2]**.
1. Clique em **[!UICONTROL Criar integração de aplicativo]**.

   O **Novo aplicativo OAuth2** é exibido.
1. Na caixa **Novo aplicativo OAuth2**, selecione **[!UICONTROL Aplicativo Web]**.
1. Digite um nome para o novo aplicativo OAuth2, como &quot;[!DNL Workfront] para ClientApp.&quot;
1. Clique em **[!UICONTROL Criar]**.
1. Preencha os campos do novo aplicativo.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID do Cliente]</td> 
      <td> <p>Este campo é gerado automaticamente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Segredo do cliente]</td> 
      <td> <p>Este campo é gerado automaticamente</p> <p><b>IMPORTANTE</b>:  <p>Copie o conteúdo desse campo para outro arquivo seguro antes de fechar esta página. Você não poderá ver essa chave secreta novamente.</p> <p>Se você perder essa chave, exclua-a e crie um Segredo do cliente.</p> 
        <ol> 
         <li value="1"> <p>Clique no ícone <img src="assets/delete.png"> <b>[!UICONTROL Excluir]</b> para excluir o Segredo do Cliente atual.</p> </li> 
         <li value="2"> <p>Clique em <b>[!UICONTROL Adicionar segredo do cliente]</b> para gerar um novo Segredo do Cliente.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Redirecionar URLs]</td> 
      <td>Os usuários serão redirecionados para este caminho após a autenticação com [!DNL Workfront].</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Atualizar rotação de token]</td> 
      <td>Habilite esta opção para emitir um novo token de atualização sempre que o token de atualização for usado. Seu aplicativo deve armazenar o novo token de atualização após cada atualização.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Expiração de token de atualização absoluta]</td> 
      <td> <p>Selecione por quanto tempo você deseja que um token de atualização exista antes de expirar. Quando ela expirar, os usuários deverão fazer logon na integração novamente. Selecione "[!UICONTROL Sem expiração]" se não quiser que o token de atualização expire.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Expiração do token para atualizar inatividade</td> 
      <td> <p>Selecione o tempo após o qual, se o usuário não tiver estado ativo no sistema, o token de atualização expirará. </p> <p>Por exemplo, se a expiração do token de atualização de inatividade for de seis meses e o usuário não fizer logon por seis meses, o token de atualização expirará mesmo que a expiração do token de atualização absoluta possa ser definida por mais tempo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Logotipo]</td> 
      <td>Você pode adicionar um logotipo para tornar este aplicativo mais identificável. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome]</td> 
      <td>Este é o mesmo nome que você deu ao aplicativo. Este campo não pode estar vazio.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrição]</td> 
      <td>Insira uma descrição para a integração.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL da Descrição do Aplicativo]</td> 
      <td>Pode ser um link para uma página "Sobre nós" ou uma página com mais informações sobre a integração.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Salvar]**.

Para obter instruções sobre como configurar e usar o aplicativo OAuth2 com credenciais de usuário (fluxo de código de autorização), consulte [Configurar e usar os aplicativos OAuth 2 personalizados da sua organização usando o fluxo de código de autorização](../../wf-api/api/oauth-app-code-token-flow.md).

### Criar um aplicativo web de página única OAuth2 usando PKCE {#create-an-oauth2-single-page-web-application-using-pkce}

{{step-1-to-setup}}

1. No painel de navegação esquerdo, clique em **[!UICONTROL Sistema]** e selecione **[!UICONTROL Aplicativos OAuth2]**.
1. Clique em **[!UICONTROL Criar integração de aplicativo]**.

   A caixa **Novo aplicativo OAuth2** é exibida.
1. Na caixa **Novo aplicativo OAuth2**, selecione **[!UICONTROL Aplicativo Web de Página Única]**.
1. Digite um nome para o novo aplicativo [!UICONTROL OAuth2], como &quot;[!DNL Workfront] para ClientApp.&quot;
1. Clique em **[!UICONTROL Criar]**.
1. Preencha os campos do novo aplicativo.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID do Cliente]</td> 
      <td> <p>Este campo é gerado automaticamente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Redirecionar URLs]</td> 
      <td>Os usuários serão redirecionados para esse caminho após a autenticação com o Workfront.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Girar token de atualização sempre que for usado]</td> 
      <td>Habilite esta opção para emitir um novo token de atualização sempre que o token de atualização for usado. Seu aplicativo deve armazenar o novo token de atualização após cada atualização.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Expiração absoluta]</td> 
      <td> <p>Selecione por quanto tempo você deseja que um token de atualização exista antes de expirar. Quando ela expirar, os usuários deverão fazer logon na integração novamente. Selecione "[!UICONTROL Sem expiração]" se não quiser que o token de atualização expire.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Expiração de inatividade]</td> 
      <td> <p>Selecione o tempo após o qual, se o usuário não tiver estado ativo no sistema, o token de atualização expirará. </p> <p>Por exemplo, se a expiração do token de atualização de inatividade for de seis meses e o usuário não fizer logon por seis meses, o token de atualização expirará mesmo que a expiração do token de atualização absoluta possa ser definida por mais tempo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Logotipo]</td> 
      <td>Você pode adicionar um logotipo para tornar este aplicativo mais identificável. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome]</td> 
      <td>Este é o mesmo nome que você deu ao aplicativo. Este campo não pode estar vazio.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrição]</td> 
      <td>Insira uma descrição para a integração.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome do desenvolvedor]</td> 
      <td>Esse é o nome do desenvolvedor que está configurando o aplicativo OAuth2.</td> 
     </tr> 
   <tr> 
      <td role="rowheader">[!UICONTROL Endereço de email do desenvolvedor]</td> 
      <td>Esse é o endereço de email do desenvolvedor que está configurando o aplicativo OAuth2.</td> 
     </tr> 
   <tr> 
      <td role="rowheader">[!UICONTROL URL da política de privacidade]</td> 
      <td>Esse é o link para onde sua organização armazena a política de privacidade.</td> 
     </tr>


   </tbody> 
   </table>

   <!-- removed this from the table, and added "Developer name" and following rows:
   [!UICONTROL App Description URL]</td> 
      <td>This can be a link to an "About us" page or a page with more information about the integration.> -->

1. Clique em **[!UICONTROL Salvar]**.

## Configurar e usar o aplicativo OAuth2 criado

A configuração e o uso adicionais do aplicativo OAuth2 criado exigem algum conhecimento técnico, incluindo chamadas de API.

* Para obter instruções sobre como configurar e usar o aplicativo OAuth2 com credenciais de usuário (fluxo de código de autorização), consulte [Configurar e usar os aplicativos OAuth 2 personalizados da sua organização usando o fluxo de código de autorização](../../wf-api/api/oauth-app-code-token-flow.md).
* Para obter instruções sobre como configurar e usar o aplicativo OAuth2 usando a autenticação de servidor (fluxo JWT), consulte [Configurar e usar os aplicativos OAuth 2 personalizados da sua organização usando o fluxo JWT](../../wf-api/api/oauth-app-jwt-flow.md).
* Para obter instruções sobre como configurar e usar o aplicativo OAuth2 usando o PKCE, consulte [Configurar e usar os aplicativos OAuth 2 personalizados de sua organização usando o fluxo de PKCE](../../wf-api/api/oauth-app-pkce-flow.md).

## Processos OAuth2 para fluxo de código de autorização

>[!NOTE]
>
>Seus usuários acessam o aplicativo [!UICONTROL OAuth2] por meio da API. Esta seção descreve a funcionalidade em termos gerais e é fornecida apenas para fins informativos.
>
>Para obter instruções específicas sobre como usar o aplicativo OAuth2, incluindo chamadas de API específicas, consulte [Configurar e usar os aplicativos OAuth 2 personalizados de sua organização usando o fluxo de código de autorização](../../wf-api/api/oauth-app-code-token-flow.md).

### Autorização com um código de autorização e um token de acesso {#authorizing-with-an-authorization-code-and-access-token}

1. O ClientApp precisa de algumas informações de [!DNL Workfront], por isso envia uma solicitação para o ponto de extremidade `/authorize` da API [!DNL Workfront]. A solicitação inclui o [!UICONTROL response_type] `code`, que indica que a solicitação deve retornar um código de autorização.
1. Isso aciona [!DNL Workfront] para enviar um prompt de autenticação ao usuário. O usuário pode inserir suas credenciais no prompt, que fornece a [!DNL Workfront] permissão para se comunicar com o ClientApp. Se o usuário já estiver conectado ao [!DNL Workfront], esta etapa pode ser ignorada.
1. A API [!DNL Workfront] envia um código de autorização para o ClientApp.
1. O ClientApp envia as seguintes informações em uma solicitação para a API [!DNL Workfront] `/token`   endpoint:

   * O código de autorização enviado ao ClientApp na etapa 3. Isso identifica a instância específica da permissão do usuário.
   * O Segredo do Cliente gerado ao configurar o aplicativo OAuth2 do ClientApp em [!DNL Workfront]. Isso permite que [!DNL Workfront] saiba que a solicitação vem do ClientApp.

1. Se o código de autorização e o segredo do cliente estiverem corretos, [!DNL Workfront] enviará um token de acesso ao ClientApp. Este token de acesso é enviado diretamente de [!DNL Workfront] para ClientApp e não pode ser visualizado, copiado ou usado por nenhum outro usuário ou aplicativo cliente.
1. O ClientApp envia o token de acesso a [!DNL Workfront] junto com a solicitação específica de informações.
1. Como o token de acesso está correto, [!DNL Workfront] envia as informações para o ClientApp.

#### Atualização de tokens de acesso

Por questões de segurança, os tokens de acesso expiram após um curto período. Para obter novos tokens de acesso sem precisar inserir credenciais todas as vezes, [!DNL OAuth2] usa tokens de atualização. Os tokens de atualização são armazenados pelo cliente.

O processo para aquisição de um token de atualização é o mesmo que o procedimento discutido na seção [Autorização com um código de autorização e token de acesso](#authorizing-with-an-authorization-code-and-access-token). A solicitação do código de autorização inclui o escopo `offline_access`, que indica que a solicitação deve retornar um token de solicitação juntamente com o código de autorização.
