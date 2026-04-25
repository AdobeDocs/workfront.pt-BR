---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Use Workfront Fusion to create a Workfront Project that has Adobe Experience Manager workflows
description: If you are creating a project through Workfront Fusion and want to include Adobe Experience Manager workflows on the project, you must use a specific Fusion module configuration, described in this article.
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps, Workfront Fusion
exl-id: b8132d5e-234d-47f6-a09c-ca46018a2d77
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 11%

---

# Usar o Workfront Fusion para converter um problema do Workfront em um projeto que inclui fluxos de trabalho do Adobe Experience Manager

If you are creating a project through Workfront Fusion and want to include Adobe Experience Manager workflows on the project, you must use a specific Fusion module configuration, described in this article.

>[!NOTE]
>
>Workflows are available only in an Adobe Experience Manager as a Cloud Service integration. They are not available in integrations with Adobe Experience Manager Assets Essentials.<br>
>Essa funcionalidade não está disponível na área de novos documentos.


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table>
  <tr>
    <td><strong>Pacote do Adobe Workfront</strong></td>
   <td> <p>Qualquer pacote de fluxo de trabalho do Adobe Workfront e qualquer pacote do Adobe Workfront Automation and Integration</p><p>Workfront Ultimate</p><p>Os pacotes Workfront Prime e Select, com uma compra adicional do Workfront Fusion.</p> </td> 
  </tr>
  <tr>
   <td><strong>Licenças do Adobe Workfront</strong></td>
   <td><p>Colaborador ou posterior</p><p>Solicitação ou posterior</p></td>
  </tr>
  <tr>
   <td><strong>Produto</strong></td>
   <td>
     <p><b>Adobe Experience Manager:</b></p>
     <ul>
       <li>
         <p>You must have Experience Manager Assets as a Cloud Service or Assets Essentials, and you must be added to the product as a user in the Admin Console.</p>
       </li>
       <li>
        <p>You must have write access to the repository in Adobe Experience Manager.</p>
       </li>
     </ul>
     <p><b>Workfront Fusion:</b></p>
     <ul>
       <li>
        <p>Se sua organização tiver um pacote Workfront Select ou Prime, ele não inclui o Workfront Automation and Integration. É necessário comprar o Adobe Workfront Fusion.</li></ul>
       </li>
     </ul>
   </td>
  </tr>
  <tr>
   <td><strong>Configurações de nível de acesso</strong>
   </td>
   <td><p>Editar acesso a documentos</p>
   </td>
  </tr>
</table>

+++

## Pré-requisitos

Antes de começar,

