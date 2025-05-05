---
title: 20.4 Outras melhorias
description: 20.4 Outras melhorias
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: bd8fcafc-00cc-4025-b2d3-e3a6f12e40fc
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---

# 20.4 Outras melhorias

Esta página descreve todas as outras melhorias feitas com a versão 20.4 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de Produção na semana de 9 de novembro de 2020.

Para obter uma lista de todas as alterações disponíveis com a versão 20.4, consulte a [visão geral da versão 20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Novo para administradores: opção de alternar ambiente do Workfront disponível

Para obter uma experiência mais eficiente e conveniente, os administradores de grupo e os administradores do Workfront agora podem alternar rapidamente entre diferentes ambientes do Workfront de qualquer página no Workfront sem precisar fazer logoff.

Na nova experiência do Workfront, a opção Alternar para o clássico aparece no Menu principal.

No Workfront Classic, a opção Alternar para a nova experiência é exibida no menu exibido ao clicar na imagem do perfil no canto superior direito da Barra de navegação global.

Este recurso agora está incluído no [Princípios básicos do administrador, Parte 1 do caminho de aprendizado](https://experienceleague.adobe.com/pt-br/docs/workfront-learn/tutorials-workfront/home) no Workfront One.

## Criptografia aprimorada para Workfront Proof

Estamos fazendo algumas alterações para melhorar a força da criptografia de dados em movimento do Workfront Proofing Application. As cifras TLS fracas serão descontinuadas em 11 de novembro de 2020.

Verifique se você está usando um navegador compatível ao acessar o Workfront. Para obter mais informações sobre navegadores compatíveis, consulte [requisitos do navegador Adobe Workfront](../../../workfront-basics/workfront-browser-requirements.md).

## Nova aparência para 3 modelos de email

Para melhorar a legibilidade e a experiência geral, os seguintes modelos de email têm uma nova aparência:

* Nova solicitação de trabalho
* Uma tarefa dependente à qual você está atribuído está pronta para começar agora
* Notificação de email da equipe com o predecessor concluída

Para habilitar emails para fins de teste no seu ambiente de Visualização, consulte a seção Gerenciamento de emails em visualização em [Modificar suas próprias notificações por email](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Novas notificações por email para equipes

Adicionamos a seguinte notificação por email para equipes:

* Um predecessor de uma tarefa atribuída à minha equipe é concluído: a equipe atribuída recebe uma notificação por email quando um predecessor de uma de suas tarefas é marcado como concluído.
* Todos os predecessores de uma tarefa atribuída à minha equipe são concluídos: a equipe atribuída recebe uma notificação por email para cada predecessor marcado como concluído.

Para obter mais informações, consulte [Notificações: informações sobre o trabalho atribuído a mim](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

## Novo para administradores: melhorias na notificação por email

Agora, com um único clique, você pode ativar ou desativar uma notificação por email de evento em Configurar. Basta clicar na opção Ligar/Desligar ao lado do nome da notificação.

Além disso, observe que nosso estilo moderno agora melhora a experiência de configuração de notificações de eventos na área Notificações por email.

Para obter informações sobre como configurar notificações por email, consulte [Configurar notificações de eventos para todos no sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

Este recurso agora está incluído no [Caminho de Aprendizado de emails e notificações no aplicativo](https://experienceleague.adobe.com/pt-br/docs/workfront-learn/tutorials-workfront/home) no Workfront One.

## Novos objetos de API que acionam atualizações de assinatura de evento

Dois novos objetos de API, documentVersion e proofApproval, foram criados e estão configurados para acionar atualizações de assinatura de evento quando um documento é versionado ou aprovado.

Para obter uma lista completa dos campos associados a cada objeto, consulte os [campos de recurso de assinatura de evento](../../../wf-api/api/event-sub-resource-fields.md).
