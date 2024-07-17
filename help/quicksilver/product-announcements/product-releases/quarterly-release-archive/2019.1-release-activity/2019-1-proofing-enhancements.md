---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: Aprimoramentos de provas do 2019.1
description: Esta página descreve todas as melhorias de prova incluídas na versão 2019.1. A funcionalidade agora está disponível no ambiente de Produção do.
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 6b9b847c-dfb5-4285-b8fc-72f33c6a54d0
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 0%

---

# Aprimoramentos de provas do 2019.1

Esta página descreve todas as melhorias de prova incluídas na versão 2019.1. A funcionalidade agora está disponível no ambiente de Produção do.

Para obter uma lista de todas as alterações feitas em 2019.1, consulte a [visão geral da atividade da versão 2019.1](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md).

## Para administradores

* [Configurar a função de prova padrão para não destinatários que abrem uma prova](#configure-default-proofing-role-for-non-recipients-who-open-a-proof)

## Para todos os usuários

* [Provar conteúdo interativo no Visualizador de provas da Web](#proof-interactive-content-in-the-web-proofing-viewer)
* [A ordem de classificação padrão para comentários no Visualizador de provas agora é da mais antiga para a mais recente](#default-sorting-order-for-comments-in-the-proofing-viewer-is-now-oldest-to-latest)
* [Revisão aprimorada para comentários no Visualizador de provas associado a um intervalo de vídeo](#enhanced-reviewing-for-comments-in-the-proofing-viewer-associated-with-a-range-of-video)
* [Link para detalhes do documento de uma notificação de prova ou do visualizador de provas](#link-to-document-details-from-a-proof-notification-or-the-proofing-viewer)
* [Alterar suas notificações por email no Visualizador de provas](#change-your-email-notifications-in-the-proofing-viewer)
* [Alterar a cor de fundo no Visualizador de provas da área de trabalho](#change-the-background-color-in-the-desktop-proofing-viewer)
* [Limpar dados do navegador em cache de uma prova no Visualizador de provas do desktop](#clear-cached-browser-data-from-a-proof-in-the-desktop-proofing-viewer)

## Configurar a função de prova padrão para não destinatários que abrem uma prova {#configure-default-proofing-role-for-non-recipients-who-open-a-proof}

Os administradores do Workfront agora podem configurar a função de prova padrão para usuários que não são designados como destinatários no fluxo de trabalho da prova, mas que têm acesso à prova por meio do objeto do Workfront (como projeto, tarefa ou problema).

Anteriormente, quando usuários e convidados tinham acesso a uma prova sem serem adicionados ao fluxo de trabalho, a função de prova padrão era Revisor.

Essa funcionalidade se aplica somente às provas criadas no Workfront, não no Workfront Proof.

## Provar conteúdo interativo no Visualizador de provas da Web {#proof-interactive-content-in-the-web-proofing-viewer}

Se as políticas de segurança de sua organização não permitirem o uso do aplicativo independente Visualizador de provas de desktop, o administrador do Workfront poderá habilitar o conteúdo interativo no Visualizador de provas de web. O conteúdo deve ser incluído em um arquivo ZIP antes de você criar a prova.

Para obter mais informações, consulte no artigo .

VÍDEO

## A ordem de classificação padrão para comentários no Visualizador de provas agora é da mais antiga para a mais recente  {#default-sorting-order-for-comments-in-the-proofing-viewer-is-now-oldest-to-latest}

No Visualizador de provas, a ordem de classificação padrão para comentários em uma prova agora é Da mais antiga para a mais recente, como em uma conversa verbal.

Anteriormente, a ordem de classificação padrão era da Mais recente para a Mais antiga.

É possível selecionar uma opção de classificação diferente e ela é lembrada por todas as outras provas abertas.

Para obter mais informações, consulte a seção no artigo .

## Revisão aprimorada para comentários no visualizador de provas associado a uma variedade de vídeos {#enhanced-reviewing-for-comments-in-the-proofing-viewer-associated-with-a-range-of-video}

Ao revisar um comentário associado a uma variedade de sequências de vídeo no Visualizador de provas, você pode clicar em Reproduzir para exibir toda a sequência de sequências de vídeo. A reprodução é pausada quando atinge o final do intervalo. O comentário permanece aberto para que você não perca a noção de onde está.

Anteriormente, ao abrir um comentário para uma variedade de sequências de vídeo, era necessário localizar o início do intervalo manualmente, observando os números de quadros exibidos no comentário antes de clicar em Reproduzir. Caso contrário, o Visualizador de provas iniciará a reprodução onde você clicou na linha do tempo do vídeo e ela não será pausada no final do intervalo. Além disso, o comentário foi recolhido ao clicar em Reproduzir, portanto, não ficou mais claro qual comentário você estava revisando.

Para obter informações sobre a revisão de provas de vídeo, consulte.

VÍDEO

## Link para detalhes do documento de uma notificação de prova ou do visualizador de provas {#link-to-document-details-from-a-proof-notification-or-the-proofing-viewer}

Ao receber um email convidando você a revisar uma prova ou ao revisar uma prova no Visualizador de provas, agora é possível acessar rapidamente a página Detalhes do documento da prova. Nesta página, você pode ver o objeto Workfront (como uma tarefa, projeto ou problema) associado à prova. Isso fornece contexto para ajudar você a entender o trabalho que precisa fazer na prova.

Essa funcionalidade pode funcionar somente para novos usuários adicionados ao sistema. Esse problema é temporário.

Para obter mais informações, consulte o artigo .

VÍDEO

## Alterar as notificações por email no Visualizador de provas {#change-your-email-notifications-in-the-proofing-viewer}

Agora, todos os revisores de prova podem especificar quais notificações de prova desejam receber para uma prova. Isso é particularmente importante ao colaborar com partes interessadas externas.

Anteriormente, somente o proprietário da prova ou o gerente de tráfego podia configurar alertas de email de uma prova para os revisores adicionados à prova. Colaboradores externos não conseguiram controlar quais alertas de email receberam sobre a prova porque não tinham o acesso necessário ao Workfront nem o nível de permissão apropriado.

Essas configurações são separadas das configurações de alerta por email que podem ser definidas no Workfront.

Para obter mais informações, consulte [Gerenciar notificações para comentários de prova e decisões](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md)

VÍDEO

## Alterar a cor de fundo no Visualizador de provas da área de trabalho {#change-the-background-color-in-the-desktop-proofing-viewer}

Agora é possível alterar a cor de fundo do Visualizador de provas de desktop da cor padrão quase preta para branco. Isso facilita a visualização de conteúdo de prova que tenha um plano de fundo transparente.

Para obter mais informações, consulte [Definir configurações do revisor de provas](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

VÍDEO

## Limpar dados do navegador em cache de uma prova no Visualizador de provas do desktop {#clear-cached-browser-data-from-a-proof-in-the-desktop-proofing-viewer}

Quando as configurações de cookie e cache do seu navegador estão definidas para bloquear conteúdo como pop-ups, esse comportamento de bloqueio também pode ocorrer no Visualizador de provas de desktop, impossibilitando que os revisores vejam e comentem o conteúdo pop-up na sua prova.

Agora é possível limpar os dados de cache do navegador que podem ser salvos com uma prova para que todo o conteúdo apareça no Visualizador de provas de desktop e os revisores possam vê-lo e comentá-lo.

Para obter mais informações, consulte [Definir configurações do revisor de provas](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

VÍDEO
