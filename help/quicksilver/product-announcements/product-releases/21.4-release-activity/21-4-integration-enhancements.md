---
title: 21.4 Melhorias da integração
description: 21.4 Melhorias da integração
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
exl-id: d3e2342e-1c44-49c2-90bc-9fd77fbb2db8
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---

# 21.4 Melhorias da integração

Esta página descreve todas as melhorias da integração feitas com a versão 21.4 para o ambiente de visualização. Esses aprimoramentos serão disponibilizados no ambiente de produção na semana de 4 de outubro de 2021.

Para obter uma lista de todas as alterações disponíveis com a versão 21.4, consulte [Visão geral da versão 21.4](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## Vincular documentos do Dropbox Business

Adicionamos o Dropbox Business como uma integração de documento disponível. Agora, você pode acessar documentos armazenados no Dropbox Business diretamente do Workfront.

O Dropbox Business permite vincular documentos compartilhados e fazer upload de documentos a pastas compartilhadas. O Dropbox (não o Dropbox Business) permite que somente o proprietário dos documentos exiba o documento no Workfront.

O administrador da Workfront pode habilitar essa integração para sua organização.

Para obter mais informações, consulte [Vincular documentos de aplicativos externos](../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Para obter informações sobre como um administrador do Workfront pode habilitar essa opção, consulte [Configurar integrações de documentos](../../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Atualizações do Workfront para o Slack

As seguintes atualizações agora estão visíveis na integração do Workfront for Slack:

* O Workfront for Slack tem uma nova aparência.
* Agora você recebe sua Workfront para notificações do Slack em tempo real.

   Por exemplo, se estiver atribuído a uma tarefa, você receberá essa notificação assim que estiver atribuído. Anteriormente, poderia haver um atraso antes da notificação aparecer no Slack.

Esta atualização requer que você reautorize seu Workfront para integração com o Slack. Para obter informações sobre como autorizar a integração, consulte [Configurar o Adobe Workfront para Slack](../../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Para obter mais informações sobre o Workfront para notificações de Slack, consulte [Receber notificações do Adobe Workfront no Slack](../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Veja mais claramente os detalhes do acesso à conta ao dar consentimento às integrações do Adobe Workfront

As telas de consentimento das integrações do Adobe Workfront foram atualizadas. Agora, é possível ver as ações e áreas específicas às quais as integrações têm acesso, para que você possa entender melhor o que está permitindo que a integração ou o aplicativo acesse.

Essa nova tela de consentimento se aplica a qualquer integração do Adobe Workfront que use o OAuth 2.0.

Para obter detalhes sobre integrações específicas, consulte a documentação da integração.

## A autenticação da chave de API não é mais necessária para integrações

As integrações da Workfront começaram recentemente a usar o OAuth2 para maior segurança e usabilidade. Como parte dessa mudança, a Workfront não precisa mais de chaves de API para autenticação de integrações.
