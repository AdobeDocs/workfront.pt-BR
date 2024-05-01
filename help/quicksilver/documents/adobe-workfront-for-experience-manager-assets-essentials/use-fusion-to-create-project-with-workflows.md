---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Usar o Workfront Fusion para criar um Projeto do Workfront com fluxos de trabalho do Adobe Experience Manager
description: Se você estiver criando um projeto por meio do Workfront Fusion e quiser incluir fluxos de trabalho do Adobe Experience Manager no projeto, deverá usar uma configuração específica do módulo Fusion, descrita neste artigo.
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps, Workfront Fusion
exl-id: b8132d5e-234d-47f6-a09c-ca46018a2d77
source-git-commit: 012aa4c15bcdb26a3e30f8c143599a7e90c9a0f3
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---

# Usar o Workfront Fusion para converter um problema do Workfront em um projeto que inclui fluxos de trabalho do Adobe Experience Manager

Se você estiver criando um projeto por meio do Workfront Fusion e quiser incluir fluxos de trabalho do Adobe Experience Manager no projeto, deverá usar uma configuração específica do módulo Fusion, descrita neste artigo.

>[!NOTE]
>
>Os fluxos de trabalho estão disponíveis somente em uma integração com o Adobe Experience Manager as a Cloud Service. Eles não estão disponíveis em integrações com o Adobe Experience Manager Assets Essentials.


## Requisitos de acesso

Você deve ter o seguinte:

<table>
  <tr>
    <td><strong>plano do Adobe Workfront*</strong></td>
    <td>Qualquer</td>
  </tr>
  <tr>
   <td><strong>Licenças da Adobe Workfront*</strong></td>
   <td>Solicitação ou superior</td>
  </tr>
  <tr>
   <td><strong>Produto</strong></td>
   <td>
     <p><b>Adobe Experience Manager:</b></p>
     <ul>
       <li>
         <p>Você deve ter o Experience Manager Assets as a Cloud Service ou Assets Essentials e ser adicionado ao produto como usuário no Admin Console.</p>
       </li>
       <li>
        <p>Você deve ter acesso de gravação ao repositório no Adobe Experience Manager.</p>
       </li>
     </ul>
     <p><b>Workfront Fusion:</b></p>
     <p>Novo:</p>
     <ul>
       <li>
         <p>Selecione ou Prime Workfront Plan: sua organização deve comprar o Adobe Workfront Fusion.</p>
       </li>
       <li> 
         <p>Plano Ultimate do Workfront: o Workfront Fusion está incluído.</p>
       </li>
     </ul>
     <p>Ou</p>
     <p>Atual: sua organização deve comprar o Adobe Workfront Fusion.</p>
   </td>
  </tr>
  <tr>
   <td><strong>Configurações de nível de acesso*</strong>
   </td>
   <td>Editar acesso a documentos
     <p>
       <strong>Nota: </strong>Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <strong>Criar ou modificar níveis de acesso personalizados</strong>.
     </p>
   </td>
  </tr>
</table>

## Pré-requisitos

Antes de começar,

