---
title: Melhorias nas solicitações 2.2.1
description: Melhorias nas solicitações 2.2.1
author: Luke
draft: Probably
feature: Product Announcements
exl-id: be6da26d-1d80-4946-8222-cd164b2b633f
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# Melhorias nas solicitações 2.2.1

Esta página descreve todas as melhorias de solicitações feitas com a versão 2.1 para o ambiente de visualização. Esses aprimoramentos serão disponibilizados no ambiente Produção

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

a semana de 17 de janeiro de 2022.

Para obter uma lista de todas as alterações disponíveis com a versão 22.1, consulte [Visão geral da versão 2.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Aprimoramento da interface para usuários que não têm acesso para criar solicitações

Para melhorar a experiência dos usuários ao trabalhar com solicitações, introduzimos uma melhoria na interface que indica ao usuário conectado que ele não tem acesso para criar solicitações. Com essa melhoria, o botão Nova solicitação fica apagado para usuários sem acesso para criar problemas. Passar o mouse sobre o botão esmaecido exibe uma dica de ferramenta que explica que o administrador do Workfront restringiu o acesso do usuário atual para criar solicitações.

Antes desse aprimoramento, o botão Nova solicitação não era exibido na área Solicitações para esses usuários. Copiar e enviar uma solicitação como nova também é restrito.

Para obter mais informações sobre como criar solicitações, consulte [Criar e enviar solicitações do Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Copiar e enviar solicitações

Para otimizar seu processo de envio de solicitações, estamos introduzindo uma nova funcionalidade que permite copiar uma solicitação existente e enviá-la como uma nova solicitação. Isso é útil quando você envia solicitações semelhantes com frequência. Nesse caso, você pode reutilizar uma solicitação existente, fazer algumas alterações e enviá-la como uma nova solicitação.

Com essa alteração, os usuários que podem exibir solicitações que outras pessoas enviaram também podem copiar essas solicitações e enviá-las como novas. Você pode impedir que isso aconteça atualizando a seguinte configuração no projeto da fila de solicitações: Pessoas da mesma empresa herdarão as mesmas permissões para todas as solicitações.

>[!NOTE]
>
>Não é possível copiar e reenviar problemas que foram enviados para uma fila de solicitações sem um tópico da fila antes do lançamento dessa funcionalidade.

Para obter mais informações, consulte [Copiar e enviar solicitações](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

## Experiência atualizada do painel Resumo na seção Enviado da área Solicitações

>[!NOTE]
>
>Esse recurso foi removido temporariamente do ambiente de Visualização em 12 de novembro de 2021. Ele será adicionado novamente em uma data posterior.

Para melhorar a visibilidade e a interação com o painel Resumo, adicionamos um rótulo ao ícone Abrir resumo na seção Enviado da área Solicitações. O rótulo agora é dinâmico e é atualizado dependendo se o painel está aberto ou fechado.

Ao abrir o painel Resumo sem selecionar uma solicitação primeiro, uma imagem mais simples agora é exibida para instruir claramente o usuário a selecionar um item antes de abrir o painel. Para obter mais informações, consulte [Localizar solicitações enviadas](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

Com essa alteração, o painel Resumo de tarefas, problemas e documentos também foi atualizado. Para obter informações sobre o painel Resumo, consulte [Visão geral do resumo](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).
