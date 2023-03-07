---
title: Configure o [!DNL SharePoint] integração
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: É possível integrar [!DNL Workfront] com [!DNL SharePoint] On-line, oferecendo aos usuários a capacidade de navegar, vincular e adicionar [!DNL SharePoint] documentos no Workfront. A funcionalidade fornecida é semelhante à de outros [!DNL Workfront] integrações, como Google Drive, Box e Dropbox.
author: Becky, Caroline
feature: System Setup and Administration, [!DNL Workfront] Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: fd45e1bc-9a35-4960-a73a-ff845216afe4
source-git-commit: 15aa025c9a35e30867f942047ec1989fdd6834e5
workflow-type: tm+mt
source-wordcount: '2517'
ht-degree: 0%

---

# Configurar o herdado [!DNL SharePoint] integração

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>O novo [!DNL SharePoint] A integração do foi lançada para produção com a versão 22.3 (julho de 2022.) Embora seus usuários ainda possam acessar documentos vinculados por meio do herdado [!DNL SharePoint] integração, eles devem usar o novo [!DNL SharePoint] integração para vincular documentos do SharePoint.
>
>* A nova integração do SharePoint não requer configuração por um administrador e pode ser definida por usuários individuais. No entanto, para garantir uma transição suave para a nova integração do SharePoint, um administrador do Workfront deve fazer algumas pequenas alterações de configurações na área Configuração do Workfront.
   >
   >    Para obter informações e instruções, consulte [Configurar a integração herdada do SharePoint para acesso contínuo aos documentos](#configure-the-legacy-sharepoint-integration-for-continued-access-to-documents) neste artigo.
>    
>* Recomendamos que os usuários vinculem documentos que estão atualmente vinculados por meio do herdado [!DNL SharePoint] integração por meio da nova integração.
   >    
   >    Para obter instruções sobre como vincular documentos, consulte [Vincular documentos de aplicativos externos](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).


É possível integrar [!DNL Workfront] com [!DNL SharePoint Online], proporcionando aos usuários a capacidade de navegar, vincular e adicionar [!DNL SharePoint] documentos no Workfront. A funcionalidade fornecida é semelhante à de outros [!DNL Workfront] integrações, como [!DNL Google Drive], [!DNL Box], e [!DNL Dropbox].

Essa integração é compatível somente com o [!DNL SharePoint Online]. Instâncias locais de [!DNL SharePoint] não são compatíveis.

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas deste artigo:

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
   <td>[!UICONTROL Plano]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador. Para obter informações sobre [!DNL Workfront] administradores, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acesso administrativo total a um usuário</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

## Pré-requisitos

Você deve ter o acesso ou as permissões necessárias no [!DNL SharePoint] para modificar ou configurar o [!DNL SharePoint].

## Vincular documentos por meio da nova integração do SharePoint

Os usuários individuais podem vincular documentos por meio da nova [!DNL SharePoint] integração. A integração não requer configuração de administrador. Em vez disso, o usuário faz logon em seu [!DNL Microsoft] ao vincular um documento, o que permite que a integração acesse documentos disponíveis no [!DNL SharePoint].

Na primeira vez que um usuário se conecta ao [!DNL Workfront] [!DNL SharePoint] integração ao seu [!DNL SharePoint] conta, eles verão e concordarão com todas as permissões que [!DNL Workfront] O usa o ao interagir com a [!UICONTROL SharePoint] conta. Permissões de leitura permitem [!DNL Workfront] para ver e acessar arquivos em [!DNL SharePoint]As permissões de gravação e do permitem que o usuário faça upload de arquivos no [!DNL SharePoint].

![Permissões do SharePoint](assets/sharepoint-permissions.png)

Para obter instruções sobre como vincular documentos por meio do novo [!DNL SharePoint] integração, consulte [Vincular um documento externo a [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

>[!NOTE]
>
>* A [!DNL SharePoint] A integração pode se conectar a um único [!DNL SharePoint] instância. Portanto, um usuário pode configurar uma integração para um [!DNL SharePoint], mas não pode configurar uma integração para um segundo [!DNL SharePoint], mesmo que eles tenham permissões para e documentos no segundo [!DNL SharePoint].
>
>* Um usuário tem acesso aos mesmos sites, coleções, pastas, subpastas e arquivos por meio do [!DNL Workfront] [!DNL SharePoint] integração, tal como acontece na sua [!DNL SharePoint] conta.


## Configurar a integração herdada do SharePoint para acesso contínuo aos documentos

Para garantir que seus usuários tenham acesso contínuo a documentos vinculados ao Workfront por meio da integração herdada do SharePoint, você deve reconfigurar o acesso à integração herdada do SharePoint e manter o SharePoint Client Secret atualizado.

* [Reconfigurar o acesso ao herdado [!DNL SharePoint] integração](#reconfigure-access-to-the-legacy-dnl-sharepoint-integration)
* [Configurar o segredo do cliente para acesso contínuo ao herdado [!DNL SharePoint] integração](#configure-the-client-secret-for-continued-access-to-the-legacy-dnl-sharepoint-integration)

### Reconfigurar o acesso ao herdado [!DNL SharePoint] integração

Para garantir que você possa acessar documentos vinculados por meio do herdado [!DNL SharePoint] integração, garantindo que os usuários não possam vincular novos documentos por meio dessa integração, conclua o procedimento a seguir.

>[!NOTE]
>
> * O legado [!DNL SharePoint] a integração é rotulada como &quot;[!DNL SharePoint].&quot;
> * O novo [!DNL SharePoint] a integração é rotulada como &quot;[!UICONTROL [!DNL SharePoint] (API gráfica)].&quot;


1. Clique em **[!UICONTROL Menu principal]** ícone ![Menu principal](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **[!UICONTROL Configuração]** ![Configuração](../get-started-wf-administration/assets/gear-icon-settings.png).
1. Selecionar **[!UICONTROL Documentos]** na navegação à esquerda, selecione **[!UICONTROL Provedores de nuvem]**.
1. Certifique-se de que a variável **[!DNL SharePoint]** opção e **[!UICONTROL [!DNL SharePoint](API gráfica)]** ambas as opções estão ativadas.
1. Clique em **[!UICONTROL Salvar]**.
1. Selecionar **[!UICONTROL Documentos]** na navegação à esquerda, selecione **[!UICONTROL [!DNL SharePoint]Integração]**.
1. Marque a marca de seleção à esquerda da lista para todas as integrações existentes e selecione **[!UICONTROL Desativar]**.


### Configurar o segredo do cliente para acesso contínuo ao herdado [!DNL SharePoint] integração

Seu [!DNL SharePoint] O segredo do cliente expira uma vez por ano. Para garantir acesso contínuo aos documentos em seu legado [!DNL SharePoint] integração, é necessário manter a [!DNL SharePoint] Segredo do cliente atualizado.

>[!IMPORTANT]
>
> Porque [!DNL SharePoint] Os segredos do cliente são tratados pelo [!DNL Microsoft], os recursos e procedimentos do Segredo do cliente podem ser alterados com base em atualizações no [!DNL SharePoint] feito por [!DNL Microsoft]. Sempre verifique o [!DNL Microsoft] documentação para obter as informações mais recentes sobre procedimentos e recursos em [!DNL SharePoint].

<!--1. Go to the site that your [!DNL SharePoint] integration uses. This may be a site that you created when setting up the integrations, or it may be your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.-->

1. Gere um novo segredo do cliente conforme descrito em [Substituir um segredo de cliente que está expirando em um [!DNL SharePoint] Suplemento](https://docs.microsoft.com/en-us/sharepoint/dev/sp-add-ins/replace-an-expiring-client-secret-in-a-sharepoint-add-in#generate-a-new-secret)
1. Copiar este Segredo do Cliente para um local seguro.
1. Efetue logon no [!DNL Workfront] como administrador.
1. No Workfront, clique no link **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).
1. No painel esquerdo, clique em **[!UICONTROL Documentos]** > **[!UICONTROL [!DNL SharePoint]Integração]**.
1. Clique no link [!DNL SharePoint] que deseja atualizar e, em seguida, clique em **[!UICONTROL Editar]**.
1. Insira o novo Segredo do cliente na caixa **[!UICONTROL Segredo do cliente]** campo.
1. Clique em **[!UICONTROL Salvar]**.



## Instruções para configurar a integração herdada do SharePoint

>[!IMPORTANT]
>
>Essa integração foi descontinuada. As instruções aqui são somente para fins informativos e serão removidas em breve.


O Workfront se conecta ao [!DNL SharePoint] On-line usando o OAuth 2.0, um padrão usado pela maioria das integrações baseadas na Web para a autenticação e autorização de usuários.

Para configurar o OAuth, é necessário criar um [!DNL SharePoint] site e um Aplicativo do site no [!DNL SharePoint]. Esse processo é descrito nas seções a seguir.

Para obter mais informações sobre OAuth, consulte [http://oauth.net](http://oauth.net/).

>[!TIP]
>
>Para facilitar a cópia e colagem de informações entre [!DNL Workfront] e [!DNL SharePoint] nestas etapas, recomendamos manter ambos os aplicativos abertos em guias separadas.

* [Criar e configurar um [!DNL SharePoint] site](#create-and-configure-a-sharepoint-site)
* [Conceder permissões de gravação ao aplicativo de site](#grant-write-permissions-to-the-site-app)
* [Criar um [!DNL Workfront] [!DNL SharePoint] instância de integração](#create-a-workfront-sharepoint-integration-instance)
* [Conclua sua integração](#complete-your-integration)
* [Adicionar documentos](#add-documents)

### Criar e configurar um [!DNL SharePoint] site  {#create-and-configure-a-sharepoint-site}

A fim de [!DNL Workfront] para autenticar com [!DNL SharePoint], [!DNL Workfront] pode usar um site principal no qual os usuários tenham a [!UICONTROL Controle completo] nível de permissão ou permissões específicas de Gerenciamento. Este site principal atua como um Ponto de Entrada de Autenticação para [!DNL Workfront].

Para criar e configurar um [!DNL SharePoint] Site:

1. (Opcional) Se você não quiser usar o site raiz da sua organização, poderá criar um site principal no [!DNL SharePoint].

   Para obter instruções, visite [Criar um site](https://docs.microsoft.com/en-us/sharepoint/create-site-collection) no [!DNL Microsoft] Documentação.

   * Selecione o **[!UICONTROL Site de equipe]** opção ao criar o site.

1. (Condicional) Se você criou um site na etapa 1, vá para o site que acabou de criar.

   Ou

   Se você não criou um site na etapa 1, vá para o site raiz da sua organização.

1. Adicionar `/_layouts/15/appregnew.aspx` ao final do URL na barra de pesquisa na parte superior da janela do navegador.
1. Configure os seguintes campos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL ID do Cliente]</p> </td> 
      <td> <p>Clique em <strong>[!UICONTROL Gerar]</strong> para gerar uma ID do cliente. Copie esta ID para um local seguro. Você o usará posteriormente ao configurar o [!DNL SharePoint] integração no [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Segredo do Cliente]</p> </td> 
      <td> <p>Clique em <strong>[!UICONTROL Gerar]</strong> para gerar um Segredo do cliente. Copiar este Segredo para um local seguro. Você o usará posteriormente ao configurar o [!DNL SharePoint] integração no [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Título</p> </td> 
      <td> <p>Insira um título, como [!DNL Workfront] Aplicativo do site. Os usuários veem esse título ao adicionar documentos.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Domínio de Aplicativo]</p> </td> 
      <td> <p><code>my.workfront.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Redirecionar URI]</p> </td> 
      <td> <p><code>https://oauth.my.workfront.com/oauth2/redirect</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Criar]**
1. Continue para [Conceder permissões de gravação ao aplicativo de site](#grant-write-permissions-to-the-site-app).

### Conceder permissões de gravação ao aplicativo de site  {#grant-write-permissions-to-the-site-app}

Neste ponto, você criou com êxito um Aplicativo de site e o registrou no [!DNL Workfront]. Este aplicativo de site também é conhecido como principal de aplicativo no [!DNL SharePoint]. Ele reside em seu locatário. Os novos aplicativos de site não têm acesso automático aos conjuntos de sites dentro do locatário. As permissões devem ser concedidas explicitamente para cada conjunto de sites. As etapas abaixo mostrarão como conceder permissão de Gravação ao novo Aplicativo de Site em um conjunto de sites. Repita essas etapas para cada um dos conjuntos de sites adicionados em [!UICONTROL Conjuntos de Sites Visíveis] nas etapas acima.

Este aplicativo de site deve ter [!UICONTROL Gravar] permissão para qualquer conjunto de sites que os usuários precisem acessar por meio do [!DNL Workfront].

1. Adicionar &#39;/_layouts/15/appinv.aspx&#39; ao URL em [!DNL Sharepoint].

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
      <td role="rowheader">[!UICONTROL ID do Aplicativo]</td> 
      <td> <p>Adicione a ID do cliente que você criou no <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Criar e configurar um [!DNL SharePoint] site </a>e clique em <strong>[!UICONTROL Pesquisa]</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client] / [!UICONTROL App Domain] / [!UICONTROL Redirecionar URL]</p> </td> 
      <td> <p>Estes são automaticamente preenchidos quando você clica em [!UICONTROL Pesquisa].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL XML de Solicitação de Permissão]</td> 
      <td> <p>Copie o seguinte XML no campo [!UICONTROL XML de Solicitação de Permissão]. Verifique se ele foi adicionado exatamente como mostrado, sem espaços adicionais, etc. para evitar erros.</p> 
      <div></a> 
      <div style="mc-code-lang: XML;" class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False"> 
       <pre></pre></div></div></td></tr></tbody></table>

1. Clique em **[!UICONTROL Criar]**.
1. Na caixa de diálogo exibida, clique em **[!UICONTROL Confiar]**.
1. Verifique se o aplicativo de site tem acesso ao conjunto de sites clicando no **[!UICONTROL Permissões do aplicativo de conjunto de sites]** link em [!UICONTROL Configurações do site].
1. Repita as etapas acima para os conjuntos de sites restantes e continue com [Criar um [!DNL Workfront] [!DNL SharePoint] instância de integração](#create-a-workfront-sharepoint-integration-instance).

### Criar um [!DNL Workfront] [!DNL SharePoint] instância de integração {#create-a-workfront-sharepoint-integration-instance}

Quando você tiver criado um aplicativo de site no [!DNL SharePoint], agora você pode copiar informações do aplicativo do site para [!DNL Workfront]. O aplicativo de site é um principal aplicativo e atua como o canal pelo qual as solicitações OAuth são feitas para acessar documentos em conjuntos de sites.

1. Efetue logon no [!DNL Workfront] como administrador.
1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **[!UICONTROL Documentos]** > **[!UICONTROL [!DNL SharePoint]Integração]**.
1. Clique em **[!UICONTROL Adicionar[!DNL SharePoint]]**.
1. Configure os seguintes campos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nome]</p> </td> 
      <td> <p>Insira um nome para o [!DNL SharePoint] integração. Os usuários veem esse nome ao clicar em [!UICONTROL Adicionar] &gt; [!UICONTROL De] 'nome da integração'. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL SharePoint] Instância do Host]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.sharepoint.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL Azure] Domínio de acesso]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.onmicrosoft.com</code> </p> <p>Refere-se ao Site Principal pelo qual os usuários usarão para se autenticar. É provavelmente o mesmo domínio que [!UICONTROL [!DNL SharePoint] Instância do Host].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>
      </p> </td> 
      <td> <b>Importante</b> Os conjuntos de sites são usados somente no herdado [!DNL SharePoint] Integração.
       <ul> 
        <li> <p><b>Se estiver usando o site raiz da sua organização</b><b>:</b> </p> <p>Enter <code>/</code></p> </li> 
        <li> <p><b>Se você estiver usando um site principal e subsites:</b> </p> <p><b>IMPORTANTE</b>: [!DNL Microsoft SharePoint] O não recomenda mais o uso de subsites.</p> <p>Insira a base de URL do conjunto de sites criado na seção acima.</p> <p>Esta é a seção do URL após .com.</p> <p>Exemplo: para o URL <code>https://mycompany.sharepoint.com/sites/mysite</code>, o caule seria <code>/sites/mysite</code>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] ID do cliente]</td> 
      <td>Insira a ID do cliente gerada no <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Criar e configurar um [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Segredo do cliente]</td> 
      <td>Digite o segredo do cliente que você gerou em <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Criar e configurar um [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Conjuntos de Sites Visíveis]</td> 
      <td> <b>Importante</b> Os conjuntos de sites são usados somente no herdado [!DNL SharePoint] integração.
       <ul> 
        <li> <p><b> Se estiver usando o site raiz da sua organização</b><b>:</b> </p> <p>Enter <code>/</code></p> </li> 
        <li> <p><b>Se você estiver usando um site principal e subsites:</b> </p> <p><b>IMPORTANTE</b>: [!DNL Microsoft SharePoint] O não recomenda mais o uso de subsites.</p> <p>Para cada subsite que você deseja adicionar ao seu [!DNL SharePoint] integração, insira a raiz do subsite.</p> <p>Exemplo: para o URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, o caule seria <code>/sites/mysite/mysubsite</code>.</p> <p><b>Nota</b>:   <p>Se você quiser testar somente sua configuração (sem subsites), insira a raiz do site principal. </p> <p>Exemplo: para o URL <code> https://mycompany.sharepoint.com/sites/mysite</code>, o caule seria <code>/sites/mysite</code>.</p> <p>Depois de testar sua configuração conforme descrito em <a href="#complete-your-integration" class="MCXref xref">Conclua sua integração</a>, você deve remover o site principal e inserir os subsites.</p> 
          <ol> 
           <li value="1">Clique em <strong>[!UICONTROL Menu Principal]</strong> ícone <img src="assets/main-menu-icon.png"> no canto superior direito de [!DNL Adobe Workfront]e, em seguida, clique em <strong>[!UICONTROL Instalação]</strong> <img src="assets/gear-icon-settings.png">.<li><p>No painel esquerdo, clique em <strong>[!UICONTROL Documentos]</strong> &gt; <strong>[!UICONTROL [!DNL SharePoint] Integração]</strong>.</p></li><li><p>Clique em [!DNL SharePoint] integração que estiver configurando e, em seguida, clique em Editar.</p></li><li><p>Exclua a raiz do site principal do campo [!UICONTROL Conjuntos de Sites Visíveis].</p></li><li><p>Para cada subsite que você deseja adicionar ao seu [!DNL SharePoint] integração, insira a raiz do subsite.</p></li><p>Exemplo: para o URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, o caule seria <code>/sites/mysite/mysubsite</code>.</p></li> 
          </ol> </p> </li> 
       </ul> <p> </p> <p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Salvar]**
1. Continue para [Conclua sua integração](#complete-your-integration).

### Conclua sua integração {#complete-your-integration}

A configuração básica está quase completa.

1. No Workfront, clique no link **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **[!UICONTROL Documentos]** ![](assets/document-icon.png).
1. Clique em **[!UICONTROL Adicionar novo]**.
1. Clique em **[!UICONTROL De]`<title of your [!DNL SharePoint] site>`** na lista suspensa.

   Uma caixa de diálogo que convida você a confiar neste site é exibida.

   >[!NOTE]
   >
   >Se essa caixa de diálogo não for exibida, suas [!DNL SharePoint] A integração do não está configurada corretamente.

1. Clique em **[!UICONTROL Confiar]**.

### Adicionar documentos {#add-documents}

Agora você pode adicionar documentos de seu [!DNL SharePoint] local.

Para obter instruções, consulte [Vincular um documento externo a [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) in [Vincular documentos de aplicativos externos](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)

>[!IMPORTANT]
>
>Se o usuário que vinculou uma pasta não tiver mais acesso ao aplicativo externo, [!DNL Workfront] O não pode mais acessar o conteúdo da pasta. Isso pode acontecer, por exemplo, se o usuário que originalmente vinculou a pasta sair da empresa. Para garantir acesso contínuo, um usuário com acesso à pasta deve vincular novamente a pasta.

## Solução de problemas

* [Problema: os usuários experimentam erros baseados em autenticação ao usar o [!DNL SharePoint] integração.](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [Problema: As a [!DNL Workfront] usuário, não consigo provisionar um novo [!DNL SharePoint] instância. Quando tento fazer, vejo um erro.](#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error)
* [Problema: ao tentar navegar [!DNL SharePoint] arquivos em [!DNL Workfront]No entanto, não vejo nenhum ou todos os conjuntos de sites.](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [Problema: não consigo acessar pastas e documentos vinculados anteriormente no [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### Problema: os usuários experimentam erros baseados em autenticação ao usar o [!DNL SharePoint] integração. {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

Soluções:

Os usuários devem ser membros de um grupo que tenha permissões apropriadas para o [!DNL SharePoint] local.

Usuários com [!UICONTROL Controle completo] ter todas as permissões necessárias para o [!DNL SharePoint] integração. Se não quiser conceder acesso de Controle total aos usuários, você deverá conceder as seguintes permissões:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Design]</p> </td> 
   <td> <p>Pode exibir, adicionar, atualizar, excluir, aprovar e personalizar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Editar]</p> </td> 
   <td> <p>Pode adicionar, editar e excluir listas; pode exibir, adicionar, atualizar e excluir itens de lista e documentos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contribute]</p> </td> 
   <td> <p>Pode exibir, adicionar, atualizar e excluir itens de lista e documentos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Somente exibição]</p> </td> 
   <td> <p>Pode exibir páginas, itens de lista e documentos (tipos de documento com manipuladores de arquivo do lado do servidor podem ser exibidos no navegador, mas não baixados)</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter instruções sobre como criar e editar níveis de permissão, consulte [Como criar e editar níveis de permissão](https://docs.microsoft.com/en-us/sharepoint/how-to-create-and-edit-permission-levels) na documentação do Microsoft.

### Problema: As a [!DNL Workfront] usuário, não consigo provisionar um novo [!DNL SharePoint] instância. Quando tento fazer, vejo um erro. {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

Soluções:

Isso pode ser causado por vários motivos, originados em [!DNL Workfront] ou [!DNL SharePoint]configuração de. Verifique se:

* A ID do cliente, o Segredo do cliente, o URL de retorno e outros campos de configuração estão mapeados corretamente entre [!DNL Workfront] [!DNL SharePoint] Instância de integração e o [!DNL SharePoint] Aplicativo do site.
* O usuário tem [!UICONTROL Controle completo] permissão para o Conjunto de Sites usado para autenticação.
* O Aplicativo do site está listado em [!UICONTROL Permissões do aplicativo do site] para o [!UICONTROL Conjunto de Sites] usado para autenticação.

### Problema: ao tentar navegar [!DNL SharePoint] arquivos em [!DNL Workfront]No entanto, não vejo nenhum ou todos os conjuntos de sites. {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

Soluções:

Para ver um conjunto de sites em [!DNL Workfront], as seguintes condições devem ser atendidas:

* O conjunto de sites deve ser registrado na [!DNL Workfront] [!DNL SharePoint] Instância de integração.

   Para verificar isso em [!DNL Workfront]:

   1. Ir para [!UICONTROL Configuração] > [!UICONTROL Documentos] > [!UICONTROL [!DNL SharePoint] Integração].
   1. Edite o [!DNL SharePoint] Informações da instância de integração.
   1. Verifique se o conjunto de sites está listado em [!UICONTROL Conjuntos de Sites Visíveis].

* O usuário deve ter acesso de visualização ao conjunto de sites em [!DNL SharePoint].
* Para verificar isso em [!DNL SharePoint], vá para [!DNL SharePoint]e abra o conjunto de sites > [!UICONTROL Configurações] > [!UICONTROL Permissões do site].
* A variável [!DNL SharePoint] O Aplicativo do Site deve ter acesso ao conjunto de sites.

   Para verificar isso em [!DNL SharePoint]:

   1. Ir para o conjunto de sites > [!UICONTROL Configurações] > [!UICONTROL Permissões do aplicativo do site].
   1. Certifique-se de que o [!UICONTROL Aplicativo do site] usado por [!DNL Workfront] está listado aqui.
   1. (Condicional) Se o Aplicativo do site não estiver listado, adicione ao conjunto de sites usando _layouts/15/appinv.aspx.

      Para obter informações sobre como adicionar o conjunto de sites, consulte Concedendo permissões de gravação ao aplicativo do site.

### Problema: não consigo acessar pastas e documentos vinculados anteriormente no [!DNL SharePoint]. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

Solução:

Se o usuário que vinculou um [!DNL SharePoint] a pasta não pode mais ser autenticada, [!DNL Workfront] O não pode mais acessar o conteúdo da pasta. Isso pode acontecer, por exemplo, se o usuário que originalmente vinculou a pasta sair da empresa.

Para garantir acesso contínuo, um usuário com acesso à pasta deve vincular novamente a pasta.

Para obter informações sobre como vincular pastas de provedores externos, consulte [Vincular documentos de aplicativos externos](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Problema: vejo um erro &quot;404 não encontrado&quot; ao tentar adicionar um documento do [!DNL Sharepoint]

#### Solução:

Esse erro pode ocorrer se um dos sites configurados no [!UICONTROL Conjuntos de Sites Visíveis] A lista foi excluída no Sharepoint. Verifique a [!UICONTROL Conjuntos de Sites Visíveis] e remova todos os sites que foram excluídos no Sharepoint.