* Your Workfront administrator must configure workflows in an Adobe Experience Manager integration. For more information, see [Configure the Experience Manager Assets as a Cloud Service integration](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).
* You must have a project template configured with an Adobe Experience Manager integration linked folder workflow.
* You must have created an OAuth application in Workfront to configure the connection for this module.

  For instructions, see [Create an OAuth application](#create-an-oauth-application) in this article.

## Module configuration

In Workfront Fusion, if you want to create a project that includes Adobe Experience Manager workflows, you must use the Workfront > Misc Action module.

1. Add the **Workfront** > **Misc Action** module to your scenario.
1. In the **Connection** field, select the Workfront connection that connects to the account this module will use.

   For instructions on creating a connection, see [Connect [!DNL Workfront] to [!DNL Workfront Fusion]](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules#connect-workfront-to-workfront-fusion) in the article Workfront modules.

   For instructions on creating the Client ID and Client Secret you will need to create a connection, see [Create an OAuth application](#create-an-oauth-application) in this article.

1. No campo **Tipo de Registro**, selecione `Issue`.
1. No campo **Ação**, selecione `convertToProject`.
1. No campo **ID**, insira ou mapeie a ID do problema que você está convertendo em um projeto.
1. Habilitar **Mostrar configurações avançadas**.
1. Role para a parte inferior do módulo e localize o campo **Projeto (Coleção avançada)**.
1. Cole o texto a seguir no campo **Projeto (Coleção Avançada)**.

   ```
   {
       "aemNativeFolderTreeIDs": ["Folder Tree ID here"],
       "aemNativeFolderWorkflowEnabled": "true",
       "name": "New project name here",
       "templateID": "Template ID here"
   }
   ```

1. Substituir `Folder tree ID here` pelas IDs da pasta.

   Para localizar IDs de árvore de pastas, consulte [Localizar IDs de árvore de pastas](#locate-folder-tree-ids) neste artigo.

   Para usar mais de uma árvore de pastas, separe as IDs com uma vírgula:

   `"aemNativeFolderTreeIDs": ["Folder tree ID here","Second folder tree ID here"],`
1. Substitua `New project name here` pelo nome que o novo projeto terá.
1. Substitua `Template ID here` pela ID do modelo que você está usando para o novo projeto.

   Você pode mapear a ID do modelo de um módulo anterior (como um módulo Workfront > Pesquisar ) ou localizá-lo no URL da página do modelo no Workfront.

1. Clique em **OK** para salvar a configuração do módulo.

## Localizar IDs de árvore de pastas

Para localizar as IDs da árvore de pastas:

>[!NOTE]
>
>Essas instruções usam o navegador Chrome.

1. No Workfront, abra o modelo que deseja usar para esse projeto. Esse modelo deve incluir a configuração do Adobe Experience Manager que você deseja usar para o projeto.
1. Abra as ferramentas do desenvolvedor do seu navegador.
1. Abra a guia **Rede** nas ferramentas do desenvolvedor.
1. Na caixa **Filtro**, digite `object-workflow`.
1. Na coluna Nome, clique na ID alfanumérica exibida.

   ![Localizando ID de pasta 1](assets/finding-folder-id-1.png)

1. Clique na guia **Visualização** à direita da ID alfanumérica.
1. Abra as seguintes seções recolhidas:
   1. `data`
   1. `objectWorkflow`
   1. `workflows`
   1. `enhancedLinkedFolderCreationWorkflow`
   1. `enhancedLinkedFolderCreationWorkflowConfigurations`

   Cada árvore de pastas é representada por um número. 0 (zero) representa a primeira pasta na lista, 1 representa a segunda e assim por diante. Se o modelo incluir apenas uma árvore de pastas, será o número 0.

1. Abra a árvore de pastas que deseja usar para o novo projeto. Anote o valor do campo `_id`. Se quiser usar mais de uma árvore de pastas, anote todos os valores de campo `_id` das árvores de pastas que deseja usar.

   ![Localizando ID de pasta 2](assets/finding-folder-id-2.png)

   Estes são os valores de `aemNativeFolderTreeIDs` que você inserirá no campo **Projeto (Coleção Avançada)** no módulo **Workfront** > **Ações Diversas** Fusion.

## Criar um aplicativo OAuth

Você deve configurar um aplicativo OAuth no Workfront para a conexão deste módulo. Só é necessário fazer isso uma vez para uma determinada conexão do Workfront no Fusion.

1. No Workfront, comece a criar um aplicativo OAuth, conforme descrito em [Criar um aplicativo OAuth2 usando credenciais de usuário (Fluxo de código de autorização)](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-application-using-user-credentials-authorization-code-flow) no artigo Criar aplicativos OAuth2 para integrações [!DNL Workfront].
1. Copie a ID do cliente e o segredo do cliente para um local seguro.
1. No campo **Redirecionar URIs**, digite o seguinte:

   ```
   http://app.workfrontfusion.com/oauth/cb/workfront-workfront
   ```

1. Clique em **Salvar**.

Você usará essa ID do cliente e o segredo do cliente ao configurar a conexão do módulo no Fusion.

Para obter instruções sobre como criar uma conexão, consulte [Conectar [!DNL Workfront] a [!DNL Workfront Fusion]](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules#connect-workfront-to-workfront-fusion) no artigo Módulos do Workfront.
