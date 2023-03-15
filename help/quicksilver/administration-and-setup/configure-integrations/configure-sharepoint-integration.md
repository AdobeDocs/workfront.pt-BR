---
title: Configure o [!DNL SharePoint] integração
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: É possível integrar [!DNL Workfront] com [!DNL SharePoint] Online, fornecendo aos usuários a capacidade de navegar, vincular e adicionar [!DNL SharePoint] documentos no Workfront. A funcionalidade fornecida é semelhante à de outras [!DNL Workfront] integrações, como Google Drive, Box e Dropbox.
author: Becky, Caroline
feature: System Setup and Administration, [!DNL Workfront] Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: fd45e1bc-9a35-4960-a73a-ff845216afe4
source-git-commit: 1290b29ce816673ffc678a1991aea16f0cf5e83f
workflow-type: tm+mt
source-wordcount: '1474'
ht-degree: 0%

---

# Configurar o herdado [!DNL SharePoint] integração

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>O novo [!DNL SharePoint] a integração foi lançada para produção com a versão 22.3 (julho de 2022). Embora os usuários ainda possam acessar documentos vinculados por meio do [!DNL SharePoint] , eles devem usar o novo [!DNL SharePoint] integração para vincular documentos do SharePoint.
>
>* A nova integração do SharePoint não requer configuração por um administrador e pode ser configurada por usuários individuais. No entanto, para garantir uma transição suave para a nova integração do SharePoint, um administrador do Workfront deve fazer algumas pequenas alterações de configurações na área Configuração do Workfront .
   >
   >    Para obter informações e instruções, consulte [Configurar a integração herdada do SharePoint para continuar o acesso aos documentos](#configure-the-legacy-sharepoint-integration-for-continued-access-to-documents) neste artigo.
>    
>* Recomendamos que os usuários vinculem documentos que estão vinculados por meio do legado [!DNL SharePoint] integração através da nova integração.
   >    
   >    Para obter instruções sobre como vincular documentos, consulte [Vincular documentos de aplicativos externos](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).


É possível integrar [!DNL Workfront] com [!DNL SharePoint Online], fornecendo aos usuários a capacidade de navegar, vincular e adicionar [!DNL SharePoint] documentos no Workfront. A funcionalidade fornecida é semelhante à de outras [!DNL Workfront] integrações, como [!DNL Google Drive], [!DNL Box]e [!DNL Dropbox].

Essa integração é compatível somente com [!DNL SharePoint Online]. Instâncias locais de [!DNL SharePoint] não são compatíveis.

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador. Para obter informações sobre [!DNL Workfront] administradores, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Pré-requisitos

Você deve ter acesso ou permissões necessárias no [!DNL SharePoint] para modificar ou configurar o [!DNL SharePoint].

## Vincular documentos por meio da nova integração com o SharePoint

Os usuários individuais podem vincular documentos através do novo [!DNL SharePoint] integração. A integração não requer configuração de administrador. Em vez disso, o usuário faz logon em seus [!DNL Microsoft] ao vincular um documento, o que permite que a integração acesse os documentos disponíveis no [!DNL SharePoint].

A primeira vez que um usuário conecta a variável [!DNL Workfront] [!DNL SharePoint] integração com a [!DNL SharePoint] verá e concordará com todas as permissões que [!DNL Workfront] usa ao interagir com seus [!UICONTROL SharePoint] conta. Permissões de leitura permitem [!DNL Workfront] para ver e acessar arquivos em [!DNL SharePoint]e permissões de gravação permitem que o usuário carregue arquivos no [!DNL SharePoint].

![Permissões do Sharepoint](assets/sharepoint-permissions.png)

Para obter instruções sobre como vincular documentos por meio do novo [!DNL SharePoint] integração, consulte [Vincular um documento externo a [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

>[!NOTE]
>
>* A [!DNL SharePoint] integração pode se conectar a um único [!DNL SharePoint] instância. Portanto, um usuário pode configurar uma integração para uma [!DNL SharePoint], mas não pode configurar uma integração para um segundo [!DNL SharePoint], mesmo que tenham permissões para e documentos no segundo [!DNL SharePoint].
>
>* Um usuário tem acesso aos mesmos sites, coleções, pastas, subpastas e arquivos por meio do [!DNL Workfront] [!DNL SharePoint] integração como têm na sua [!DNL SharePoint] conta.


## Informações de segurança, acesso e autorização do [!DNL SharePoint] integração

### Autenticação e autorização

[!DNL Workfront] O usa o OAuth2 para recuperar um token de acesso e um token de atualização. Este token de acesso é usado para autorização com todos [!DNL SharePoint] áreas.

### Acesso e permissões

A primeira vez que um usuário adiciona um documento a [!DNL Workfront] from [!DNL SharePoint], elas são direcionadas a uma tela que solicita as seguintes permissões:

| Acesso | Motivo |
|---|---|
| Ter acesso total aos seus arquivos | Permite [!DNL Workfront] para acessar os arquivos de um usuário para vincular o ativo. Quando os documentos são enviados de [!DNL Workfront] para [!DNL SharePoint], [!DNL Workfront] requer acesso para criar o ativo. |
| Ler itens em todas as coleções de sites | Permite [!DNL Workfront] para ler ativos para ativar a navegação do usuário. |
| Editar ou excluir itens em todas as coleções de sites | Permite [!DNL Workfront] para criar ativos em sites e na coleção de sites. Excluir é usado somente ao limpar após tentativas malsucedidas de link. |
| Manter acesso aos dados aos quais você concedeu acesso | Permite [!DNL Workfront] para gerar um token de atualização. |
| Fazer logon e ler o perfil do usuário | Permite [!DNL Workfront] para usar o token de acesso para agir em nome do usuário, por meio do fluxo de logon OAuth2. |

Esse acesso é concedido pelo usuário na primeira vez que ele usa a integração e pode ser revogado a qualquer momento.

Considere o seguinte em relação ao acesso a [!DNL SharePoint] através da [!DNL Workfront] [!DNL SharePoint] integração:

* [!DNL Workfront] solicita o acesso mínimo necessário para executar operações na integração.
* Acesso para exibir, editar ou excluir um [!DNL Adobe Workfront] documento vinculado a [!DNL SharePoint] é baseado no acesso do usuário no [!DNL Workfront]. No entanto, qualquer navegação, download ou edição de um [!DNL SharePoint] arquivo ou pasta requer acesso a [!DNL SharePoint]e o acesso a essas ações é controlado por [!DNL SharePoint].
* Os usuários podem visualizar miniaturas e visualizar imagens provenientes de [!DNL SharePoint]e pode ver os nomes de arquivo e pasta em [!DNL SharePoint], sem fazer logon em [!DNL SharePoint].
* O token de acesso de um usuário é usado somente quando ele está offline e outro usuário visualiza o conteúdo de uma pasta vinculada a [!DNL Workfront]. O token de acesso é usado para descobrir se quaisquer documentos na pasta foram adicionados, removidos ou editados.

### Segurança

Todas as comunicações entre [!DNL Workfront] e [!DNL SharePoint] é realizada por meio de HTTPS, que criptografa as informações.

[!DNL Workfront] não armazena, copia ou duplica dados do [!DNL SharePoint]. A única exceção é que [!DNL Workfront] armazena miniaturas de [!DNL SharePoint] para exibir na exibição de lista e em Visualização.

Se um ativo tiver sido carregado pela primeira vez no [!DNL Workfront]e, em seguida, enviadas para [!DNL SharePoint], [!DNL Workfront] retém os dados do primeiro arquivo, pois os usuários podem baixar uma versão anterior de um [!DNL Workfront] documento. Se um documento foi criado em [!DNL SharePoint], [!DNL Workfront] não armazena esses dados de arquivo.

## Configure o [!DNL SharePoint] integração para acesso continuado a documentos

Para garantir que seus usuários tenham acesso contínuo a documentos vinculados ao Workfront por meio do herdado [!DNL SharePoint] , você deve reconfigurar o acesso ao antigo [!DNL SharePoint] integração e mantenha o Segredo do cliente do SharePoint atualizado.

* [Reconfigure o acesso ao herdado [!DNL SharePoint] integração](#reconfigure-access-to-the-legacy-dnl-sharepoint-integration)
* [Configure o Segredo do cliente para continuar com o acesso ao antigo [!DNL SharePoint] integração](#configure-the-client-secret-for-continued-access-to-the-legacy-dnl-sharepoint-integration)

### Reconfigure o acesso ao herdado [!DNL SharePoint] integração

Para garantir que você possa acessar documentos vinculados por meio do [!DNL SharePoint] , garantindo que seus usuários não possam vincular novos documentos por meio dessa integração, conclua o procedimento a seguir.

>[!NOTE]
>
> * O legado [!DNL SharePoint] a integração é rotulada como &quot;[!DNL SharePoint].&quot;
> * O novo [!DNL SharePoint] a integração é rotulada como &quot;[!UICONTROL [!DNL SharePoint] (API de gráfico)].&quot;


1. Clique no botão **[!UICONTROL Menu principal]** ícone ![Menu principal](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **[!UICONTROL Configuração]** ![Configuração](../get-started-wf-administration/assets/gear-icon-settings.png).
1. Selecionar **[!UICONTROL Documentos]** na navegação à esquerda, selecione **[!UICONTROL Provedores de nuvem]**.
1. Certifique-se de que a variável **[!DNL SharePoint]** e **[!UICONTROL [!DNL SharePoint](API de gráfico)]** estão ativadas.
1. Clique em **[!UICONTROL Salvar]**.
1. Selecionar **[!UICONTROL Documentos]** na navegação à esquerda, selecione **[!UICONTROL [!DNL SharePoint]Integração]**.
1. Selecione a marca de seleção à esquerda da lista para todas as integrações existentes e selecione **[!UICONTROL Desativar]**.


### Configure o Segredo do cliente para continuar com o acesso ao antigo [!DNL SharePoint] integração

Seu [!DNL SharePoint] Segredo do cliente expira uma vez por ano. Para garantir o acesso contínuo aos documentos em seu legado [!DNL SharePoint] integração, você deve manter [!DNL SharePoint] Segredo do cliente atualizado.

>[!IMPORTANT]
>
> Porque [!DNL SharePoint] Segredos do cliente são tratados por [!DNL Microsoft], os recursos e os procedimentos do Segredo do cliente podem ser alterados com base em atualizações de [!DNL SharePoint] feito por [!DNL Microsoft]. Sempre verifique o [!DNL Microsoft] documentação para obter as informações mais recentes sobre procedimentos e recursos no [!DNL SharePoint].

<!--1. Go to the site that your [!DNL SharePoint] integration uses. This may be a site that you created when setting up the integrations, or it may be your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.-->

1. Gere um novo segredo de cliente, conforme descrito em [Substituir um segredo de cliente que está expirando em um [!DNL SharePoint] Suplemento](https://docs.microsoft.com/en-us/sharepoint/dev/sp-add-ins/replace-an-expiring-client-secret-in-a-sharepoint-add-in#generate-a-new-secret)
1. Copie este Segredo do Cliente para um local seguro.
1. Faça logon [!DNL Workfront] como administrador.
1. No Workfront, clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).
1. No painel esquerdo, clique em **[!UICONTROL Documentos]** > **[!UICONTROL [!DNL SharePoint]Integração]**.
1. Clique no botão [!DNL SharePoint] integração que deseja atualizar, em seguida, clique em **[!UICONTROL Editar]**.
1. Insira o novo Segredo do cliente no **[!UICONTROL Segredo do cliente]** campo.
1. Clique em **[!UICONTROL Salvar]**.

<!--

## Instructions for setting up the legacy SharePoint integration

>[!IMPORTANT]
>
>This integration has been deprecated. The instructions here are for information only and will be removed in the near future.


Workfront connects to [!DNL SharePoint] Online using OAuth 2.0, a standard used by most web-based integrations for the authentication and authorization of users.

To configure OAuth, you need to create a [!DNL SharePoint] site and a Site App within [!DNL SharePoint]. This process is described in the following sections.

For more information about OAuth, see [http://oauth.net](http://oauth.net/).

>[!TIP]
>
>To make it easy to copy and paste information between [!DNL Workfront] and [!DNL SharePoint] in these steps, we recommend keeping both applications open in separate tabs.

* [Create and configure a [!DNL SharePoint] site](#create-and-configure-a-sharepoint-site) 
* [Grant write permissions to the site app](#grant-write-permissions-to-the-site-app) 
* [Create a [!DNL Workfront] [!DNL SharePoint] integration instance](#create-a-workfront-sharepoint-integration-instance) 
* [Complete your integration](#complete-your-integration) 
* [Add documents](#add-documents)

### Create and configure a [!DNL SharePoint] site  {#create-and-configure-a-sharepoint-site}

In order for [!DNL Workfront] to authenticate with [!DNL SharePoint], [!DNL Workfront] ca use a master site where users have the [!UICONTROL Full Control] permission level or specific Manage permissions. This master site acts as an Authentication Entry Point for [!DNL Workfront].

To create and configure a [!DNL SharePoint] Site:

1. (Optional) If you do not want to use your organization's root site, you can create a master site in [!DNL SharePoint].

   For instructions, visit [Create a site](https://docs.microsoft.com/en-us/sharepoint/create-site-collection) in the [!DNL Microsoft] Documentation.

   * Select the **[!UICONTROL Team Site]** option when creating the site.

1. (Conditional) If you created a site in step 1, go to the site you just created.

   Or

   If you did not create a site in step 1, go to your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.
1. Configure the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client ID]</p> </td> 
      <td> <p>Click <strong>[!UICONTROL Generate]</strong> to generate a Client ID. Copy this ID to a secure location. You will use it later when you set up the [!DNL SharePoint] integration in [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client Secret]</p> </td> 
      <td> <p>Click <strong>[!UICONTROL Generate]</strong> to generate a Client Secret. Copy this Secret to a secure location. You will use it later when you set up the [!DNL SharePoint] integration in [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Title</p> </td> 
      <td> <p>Enter a title, such as [!DNL Workfront] Site App. Users see this title when adding documents..</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL App Domain]</p> </td> 
      <td> <p><code>my.workfront.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Redirect URI]</p> </td> 
      <td> <p><code>https://oauth.my.workfront.com/oauth2/redirect</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Create]**
1. Continue to [Grant write permissions to the site app](#grant-write-permissions-to-the-site-app).

### Grant write permissions to the site app  {#grant-write-permissions-to-the-site-app}

At this point, you have successfully created a Site App and registered it within [!DNL Workfront]. This site app is also known as an app principal in [!DNL SharePoint]. It resides within your tenant. New site apps do not automatically have access to site collections within the tenant. Permissions must be granted explicitly, for each site collection. The steps below will show you how to grant Write permission to the new Site App a site collection. Repeat these steps for each of the site collections you added under [!UICONTROL Visible Site Collections] in the steps above.

This site app must have [!UICONTROL Write] permission to any site collections that users need to access through [!DNL Workfront].

1. Add '/_layouts/15/appinv.aspx' to the URL in [!DNL Sharepoint].

   **Example:**

   ```
   https://mycompany.sharepoint.com/sites/mysite/_layouts/15/appinv.aspx
   ```

1. Configure the following fields

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL App ID]</td> 
      <td> <p>Add the Client ID that you created in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>and click <strong>[!UICONTROL Lookup]</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client] / [!UICONTROL App Domain] / [!UICONTROL Redirect URL]</p> </td> 
      <td> <p>These automatically fill when you click [!UICONTROL Lookup].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Permission Request XML]</td> 
      <td> <p>Copy the following XML to the [!UICONTROL Permission Request XML] field. Make sure that it is added exactly as shown without additional spaces etc. in order to avoid errors.</p> 
      <div></a> 
      <div style="mc-code-lang: XML;" class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False"> 
       <pre><code><span style="color: #63a35c; ">&lt;AppPermissionRequests&gt;</span><br><span style="color: #63a35c; ">&lt;AppPermissionRequest <span style="color: #795da3; ">Scope</span><span style="color: #df5000; ">="http://sharepoint/content/sitecollection/web"</span> <span style="color: #795da3; ">Right</span><span style="color: #df5000; ">="Write"</span>/&gt;</span><br><span style="color: #63a35c; ">&lt;/AppPermissionRequests&gt;</span></code></pre> 
      </div> 
      </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Create]**. 
1. In the dialog that appears, click **[!UICONTROL Trust it]**.
1. Verify that the site app has access to the site collection by clicking the **[!UICONTROL Site collection app permissions]** link in [!UICONTROL Site Settings].
1. Repeat the steps above for the remaining site collections, then continue with [Create a [!DNL Workfront] [!DNL SharePoint] integration instance](#create-a-workfront-sharepoint-integration-instance).

### Create a [!DNL Workfront] [!DNL SharePoint] integration instance {#create-a-workfront-sharepoint-integration-instance}

When you have created a site app in [!DNL SharePoint], you can now copy information from the site app into [!DNL Workfront]. The site app is an app principal and acts as the conduit through which OAuth requests are made to access documents within site collections.

1. Log into [!DNL Workfront] as an administrator.
1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. In the left panel, click **[!UICONTROL Documents]** > **[!UICONTROL [!DNL SharePoint] Integration]**.
1. Click **[!UICONTROL Add [!DNL SharePoint]]**.
1. Configure the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Name]</p> </td> 
      <td> <p>Enter a name for the [!DNL SharePoint] integration. Users see this name when they click [!UICONTROL Add] &gt; [!UICONTROL From] 'name of integration'. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL SharePoint] Host Instance]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.sharepoint.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL Azure] Access Domain]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.onmicrosoft.com</code> </p> <p>This refers to the Master Site that users will use to authenticate through. It is likely the same domain as the [!UICONTROL [!DNL SharePoint] Host Instance].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>
      </p> </td> 
      <td> <b>Important</b> Site collections are used only in the Legacy [!DNL SharePoint] Integration.
       <ul> 
        <li> <p><b>If you are using your organization's root site</b><b>:</b> </p> <p>Enter <code>/</code></p> </li> 
        <li> <p><b>If you are using a master site and subsites:</b> </p> <p><b>IMPORTANT</b>: [!DNL Microsoft SharePoint] no longer recommends the use of subsites.</p> <p>Enter the URL stem for the site collection that you created in the section above.</p> <p>This is the section of the URL after .com.</p> <p>Example: for the URL <code>https://mycompany.sharepoint.com/sites/mysite</code>, the stem would be <code>/sites/mysite</code>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Client ID]</td> 
      <td>Enter the Client ID that you generated in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Client Secret]</td> 
      <td>Enter the Client Secret that you generated in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Visible Site Collections]</td> 
      <td> <b>Important</b> Site collections are used only in the Legacy [!DNL SharePoint] integration.
       <ul> 
        <li> <p><b> If you are using your organization's root site</b><b>:</b> </p> <p>Enter <code>/</code></p> </li> 
        <li> <p><b>If you are using a master site and subsites:</b> </p> <p><b>IMPORTANT</b>: [!DNL Microsoft SharePoint] no longer recommends the use of subsites.</p> <p>For each subsite you want to add to your [!DNL SharePoint] integration, enter the stem of the subsite.</p> <p>Example: for the URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, the stem would be <code>/sites/mysite/mysubsite</code>.</p> <p><b>NOTE</b>:   <p>If you want to test your configuration only (no subsites), enter the stem of the master site. </p> <p>Example: for the URL <code> https://mycompany.sharepoint.com/sites/mysite</code>, the stem would be <code>/sites/mysite</code>.</p> <p>When you have tested your configuration as described in <a href="#complete-your-integration" class="MCXref xref">Complete your integration</a>, you must remove the master site and enter the subsites.</p> 
          <ol> 
           <li value="1">Click the <strong>[!UICONTROL Main Menu]</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of [!DNL Adobe Workfront], then click <strong>[!UICONTROL Setup]</strong> <img src="assets/gear-icon-settings.png">.<li><p>In the left panel, click <strong>[!UICONTROL Documents]</strong> &gt; <strong>[!UICONTROL [!DNL SharePoint] Integration]</strong>.</p></li><li><p>Click the [!DNL SharePoint] integration you are setting up, then click Edit.</p></li><li><p>Delete the stem for the master site from the [!UICONTROL Visible Site Collections] field.</p></li><li><p>For each subsite you want to add to your [!DNL SharePoint] integration, enter the stem of the subsite.</p></li><p>Example: for the URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, the stem would be <code>/sites/mysite/mysubsite</code>.</p></li> 
          </ol> </p> </li> 
       </ul> <p> </p> <p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Save]**
1. Continue to [Complete your integration](#complete-your-integration).

### Complete your integration {#complete-your-integration}

The basic configuration is almost complete.

1. In Workfront, Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Documents]** ![](assets/document-icon.png).
1. Click **[!UICONTROL Add new]**.
1. Click **[!UICONTROL From] `<title of your [!DNL SharePoint] site>`** in the dropdown.

   A dialog that invites you to Trust this site appears.

   >[!NOTE]
   >
   >If this dialog does not appear, your [!DNL SharePoint] integration is not configured correctly.

1. Click **[!UICONTROL Trust it]**.

### Add documents {#add-documents}

You can now add documents from your [!DNL SharePoint] site.

For instructions, see [Link an external document to [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) in [Link documents from external applications](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)

>[!IMPORTANT]
>
>If the user who linked a folder no longer has access to the external application, [!DNL Workfront] can no longer access the contents of the folder. This may happen, for example, if the user who originally linked the folder leaves the company. To ensure continued access, a user with access to the folder must re-link the folder.
> 

-->

## Solução de problemas

* [Problema: Os usuários experimentam erros baseados em autenticação ao usar a variável [!DNL SharePoint] integração.](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [Problema: Ao tentar navegar [!DNL SharePoint] arquivos em [!DNL Workfront], não vejo nenhuma ou todas as coleções do meu site.](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [Problema: Não consigo acessar pastas e documentos vinculados anteriormente em [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### Problema: Os usuários experimentam erros baseados em autenticação ao usar a variável [!DNL SharePoint] integração. {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

Soluções:

Os usuários devem ter as permissões apropriadas para [!DNL SharePoint] site.

Usuários com [!UICONTROL Controle completo] o acesso tenha todas as permissões necessárias para sua [!DNL SharePoint] integração. Se não quiser conceder acesso ao Controle completo aos usuários, é necessário conceder as seguintes permissões:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Design]</p> </td> 
   <td> <p>Pode visualizar, adicionar, atualizar, excluir, aprovar e personalizar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Editar]</p> </td> 
   <td> <p>Pode adicionar, editar e excluir listas; pode exibir, adicionar, atualizar e excluir itens e documentos da lista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contribute]</p> </td> 
   <td> <p>Pode exibir, adicionar, atualizar e excluir itens de lista e documentos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Exibir somente]</p> </td> 
   <td> <p>Pode exibir páginas, itens de lista e documentos (os tipos de documentos com manipuladores de arquivos do lado do servidor podem ser exibidos no navegador, mas não baixados)</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter instruções sobre como criar e editar níveis de permissões, consulte [Como criar e editar níveis de permissão](https://docs.microsoft.com/en-us/sharepoint/how-to-create-and-edit-permission-levels) na documentação do Microsoft.

<!--

### Problem: As a [!DNL Workfront] user, I am unable to provision a new [!DNL SharePoint] instance. When I attempt to do I see an error. {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

Solutions:

This can be caused by a number of things, originating in either [!DNL Workfront] or [!DNL SharePoint]'s configuration. Verify that:

* The Client ID, Client Secret, return URL and other configuration fields are correctly mapped between the [!DNL Workfront] [!DNL SharePoint] Integration instance and the [!DNL SharePoint] Site App.
* The user has [!UICONTROL Full Control] permission to the Site Collection used for authentication.
* The Site App is listed under [!UICONTROL Site App Permissions] for the [!UICONTROL Site Collection] used for authentication.

-->

### Problema: Ao tentar navegar [!DNL SharePoint] arquivos em [!DNL Workfront], não vejo nenhuma ou todas as coleções do meu site. {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

Soluções:

Para ver uma coleção de sites em [!DNL Workfront], devem ser cumpridas as seguintes condições:

<!--

* The site collection must be registered in the [!DNL Workfront] [!DNL SharePoint] Integration instance.

  To verify this in [!DNL Workfront]:

   1. Go to [!UICONTROL Setup] > [!UICONTROL Documents] > [!UICONTROL [!DNL SharePoint] Integration].
   1. Edit the [!DNL SharePoint] Integration instance information.
   1. Verify that the site collection is listed under [!UICONTROL Visible Site Collections].
   -->

* O usuário deve ter acesso de visualização ao conjunto de sites em [!DNL SharePoint].

   Para verificar isso em [!DNL SharePoint], vá para [!DNL SharePoint]e abra o conjunto de sites > [!UICONTROL Configurações] > [!UICONTROL Permissões do site].
<!--* The [!DNL SharePoint] Site App must have access to the site collection.

  To verify this in [!DNL SharePoint]:

   1. Go to the site collection > [!UICONTROL Settings] > [!UICONTROL Site app permissions].
   1. Ensure that the [!UICONTROL Site App] used by [!DNL Workfront] is listed here.
   1. (Conditional) If the Site App is not listed, add to the site collection using _layouts/15/appinv.aspx.

      For information about adding the site collection, see Granting Write Permissions To The Site App.
      
-->

### Problema: Não consigo acessar pastas e documentos vinculados anteriormente em [!DNL SharePoint]. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

Solução:

Se o usuário que vinculou um [!DNL SharePoint] a pasta não pode mais ser autenticada, [!DNL Workfront] não pode mais acessar o conteúdo da pasta. Isso pode acontecer, por exemplo, se o usuário que vinculou originalmente a pasta sair da empresa.

Para garantir o acesso contínuo, um usuário com acesso à pasta deve vincular novamente a pasta.

Para obter informações sobre vinculação de pastas de provedores externos, consulte [Vincular documentos de aplicativos externos](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<!--

### Problem: I see a "404 not found" error when attempting to add a document from [!DNL Sharepoint]

#### Solution:

This error might occur if one of the sites configured in the [!UICONTROL Visible Site Collections] list has been deleted in Sharepoint. Check the [!UICONTROL Visible Site Collections] list, and remove any sites that have been deleted in Sharepoint.-->