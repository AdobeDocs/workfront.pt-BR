---
product-area: documents
navigation-topic: approvals
title: Usar o Adobe Experience Manager com a integração do Frame.io
description: Usar o Adobe Experience Manager com a integração do Frame.io
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
source-git-commit: cb2a17991a5562c6e734eaa0ada781d706dc5a77
workflow-type: tm+mt
source-wordcount: '1614'
ht-degree: 0%

---


# Usar o Adobe Experience Manager com a integração do Frame.io

Você pode usar o [!DNL Experience Manager Assets]&#x200B;&#x200B; para gerenciar e armazenar seus ativos digitais que passaram pelo ciclo de revisão e aprovação. Essa integração permite aproveitar os recursos do Adobe Experience Manager, Frame.io e Workfront para simplificar seus processos de colaboração e gerenciamento de conteúdo.

## Configurar a integração do Experience Manager Assets

Você pode conectar seu trabalho ao seu conteúdo no [!DNL Experience Manager Assets]&#x200B;:

* Enviar ativos e metadados de [!DNL Adobe Workfront] para [!DNL Experience Manager Assets]&#x200B;
* Facilitar casos de uso de controle de versão
* Rastrear metadados para ativos
* Sincronizar metadados de projeto entre [!DNL Workfront] e [!DNL Experience Manager Assets]

>[!NOTE]
>
>Você também pode conectar vários repositórios [!DNL Experience Manager Assets] a um ambiente [!UICONTROL Workfront], ou vários ambientes [!DNL Workfront] a um repositório [!DNL Experience Manager Assets] em IDs de organização. Siga as instruções de configuração neste artigo para cada integração que você deseja configurar.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table>
  <tr>
   <td>Pacote do Adobe Workfront
   </td>
   <td> <p>Prime ou Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr>
    <tr>
   <td>Licenças do Adobe Workfront
   </td>
   <td>
  <p>Para configurar a integração:</p>
   <p>Standard</p>
   <p>Plano</p>

<p>Para enviar documentos ao Experience Manager Assets:</p>
   <p>Colaborador ou superior</p>
   <p>Solicitação ou superior</p>
   </td>
  </tr>
  </tr>
    <tr>
   <td>Licenças do Adobe Experience Manager
   </td>
   <td>Standard
   </td>
  </tr>
  <tr>
   <td>Produtos adicionais
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
* Sua instância do Workfront deve estar usando o Adobe Enterprise Storage.


## Configurar as informações de integração

{{step-1-to-setup}}

1. Selecione **[!UICONTROL Documentos]** no painel esquerdo e **[!UICONTROL [!DNL Experience Manager]Integração]**.
1. Selecione **[!UICONTROL Adicionar [!DNL Experience Manager] Integração]**.
1. No campo **[!UICONTROL Nome]**, digite o nome que você deseja que os usuários vejam ao interagir com essa integração no Workfront e no Experience Manager Assets.
1. No campo **[!UICONTROL URL de Navegação]**, o sistema preenche automaticamente a URL de Navegação. Esta URL somente leitura é usada para vincular à instância [!DNL Experience Manager] da sua organização a partir do [!UICONTROL Menu Principal] para acesso rápido.
1. Escolha um repositório no menu suspenso **[!UICONTROL [!DNL Experience Manager]repositório Assets]**. O sistema preenche automaticamente todos os repositórios do [!DNL Experience Manager] associados à ID da organização à qual o perfil de usuário está atribuído.
   ![escolher repositório do experience manager](assets/setup-information.png)

