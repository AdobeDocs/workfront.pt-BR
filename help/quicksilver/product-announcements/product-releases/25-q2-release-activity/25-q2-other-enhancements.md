---
title: Outras melhorias durante o período da versão do segundo trimestre de 2025
description: Outras melhorias durante o período do segundo trimestre de 2025
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 214f0e67-1da4-4abd-b942-09889e8bd92b
source-git-commit: d603edee0099b6ce3e4f8d3414d1b31f94209196
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# Outras melhorias durante o período da versão do segundo trimestre de 2025

Esta página descreve as melhorias feitas com a versão do segundo trimestre de 2025 para o ambiente de Pré-visualização. Esses aprimoramentos serão disponibilizados no ambiente de Produção, conforme observado.

Para obter uma lista de todas as alterações disponíveis neste momento no ciclo de lançamento do Segundo trimestre de 2025, consulte [Visão geral da versão do Segundo trimestre de 2025](/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-release-overview.md).

## Atualize para a nova versão de assinatura de evento com pontos de extremidade de atualização de versão

>[!NOTE]
>
>Produção para todos os clientes: 6 de março de 2025

O Workfront agora tem versões de assinaturas de eventos. A nova versão não é uma alteração na API do Workfront, mas uma alteração na funcionalidade de assinatura do evento.

A capacidade de atualizar ou fazer downgrade de assinaturas de eventos garante que, quando alterações forem feitas na estrutura dos eventos, as assinaturas existentes não sejam interrompidas, permitindo testar e atualizar para a nova versão sem uma lacuna na assinatura do evento.

Para obter mais informações sobre as diferenças entre as duas versões, consulte o artigo [Versão de assinatura do evento](/help/quicksilver/wf-api/general/event-subs-versioning.md).

Para obter informações sobre os pontos de extremidade usados para atualizar ou baixar uma assinatura de evento entre versões, consulte a seção [Versão de assinatura de evento](/help/quicksilver/wf-api/general/event-subs-api.md#event-subscription-versioning) no artigo API de assinatura de evento.

## Representar as alterações de usuário do Adobe Admin Console como &quot;Sistema&quot; no feed de atualização do Workfront

>[!NOTE]
>
>Versão de pré-visualização: 23 de janeiro de 2025; Produção para lançamento rápido: Com o lançamento 25.2 (13 de fevereiro de 2025); Produção para lançamento trimestral: Com o lançamento 25.4 (abril de 2025)

Agora, quando o administrador do Adobe Admin Console faz uma alteração nas informações de usuário de um usuário do Workfront, o Workfront registra essa alteração na guia Atividade do sistema da área Atualizações do usuário, como pertencente ao &quot;Sistema&quot;. Refere-se ao administrador do Adobe Admin Console.

Antes dessa atualização, as alterações do usuário feitas pelo administrador do Admin Console eram registradas como feitas pelo administrador principal do sistema do Workfront.

Para obter informações sobre como gerenciar usuários na Adobe Admin Console, consulte [Gerenciar usuários na Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)
