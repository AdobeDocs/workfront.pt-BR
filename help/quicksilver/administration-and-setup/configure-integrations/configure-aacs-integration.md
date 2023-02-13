---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Integrações do Adobe Experience Manager Assets
description: Você pode conectar seu trabalho com as seguintes Integrações de ativos da Adobe Experience Manager.
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: f3af39e760b2b407cda5ab78497cdc775defdcf6
workflow-type: tm+mt
source-wordcount: '850'
ht-degree: 0%

---

# Configure o [!UICONTROL Experience Manager Assets as a Cloud Service] integração

Você pode conectar seu trabalho com seu conteúdo em [!DNL Experience Manager Assets]&#x200B;:

* Encaminhar ativos e metadados de [!DNL Adobe Workfront] para [!DNL Experience Manager Assets]&#x200B;
* Vincular ativos de [!DNL Experience Manager Assets] para seus projetos e tarefas em [!DNL Workfront&#x200B;]
* Facilitar casos de uso de controle de versão
* Criar pastas vinculadas a [!DNL Experience Manager Assets]
* Rastrear metadados para ativos e pastas
* Sincronizar metadados do projeto entre [!DNL Workfront] e [!DNL Experience Manager Assets]


## Requisitos de acesso

Você deve ter o seguinte:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plano*</strong>
   </td>
   <td>Qualquer Um
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenças*</strong>
   </td>
   <td>[!UICONTROL Plan]
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Experience Manager] licença</strong>
   </td>
   <td>[!UICONTROL Padrão]
   </td>
  </tr>
  <tr>
   <td><strong>Produto</strong>
   </td>
   <td>Você deve ter [!DNL Experience Manager Assets as a Cloud Service]e você deve ser adicionado ao produto como um usuário.
   </td>
  </tr>
  <tr>
   <td>Configurações de nível de acesso*
   </td>
   <td>Você deve ser um [!DNL Workfront] administrador. Para obter informações sobre [!DNL Workfront] administradores, consulte <strong>Conceder ao usuário acesso administrativo total</strong>.
   </td>
  </tr>
</table>


*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.


## Pré-requisitos

Antes de começar,

