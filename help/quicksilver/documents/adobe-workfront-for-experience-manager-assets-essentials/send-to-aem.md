---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Enviar um documento para o Experience Manager Assets ou Assets Essentials
description: Você pode enviar documentos do Workfront para o Experience Manager Assets ou Assets Essentials. Os documentos carregados e enviados do Workfront para o Assets Essentials ainda contam em relação ao armazenamento geral de documentos. Os ativos vinculados do Assets Essentials não contam para o armazenamento geral.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 7942e77b-9466-4dff-9737-97b17647ac48
source-git-commit: 6bedca2f3394fadc6d6ffbb34654fd1f0194a5d6
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---

# Enviar um documento para o Experience Manager Assets ou Assets Essentials


Você pode enviar documentos do Workfront para o Experience Manager Assets ou Assets Essentials. Os documentos carregados e enviados do Workfront para o Assets Essentials ainda contam em relação ao armazenamento geral de documentos. Os ativos vinculados do Assets Essentials não contam para o armazenamento geral.

Os campos de metadados são mapeados pela primeira vez ao enviar um ativo do Workfront para a Experience Manager Assets ou Assets Essentials. Todos os metadados configurados para mapear objetos pai também são enviados. Para obter mais informações sobre como configurar o mapeamento de metadados, consulte [Configurar a integração as a Cloud Service do Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configurar a integração do Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**Exemplo** Ao enviar um ativo anexado a uma tarefa pela primeira vez, os metadados da tarefa são mapeados para o Experience Manager Assets ou Assets Essentials, bem como quaisquer metadados mapeados de objetos pai, como um projeto, portfólio e programa.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Plano Adobe Workfront</a>*</td> 
   <td> <p> Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Visão geral das licenças do Adobe Workfront</a>*</td> 
   <td> <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Você deve ter o Experience Manager as a Cloud Service ou Assets Essentials e deve ser adicionado ao produto como um usuário no Admin Console.
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir acesso ou superior em Documentos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Antes de começar,

* O administrador do Workfront deve configurar uma integração com o Experience Manager. Para obter mais informações, consulte [Configurar a integração as a Cloud Service do Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configurar a integração do Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Enviar um documento do Workfront

Quando um usuário envia um documento do Workfront para o Experience Manager Assets ou Assets Essentials, os metadados mapeados são transferidos ao longo do documento. Depois que o documento é enviado, as alterações feitas nos metadados do documento no Workfront não são refletidas no Assets ou no Assets Essentials. Se um campo mapeado no Workfront for alterado, você deverá enviar uma nova versão do documento com os metadados atualizados para Assets ou Assets Essentials. Para configurar ou editar metadados, consulte [Configurar a integração as a Cloud Service do Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configurar a integração do Experience Manager Assets Essentials](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

Para enviar um documento:

1. Vá para o **Documentos** no Workfront e selecione o documento que deseja enviar.
1. Clique em **Enviar para** e escolha a integração do Experience Manager configurada pelo administrador.

   >[!NOTE]
   >
   >O administrador do Workfront pode escolher qualquer nome para essa integração, de modo que pode não mencionar especificamente o Assets ou o Assets Essentials.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Escolha para onde deseja direcionar o ativo e clique em **Selecionar pasta**.
1. Ao encontrar o destino desejado, clique em **Salvar**.

## Enviar uma nova versão

Você pode adicionar uma nova versão a um documento que tenha carregado anteriormente no Workfront. Para obter mais informações, consulte [Fazer upload de uma nova versão de um documento](../../documents/managing-documents/upload-new-document-version.md). Depois que a versão mais recente for carregada, você poderá enviá-la para o Assets Essentials. Se um campo mapeado no Workfront tiver sido alterado, a nova versão atualizará os metadados no Assets Essentials quando ele enviar.

>[!IMPORTANT]
>
>Antes de fazer upload de uma nova versão para o Workfront, recomendamos renomear o arquivo. Se você carregar uma nova versão com exatamente o mesmo nome de arquivo de uma versão anterior, somente a versão mais recente poderá ser baixada do Workfront. Todas as versões podem ser baixadas do Experience Manager Assets ou do Assets Essentials, independentemente do nome do arquivo.

Para enviar a versão mais recente:

1. Vá para o **Documentos** no Workfront e localize o documento.
1. Selecionar **Enviar para** e escolha a integração do Experience Manager configurada pelo administrador.

   >[!NOTE]
   >
   >O administrador do Workfront pode escolher qualquer nome para essa integração, de modo que talvez não mencione especificamente os Ativos ou o Assets Essentials.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Clique em **Salvar**. A nova versão salva no mesmo local que a versão anterior.
