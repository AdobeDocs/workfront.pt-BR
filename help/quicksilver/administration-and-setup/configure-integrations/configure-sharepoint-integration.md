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
source-git-commit: 5292069412a73f824dbcd967d47737cff5ef58fa
workflow-type: tm+mt
source-wordcount: '2515'
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

Para obter instruções sobre como vincular documentos por meio do novo [!DNL SharePoint] integração, consulte [Vincular um documento externo a [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

>[!NOTE]
>
>* A [!DNL SharePoint] integração pode se conectar a um único [!DNL SharePoint] instância. Portanto, um usuário pode configurar uma integração para uma [!DNL SharePoint], mas não pode configurar uma integração para um segundo [!DNL SharePoint], mesmo que tenham permissões para e documentos no segundo [!DNL SharePoint].
>
>* Um usuário tem acesso aos mesmos sites, coleções, pastas, subpastas e arquivos por meio do [!DNL Workfront] [!DNL SharePoint] integração como têm na sua [!DNL SharePoint] conta.


## Configurar a integração herdada do SharePoint para continuar o acesso aos documentos

Para garantir que seus usuários tenham acesso contínuo a documentos vinculados ao Workfront por meio da integração herdada do SharePoint, você deve reconfigurar o acesso à integração herdada do SharePoint e manter o SharePoint Client Secret atualizado.

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



## Instruções para configuração da integração herdada do SharePoint

>[!IMPORTANT]
>
>Essa integração foi substituída. As instruções aqui são apenas para informações e serão removidas em breve.


O Workfront se conecta a [!DNL SharePoint] Online usando o OAuth 2.0, um padrão usado pela maioria das integrações baseadas na Web para a autenticação e a autorização dos usuários.

Para configurar o OAuth, é necessário criar um [!DNL SharePoint] e um aplicativo de site dentro de [!DNL SharePoint]. Esse processo é descrito nas seções a seguir.

Para obter mais informações sobre OAuth, consulte [http://oauth.net](http://oauth.net/).

>[!TIP]
>
>Para facilitar a cópia e colagem de informações entre [!DNL Workfront] e [!DNL SharePoint] nessas etapas, recomendamos manter ambos os aplicativos abertos em guias separadas.

* [Criar e configurar um [!DNL SharePoint] site](#create-and-configure-a-sharepoint-site)
* [Conceder permissões de gravação ao aplicativo do site](#grant-write-permissions-to-the-site-app)
* [Crie um [!DNL Workfront] [!DNL SharePoint] instância de integração](#create-a-workfront-sharepoint-integration-instance)
* [Concluir a integração](#complete-your-integration)
* [Adicionar documentos](#add-documents)

### Criar e configurar um [!DNL SharePoint] site  {#create-and-configure-a-sharepoint-site}

Para [!DNL Workfront] para autenticar com [!DNL SharePoint], [!DNL Workfront] pode usar um site principal em que os usuários têm a variável [!UICONTROL Controle completo] nível de permissão ou permissões específicas de gerenciamento. Este site principal atua como um Ponto de Entrada de Autenticação para [!DNL Workfront].

Para criar e configurar um [!DNL SharePoint] Site:

1. (Opcional) Se você não quiser usar o site raiz de sua organização, poderá criar um site principal em [!DNL SharePoint].

   Para obter instruções, visite [Criar um site](https://docs.microsoft.com/en-us/sharepoint/create-site-collection) no [!DNL Microsoft] Documentação.

   * Selecione o **[!UICONTROL Site da equipe]** ao criar o site.

1. (Condicional) Se você criou um site na etapa 1, vá para o site que você acabou de criar.

   Ou

   Se você não criou um site na etapa 1, vá para o site raiz de sua organização.

1. Adicionar `/_layouts/15/appregnew.aspx` ao final do URL na barra de pesquisa na parte superior da janela do navegador.
1. Configure os seguintes campos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client ID]</p> </td> 
      <td> <p>Clique em <strong>[!UICONTROL Gerar]</strong> para gerar uma ID do cliente. Copie essa ID para um local seguro. Você o usará posteriormente ao configurar a variável [!DNL SharePoint] integração no [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Segredo do cliente]</p> </td> 
      <td> <p>Clique em <strong>[!UICONTROL Gerar]</strong> para gerar um Segredo do Cliente. Copie este segredo para um local seguro. Você o usará posteriormente ao configurar a variável [!DNL SharePoint] integração no [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Título</p> </td> 
      <td> <p>Insira um título, como [!DNL Workfront] Aplicativo de site. Os usuários veem esse título ao adicionar documentos.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Domínio de aplicativo]</p> </td> 
      <td> <p><code>my.workfront.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Redirecionar URI]</p> </td> 
      <td> <p><code>https://oauth.my.workfront.com/oauth2/redirect</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Criar]**
1. Continue para [Conceder permissões de gravação ao aplicativo do site](#grant-write-permissions-to-the-site-app).

### Conceder permissões de gravação ao aplicativo do site  {#grant-write-permissions-to-the-site-app}

Neste ponto, você criou com êxito um aplicativo de site e o registrou em [!DNL Workfront]. Este aplicativo de site também é conhecido como principal do aplicativo no [!DNL SharePoint]. Ele reside dentro do seu locatário. Os novos aplicativos de site não têm acesso automático às coleções de site no locatário. As permissões devem ser concedidas explicitamente para cada coleção de sites. As etapas abaixo mostrarão como conceder permissão de gravação ao novo aplicativo do site em um conjunto de sites. Repita essas etapas para cada um dos conjuntos de sites adicionados em [!UICONTROL Coleções de site visíveis] nas etapas acima.

Este aplicativo de site deve ter [!UICONTROL Gravar] permissão para qualquer coleção de sites que os usuários precisam acessar por meio de [!DNL Workfront].

1. Adicione &#39;/_layouts/15/appinv.aspx&#39; ao URL em [!DNL Sharepoint].

   **Exemplo:**

   ```
   https://mycompany.sharepoint.com/sites/mysite/_layouts/15/appinv.aspx
   ```

1. Configure os seguintes campos

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL App ID]</td> 
      <td> <p>Adicionar a ID do cliente que você criou em <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Criar e configurar um [!DNL SharePoint] site </a>e clique em <strong>[!UICONTROL Lookup]</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client] / [!UICONTROL App Domain] / [!UICONTROL Redirect URL]</p> </td> 
      <td> <p>Eles são preenchidos automaticamente quando você clica em [!UICONTROL Lookup].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Solicitação de permissão XML]</td> 
      <td> <p>Copie o XML a seguir para o campo [!UICONTROL Solicitação de permissão XML] . Certifique-se de adicioná-lo exatamente como mostrado, sem espaços adicionais, etc. para evitar erros.</p> 
      <div></a> 
      <div style="mc-code-lang: XML;" class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False"> 
       <pre></pre></div></div></td></tr></tbody></table>

1. Clique em **[!UICONTROL Criar]**.
1. Na caixa de diálogo exibida, clique em **[!UICONTROL Confie nele]**.
1. Verifique se o aplicativo do site tem acesso ao conjunto do site clicando no botão **[!UICONTROL Permissões do aplicativo de coleção de sites]** link em [!UICONTROL Configurações do site].
1. Repita as etapas acima para as coleções de site restantes e continue com [Crie um [!DNL Workfront] [!DNL SharePoint] instância de integração](#create-a-workfront-sharepoint-integration-instance).

### Crie um [!DNL Workfront] [!DNL SharePoint] instância de integração {#create-a-workfront-sharepoint-integration-instance}

Quando você cria um aplicativo de site no [!DNL SharePoint], agora você pode copiar informações do aplicativo do site para [!DNL Workfront]. O aplicativo de site é um principal de aplicativo e atua como o canal através do qual as solicitações do OAuth são feitas para acessar documentos em coleções de site.

1. Faça logon [!DNL Workfront] como administrador.
1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **[!UICONTROL Documentos]** > **[!UICONTROL [!DNL SharePoint]Integração]**.
1. Clique em **[!UICONTROL Adicionar[!DNL SharePoint]]**.
1. Configure os seguintes campos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Name]</p> </td> 
      <td> <p>Insira um nome para o [!DNL SharePoint] integração. Os usuários veem esse nome ao clicar em [!UICONTROL Adicionar] &gt; [!UICONTROL De] 'nome da integração'. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL SharePoint] Instância do host]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.sharepoint.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL Azure] Domínio de acesso]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.onmicrosoft.com</code> </p> <p>Refere-se ao Site Principal pelo qual os usuários serão usados para autenticar. Provavelmente, o mesmo domínio que o [!UICONTROL] [!DNL SharePoint] Instância do host].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>
      </p> </td> 
      <td> <b>Importante</b> As coleções de site são usadas somente no Legado [!DNL SharePoint] Integração.
       <ul> 
        <li> <p><b>Se estiver usando o site raiz da sua organização</b><b>:</b> </p> <p>Enter <code>/</code></p> </li> 
        <li> <p><b>Se você estiver usando um site principal e subsites:</b> </p> <p><b>IMPORTANTE</b>: [!DNL Microsoft SharePoint] O não recomenda mais o uso de subsites.</p> <p>Insira o fluxo de URL do conjunto de sites criado na seção acima.</p> <p>Esta é a seção do URL após .com.</p> <p>Exemplo: para o URL <code>https://mycompany.sharepoint.com/sites/mysite</code>, o tronco seria <code>/sites/mysite</code>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] ID do cliente]</td> 
      <td>Insira a ID do cliente gerada em <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Criar e configurar um [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Segredo do cliente]</td> 
      <td>Insira o Segredo do Cliente gerado em <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Criar e configurar um [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Coleções de site visíveis]</td> 
      <td> <b>Importante</b> As coleções de site são usadas somente no Legado [!DNL SharePoint] integração.
       <ul> 
        <li> <p><b> Se estiver usando o site raiz da sua organização</b><b>:</b> </p> <p>Enter <code>/</code></p> </li> 
        <li> <p><b>Se você estiver usando um site principal e subsites:</b> </p> <p><b>IMPORTANTE</b>: [!DNL Microsoft SharePoint] O não recomenda mais o uso de subsites.</p> <p>Para cada subsite que deseja adicionar ao seu [!DNL SharePoint] , insira o sistema do subsite.</p> <p>Exemplo: para o URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, o tronco seria <code>/sites/mysite/mysubsite</code>.</p> <p><b>Nota</b>:   <p>Se quiser testar sua configuração somente (sem subsites), insira o sistema do site principal. </p> <p>Exemplo: para o URL <code> https://mycompany.sharepoint.com/sites/mysite</code>, o tronco seria <code>/sites/mysite</code>.</p> <p>Ao testar sua configuração, conforme descrito em <a href="#complete-your-integration" class="MCXref xref">Concluir a integração</a>, é necessário remover o site principal e inserir os subsites.</p> 
          <ol> 
           <li value="1">Clique no botão <strong>[!UICONTROL Menu principal]</strong> ícone <img src="assets/main-menu-icon.png"> no canto superior direito de [!DNL Adobe Workfront], depois clique em <strong>[!UICONTROL Configuração]</strong> <img src="assets/gear-icon-settings.png">.<li><p>No painel esquerdo, clique em <strong>[!UICONTROL Documentos]</strong> &gt; <strong>[!UICONTROL [!DNL SharePoint] Integração]</strong>.</p></li><li><p>Clique no botão [!DNL SharePoint] integração que você está configurando e clique em Editar.</p></li><li><p>Exclua o tronco do site principal do campo [!UICONTROL Coleções de site visíveis].</p></li><li><p>Para cada subsite que deseja adicionar ao seu [!DNL SharePoint] , insira o sistema do subsite.</p></li><p>Exemplo: para o URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, o tronco seria <code>/sites/mysite/mysubsite</code>.</p></li> 
          </ol> </p> </li> 
       </ul> <p> </p> <p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Salvar]**