* O administrador do Workfront deve configurar os workflows em uma integração com o Adobe Experience Manager. Para obter mais informações, consulte [Configurar a integração as a Cloud Service do Experience Manager Assets](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).
* Você deve ter um modelo de projeto configurado com um fluxo de trabalho de pasta vinculado à integração do Adobe Experience Manager.
* Você deve ter criado um aplicativo OAuth no Workfront para configurar a conexão para esse módulo.

  Para obter instruções, consulte [Criar um aplicativo OAuth](#create-an-oauth-application) neste artigo.

## Configuração do módulo

No Workfront Fusion, se quiser criar um projeto que inclua fluxos de trabalho do Adobe Experience Manager, use o módulo Workfront > Ação diversa.

1. Adicione o **Workfront** > **Ação Diversa** para o seu cenário.
1. No **Conexão** , selecione a conexão do Workfront que se conecta à conta que esse módulo usará.

   Para obter instruções sobre como criar uma conexão, consulte [Conectar [!DNL Workfront] para [!DNL Workfront Fusion]](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#connect-workfront-to-workfront-fusion) no artigo módulos do Workfront.

   Para obter instruções sobre como criar a ID do cliente e o Segredo do cliente, será necessário criar uma conexão, consulte [Criar um aplicativo OAuth](#create-an-oauth-application) neste artigo.

1. No **Tipo de registro** selecione `Issue`.
1. No **Ação** selecione `convertToProject`.
1. No **ID** insira ou mapeie a ID do problema que você está convertendo em um projeto.
1. Ativar **Mostrar configurações avançadas**.
1. Role para a parte inferior do módulo e localize a **Projeto (Coleção Avançada)** campo.
1. Cole o texto a seguir na **Projeto (Coleção Avançada)** campo.

   ```
   {
       "aemNativeFolderTreeIDs": ["Folder Tree ID here"],
       "aemNativeFolderWorkflowEnabled": "true",
       "name": "New project name here",
       "templateID": "Template ID here"
   }
   ```

1. Substituir `Folder tree ID here` com as IDs da pasta.

   Para localizar IDs de árvore de pastas, consulte [Localizar IDs de árvore de pastas](#locate-folder-tree-ids) neste artigo.

   Para usar mais de uma árvore de pastas, separe as IDs com uma vírgula:

   `"aemNativeFolderTreeIDs": ["Folder tree ID here","Second folder tree ID here"],`
1. Substituir `New project name here` com o nome que o novo projeto terá.
1. Substituir `Template ID here` com a ID do modelo que você está usando para o novo projeto.

   Você pode mapear a ID do modelo de um módulo anterior (como um módulo Workfront > Pesquisar ) ou localizá-lo no URL da página do modelo no Workfront.

1. Clique em **OK** para salvar a configuração do módulo.

## Localizar IDs de árvore de pastas

Para localizar as IDs da árvore de pastas:

>[!NOTE]
>
>Essas instruções usam o navegador Chrome.

1. No Workfront, abra o modelo que deseja usar para esse projeto. Esse modelo deve incluir a configuração do Adobe Experience Manager que você deseja usar para o projeto.
1. Abra as ferramentas do desenvolvedor do seu navegador.
1. Abra o **Rede** nas ferramentas do desenvolvedor.
1. No **Filtro** , insira `object-workflow`.
1. Na coluna Nome, clique na ID alfanumérica exibida.

   ![Localizando ID de pasta 1](assets/finding-folder-id-1.png)

1. Clique em **Visualizar** à direita da ID alfanumérica.
1. Abra as seguintes seções recolhidas:
   1. `data`
   1. `objectWorkflow`
   1. `workflows`
   1. `enhancedLinkedFolderCreationWorkflow`
   1. `enhancedLinkedFolderCreationWorkflowConfigurations`

   Cada árvore de pastas é representada por um número. 0 (zero) representa a primeira pasta na lista, 1 representa a segunda e assim por diante. Se o modelo incluir apenas uma árvore de pastas, será o número 0.

1. Abra a árvore de pastas que deseja usar para o novo projeto. Anote o `_id` valor do campo. Se quiser usar mais de uma árvore de pastas, anote todas as `_id` valores de campo para as árvores de pastas que deseja usar.

   ![Localizando ID de pasta 2](assets/finding-folder-id-2.png)

   Estas são as `aemNativeFolderTreeIDs`  valores que você inserirá na variável **Projeto (Coleção Avançada)** no campo **Workfront** > **Ações diversas** Módulo Fusion.

## Criar um aplicativo OAuth

Você deve configurar um aplicativo OAuth no Workfront para a conexão deste módulo. Só é necessário fazer isso uma vez para uma determinada conexão do Workfront no Fusion.

1. No Workfront, comece criando um aplicativo OAuth, conforme descrito em [Criar um aplicativo OAuth2 usando credenciais do usuário (Fluxo de código de autorização)](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-application-using-user-credentials-authorization-code-flow) no artigo Criar aplicativos OAuth2 para o [!DNL Workfront] integrações.
1. Copie a ID do cliente e o segredo do cliente para um local seguro.
1. No **URIs de redirecionamento** insira o seguinte:

   ```
   http://app.workfrontfusion.com/oauth/cb/workfront-workfront
   ```

1. Clique em **Salvar**.

Você usará essa ID do cliente e o segredo do cliente ao configurar a conexão do módulo no Fusion.

Para obter instruções sobre como criar uma conexão, consulte [Conectar [!DNL Workfront] para [!DNL Workfront Fusion]](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#connect-workfront-to-workfront-fusion) no artigo módulos do Workfront.
