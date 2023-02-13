---
title: Chame a API REST do MS Graph por meio do [!DNL Adobe Workfront Fusion] HTTP &gt; Faça um módulo de solicitação do OAuth 2.0
description: Chame a API REST do MS Graph por meio do [!DNL Adobe Workfront Fusion] HTTP &gt; Faça um módulo de solicitação do OAuth 2.0
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 1%

---

# Chame o[!UICONTROL  API REST do MS Graph] através da [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Fazer uma solicitação do OAuth 2.0] módulo

Muitas [!DNL Microsoft] os serviços da Web são acessados por meio do [!DNL Microsoft Graph API]. Este artigo descreve como criar uma conexão com essa API usando o [!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL Fazer uma solicitação do OAuth 2.0] módulo.

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

## Registrar [!DNL Workfront Fusion] no [!DNL Microsoft Application Registration Portal]

Para criar uma conexão com o [!DNL Microsoft Graph REST API], você deve primeiro se registrar [!DNL Adobe Workfront Fusion].

1. Começar a registrar um novo aplicativo conforme descrito em [Registrar seu aplicativo](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) no [!DNL Microsoft] documentação.

   Como parte do registro, [!DNL Microsoft] O exige as seguintes informações:

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Application name]</td>
        <td>Insira um nome para o aplicativo, como "Meu [!DNL Workfront Fusion] aplicativo."</td>
      </tr>
      <tr>
        <td>[!UICONTROL Redirecionar URL]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. Depois de concluir o registro do aplicativo, anote o [!UICONTROL ID do aplicativo].

   >[!IMPORTANT]
   >
   >Você precisará da ID do aplicativo para configurar a conexão no [!DNL Workfront Fusion].

1. Gere um [!UICONTROL Segredo do aplicativo]. Anote este segredo.

   Para obter instruções, consulte [Registrar seu aplicativo](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) no [!DNL Microsoft] documentação.

   >[!IMPORTANT]
   >
   >Você precisará do [!UICONTROL Segredo do aplicativo] para configurar sua conexão no [!DNL Workfront Fusion].

1. Configure as permissões para seu aplicativo.

   Para obter detalhes específicos sobre como localizar e configurar esses campos, consulte a seção &quot;Configurar permissões para o Gráfico Microsoft&quot; em [Obter acesso sem um usuário](https://docs.microsoft.com/en-us/graph/auth-v2-service) no [!UICONTROL Microsoft] documentação.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Que tipo de permissões seu aplicativo requer?]</td> 
      <td>Selecionar <code>[!UICONTROL Delegated permissions]</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Selecionar permissões]</td> 
      <td> <p>Selecione as seguintes permissões:</p> 
       <ul> 
        <li> <p><code>offline_access</code> </p> </li> 
        <li> <p><code>openid</code> </p> </li> 
        <li> <p>Quaisquer outras permissões necessárias às integrações (Exemplo: <code>User.Read</code>)</p> </li> 
       </ul> <p>Importante: Você precisará das permissões selecionadas para configurar a conexão no [!DNL Workfront Fusion].</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Prossiga para [Configure seu [!DNL MS Graph API] conexão em [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion).

## Configure seu [!DNL MS Graph API] conexão em [!DNL Workfront Fusion]

Depois de se registrar [!DNL Workfront Fusion] como discutido no [Registrar [!DNL Workfront Fusion] no [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal), você pode configurar sua conexão no [!UICONTROL HTTP] >[!UICONTROL Faça um Oauth 2.0] módulo de solicitação.

1. Adicione um [!UICONTROL HTTP] >[!UICONTROL Faça uma chamada OAuth 2.0] para o seu cenário.
1. Clique em **[!UICONTROL Adicionar]** ao lado do [!UICONTROL conexão] campo.
1. Configure os campos de conexão da seguinte maneira:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome da conexão]</td> 
      <td>Digite um nome para a conexão.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Tipo de fluxo]</p> </td> 
      <td><code>[!UICONTROL Authorization Code]</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Autorizar URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/authorize</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Escopo]</td> 
      <td> <p>Insira as permissões selecionadas na etapa 4 de <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registrar [!DNL Workfront Fusion] no [!DNL Microsoft Application Registration Portal]</a>.</p> <p>Para cada escopo, clique em <b>[!UICONTROL Adicionar]</b> e digite a permissão.</p> <p>Exemplo: <code>offline_access</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Separador de escopo]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td>Insira a [!UICONTROL Application ID] da etapa 2 em <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registrar [!DNL Workfront Fusion] no [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Segredo do cliente]</td> 
      <td>Insira o [!UICONTROL Application Secret] que você gerou na etapa 2 em <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registrar [!DNL Workfront Fusion] no [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Autorizar parâmetros]</td> 
      <td> <p>Adicione os seguintes parâmetros de Autorização:</p> 
       <ul> 
        <li> <p>[!UICONTROL Chave]:<code> response_mode</code> [!UICONTROL Valor]: <code>query</code></p> </li> 
        <li> <p>[!UICONTROL Chave]: <code>prompt </code>[!UICONTROL Valor]: <code>consent</code></p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Acessar parâmetros de token]</td> 
      <td>Não é necessário inserir nada neste campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Atualizar parâmetros de token]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Clique em <b>[!UICONTROL Adicionar]</b>.</p> </li> 
        <li value="2"> <p>No <b>[!UICONTROL Chave]</b> , insira <code>scope</code>.</p> </li> 
        <li value="3"> <p>No <b>[!UICONTROL Valor]</b> , insira todos os [!UICONTROL escopos] que você inseriu no campo de escopo, separados por espaços.</p> <p>Exemplo: <code>offline_access openid User.Read</code></p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Cabeçalhos personalizados]</td> 
      <td>Não é necessário inserir nada neste campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Inserção de token]</td> 
      <td><code>[!UICONTROL In the header]</code> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Continuar]**.
1. Na janela exibida, clique em **[!UICONTROL Aceitar]** para concluir a conexão e retornar ao módulo.
