---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Enviar um documento para o Experience Manager Assets ou o Assets Essentials
description: Você pode enviar documentos do Workfront para o Experience Manager Assets ou o Assets Essentials. Os documentos carregados e enviados do Workfront para o Assets Essentials ainda contam para o armazenamento geral de documentos. O Assets vinculado do Assets Essentials não conta para o armazenamento geral.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 7942e77b-9466-4dff-9737-97b17647ac48
source-git-commit: 430751f0e38c6c45145c965398990ee3652f36fe
workflow-type: tm+mt
source-wordcount: '868'
ht-degree: 0%

---

# Enviar um documento para o Experience Manager Assets ou o Assets Essentials

Você pode enviar documentos do Workfront para o Experience Manager Assets ou o Assets Essentials. Os documentos carregados e enviados do Workfront para o Assets Essentials ainda contam para o armazenamento geral de documentos. O Assets vinculado do Assets Essentials não conta para o armazenamento geral.

O Assets enviado para o Experience Manager por meio dessa integração tem um limite de tamanho de **5 GB**.

No ambiente de Pré-visualização, o Assets enviado ao Experience Manager por meio dessa integração tem um limite de tamanho de **30 GB**.

Os campos de metadados são mapeados pela primeira vez quando você envia um ativo do Workfront para o Experience Manager Assets ou o Assets Essentials. Todos os metadados configurados para mapear para objetos principais também são enviados. Para obter mais informações sobre como configurar o mapeamento de metadados, consulte [Configurar a integração do Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configurar a integração do Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**Exemplo** Quando você envia pela primeira vez um ativo anexado a uma tarefa, os metadados da tarefa são mapeados para o Experience Manager Assets ou para o Assets Essentials, bem como quaisquer metadados mapeados de objetos principais, como um projeto, portfólio e programa.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p> Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenças do Adobe Workfront</td> 
   <td> 
   <p>Colaborador ou superior</p> 
   <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produtos adicionais</td> 
   <td>Você deve ter o Experience Manager as a Cloud Service ou o Assets Essentials e deve ser adicionado ao produto como usuário na Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Permissões do Experience Manager</td> 
    <td>Você deve ter acesso de gravação à pasta.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a documentos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir acesso ou superior</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Antes de começar,

* O administrador do Workfront deve configurar uma integração do Experience Manager. Para obter mais informações, consulte [Configurar a integração do Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configurar a integração do Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Enviar um documento do Workfront

Quando um usuário envia um documento do Workfront para o Experience Manager Assets ou o Assets Essentials, os metadados mapeados são transferidos ao longo do documento. Depois que o documento é enviado, as alterações feitas nos metadados do documento no Workfront não são refletidas no Assets ou no Assets Essentials. Se um campo mapeado no Workfront for alterado, você deverá enviar uma nova versão do documento com os metadados atualizados para o Assets ou o Assets Essentials. Para configurar ou editar metadados, consulte [Configurar a integração do Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configurar a integração do Experience Manager Assets Essentials](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

Para enviar um documento:

1. Vá para a área **Documentos** do Workfront e selecione o documento que deseja enviar.
1. Clique em **Enviar para** e escolha a integração do Experience Manager configurada pelo administrador.

   >[!NOTE]
   >
   >O administrador do Workfront pode escolher qualquer nome para essa integração, portanto, talvez ele não mencione especificamente o Assets ou o Assets Essentials.

   ![Enviar para](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Escolha para onde deseja que o ativo vá e clique em **Selecionar pasta**.
1. Ao encontrar o destino desejado, clique em **Salvar**.

## Enviar uma nova versão

É possível adicionar uma nova versão a um documento carregado anteriormente no Workfront. Para obter mais informações, consulte [Carregar uma nova versão de um documento](../../documents/managing-documents/upload-new-document-version.md). Depois que a versão mais recente for carregada, você poderá enviá-la para o Assets Essentials. Se um campo mapeado no Workfront tiver sido alterado, a nova versão atualizará os metadados no Assets Essentials quando enviada.

>[!IMPORTANT]
>
>Antes de fazer upload de uma nova versão para o Workfront, recomendamos renomear o arquivo. Se você fizer upload de uma nova versão com exatamente o mesmo nome de arquivo de uma versão anterior, somente a versão mais recente poderá ser baixada do Workfront. Todas as versões podem ser baixadas do Experience Manager Assets ou do Assets Essentials, independentemente do nome do arquivo.

Para enviar a versão mais recente:

1. Vá para a área **Documentos** no Workfront e localize o documento.
1. Selecione **Enviar para** e escolha a integração do Experience Manager configurada pelo administrador.

   >[!NOTE]
   >
   >O administrador do Workfront pode escolher qualquer nome para essa integração, portanto, pode não mencionar especificamente o Assets ou o Assets Essentials.

   ![Enviar para](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Clique em **Salvar**. A nova versão é salva no mesmo local da versão anterior.

## Mover um documento para uma pasta vinculada no Experience Manager Assets

>[!NOTE]
>
>Essa funcionalidade só está disponível para o Experience Manager Assets as a Cloud Service. Não está disponível para o Experience Manager Assets Essentials.

Você poderá mover um documento para uma pasta vinculada no Experience Manager Assets se o documento e a pasta vinculada estiverem na mesma lista de documentos (como a área de documento de um projeto).

1. Localize o documento que deseja mover.
1. Arraste e solte o documento na pasta vinculada do Experience Manager Assets para a qual você deseja movê-lo.

As opções de documento não estarão disponíveis enquanto o documento estiver em processo de movimentação. Depois que o documento é movido para o Experience Manager Assets, o não fica mais visível na lista de documentos no Workfront.

>[!NOTE]
>
> As ações ou edições feitas no documento enquanto ele está sendo movido não aparecerão no documento no Experience Manager Assets e, portanto, serão perdidas.

