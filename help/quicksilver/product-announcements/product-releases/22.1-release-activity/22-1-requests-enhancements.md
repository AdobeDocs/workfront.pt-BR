---
title: 22.1 Solicitações de melhorias
description: 22.1 Solicitações de melhorias
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: be6da26d-1d80-4946-8222-cd164b2b633f
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# 22.1 Solicitações de melhorias

Esta página descreve todas as melhorias nas Solicitações feitas com a versão 22.1 para o ambiente de Pré-visualização. Esses aprimoramentos serão disponibilizados no ambiente de produção

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

a semana de 17 de janeiro de 2022.

Para obter uma lista de todas as alterações disponíveis com a versão 22.1, consulte a [Visão geral da versão 22.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Aprimoramento da interface para usuários que não têm acesso à criação de solicitações

Para melhorar a experiência dos usuários ao trabalhar com solicitações, introduzimos uma melhoria na interface que indica ao usuário conectado que ele não tem acesso para criar solicitações. Com essa melhoria, o botão Nova solicitação fica esmaecido para usuários sem acesso para criar problemas. Passar o mouse sobre o botão esmaecido exibe uma dica de ferramenta que explica que o administrador do Workfront restringiu o acesso do usuário atual para criar solicitações.

Antes desse aprimoramento, o botão Nova solicitação não era exibido na área Solicitações para esses usuários. Copiar e enviar uma solicitação como nova também é restrito.

Para obter mais informações sobre como criar solicitações, consulte [Criar e enviar solicitações do Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Copiar e enviar solicitações

Para otimizar seu processo de envio de solicitações, estamos introduzindo uma nova funcionalidade que permite copiar uma solicitação existente e enviá-la como uma nova solicitação. Isso é útil quando você envia solicitações semelhantes com frequência. Nesse caso, você pode reutilizar uma solicitação existente, fazer algumas alterações e enviá-la como uma nova solicitação.

Com essa alteração, os usuários que podem exibir solicitações enviadas por outras pessoas também podem copiá-las e enviá-las como novas. Você pode impedir que isso aconteça atualizando a seguinte configuração no projeto de fila de solicitações: as pessoas da mesma empresa herdarão as mesmas permissões para todas as solicitações.

>[!NOTE]
>
>Não é possível copiar e reenviar problemas que foram enviados para uma fila de solicitações sem um tópico da fila antes dessa funcionalidade ser lançada.

Para obter mais informações, consulte [Copiar e enviar solicitações](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

## Experiência atualizada do painel Resumo na seção Enviado da área Solicitações

>[!NOTE]
>
>Esse recurso foi removido temporariamente do ambiente de Pré-visualização em 12 de novembro de 2021. Ele será adicionado novamente em uma data posterior.

Para melhorar a visibilidade e a interação com o painel Resumo, adicionamos um rótulo ao ícone Abrir resumo na seção Enviado da área Solicitações. O rótulo agora é dinâmico e é atualizado dependendo se o painel está aberto ou fechado.

Ao abrir o painel Resumo sem primeiro selecionar uma solicitação, uma imagem mais simples agora é exibida para instruir claramente o usuário a selecionar um item antes de abrir o painel. Para obter mais informações, consulte [Localizar solicitações enviadas](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

Com essa alteração, o painel Resumo para tarefas, problemas e documentos também foi atualizado. Para obter informações sobre o painel Resumo, consulte [Visão geral do resumo](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).
