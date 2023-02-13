---
title: 20.4 Outras melhorias
description: 20.4 Outras melhorias
author: Luke
draft: Probably
feature: Product Announcements
exl-id: bd8fcafc-00cc-4025-b2d3-e3a6f12e40fc
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# 20.4 Outras melhorias

Esta página descreve todas as outras melhorias feitas com a versão 20.4 para o ambiente de visualização. Esses aprimoramentos serão disponibilizados no ambiente de Produção na semana de 9 de novembro de 2020.

Para obter uma lista de todas as alterações disponíveis com a versão 20.4, consulte [Visão geral da versão 20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Novo para administradores: Alternar a opção de ambiente Workfront disponível

Para obter uma experiência mais eficiente e conveniente, os administradores de grupo e os administradores do Workfront agora podem alternar rapidamente entre diferentes ambientes Workfront de qualquer página no Workfront sem precisar fazer logoff.

Na nova experiência do Workfront, a opção Alternar para o Classic é exibida no Menu principal.

No Workfront Classic, a opção Alternar para a nova experiência aparece no menu que é exibido ao clicar na imagem do perfil no canto superior direito da Barra de navegação global.

Esse recurso agora está incluído na variável [Fundamentos do administrador, caminho de aprendizagem da parte 1](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) no Workfront One.

## Criptografia aprimorada para Workfront Proof

Estamos fazendo algumas alterações para melhorar a força da criptografia de dados em movimento do aplicativo Workfront Proofing. As cifras TLS fracas serão descontinuadas em 11 de novembro de 2020.

Verifique se você está usando um navegador compatível ao acessar o Workfront. Para obter mais informações sobre navegadores compatíveis, consulte [Requisitos do navegador Adobe Workfront](../../../workfront-basics/workfront-browser-requirements.md).

## Nova aparência para três modelos de email

Para melhorar a legibilidade e a experiência geral, os seguintes modelos de email têm uma nova aparência:

* Nova solicitação de trabalho
* Uma tarefa dependente atribuída agora está pronta para iniciar
* Notificação por email de equipe com o antecessor concluído

Para ativar o email para fins de teste no ambiente de Visualização, consulte a seção Gerenciamento de emails na visualização em [Ativar ou desativar suas próprias notificações de evento](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Novas notificações por email para equipes

Adicionamos a seguinte notificação por email para equipes:

* Um antecessor de uma tarefa atribuída à minha equipe está concluído: A equipe atribuída recebe uma notificação por email quando um antecessor de uma de suas tarefas é marcado como concluído.
* Todos os antecessores de uma tarefa atribuída à minha equipe são concluídos: A equipe atribuída recebe uma notificação por email para cada antecessor marcado como concluído.

Para obter mais informações, consulte [Notificações: Informações sobre o trabalho que me foi atribuído](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

## Novo para administradores: Melhorias na notificação por email

Agora, com um único clique, você pode ativar ou desativar uma notificação de e-mail de evento em Configurar. Basta clicar no botão Ligar/Desligar ao lado do nome da notificação.

Além disso, observe nosso estilo moderno agora melhorando a experiência de configuração de notificações de eventos na área Notificações de email .

Para obter informações sobre como configurar notificações por email, consulte [Configurar notificações de evento para todos no sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

Esse recurso agora está incluído na variável [Caminho de aprendizado das notificações por email e no aplicativo](https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-20Y4X000000CaZGUA0) no Workfront One.

## Novos objetos de API que acionam atualizações de assinatura de evento

Dois novos objetos de API, documentVersion e proofApproval, foram criados e configurados para acionar atualizações de assinatura de evento quando um documento é com controle de versão ou aprovado.

Para obter uma lista completa dos campos associados a cada objeto, consulte [Campos de recurso de assinatura de evento](../../../wf-api/api/event-sub-resource-fields.md).