* Você deve ter [!DNL Workfront] e [!DNL Adobe Experience Manager Assets] associada a uma ID da organização na [!DNL Adobe Admin Consol]e. Para obter mais informações, consulte [Diferenças de administração baseadas em plataforma ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


## Configurar as informações de integração

1. Clique no botão **[!UICONTROL Menu principal]** no canto superior direito do Adobe Workfront, em seguida, clique em **[!UICONTROL Configuração]** .
1. Selecionar **[!UICONTROL Documentos]** no painel esquerdo e selecione **[!UICONTROL [!DNL Experience Manager]Integração]**.
   >[!NOTE]
   >
   >Essa área de configuração aparece somente se sua [!DNL Workfront] o ambiente está incluído em um [!DNL Adobe Admin Console].

1. Selecionar **[!UICONTROL Adicionar [!DNL Experience Manager] Integração]**.
1. No **[!UICONTROL Nome]** , insira o nome que deseja que os usuários vejam ao interagir com essa integração no Workfront e no Experience Manager Assets.
1. No **[!UICONTROL URL de navegação]** , o sistema preenche automaticamente o URL de navegação. Esse URL somente leitura é usado para vincular ao [!DNL Experience Manager] da [!UICONTROL Menu principal] para acesso rápido.
1. Escolha um repositório no **[!UICONTROL [!DNL Experience Manager]Repositório de ativos]** menu suspenso. O sistema preenche qualquer [!DNL Experience Manager] repositórios associados à ID da organização à qual o perfil do usuário está atribuído.
   ![escolha o repositório do experience manager](assets/setup-information.png)

1. Clique em **[!UICONTROL Salvar]** ou vá para a [Configurar metadados (opcional)](#set-up-metadata-optional) neste artigo.

   >[!NOTE]
   >
   >Devido à complexidade da integração, não é possível alterar o repositório depois de salvar a configuração inicial.

## Configurar metadados (opcional)

Você pode mapear [!DNL Workfront] dados de objeto para campos de mídia de ativos em [!DNL Experience Manager] Ativos.

>[!IMPORTANT]
>
>Você pode mapear metadados somente em uma direção: from [!DNL Workfront] para [!DNL Experience Manager]. Metadados para documentos vinculados a [!DNL Workfront] from [!DNL Experience Manager] não pode ser transferido para [!DNL Workfront].



### Configurar campos de metadados

1. Configurar um esquema de metadados em [!DNL Experience Manager Assets] como explicado em [Configurar o mapeamento de metadados de ativos entre o Adobe [!DNL Workfront] e [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
1. Configure campos de formulário personalizados no Workfront. [!DNL Workfront] O tem muitos campos personalizados incorporados que podem ser usados. No entanto, também é possível criar seus próprios campos personalizados, conforme explicado em [Criar ou editar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).


### Ativos

Os metadados mapeiam quando um ativo é enviado de [!DNL Workfront] pela primeira vez. Documentos com os campos incorporados ou personalizados são mapeados automaticamente para os campos especificados na primeira vez que um ativo é enviado para [!DNL Experience Manager Assets].

>[!NOTE]
>
>Essa integração não oferece suporte a metadados personalizados do [!DNL Adobe Experience Manager].

Para mapear metadados para ativos:

1. Selecionar **[!UICONTROL Ativos]** acima da tabela de metadados.
1. No **[!UICONTROL [!DNL Workfront]campo]** escolha um campo Workfront incorporado ou personalizado.

   >[!NOTE]
   >
   >Você pode mapear um único [!DNL Workfront] campo para vários [!UICONTROL Experience Manager Assets] campos. Não é possível mapear vários [!DNL Workfront] campos para um único [!DNL Experience Manager Assets] campo.

1. No [!DNL Experience Manager Assets] , pesquise pelas categorias pré-preenchidas ou insira pelo menos duas letras no campo de pesquisa para acessar categorias adicionais.
1. Repita as etapas 2 e 3 conforme necessário.
   ![campos de metadados](assets/asset-metadata.png)
1. Clique em [!UICONTROL Salvar] ou vá para a [Pastas](#folders) neste artigo.

### Pastas

Quando os usuários criam uma pasta vinculada em um projeto, os dados associados do projeto, do portfólio e do programa são mapeados para os campos de metadados da pasta em [!DNL Experience Manager Assets].

>[!NOTE]
>
>Essa integração não oferece suporte a metadados personalizados do [!DNL Adobe Experience Manager].

Para mapear metadados para pastas:

1. Selecionar **[!UICONTROL Pastas]** acima da tabela de metadados.
1. No **[!UICONTROL [!DNL Workfront]campo]** escolha um campo Workfront incorporado ou personalizado.

   >[!NOTE]
   >
   >Você pode mapear um único campo do Workfront para vários campos do Experience Manager Assets. Não é possível mapear vários [!DNL Workfront] campos para um único [!DNL Experience Manager Assets] campo.

1. No **[!DNL Experience Manager Assets]** , pesquise pelas categorias pré-preenchidas ou insira pelo menos duas letras no campo de pesquisa para acessar categorias adicionais.
1. Repita as etapas 2 e 3 conforme necessário.
   ![metadados da pasta](assets/folder-metadata.png)
1. Clique em **[!UICONTROL Salvar]** ou vá para a [Sincronização de metadados do projeto](#project-metadata-sync) neste artigo.


### Sincronização de metadados do objeto

Um [!DNL Experience Manager] campos mapeados para [!DNL Workfront] os campos portfólio, programa, projeto, tarefa, emissão e documento são atualizados automaticamente quando o campo é alterado em [!DNL Workfront].

>[!IMPORTANT]
>
>Os usuários devem ter acesso de gravação em [!DNL Experience Manager] para ativos que vivem no objeto para que os metadados sejam sincronizados quando atualizados.

1. Ative o **[!UICONTROL Sincronizar metadados do objeto]** campo.
1. Clique em Salvar ou vá para a página [Configurar pastas vinculadas (Opcional)](#set-up-linked-folders-optional) neste artigo.

## Configurar pastas vinculadas (Opcional)

Você pode permitir que os usuários criem pastas vinculadas a [!DNL Experience Manager] em um [!DNL Workfront] projeto. Quando uma pasta é vinculada, qualquer ativo adicionado à pasta é exibido automaticamente em [!DNL Workfront] e [!DNL Experience Manager]. Quando um ativo é adicionado à pasta vinculada em [!DNL Workfront] pela primeira vez, os metadados do ativo são enviados para [!DNL Experience Manager Assets].

Nas etapas abaixo, você indica onde deseja que as pastas vinculadas sejam criadas. Cada integração pode ter somente um local para todas as pastas vinculadas.

Para configurar pastas vinculadas:

1. Ative o **[!UICONTROL Habilitar pasta Vinculada]** em.
1. Escolha um caminho de pasta para indicar onde deseja que todas as pastas vinculadas sejam associadas a essa integração.

   >[!NOTE]
   >
   >Os usuários precisam ter acesso de gravação em [!DNL Adobe Experience Manager Assets] à pasta especificada para criar uma pasta vinculada.

1. Clique em **[!UICONTROL Salvar]**.
