---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Usar o Workfront Fusion para criar um Projeto do Workfront com fluxos de trabalho do Adobe Experience Manager
description: Se você estiver criando um projeto por meio do Workfront Fusion e quiser incluir fluxos de trabalho do Adobe Experience Manager no projeto, deverá usar uma configuração específica do módulo Fusion, descrita neste artigo.
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps, Workfront Fusion
exl-id: b8132d5e-234d-47f6-a09c-ca46018a2d77
source-git-commit: 6a21465ab8c92888c83344f33574302c5cc446e8
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 0%

---

# Usar o Workfront Fusion para converter um problema do Workfront em um projeto que inclui fluxos de trabalho do Adobe Experience Manager

Se você estiver criando um projeto por meio do Workfront Fusion e quiser incluir fluxos de trabalho do Adobe Experience Manager no projeto, deverá usar uma configuração específica do módulo Fusion, descrita neste artigo.

>[!NOTE]
>
>Os fluxos de trabalho estão disponíveis somente em uma integração com o Adobe Experience Manager as a Cloud Service. Não estão disponíveis em integrações com o Adobe Experience Manager Assets Essentials.


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table>
  <tr>
    <td><strong>Pacote do Adobe Workfront</strong></td>
   <td> <p>Qualquer pacote de fluxo de trabalho do Adobe Workfront e qualquer pacote de Automação e Integração do Adobe Workfront</p><p>Workfront Ultimate</p><p>Workfront Prime e pacotes Select, com uma compra adicional do Workfront Fusion.</p> </td> 
  </tr>
  <tr>
   <td><strong>Licenças do Adobe Workfront</strong></td>
   <td><p>Colaborador ou superior</p><p>Solicitação ou superior</p></td>
  </tr>
  <tr>
   <td><strong>Produto</strong></td>
   <td>
     <p><b>Adobe Experience Manager:</b></p>
     <ul>
       <li>
         <p>Você deve ter o Experience Manager Assets as a Cloud Service ou o Assets Essentials e deve ser adicionado ao produto como usuário na Admin Console.</p>
       </li>
       <li>
        <p>Você deve ter acesso de gravação ao repositório no Adobe Experience Manager.</p>
       </li>
     </ul>
     <p><b>Workfront Fusion:</b></p>
     <ul>
       <li>
        <p>Se sua organização tiver um pacote Select ou Prime Workfront que não inclua a Automação e Integração do Workfront, ela deverá comprar o Adobe Workfront Fusion.</li></ul>
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

* O administrador do Workfront deve configurar os workflows em uma integração com o Adobe Experience Manager. Para obter mais informações, consulte [Configurar a integração do Experience Manager Assets as a Cloud Service](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).
* Você deve ter um modelo de projeto configurado com um fluxo de trabalho de pasta vinculado à integração do Adobe Experience Manager.
* Você deve ter criado um aplicativo OAuth no Workfront para configurar a conexão para esse módulo.

  Para obter instruções, consulte [Criar um aplicativo OAuth](#create-an-oauth-application) neste artigo.

## Configuração do módulo

No Workfront Fusion, se quiser criar um projeto que inclua fluxos de trabalho do Adobe Experience Manager, use o módulo Workfront > Ação diversa.

1. Adicione o módulo **Workfront** > **Misc Action** ao seu cenário.
1. No campo **Conexão**, selecione a conexão do Workfront que se conecta à conta que esse módulo usará.

   Para obter instruções sobre como criar uma conexão, consulte [Conectar [!DNL Workfront] a [!DNL Workfront Fusion]](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules#connect-workfront-to-workfront-fusion) no artigo Módulos do Workfront.

   Para obter instruções sobre como criar a ID do cliente e o Segredo do cliente, será necessário criar uma conexão, consulte [Criar um aplicativo OAuth](#create-an-oauth-application) neste artigo.

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