1. Continue para [Concluir a integração](#complete-your-integration).

### Concluir a integração {#complete-your-integration}

A configuração básica está quase concluída.

1. No Workfront, clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **[!UICONTROL Documentos]** ![](assets/document-icon.png).
1. Clique em **[!UICONTROL Adicionar novo]**.
1. Clique em **[!UICONTROL De]`<title of your [!DNL SharePoint] site>`** na lista suspensa.

   Uma caixa de diálogo que convida você a Confiar neste site é exibida.

   >[!NOTE]
   >
   >Se essa caixa de diálogo não aparecer, sua [!DNL SharePoint] a integração não está configurada corretamente.

1. Clique em **[!UICONTROL Confie nele]**.

### Adicionar documentos {#add-documents}

Agora você pode adicionar documentos de [!DNL SharePoint] site.

Para obter instruções, consulte [Vincular um documento externo a [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) em [Vincular documentos de aplicativos externos](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)

>[!IMPORTANT]
>
>Se o usuário que vinculou uma pasta não tiver mais acesso ao aplicativo externo, [!DNL Workfront] não pode mais acessar o conteúdo da pasta. Isso pode acontecer, por exemplo, se o usuário que vinculou originalmente a pasta sair da empresa. Para garantir o acesso contínuo, um usuário com acesso à pasta deve vincular novamente a pasta.

## Solução de problemas

* [Problema: Os usuários experimentam erros baseados em autenticação ao usar a variável [!DNL SharePoint] integração.](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [Problema: Como um [!DNL Workfront] usuário, não consigo provisionar um novo [!DNL SharePoint] instância. Quando tento fazer isso, vejo um erro.](#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error)
* [Problema: Ao tentar navegar [!DNL SharePoint] arquivos em [!DNL Workfront], não vejo nenhuma ou todas as coleções do meu site.](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [Problema: Não consigo acessar pastas e documentos vinculados anteriormente em [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### Problema: Os usuários experimentam erros baseados em autenticação ao usar a variável [!DNL SharePoint] integração. {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

Soluções:

Os usuários devem ser membros de um grupo que tenha as permissões apropriadas para [!DNL SharePoint] site.

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

### Problema: Como um [!DNL Workfront] usuário, não consigo provisionar um novo [!DNL SharePoint] instância. Quando tento fazer isso, vejo um erro. {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

Soluções:

Isso pode ser causado por uma série de coisas, originárias de [!DNL Workfront] ou [!DNL SharePoint]Configuração do . Verifique se:

* A ID do cliente, o Segredo do cliente, o URL de retorno e outros campos de configuração são mapeados corretamente entre as [!DNL Workfront] [!DNL SharePoint] Instância de integração e [!DNL SharePoint] Aplicativo de site.
* O usuário tem [!UICONTROL Controle completo] permissão para o conjunto de sites usado para autenticação.
* O aplicativo de site está listado em [!UICONTROL Permissões para o aplicativo do site] para [!UICONTROL Coleção de sites] usado para autenticação.

### Problema: Ao tentar navegar [!DNL SharePoint] arquivos em [!DNL Workfront], não vejo nenhuma ou todas as coleções do meu site. {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

Soluções:

Para ver uma coleção de sites em [!DNL Workfront], devem ser cumpridas as seguintes condições:

* O conjunto de sites deve ser registrado no [!DNL Workfront] [!DNL SharePoint] Instância de integração.

   Para verificar isso em [!DNL Workfront]:

   1. Ir para [!UICONTROL Configuração] > [!UICONTROL Documentos] > [!UICONTROL [!DNL SharePoint] Integração].
   1. Edite o [!DNL SharePoint] Informações da instância de integração.
   1. Verifique se o conjunto de sites está listado em [!UICONTROL Coleções de site visíveis].

* O usuário deve ter acesso de visualização ao conjunto de sites em [!DNL SharePoint].
* Para verificar isso em [!DNL SharePoint], vá para [!DNL SharePoint]e abra o conjunto de sites > [!UICONTROL Configurações] > [!UICONTROL Permissões do site].
* O [!DNL SharePoint] O aplicativo do site deve ter acesso ao conjunto do site.

   Para verificar isso em [!DNL SharePoint]:

   1. Vá para a coleção de sites > [!UICONTROL Configurações] > [!UICONTROL Permissões do aplicativo do site].
   1. Certifique-se de que [!UICONTROL Aplicativo de site] usado por [!DNL Workfront] está listado aqui.
   1. (Condicional) Se o aplicativo de site não estiver listado, adicione ao conjunto de sites usando _layouts/15/appinv.aspx.

      Para obter informações sobre como adicionar o conjunto de sites, consulte Concessão de permissões de gravação ao aplicativo do site.

### Problema: Não consigo acessar pastas e documentos vinculados anteriormente em [!DNL SharePoint]. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

Solução:

Se o usuário que vinculou um [!DNL SharePoint] a pasta não pode mais ser autenticada, [!DNL Workfront] não pode mais acessar o conteúdo da pasta. Isso pode acontecer, por exemplo, se o usuário que vinculou originalmente a pasta sair da empresa.

Para garantir o acesso contínuo, um usuário com acesso à pasta deve vincular novamente a pasta.

Para obter informações sobre vinculação de pastas de provedores externos, consulte [Vincular documentos de aplicativos externos](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Problema: Vejo um erro &quot;404 não encontrado&quot; ao tentar adicionar um documento de [!DNL Sharepoint]

#### Solução:

Esse erro pode ocorrer se um dos sites configurados no [!UICONTROL Coleções de site visíveis] lista foi excluída no Sharepoint. Verifique a [!UICONTROL Coleções de site visíveis] e remover quaisquer sites que tenham sido excluídos no Sharepoint.
