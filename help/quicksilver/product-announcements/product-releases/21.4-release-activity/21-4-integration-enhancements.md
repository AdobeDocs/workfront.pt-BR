---
title: Aprimoramentos na integração na 21.4
description: Aprimoramentos na integração na 21.4
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: d3e2342e-1c44-49c2-90bc-9fd77fbb2db8
TQID: https://experienceleague.adobe.com/dCRr9YQiXiX82Jw7wyeT786T8oJ74-u6kOuevYy-SWY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: e4fedd42-4a54-4109-859f-13c7f0366a72
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 367
ht-degree: 2%

---

# Aprimoramentos na integração na 21.4

Esta página descreve todas as melhorias de Integração feitas com a versão 21.4 para o ambiente de Pré-visualização. Esses aprimoramentos serão disponibilizados no ambiente de Produção na semana de 4 de outubro de 2021.

Para obter uma lista de todas as alterações disponíveis com a versão 21.4, consulte a [Visão geral da versão 21.4](../../../product-announcements/product-releases/21.4-release-activity/21-4-release-overview.md).

## Vincular documentos do Dropbox Business

Adicionamos o Dropbox Business como uma integração de documentos disponível. Agora, você pode acessar documentos armazenados no Dropbox Business diretamente da Workfront.

O Dropbox Business permite vincular documentos compartilhados e carregá-los em pastas compartilhadas. O Dropbox (não o Dropbox Business) permite que somente o proprietário dos documentos visualize o documento no Workfront.

O administrador do Workfront pode habilitar essa integração para sua organização.

Para obter mais informações, consulte [Vincular documentos de aplicativos externos](../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Para obter informações sobre como um administrador do Workfront pode habilitar esta opção, consulte [Configurar integrações de documentos](../../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Atualizações do Workfront para Slack

As seguintes atualizações estão visíveis na integração do Workfront para Slack:

* O Workfront para Slack tem uma nova aparência.
* Agora você recebe as notificações do Workfront for Slack em tempo real.

  Por exemplo, se estiver atribuído a uma tarefa, você receberá essa notificação assim que for atribuído. Anteriormente, podia haver um atraso antes de a notificação aparecer no Slack.

Esta atualização requer que você autorize novamente sua integração do Workfront para Slack. Para obter informações sobre como autorizar a integração, consulte [Configurar Adobe Workfront para Slack](../../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Para obter mais informações sobre notificações do Workfront para Slack, consulte [Receber notificações do Adobe Workfront no Slack](../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Veja mais claramente os detalhes de acesso à conta ao consentir com integrações do Adobe Workfront

As telas de consentimento para integrações do Adobe Workfront foram atualizadas. Agora é possível ver as ações e áreas específicas às quais as integrações têm acesso, para que você possa entender melhor o que está permitindo que a integração ou o aplicativo tenha acesso.

Essa nova tela de consentimento se aplica a qualquer integração do Adobe Workfront que use o OAuth 2.0.

Para obter detalhes sobre integrações específicas, consulte a documentação dessa integração.

## A autenticação da chave de API não é mais necessária para integrações

As integrações do Workfront começaram recentemente a usar o OAuth2 para maior segurança e usabilidade. Como parte dessa mudança, o Workfront não exige mais chaves de API para autenticação de integrações.
