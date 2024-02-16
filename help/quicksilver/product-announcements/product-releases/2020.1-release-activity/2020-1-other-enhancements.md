---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: 2020.1 Outras melhorias
description: Esta página descreve todas as melhorias feitas nas áreas gerais do Workfront com a versão 2020.1. Esses aprimoramentos estão disponíveis atualmente no ambiente de Pré-visualização e serão disponibilizados no ambiente Produção no final de março ou início de abril de 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a716590c-c833-458a-a138-9bc0723e5896
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# 2020.1 Outras melhorias

Esta página descreve todas as melhorias feitas nas áreas gerais do Workfront com a versão 2020.1. Esses aprimoramentos estão disponíveis atualmente no ambiente de Pré-visualização e serão disponibilizados no ambiente Produção no final de março ou início de abril de 2020.

Para obter uma lista de todas as alterações disponíveis com a versão 2020.1, consulte [Visão geral da versão 2020.1](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md).

## Alteração necessária para adicionar provas ao arquivo de inclui na lista de permissões

>[!NOTE]
>
>Este recurso foi removido da versão 2020.1. Ele será disponibilizado posteriormente.

O domínio de comprovação está alterando from proofhq.com para workfront.com.

Se o firewall ou servidor de email estiver configurado para permitir acesso apenas a fornecedores específicos, você deverá adicionar o seguinte URL adicional ao seu arquivo de inclui na lista de permissões para garantir que os usuários em sua organização possam exibir provas no Workfront tanto no visualizador de prova de navegador quanto no visualizador de prova de desktop:

&#42;.workfront.com

A variável &#42;O URL do proofhq.com também é obrigatório.

Para obter mais informações sobre a atualização da sua inclui na lista de permissões, consulte [Incluir na lista de permissões Configurar o arquivo de pesquisa do firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

>[!NOTE]
>
>Essa atualização se aplica somente à prova no Workfront; não se aplica ao usar o aplicativo independente do Workfront Proof.

## Comportamento de cookie do Workfront atualizado para manter a compatibilidade com o Chrome

Para manter a compatibilidade com uma atualização futura do Google Chrome (Chrome v80), atualizamos a plataforma do Workfront para garantir que os cookies sejam enviados adequadamente com as solicitações.

Essa atualização do Chrome altera o valor padrão do atributo de cookie SameSite. Se você quiser testar como sua instância do Workfront se comportará após a atualização do Google Chrome, ajuste os sinalizadores no Chrome e ative as seguintes opções:

* &quot;Cookies SameSite por padrão&quot;
* &quot;Cookies sem SameSite devem ser seguros&quot;

## Sincronização de comentários do Workfront com o Jira

A integração do Workfront para Jira agora sincroniza seus comentários do Workfront com a sequência de comentários nativa do Jira.

Anteriormente, você podia sincronizar comentários do Jira com o Workfront, mas não do Workfront com o Jira.

Para obter mais informações, consulte [Configurar Adobe Workfront para Jira](../../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## O Otimizador de Portfolio de Flash foi removido

Removemos a capacidade de alternar entre o novo e o herdado (com base no Flash) Portfolio Otimizer do ambiente Workfront Classic para todos os clientes. O Otimizador de Portfolio herdado é um recurso obsoleto e as novas ferramentas fornecem a mesma funcionalidade hoje em dia.

Para obter informações sobre o otimizador de portfólio, consulte https://experience.workfront.com/s/article/Understanding-the-Portfolio-Optimizer-356650079

Para obter informações sobre como descontinuar as ferramentas baseadas no Flash no Workfront, consulte [Substituição de ferramentas baseadas em Flashes no Adobe Workfront](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).
