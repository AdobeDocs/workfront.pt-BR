---
title: Chame a API REST do MS Graph por meio de [!DNL Adobe Workfront Fusion] HTTP &gt; Criar um módulo de solicitação OAuth 2.0
description: Chame a API REST do MS Graph por meio de [!DNL Adobe Workfront Fusion] HTTP &gt; Criar um módulo de solicitação OAuth 2.0
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 0%

---

# Chame o[!UICONTROL  API REST do MS Graph] por meio da [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Fazer uma solicitação do OAuth 2.0] módulo

Muitos [!DNL Microsoft] os serviços da web são acessados por meio da [!DNL Microsoft Graph API]. Este artigo descreve como criar uma conexão com essa API, usando o [!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL Fazer uma solicitação do OAuth 2.0] módulo.

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

## Registrar [!DNL Workfront Fusion] no [!DNL Microsoft Application Registration Portal]

Para criar uma conexão com o [!DNL Microsoft Graph REST API], você deve primeiro se registrar [!DNL Adobe Workfront Fusion].

1. Comece a registrar um novo aplicativo conforme descrito em [Registre seu aplicativo](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) no [!DNL Microsoft] documentação.

   Como parte do registro, [!DNL Microsoft] O requer as seguintes informações:

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Nome do aplicativo]</td>
        <td>Insira um nome para o aplicativo, como "Meu [!DNL Workfront Fusion] aplicação."</td>
      </tr>
      <tr>
        <td>[!UICONTROL Redirecionar URL]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. Após concluir o registro do aplicativo, anote o [!UICONTROL ID do aplicativo].

   >[!IMPORTANT]
   >
   >Você precisará da ID do aplicativo para configurar sua conexão no [!DNL Workfront Fusion].

1. Gerar um [!UICONTROL Application Secret]. Anote este segredo.

   Para obter instruções, consulte [Registre seu aplicativo](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) no [!DNL Microsoft] documentação.

   >[!IMPORTANT]
   >
   >Você precisará do [!UICONTROL Application Secret] para configurar sua conexão no [!DNL Workfront Fusion].

1. Configure as permissões para seu aplicativo.

   Para obter informações específicas sobre como localizar e configurar esses campos, consulte a seção &quot;Configurar permissões para o Gráfico do Microsoft&quot; em [Obter acesso sem um usuário](https://docs.microsoft.com/en-us/graph/auth-v2-service) no [!UICONTROL Microsoft] documentação.

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
        <li> <p>Quaisquer outras permissões necessárias às suas integrações (Exemplo: <code>User.Read</code>)</p> </li> 
       </ul> <p>Importante: você precisará das permissões selecionadas para configurar sua conexão no [!DNL Workfront Fusion].</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Vá para [Configurar o [!DNL MS Graph API] conexão em [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion).

## Configurar o [!DNL MS Graph API] conexão em [!DNL Workfront Fusion]

Depois de se registrar [!DNL Workfront Fusion] conforme discutido em [Registrar [!DNL Workfront Fusion] no [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal), você poderá configurar sua conexão no campo [!UICONTROL HTTP] >[!UICONTROL Criar um Oauth 2.0] módulo de solicitação.

1. Adicionar um [!UICONTROL HTTP] >[!UICONTROL Fazer uma chamada OAuth 2.0] para o seu cenário.
1. Clique em **[!UICONTROL Adicionar]** ao lado da [!UICONTROL conexão] campo.
1. Configure os campos de conexão da seguinte maneira:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome da Conexão]</td> 
      <td>Insira um nome para a conexão.</td> 
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
      <td> <p>Insira as permissões que você selecionou na etapa 4 do <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registrar [!DNL Workfront Fusion] no [!DNL Microsoft Application Registration Portal]</a>.</p> <p>Para cada escopo, clique em <b>[!UICONTROL Adicionar]</b> e digite a permissão.</p> <p>Exemplo: <code>offline_access</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Separador de escopo]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID do Cliente]</td> 
      <td>Insira a [!UICONTROL ID do Aplicativo] a partir da etapa 2 em <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registrar [!DNL Workfront Fusion] no [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Segredo do Cliente]</td> 
      <td>Insira o [!UICONTROL Application Secret] que você gerou na etapa 2 em <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registrar [!DNL Workfront Fusion] no [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Autorizar parâmetros]</td> 
      <td> <p>Adicione os seguintes parâmetros Authorize:</p> 
       <ul> 
        <li> <p>[!UICONTROL Chave]:<code> response_mode</code> [!UICONTROL Valor]: <code>query</code></p> </li> 
        <li> <p>[!UICONTROL Chave]: <code>prompt </code>[!UICONTROL Valor]: <code>consent</code></p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Parâmetros de token de acesso]</td> 
      <td>Não é necessário inserir nada nesse campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Atualizar parâmetros de token]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Clique em <b>[!UICONTROL Adicionar]</b>.</p> </li> 
        <li value="2"> <p>No <b>[!UICONTROL Chave]</b> insira <code>scope</code>.</p> </li> 
        <li value="3"> <p>No <b>[!UICONTROL Valor]</b> insira todos os [!UICONTROL scope]s inseridos no campo de escopo, separados por espaços.</p> <p>Exemplo: <code>offline_access openid User.Read</code></p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Cabeçalhos Personalizados]</td> 
      <td>Não é necessário inserir nada nesse campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Posicionamento de Token]</td> 
      <td><code>[!UICONTROL In the header]</code> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Continuar]**.
1. Na janela exibida, clique em **[!UICONTROL Aceitar]** para concluir a conexão e retornar ao módulo.
