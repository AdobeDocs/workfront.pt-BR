---
title: Chame a API REST do MS Graph por meio do módulo de solicitação  [!DNL Adobe Workfront Fusion] HTTP &gt; Make an OAuth 2.0
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 1%

---

# Chame a [!UICONTROL  API REST do MS Graph] por meio do [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Faça uma solicitação OAuth 2.0] para o módulo

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Chamar a API REST do MS Graph](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/call-the-ms-graph-rest-api.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

<!-- Audited: 3/2024-->

Muitos serviços Web do [!DNL Microsoft] são acessados por meio do [!DNL Microsoft Graph API]. Você pode criar uma conexão com [!DNL Microsoft Graph API], usando o módulo [!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL Fazer uma solicitação OAuth 2.0].

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
   <p>Novo:</p> <ul><li>[!UICONTROL Select] ou [!UICONTROL Prime] Plano [!DNL Workfront]: sua organização deve comprar [!DNL Adobe Workfront Fusion].</li><li>Plano [!DNL Workfront] da [!UICONTROL Ultimate] [!DNL Workfront Fusion] incluído.</li></ul>
   <p>Ou</p>
   <p>Atual: sua organização deve comprar o [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Registrar [!DNL Workfront Fusion] no [!DNL Microsoft Application Registration Portal]

Para criar uma conexão com o [!DNL Microsoft Graph REST API], primeiro você deve registrar [!DNL Adobe Workfront Fusion].

1. Comece a registrar um novo aplicativo conforme descrito em [Registre seu aplicativo](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) na documentação do [!DNL Microsoft].

   Como parte do registro, [!DNL Microsoft] requer as seguintes informações:

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Nome do aplicativo]</td>
        <td>Digite um nome para o aplicativo, como "Meu aplicativo [!DNL Workfront Fusion]".</td>
      </tr>
      <tr>
        <td>[!UICONTROL Redirecionar URL]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. Após concluir o registro do aplicativo, anote a [!UICONTROL ID do aplicativo].

   >[!IMPORTANT]
   >
   >Você precisará da ID do Aplicativo para configurar sua conexão no [!DNL Workfront Fusion].

1. Gerar um [!UICONTROL Segredo do Aplicativo]. Anote este segredo.

   Para obter instruções, consulte [Registrar seu aplicativo](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) na documentação do [!DNL Microsoft].

   >[!IMPORTANT]
   >
   >Você precisará do [!UICONTROL Application Secret] para configurar sua conexão em [!DNL Workfront Fusion].

1. Configure as permissões para seu aplicativo.

   Para obter informações específicas sobre como localizar e configurar esses campos, consulte a seção &quot;Configurar permissões para o Gráfico do Microsoft&quot; em [Obter acesso sem um usuário](https://docs.microsoft.com/en-us/graph/auth-v2-service) na documentação do [!UICONTROL Microsoft].

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Que tipo de permissões seu aplicativo requer?]</td> 
      <td>Selecione <code>[!UICONTROL Delegated permissions]</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Selecionar permissões]</td> 
      <td> <p>Selecione as seguintes permissões:</p> 
       <ul> 
        <li> <p><code>offline_access</code> </p> </li> 
        <li> <p><code>openid</code> </p> </li> 
        <li> <p>Quaisquer outras permissões necessárias às suas integrações (Exemplo: <code>User.Read</code>)</p> </li> 
       </ul> <p><b>Importante</b>: você precisará das permissões selecionadas para configurar sua conexão em [!DNL Workfront Fusion].</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Prossiga para [Configurar sua [!DNL MS Graph API] conexão em [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion).

## Configurar a conexão do [!DNL MS Graph API] no [!DNL Workfront Fusion]

Depois de registrar [!DNL Workfront Fusion] como discutido em [Registrar [!DNL Workfront Fusion] no [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal), você poderá configurar sua conexão no módulo de solicitação [!UICONTROL HTTP] > [!UICONTROL Criar um Oauth 2.0].

1. Adicione um módulo [!UICONTROL HTTP] > [!UICONTROL Fazer uma chamada OAuth 2.0] ao seu cenário.
1. Clique em **[!UICONTROL Adicionar]** ao lado do campo [!UICONTROL conexão].
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
      <td> <p>Insira as permissões que você selecionou na etapa 4 de <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registrar [!DNL Workfront Fusion] em [!DNL Microsoft Application Registration Portal]</a>.</p> <p>Para cada escopo, clique em <b>[!UICONTROL Adicionar]</b> e digite a permissão.</p> <p>Exemplo: <code>offline_access</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Separador de escopo]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID do Cliente]</td> 
      <td>Insira o [!UICONTROL Application ID] da etapa 2 em <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registrar [!DNL Workfront Fusion] em [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Segredo do Cliente]</td> 
      <td>Insira o [!UICONTROL Application Secret] que você gerou na etapa 3 em <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registrar [!DNL Workfront Fusion] em [!DNL Microsoft Application Registration Portal]</a>.</td> 
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
        <li value="2"> <p>No campo <b>[!UICONTROL Chave]</b>, digite <code>scope</code>.</p> </li> 
        <li value="3"> <p>No campo <b>[!UICONTROL Valor]</b>, insira todos os [!UICONTROL escopo]s inseridos no campo de escopo, separados por espaços.</p> <p>Exemplo: <code>offline_access openid User.Read</code></p> </li> 
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
