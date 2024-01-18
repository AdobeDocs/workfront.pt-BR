---
title: 21.4 Aprimoramentos de integração
description: 21.4 Aprimoramentos de integração
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: d3e2342e-1c44-49c2-90bc-9fd77fbb2db8
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# 21.4 Aprimoramentos de integração

Esta página descreve todas as melhorias de Integração feitas com a versão 21.4 para o ambiente de Pré-visualização. Esses aprimoramentos serão disponibilizados no ambiente de Produção na semana de 4 de outubro de 2021.

Para obter uma lista de todas as alterações disponíveis com a versão 21.4, consulte [21.4 Visão geral da versão](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## Vincular documentos do Dropbox Business

Adicionamos o Dropbox Business como uma integração de documentos disponível. Agora, você pode acessar os documentos armazenados no Dropbox Business diretamente da Workfront.

O Dropbox Business permite vincular documentos compartilhados e carregá-los em pastas compartilhadas. O Dropbox (não o Dropbox Business) permite que somente o proprietário dos documentos visualize o documento no Workfront.

O administrador do Workfront pode habilitar essa integração para sua organização.

Para obter mais informações, consulte [Vincular documentos de aplicativos externos](../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Para obter informações sobre como um administrador do Workfront pode ativar essa opção, consulte [Configurar integrações de documentos](../../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Atualizações do Workfront para Slack

As seguintes atualizações estão agora visíveis no Workfront para integração de Slack:

* O Workfront for Slack tem uma nova aparência.
* Agora você recebe seu Workfront para notificações de Slack em tempo real.

  Por exemplo, se estiver atribuído a uma tarefa, você receberá essa notificação assim que for atribuído. Anteriormente, podia haver um atraso antes de a notificação aparecer no Slack.

Esta atualização exige que você reautorize seu Workfront para integração com o Slack. Para obter informações sobre como autorizar a integração, consulte [Configurar Adobe Workfront para Slack](../../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Para obter mais informações sobre o Workfront para notificações Slack, consulte [Receber notificações do Adobe Workfront no Slack](../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Veja mais claramente os detalhes de acesso à conta ao consentir com integrações do Adobe Workfront

As telas de consentimento para integrações do Adobe Workfront foram atualizadas. Agora é possível ver as ações e áreas específicas às quais as integrações têm acesso, para que você possa entender melhor o que está permitindo que a integração ou o aplicativo tenha acesso.

Essa nova tela de consentimento se aplica a qualquer integração do Adobe Workfront que use o OAuth 2.0.

Para obter detalhes sobre integrações específicas, consulte a documentação dessa integração.

## A autenticação da chave de API não é mais necessária para integrações

As integrações do Workfront começaram recentemente a usar o OAuth2 para maior segurança e usabilidade. Como parte dessa mudança, o Workfront não exige mais chaves de API para autenticação de integrações.