1. Clique em **[!UICONTROL Salvar]** ou vá para a seção [Configurar metadados (Opcional)](#set-up-metadata-optional) deste artigo.

   >[!IMPORTANT]
   >
   >Devido à complexidade da integração, não é possível alterar o repositório depois de salvar a configuração inicial.


## Configurar metadados (opcional)

Você pode mapear dados de objeto [!DNL Workfront] para campos de mídia de ativos no Assets [!DNL Experience Manager].

>[!NOTE]
>
>Você pode mapear metadados somente em uma direção: de [!DNL Workfront] a [!DNL Experience Manager]. Os metadados de documentos vinculados a [!DNL Workfront] de [!DNL Experience Manager] não podem ser transferidos para [!DNL Workfront].

### Configurar campos de metadados

Antes de começar a mapear campos de metadados, você deve configurar campos de metadados no Workfront e no Experience Manager Assets.

Para configurar campos de metadados:

1. Configure um esquema de metadados em [!DNL Experience Manager Assets] conforme explicado em [Configurar o mapeamento de metadados de ativos entre o Adobe [!DNL Workfront] e [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping).


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
>![Estrutura de pastas no AEM](assets/aem-folder-structure-with-red-boxes.png)


Depois de criar as tags na Experience Manager Assets, elas aparecerão no menu suspenso Tags na seção Metadados. Para vincular um campo a uma marca, selecione `xcm:keywords` na lista suspensa de campos do Experience Manager Assets na área de mapeamento de metadados.

Para obter mais informações sobre tags na Experience Manager Assets, incluindo como criar e gerenciar tags, consulte [Administração de Tags](https://experienceleague.adobe.com/pt-br/docs/experience-manager-64/administering/contentmanagement/tags).

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
1. Clique em [!UICONTROL **Salvar**] ou mova para a seção [Sincronização de metadados de objeto](#object-metadata-sync) neste artigo.



### Sincronização de metadados de objeto

Um [!DNL Experience Manager] campos mapeados para [!DNL Workfront] campos de portfólio, programa, projeto, tarefa, problema e documento são atualizados automaticamente quando o campo é alterado em [!DNL Workfront].

Quando essa opção está ativada, qualquer ativo enviado para o Adobe Experience Manager exibe uma visualização em tempo real dos metadados do Adobe Experience Manager do documento na página Detalhes do documento no Workfront.

1. Habilite o campo **[!UICONTROL Sincronizar metadados do objeto]** e clique em **Salvar**.

>[!IMPORTANT]
>
>Os usuários devem ter acesso de gravação em [!DNL Experience Manager] para ativos que vivem no objeto para que os metadados sejam sincronizados quando forem atualizados.


## Enviar um documento para o Experience Manager Assets ou o Assets Essentials

Você pode enviar documentos do Workfront para o Experience Manager Assets ou o Assets Essentials. Os documentos carregados e enviados do Workfront para o Assets Essentials ainda contam para o armazenamento geral de documentos.

O Assets enviado para o Experience Manager por meio dessa integração tem um limite de tamanho de **5 GB**.

<!--In the Preview environment, Assets sent to Experience Manager through this integration have a size limit of **30 GB**.-->

Os campos de metadados são mapeados pela primeira vez quando você envia um ativo do Workfront para o Experience Manager Assets ou o Assets Essentials. Todos os metadados configurados para mapear para objetos principais também são enviados. Para obter mais informações sobre como configurar o mapeamento de metadados, consulte [Configurar a integração do Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configurar a integração do Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**Exemplo** Quando você envia pela primeira vez um ativo anexado a um projeto, os metadados são mapeados para o Experience Manager Assets ou para o Assets Essentials, bem como quaisquer metadados mapeados de objetos principais, como um portfólio e programa.



### Enviar um documento do Workfront

Quando um usuário envia um documento do Workfront para o Experience Manager Assets ou o Assets Essentials, os metadados mapeados são transferidos ao longo do documento. Depois que o documento é enviado, as alterações feitas nos metadados do documento no Workfront não são refletidas no Assets ou no Assets Essentials. Se um campo mapeado no Workfront for alterado, você deverá enviar uma nova versão do documento com os metadados atualizados para o Assets ou o Assets Essentials.

Para enviar um documento:

1. Vá para a área **Documentos** do Workfront e selecione o documento que deseja enviar.
1. Clique em **Enviar para** e escolha a integração do Experience Manager configurada pelo administrador.

   >[!NOTE]
   >
   >O administrador do Workfront pode escolher qualquer nome para essa integração, portanto, talvez ele não mencione especificamente o Assets ou o Assets Essentials.

   ![Enviar para](assets/send-to-aem.png)

1. Escolha para onde deseja que o ativo vá e clique em **Selecionar pasta**.
1. Ao encontrar o destino desejado, clique em **Salvar**.

### Enviar uma nova versão

É possível adicionar uma nova versão a um documento carregado anteriormente no Workfront. Para obter mais informações, consulte [Carregar uma nova versão de um documento](/help/quicksilver/documents/managing-documents/upload-new-document-version.md). Depois que a versão mais recente for carregada, você poderá enviá-la para o Assets Essentials. Se um campo mapeado no Workfront tiver sido alterado, a nova versão atualizará os metadados no Assets Essentials quando enviada.

>[!IMPORTANT]
>
>Antes de fazer upload de uma nova versão para o Workfront, recomendamos renomear o arquivo. Se você fizer upload de uma nova versão com exatamente o mesmo nome de arquivo de uma versão anterior, somente a versão mais recente poderá ser baixada do Workfront. Todas as versões podem ser baixadas do Experience Manager Assets ou do Assets Essentials, independentemente do nome do arquivo. <!--Is this still a thing with ESM?-->

Para enviar a versão mais recente:

1. Vá para a área **Documentos** no Workfront e localize o documento.
1. Selecione **Enviar para** e escolha a integração do Experience Manager configurada pelo administrador.

   >[!NOTE]
   >
   >O administrador do Workfront pode escolher qualquer nome para essa integração, portanto, pode não mencionar especificamente o Assets ou o Assets Essentials.

   ![Enviar para](assets/send-to-aem.png)

1. Clique em **Salvar**. A nova versão é salva no mesmo local da versão anterior.
