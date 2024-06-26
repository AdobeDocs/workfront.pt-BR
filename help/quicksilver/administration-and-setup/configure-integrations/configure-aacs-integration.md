---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Configure o [!UICONTROL Experience Manager Assets as a Cloud Service] integração
description: Você pode conectar seu trabalho ao seu conteúdo no [!DNL Experience Manager Assets].
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '1678'
ht-degree: 0%

---

# Configure o [!UICONTROL Experience Manager Assets as a Cloud Service] integração

<!-- Audited: 1/2024 -->


>[!IMPORTANT]
>
>Essa funcionalidade está disponível somente para organizações que foram integradas à [!DNL Adobe Admin Console].

Você pode conectar seu trabalho ao seu conteúdo no [!DNL Experience Manager Assets]&#x200B;:

* Enviar ativos e metadados do [!DNL Adobe Workfront] para [!DNL Experience Manager Assets]&#x200B;
* Vincular ativos de [!DNL Experience Manager Assets] aos seus projetos e tarefas no [!DNL Workfront&#x200B;]
* Facilitar casos de uso de controle de versão
* Criar pastas vinculadas a [!DNL Experience Manager Assets]
* Rastrear metadados de ativos e pastas
* Sincronizar metadados de projeto entre [!DNL Workfront] e [!DNL Experience Manager Assets]

>[!NOTE]
>
>Também é possível conectar vários [!DNL Experience Manager Assets] repositórios para um [!UICONTROL Workfront] ambiente ou várias [!DNL Workfront] ambientes para um [!DNL Experience Manager Assets] repositório em IDs de organização. Siga as instruções de configuração neste artigo para cada integração que você deseja configurar.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plano</strong>
   </td>
   <td>Qualquer
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenças</strong>
   </td>
   <td>Atual: [!UICONTROL Plano] <br>
   Novo: [!UICONTROL Padrão]
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
   <td>Você deve ter [!DNL Experience Manager Assets as a Cloud Service]e você deve ser adicionado ao produto como usuário.
   </td>
  </tr>
  <tr>
   <td>Configurações de nível de acesso*
   </td>
   <td>Você deve ser um [!DNL Workfront] administrador.
   </td>
  </tr>
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Pré-requisitos

Antes de começar,

* Você deve ter [!DNL Workfront] e [!DNL Adobe Experience Manager Assets] associado a uma ID da organização na [!DNL Adobe Admin Console]. Para obter mais informações, consulte [Diferenças de administração baseadas em plataforma ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


## Configurar as informações de integração

{{step-1-to-setup}}

1. Selecionar **[!UICONTROL Documentos]** no painel esquerdo, selecione **[!UICONTROL [!DNL Experience Manager]Integração]**.

   >[!NOTE]
   >
   >Essa área de configuração será exibida somente se o [!DNL Workfront] O ambiente está incluído em um [!DNL Adobe Admin Console].

1. Selecionar **[!UICONTROL Adicionar [!DNL Experience Manager] Integração]**.
1. No **[!UICONTROL Nome]** digite o nome que você deseja que os usuários vejam ao interagir com essa integração no Workfront e no Experience Manager Assets.
1. No **[!UICONTROL URL de navegação]** , o sistema preenche automaticamente o URL de navegação. Esse URL somente leitura é usado para vincular à conta do [!DNL Experience Manager] instância do [!UICONTROL Menu principal] para acesso rápido.
1. Escolha um repositório na lista **[!UICONTROL [!DNL Experience Manager]Repositório de ativos]** menu suspenso. O sistema preenche automaticamente qualquer [!DNL Experience Manager] repositórios associados à ID da organização à qual o perfil de usuário está atribuído.
   ![escolha o repositório do experience manager](assets/setup-information.png)

1. Clique em **[!UICONTROL Salvar]** ou vá para a página [Configurar metadados (opcional)](#set-up-metadata-optional) neste artigo.

   >[!NOTE]
   >
   >Devido à complexidade da integração, não é possível alterar o repositório depois de salvar a configuração inicial.

## Configurar metadados (opcional)

Você pode mapear [!DNL Workfront] dados do objeto para campos de mídia do ativo no [!DNL Experience Manager] Assets.

>[!IMPORTANT]
>
>Você pode mapear metadados somente em uma direção: de [!DNL Workfront] para [!DNL Experience Manager]. Metadados para documentos vinculados a [!DNL Workfront] de [!DNL Experience Manager] não pode ser transferido para [!DNL Workfront].

### Configurar campos de metadados

Antes de começar a mapear campos de metadados, você deve configurar campos de metadados no Workfront e no Experience Manager Assets.

Para configurar campos de metadados:

1. Configurar um esquema de metadados no [!DNL Experience Manager Assets] conforme explicado em [Configurar o mapeamento de metadados de ativos entre o Adobe [!DNL Workfront] e [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).


1. Configure campos de formulário personalizados no Workfront. [!DNL Workfront] O tem muitos campos personalizados internos que você pode usar. No entanto, você também pode criar seus próprios campos personalizados, conforme explicado em [Criar ou editar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

+++ **Expanda para ver mais informações sobre campos do Workfront e do Experience Manager Assets compatíveis**

**Tags do Experience Manager Assets**

Você pode mapear qualquer campo compatível com o Workfront para uma tag no Experience Manager Assets. Para fazer isso, é necessário garantir que os valores de tag na Experience Manager Assets correspondam à Workfront.

* Os valores dos campos Tags e Workfront devem corresponder exatamente à ortografia e ao formato.
* Os valores de campo do Workfront mapeados para as tags do Experience Manager Assets devem estar todos em minúsculas, mesmo se a tag no Experience Manager Assets parecer ter letras maiúsculas.
* Os valores de campo do Workfront não devem incluir espaços.
* O valor do campo no Workfront também deve incluir a estrutura de pastas da tag do Experience Manager Assets.
* Para mapear vários campos de texto de linha única para tags, insira uma lista separada por vírgulas dos valores de tag no lado Workfront do mapeamento de metadados e `xcm:keywords` no lado do Experience Manager Assets. Cada valor de campo mapeia para uma tag separada. Você pode usar um campo calculado para combinar vários campos do Workfront em um único campo de texto separado por vírgulas.
* Você pode mapear valores de campos suspensos, de botão de opção ou de caixa de seleção inserindo uma lista separada por vírgulas dos valores disponíveis nesse campo.


>[!INFO]
>
>**Exemplo**: para corresponder à tag mostrada na estrutura de pastas aqui, o valor do campo no Workfront seria `landscapes:trees/spruce`. Observe as letras minúsculas no valor do campo Workfront.
>
>Se você quiser que a tag seja o item mais à esquerda da árvore de tags, ela deverá ser seguida por dois pontos. Neste exemplo, para mapear para a tag paisagens, o valor do campo no Workfront seria `landscapes:`.
>
>![Estrutura de pastas no AEM](assets/aem-folder-structure-with-red-boxes.png)


Depois de criar as tags na Experience Manager Assets, elas aparecerão no menu suspenso Tags na seção Metadados. Para vincular um campo a uma tag, selecione `xcm:keywords` na lista suspensa do campo Experience Manager Assets, na área mapeamento de metadados.

Para obter mais informações sobre tags na Experience Manager Assets, incluindo como criar e gerenciar tags, consulte [Administração de tags](https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html).

**Campos de esquema de metadados personalizados do Experience Manager Assets**

Você pode mapear campos Workfront incorporados e personalizados para campos de esquema de metadados personalizados no Experience Manager Assets.

Os campos de metadados personalizados criados no Experience Manager Assets são organizados em sua própria seção na área Configuração de metadados.

![seção de metadados personalizada](assets/custom-metadata.png)

<!-- 
link to documentation about creating schema - waiting on response from Anuj about best article to link to
-->

**Campos do Workfront**

Você pode mapear campos do Workfront incorporados e personalizados para o Experience Manager Assets. Os seguintes valores de campo devem corresponder em letras maiúsculas e minúsculas e à ortografia entre o Workfront e o Experience Manager Assets:

* Campos suspensos
* Campos de seleção múltipla

>[!TIP]
>
> Para verificar se os valores de campo correspondem exatamente, vá para
>
> * Configuração > Forms personalizado no Workfront ou o campo no objeto
> * Ativos > esquemas de metadados no Experience Manager Assets

+++

### Mapear metadados para ativos

Os metadados são mapeados quando um ativo é enviado por push de [!DNL Workfront] pela primeira vez. Documentos com campos incorporados ou personalizados são mapeados automaticamente para os campos especificados na primeira vez que um ativo é enviado para o [!DNL Experience Manager Assets].

Para mapear metadados de ativos:

<!--
1. Select **[!UICONTROL Assets]** above the metadata table.
-->
1. No **[!UICONTROL [!DNL Workfront]campo]** escolha um campo Workfront incorporado ou personalizado.

   >[!NOTE]
   >
   >Você pode mapear um único [!DNL Workfront] campo para vários [!UICONTROL Experience Manager Assets] campos. Não é possível mapear vários [!DNL Workfront] para um único [!DNL Experience Manager Assets] campo.
   ><!--To map a Workfront field to an Experience Manager Assets tag, see -->

1. No [!DNL Experience Manager Assets] , pesquise as categorias pré-preenchidas ou insira pelo menos duas letras no campo de pesquisa para acessar categorias adicionais.
1. Repita as etapas 2 e 3 conforme necessário.
   ![campos de metadados](assets/metadata-no-asset-toggle.png)
1. Clique em [!UICONTROL Salvar] ou vá para a página [Configurar fluxos de trabalho](#set-up-workflows-optional) neste artigo.

<!--

### Map metadata for folders

When users create a linked folder on a project, the associated project, portfolio, and program data is mapped to folder metadata fields in [!DNL Experience Manager Assets].

>[!NOTE]
>
>This integration does not support custom metadata from [!DNL Adobe Experience Manager].

To map metadata for folders: 

1. Select **[!UICONTROL Folders]** above the metadata table.
1. In the **[!UICONTROL [!DNL Workfront] field]** column, choose a built-in or custom Workfront field.

    >[!NOTE]
    >
    >You can map a single Workfront field to multiple Experience Manager Assets fields. You can't map multiple [!DNL Workfront] fields to a single [!DNL Experience Manager Assets] field.

1. In the **[!DNL Experience Manager Assets]** field, search through the pre-populated categories or enter at least two letters in the search field to access additional categories.
1. Repeat steps 2 and 3 as needed.
![folder metadata](assets/folder-metadata.png)
1. Click **[!UICONTROL Save]** or move on to the [Project metadata sync](#project-metadata-sync) section in this article.


### Object metadata sync

An [!DNL Experience Manager] fields that is mapped to [!DNL Workfront] portfolio, program, project, task, issue, and document fields update automatically when the field is changed in [!DNL Workfront].

When this option is enabled, any asset that has been pushed to Adobe Experience manager includes a card on the Document Details page that displays a real-time view of the document's Adobe Experience Manager metadata.

>[!IMPORTANT]
>
>Users must have write access in [!DNL Experience Manager] for assets living in the object in order for the metadata to sync when it's updated.

1. Enable the **[!UICONTROL Sync object metadata]** field.
1. Click **Save** or move on to the [Set up workflows (Optional)](#set-up-workflows-optional) section in this article.-->

## Configurar fluxos de trabalho (opcional)

Um fluxo de trabalho é um conjunto de ações que conectam o Workfront ao Adobe Experience Manager as a Cloud Service. Como administrador do Workfront, você pode configurar fluxos de trabalho no Workfront e atribuí-los a Modelos de projeto. Quando um Projeto é criado usando um Modelo de projeto ao qual um fluxo de trabalho é atribuído, as ações definidas no fluxo de trabalho são acionadas.

Os fluxos de trabalho são ativados e configurados para a Adobe Experience Manager como um todo. Esses fluxos de trabalho podem ser aplicados a modelos de projeto e ajustados ou personalizados no nível do modelo ou do projeto.

Os seguintes fluxos de trabalho estão disponíveis na integração do Adobe Experience Manager:

* [Criar pastas vinculadas do Adobe Experience Manager](#create-adobe-experience-manager-linked-folders)
* [Publicar ativos enviados para o Adobe Experience Manager Assets](#publish-assets-that-are-sent-to-adobe-experience-manager-assets)

### Criar pastas vinculadas do Adobe Experience Manager

1. Alterne a **[!UICONTROL Criar Pasta vinculada]** em.
1. Insira um nome para a pasta vinculada que você está criando.
1. (Condicional) Ative a variável **Árvore de pastas padrão** opção se desejar que essa pasta vinculada seja a pasta padrão para projetos criados com modelos que usam essa integração. É possível selecionar uma ou mais pastas padrão.
1. Escolha um caminho de pasta para indicar onde deseja que todas as pastas vinculadas sejam associadas a essa integração.
1. (Condicional) Para adicionar uma árvore de pastas (pastas aninhadas) a essa integração, faça o seguinte:

   1. Clique em **Adicionar pasta** ícone ![Adicionar pasta](assets/add-folder-aem.png).
   1. No **Tipo de nome** selecione como deseja nomear a pasta:

      * **Nome**: digite um nome para a pasta.
      * **Dados do objeto**: selecione a origem do nome da pasta, como Nome do projeto.

      >[!NOTE]
      >
      >* Os nomes de pasta devem ter menos de 100 caracteres.
      >* Os seguintes caracteres serão removidos dos nomes das pastas:
      >
      >   `/`, `:`, `[`, `]`, `|`, `*`

   1. Para adicionar uma pasta aninhada à árvore de pastas, clique no menu de três pontos ao lado da pasta na qual deseja criar uma pasta aninhada e selecione **Adicionar pasta**. Preencha os campos conforme descrito em Etapa da etapa anterior.
   1. Para vincular uma pasta ao Workfront, selecione a pasta e clique no link **Criar pasta vinculada**   ícone ![Vincular pasta](assets/link-folder.png).
   1. (Opcional) Para editar uma pasta, selecione-a e clique no **Editar pasta** ícone ![Ícone Editar](assets/edit-icon.png).
   1. (Opcional) Para excluir uma pasta, selecione-a e clique no **Excluir pasta** ícone ![Excluir pasta](assets/delete-folder.png).
1. (Condicional) Para adicionar outra árvore de pastas, clique em **+ Adicionar árvore de pastas** e siga as etapas da Etapa 5.

1. Clique em **[!UICONTROL Salvar]**, ou passe para a [Publicar ativos enviados para o Adobe Experience Manager Assets](#publish-assets-that-are-sent-to-adobe-experience-manager-assets) neste artigo.

>[!NOTE]
>
>* Essa integração criará no máximo 100 pastas, independentemente de quantas árvores de pastas forem criadas. Por exemplo, uma integração com quatro árvores de pastas pode criar até 100 pastas, não 400 pastas.
>* A primeira pasta na árvore de pastas é marcada automaticamente como vinculada ao Workfront. Se não quiser que essa pasta seja vinculada, desvincule-a.
>* Se nenhuma árvore de pastas for fornecida, a pasta raiz se tornará a pasta vinculada.


### Publicar ativos enviados para o Adobe Experience Manager Assets

1. Ativar/desativar **[!UICONTROL Publicar ativos automaticamente]**.
1. Marque a caixa ao lado do local em que deseja publicar ativos enviados para o Adobe Experience Manager Assets. Você pode ativar uma ou ambas as opções.
1. (Condicional) Se você ativou a opção Brand Portal, selecione a Brand Portal na qual deseja publicar ativos.
1. Clique em **[!UICONTROL Salvar]** ou vá para a página [Configurar pastas vinculadas (opcional)](#set-up-linked-folders-optional) neste artigo.

## Configurar pastas vinculadas (opcional)

Você pode permitir que os usuários criem pastas vinculadas a [!DNL Experience Manager] enquanto em um [!DNL Workfront] projeto. Quando uma pasta é vinculada, qualquer ativo adicionado à pasta é exibido automaticamente em ambos [!DNL Workfront] e [!DNL Experience Manager]. Quando um ativo é adicionado à pasta vinculada no [!DNL Workfront] pela primeira vez, os metadados do ativo são enviados para [!DNL Experience Manager Assets].

Nas etapas abaixo, você indica onde deseja criar as pastas vinculadas. Cada integração pode ter apenas um local para todas as pastas vinculadas.

Para configurar pastas vinculadas:

1. Alterne a **[!UICONTROL Habilitar Pasta vinculada]** em.
1. Escolha um caminho de pasta para indicar onde deseja que todas as pastas vinculadas sejam associadas a essa integração.

   >[!NOTE]
   >
   >Os usuários precisam de acesso de gravação no [!DNL Adobe Experience Manager Assets] à pasta especificada para criar uma pasta vinculada.

1. Clique em **[!UICONTROL Salvar]**.
