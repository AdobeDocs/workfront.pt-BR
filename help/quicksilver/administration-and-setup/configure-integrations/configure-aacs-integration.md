---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Configurar a Integração do [!UICONTROL Experience Manager Assets as a Cloud Service]
description: Você pode conectar seu trabalho ao seu conteúdo no [!DNL Experience Manager Assets].
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '1697'
ht-degree: 0%

---

# Configurar a integração do [!UICONTROL Experience Manager Assets as a Cloud Service]

<!-- Audited: 1/2024 -->


>[!IMPORTANT]
>
>Essa funcionalidade está disponível somente para organizações que foram integradas ao [!DNL Adobe Admin Console].

Você pode conectar seu trabalho ao seu conteúdo no [!DNL Experience Manager Assets]&#x200B;:

* Enviar ativos e metadados de [!DNL Adobe Workfront] para [!DNL Experience Manager Assets]&#x200B;
* Vincular ativos do [!DNL Experience Manager Assets] aos seus projetos e tarefas no [!DNL Workfront&#x200B;]
* Facilitar casos de uso de controle de versão
* Criar pastas vinculadas a [!DNL Experience Manager Assets]
* Rastrear metadados de ativos e pastas
* Sincronizar metadados de projeto entre [!DNL Workfront] e [!DNL Experience Manager Assets]

>[!NOTE]
>
>Você também pode conectar vários repositórios [!DNL Experience Manager Assets] a um ambiente [!UICONTROL Workfront], ou vários ambientes [!DNL Workfront] a um repositório [!DNL Experience Manager Assets] em IDs de organização. Siga as instruções de configuração neste artigo para cada integração que você deseja configurar.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table>
  <tr>
   <td>[!DNL Adobe Workfront] plano
   </td>
   <td>Qualquer
   </td>
  </tr>
  <tr>
   <td>[!DNL Adobe Workfront] licença
   </td>
   <td><p>Atual: [!UICONTROL Plano]</p>
   <p>Novo: [!UICONTROL Padrão]</p></td>
  </tr>
  <tr>
   <td>[!DNL Experience Manager] licença
   </td>
   <td>[!UICONTROL Padrão]
   </td>
  </tr>
  <tr>
   <td>Produto
   </td>
   <td>Você deve ter [!DNL Experience Manager Assets as a Cloud Service] e ser adicionado ao produto como um usuário.
   </td>
  </tr>
  <tr>
   <td>Configurações de nível de acesso
   </td>
   <td>Você deve ser um administrador [!DNL Workfront].
   </td>
  </tr>
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Antes de começar,

* Você deve ter [!DNL Workfront] e [!DNL Adobe Experience Manager Assets] associados a uma ID de organização na [!DNL Adobe Admin Console]. Para obter mais informações, consulte [Diferenças de administração baseadas em plataforma ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


## Configurar as informações de integração

{{step-1-to-setup}}

1. Selecione **[!UICONTROL Documentos]** no painel esquerdo e **[!UICONTROL [!DNL Experience Manager]Integração]**.

   >[!NOTE]
   >
   >Esta área de configuração aparece somente se o ambiente [!DNL Workfront] estiver incluído em um [!DNL Adobe Admin Console].

1. Selecione **[!UICONTROL Adicionar [!DNL Experience Manager] Integração]**.
1. No campo **[!UICONTROL Nome]**, digite o nome que você deseja que os usuários vejam ao interagir com essa integração no Workfront e no Experience Manager Assets.
1. No campo **[!UICONTROL URL de Navegação]**, o sistema preenche automaticamente a URL de Navegação. Esta URL somente leitura é usada para vincular à instância [!DNL Experience Manager] da sua organização a partir do [!UICONTROL Menu Principal] para acesso rápido.
1. Escolha um repositório no menu suspenso **[!UICONTROL [!DNL Experience Manager]repositório Assets]**. O sistema preenche automaticamente todos os repositórios do [!DNL Experience Manager] associados à ID da organização à qual o perfil de usuário está atribuído.
   ![escolher repositório do experience manager](assets/setup-information.png)

1. Clique em **[!UICONTROL Salvar]** ou vá para a seção [Configurar metadados (Opcional)](#set-up-metadata-optional) deste artigo.

   >[!NOTE]
   >
   >Devido à complexidade da integração, não é possível alterar o repositório depois de salvar a configuração inicial.

## Configurar metadados (opcional)

Você pode mapear dados de objeto [!DNL Workfront] para campos de mídia de ativos no Assets [!DNL Experience Manager].

>[!IMPORTANT]
>
>Você pode mapear metadados somente em uma direção: de [!DNL Workfront] a [!DNL Experience Manager]. Os metadados de documentos vinculados a [!DNL Workfront] de [!DNL Experience Manager] não podem ser transferidos para [!DNL Workfront].

### Configurar campos de metadados

Antes de começar a mapear campos de metadados, você deve configurar campos de metadados no Workfront e no Experience Manager Assets.

Para configurar campos de metadados:

1. Configure um esquema de metadados em [!DNL Experience Manager Assets] conforme explicado em [Configure o mapeamento de metadados de ativos entre Adobe [!DNL Workfront] e [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).


1. Configure campos de formulário personalizados no Workfront. [!DNL Workfront] tem muitos campos personalizados internos que você pode usar. No entanto, você também pode criar seus próprios campos personalizados, conforme explicado em [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

+++ **Expanda para ver mais informações sobre campos do Workfront e do Experience Manager Assets compatíveis**

**Marcas do Experience Manager Assets**

Você pode mapear qualquer campo compatível com o Workfront para uma tag no Experience Manager Assets. Para fazer isso, é necessário garantir que os valores de tag na Experience Manager Assets correspondam à Workfront.

* Os valores dos campos Tags e Workfront devem corresponder exatamente à ortografia e ao formato.
* Os valores de campo do Workfront mapeados para as tags do Experience Manager Assets devem estar todos em minúsculas, mesmo se a tag no Experience Manager Assets parecer ter letras maiúsculas.
* Os valores de campo do Workfront não devem incluir espaços.
* O valor do campo no Workfront também deve incluir a estrutura de pastas da tag do Experience Manager Assets.
* Para mapear vários campos de texto de linha única para marcas de formatação, insira uma lista separada por vírgulas dos valores de marca no lado Workfront do mapeamento de metadados e `xcm:keywords` no lado Experience Manager Assets. Cada valor de campo mapeia para uma tag separada. Você pode usar um campo calculado para combinar vários campos do Workfront em um único campo de texto separado por vírgulas.
* Você pode mapear valores de campos suspensos, de botão de opção ou de caixa de seleção inserindo uma lista separada por vírgulas dos valores disponíveis nesse campo.


>[!INFO]
>
>**Exemplo**: para corresponder à marca mostrada na estrutura de pastas aqui, o valor do campo no Workfront seria `landscapes:trees/spruce`. Observe as letras minúsculas no valor do campo Workfront.
>
>Se você quiser que a tag seja o item mais à esquerda da árvore de tags, ela deverá ser seguida por dois pontos. Neste exemplo, para mapear para a tag de paisagens, o valor do campo no Workfront seria `landscapes:`.
>
>![Estrutura de pasta no AEM](assets/aem-folder-structure-with-red-boxes.png)


Depois de criar as tags na Experience Manager Assets, elas aparecerão no menu suspenso Tags na seção Metadados. Para vincular um campo a uma marca, selecione `xcm:keywords` na lista suspensa de campos do Experience Manager Assets na área de mapeamento de metadados.

Para obter mais informações sobre tags na Experience Manager Assets, incluindo como criar e gerenciar tags, consulte [Administração de Tags](https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html).

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
> * Assets > esquemas de metadados no Experience Manager Assets

+++

### Mapear metadados para ativos

Os metadados são mapeados quando um ativo é enviado por push de [!DNL Workfront] pela primeira vez. Documentos com campos personalizados ou internos são mapeados automaticamente para os campos especificados na primeira vez que um ativo é enviado para [!DNL Experience Manager Assets].

Para mapear metadados de ativos:

<!--
1. Select **[!UICONTROL Assets]** above the metadata table.
-->
1. Na coluna **[!UICONTROL [!DNL Workfront]campo]**, escolha um campo interno ou personalizado do Workfront.

   >[!NOTE]
   >
   >Você pode mapear um único campo [!DNL Workfront] para vários campos [!UICONTROL Experience Manager Assets]. Não é possível mapear vários campos [!DNL Workfront] para um único campo [!DNL Experience Manager Assets].
   ><!--To map a Workfront field to an Experience Manager Assets tag, see -->

1. No campo [!DNL Experience Manager Assets], pesquise pelas categorias pré-preenchidas ou insira pelo menos duas letras no campo de pesquisa para acessar categorias adicionais.
1. Repita as etapas 2 e 3 conforme necessário.
   ![campos de metadados](assets/metadata-no-asset-toggle.png)
1. Clique em [!UICONTROL Salvar] ou vá para a seção [Configurar fluxos de trabalho](#set-up-workflows-optional) neste artigo.

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

Um fluxo de trabalho é um conjunto de ações que conectam o Workfront ao Adobe Experience Manager as a Cloud Service. Como administrador do Workfront, você pode configurar fluxos de trabalho no Workfront e atribuí-los a Modelos de projeto.

Quando um Projeto é criado usando um Modelo de projeto ao qual um fluxo de trabalho é atribuído, as ações definidas no fluxo de trabalho são acionadas.

Os fluxos de trabalho são ativados e configurados para a Adobe Experience Manager como um todo. Esses fluxos de trabalho podem ser aplicados a modelos de projeto. Elas podem ser ajustadas ou personalizadas no nível do modelo ou no nível do projeto quando um projeto é criado a partir desse modelo.

Os seguintes fluxos de trabalho estão disponíveis na integração do Adobe Experience Manager:

* [Criar pastas vinculadas do Adobe Experience Manager](#create-adobe-experience-manager-linked-folders)
* [Ativos do Publish enviados para o Adobe Experience Manager Assets](#publish-assets-that-are-sent-to-adobe-experience-manager-assets)

### Criar pastas vinculadas do Adobe Experience Manager

1. Ative a **[!UICONTROL Criar pasta vinculada]**.
1. Insira um nome para a pasta vinculada que você está criando.
1. (Condicional) Ative a opção **Árvore de pastas padrão** se desejar que essa pasta vinculada seja a pasta padrão para projetos criados com modelos que usam essa integração. É possível selecionar uma ou mais pastas padrão.
1. Escolha um caminho de pasta para indicar onde deseja que todas as pastas vinculadas sejam associadas a essa integração.
1. (Condicional) Para adicionar uma árvore de pastas (pastas aninhadas) a essa integração, faça o seguinte:

   1. Clique no ícone **Adicionar pasta** ![Adicionar pasta](assets/add-folder-aem.png).
   1. No campo **Tipo de nome**, selecione como deseja nomear a pasta:

      * **Nome**: digite um nome para a pasta.
      * **Dados do objeto**: selecione a origem do nome da pasta, como Nome do projeto.

      >[!NOTE]
      >
      >* Os nomes de pasta devem ter menos de 100 caracteres.
      >* Os seguintes caracteres serão removidos dos nomes das pastas:
      >
      >   `/`, `:`, `[`, `]`, `|`, `*`

   1. Para adicionar uma pasta aninhada à árvore de pastas, clique no menu de três pontos ao lado da pasta na qual deseja criar uma pasta aninhada e selecione **Adicionar pasta**. Preencha os campos conforme descrito em Etapa da etapa anterior.
   1. Para vincular uma pasta à Workfront, selecione a pasta e clique em **Criar pasta vinculada**   ícone ![Vincular pasta](assets/link-folder.png).
   1. (Opcional) Para editar uma pasta, selecione-a e clique no **ícone Editar Pasta** ![ícone Editar](assets/edit-icon.png).
   1. (Opcional) Para excluir uma pasta, selecione-a e clique no ícone **Excluir Pasta** ![Excluir pasta](assets/delete-folder.png).
1. (Condicional) Para adicionar outra árvore de pastas, clique em **+ Adicionar árvore de pastas** e siga as etapas da Etapa 5.

1. Clique em **[!UICONTROL Salvar]** ou vá para a seção [Ativos do Publish enviados para o Adobe Experience Manager Assets](#publish-assets-that-are-sent-to-adobe-experience-manager-assets) neste artigo.

>[!NOTE]
>
>* Essa integração criará no máximo 100 pastas, independentemente de quantas árvores de pastas forem criadas. Por exemplo, uma integração com quatro árvores de pastas pode criar até 100 pastas, não 400 pastas.
>* A primeira pasta na árvore de pastas é marcada automaticamente como vinculada ao Workfront. Se não quiser que essa pasta seja vinculada, desvincule-a.
>* Se nenhuma árvore de pastas for fornecida, a pasta raiz se tornará a pasta vinculada.


### Ativos do Publish enviados para o Adobe Experience Manager Assets

1. Ative **[!UICONTROL ativos do Publish automaticamente]**.
1. Marque a caixa ao lado do local em que deseja publicar ativos enviados para o Adobe Experience Manager Assets. Você pode ativar uma ou ambas as opções.
1. (Condicional) Se você ativou a opção Brand Portal, selecione a Brand Portal na qual deseja publicar ativos.
1. Clique em **[!UICONTROL Salvar]** ou vá para a seção [Configurar pastas vinculadas (Opcional)](#set-up-linked-folders-optional) neste artigo.

## Configurar pastas vinculadas (opcional)

Você pode permitir que os usuários criem pastas vinculadas a [!DNL Experience Manager] enquanto estiver em um projeto [!DNL Workfront]. Quando uma pasta é vinculada, qualquer ativo adicionado à pasta é exibido automaticamente no [!DNL Workfront] e no [!DNL Experience Manager]. Quando um ativo é adicionado à pasta vinculada no [!DNL Workfront] pela primeira vez, os metadados do ativo são enviados para [!DNL Experience Manager Assets].

Nas etapas abaixo, você indica onde deseja criar as pastas vinculadas. Cada integração pode ter apenas um local para todas as pastas vinculadas.

Para configurar pastas vinculadas:

1. Ative a **[!UICONTROL Habilitar Pasta vinculada]**.
1. Escolha um caminho de pasta para indicar onde deseja que todas as pastas vinculadas sejam associadas a essa integração.

   >[!NOTE]
   >
   >Os usuários precisam de acesso de gravação em [!DNL Adobe Experience Manager Assets] à pasta especificada para criar uma pasta vinculada.

1. Clique em **[!UICONTROL Salvar]**.
