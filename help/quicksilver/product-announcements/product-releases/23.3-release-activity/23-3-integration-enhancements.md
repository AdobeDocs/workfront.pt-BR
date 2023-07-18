---
title: 23.3 Aprimoramentos de integração
description: 23.3 Aprimoramentos de integração
author: Lisa
feature: Product Announcements
source-git-commit: 75e035bcdf75501e34fd9de57dd6eab85d9e5542
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 0%

---

# 23.3 Aprimoramentos de integração

Esta página descreve todas as melhorias de integração feitas com a versão 23.3 para o ambiente de Pré-visualização. Esses aprimoramentos serão disponibilizados no ambiente de produção com a versão 23.3.

Para obter uma lista de todas as alterações disponíveis neste ponto do ciclo de versão 23.3, consulte [23.3 Visão geral da versão](/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-release-overview.md).

## Nova integração do G Suite disponível

Uma nova integração do G Suite agora está disponível no Google Marketplace. A nova integração é autenticada usando o OAuth2 e substitui a integração anterior.

A integração G Suite anterior agora está obsoleta e será automaticamente desinstalada.

Para obter instruções sobre como instalar a nova integração, consulte [Instalar [!DNL Adobe Workfront for G Suite]](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

Para obter mais informações sobre o Workfront para G Suite, consulte [Workfront para G Suite](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/workfront-for-gsuite.md).

## As integrações do Adobe Creative Cloud agora oferecem suporte a vários usuários atribuídos

A integração do Adobe Creative Cloud agora oferece suporte à capacidade de escolher entre &quot;Concluído com minha parte&quot; e &quot;Concluído&quot; (ou &quot;Resolvido&quot;) quando uma tarefa ou problema tiver vários usuários atribuídos.

Anteriormente, a integração permitia que os usuários marcassem uma tarefa como concluída, sem especificar &quot;Concluída com minha parte&quot; ou &quot;Concluída&quot;/&quot;Resolvida&quot;.

Para aproveitar essa funcionalidade, baixe e instale os plug-ins mais recentes do Workfront for Creative Cloud.

Para obter mais informações sobre a funcionalidade, consulte [Marcar itens de trabalho como concluídos usando o plug-in do Adobe Workfront](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-complete.md).

Para obter informações sobre como instalar os plug-ins do Workfront para Creative Cloud, consulte [Instalar o plug-in do Adobe Workfront para aplicativos Creative Cloud](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

## Exibir e gerenciar notificações do Workfront na Workfront para plug-ins do Creative Cloud

Para facilitar o recebimento das notificações necessárias, possibilitamos a exibição e o gerenciamento das notificações do Workfront sem sair da Adobe Creative Cloud. Agora, você pode visualizar as notificações e acessar os itens de trabalho e comentários relacionados a essas notificações diretamente da janela de plug-in do Workfront no aplicativo Creative Cloud.

Anteriormente, as notificações só estavam disponíveis no Workfront e por email.

Para aproveitar essa funcionalidade, baixe e instale os plug-ins mais recentes do Workfront for Creative Cloud.

Para obter mais informações, consulte [Exibir e gerenciar [!DNL Adobe Workfront] notificações do Adobe Creative Cloud](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-notifications.md).

Para obter informações sobre como instalar os plug-ins do Workfront para Creative Cloud, consulte [Instalar o plug-in do Adobe Workfront para aplicativos Creative Cloud](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

<!--

## Improved experience when moving a document to a linked folder with drag and drop

We've added some transparency to the process of dragging and dropping a document into a linked folder. Now, the document that you moved to a linked folder remains in the document list until it has fully moved. The document options are disabled, but you can still open the document for view while it is moving. When the document has completed the transfer, it disappears from the document list, because it is now fully located in the linked folder.

Previously, documents would immediately disappear from the document list, before they had finished moving to the linked folder.

For more information, see [Link documents from external applications](/help/quicksilver/documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

-->

## Criar automaticamente pastas vinculadas ao Adobe Experience Manager Assets ao criar um projeto

Com o novo fluxo de trabalho Criar pasta vinculada para a integração do Adobe Experience Manager, é possível configurar a integração com um caminho para uma pasta do Adobe Experience Manager Assets. Quando a integração é adicionada a um modelo de projeto, qualquer projeto criado a partir do modelo criará automaticamente uma subpasta vinculada no Experience Manager Assets na pasta especificada.

Anteriormente, a criação de pastas vinculadas exigia uma ação por parte do usuário.

Essa funcionalidade só está disponível com uma integração do Adobe Experience Manager as a Cloud Service no Workfront. Isso não está disponível no conector aprimorado do Adobe Experience Manager.

Para obter mais informações, consulte [Usar fluxos de trabalho na integração do Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).

## Mapear valores de campo do Workfront para tags na Experience Manager Assets

Agora, você pode categorizar e encontrar rapidamente ativos com base em dados da Workfront. Você pode mapear esses dados como parte da configuração de metadados na integração do Workfront para Experience Manager Assets.

Anteriormente, o mapeamento de dados do Workfront para tags da Experience Manager Assets não estava disponível.

Para obter mais informações sobre essa funcionalidade no Experience Manager Assets as a Cloud Service, consulte [Configure o [!UICONTROL Experience Manager Assets as a Cloud Service] integração](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
Para obter mais informações sobre essa funcionalidade no Experience Manager Assets Essentials, consulte [Configurar a integração do Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Mapear campos do Workfront para campos de metadados personalizados do Experience Manager Assets

Com a integração nativa, agora é possível mapear campos nativos e integrados do Workfront para campos de esquema de metadados personalizados no Experience Manager Assets as a Cloud Service.

Para obter mais informações sobre essa funcionalidade no Experience Manager Assets as a Cloud Service, consulte [Configure o [!UICONTROL Experience Manager Assets as a Cloud Service] integração](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
Para obter mais informações sobre essa funcionalidade no Experience Manager Assets Essentials, consulte [Configurar a integração do Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Ajustar as configurações do modelo de fluxo de trabalho de prova automatizada usando Adobe Workfront for Creative Cloud

Agora você pode ajustar as configurações existentes do modelo de fluxo de trabalho automatizado diretamente no Creative Cloud. Depois de escolher um template de workflow automatizado existente, você pode:

* Desabilitar estágios
* Adicionar mais destinatários
* Alterar funções de prova
* Ajustar o prazo
* Atualizar notificações por email
* E muito mais!

Para obter mais informações, consulte [Fazer upload de documentos e provas com o [!DNL Adobe Workfront] plug-in para [!DNL Creative Cloud] Aplicativos](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-docs-proofs-toc.md).

Esses aprimoramentos estão disponíveis para os seguintes aplicativos Creative Cloud:

* Photoshop
* XD
* InDesign
* Illustrator
