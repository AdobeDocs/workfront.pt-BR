---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: Outros aprimoramentos na 2020.1
description: Esta página descreve todas as melhorias feitas nas áreas gerais do Workfront com a versão 2020.1. Esses aprimoramentos estão disponíveis atualmente no ambiente de Pré-visualização e serão disponibilizados no ambiente Produção no final de março ou início de abril de 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a716590c-c833-458a-a138-9bc0723e5896
TQID: https://experienceleague.adobe.com/I5djuVv0ixHspF6afQaa5-jTkl0uXl26VlKf8BXqhO4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: b8ea32d4-f1fe-4c71-8871-afe5a702a009
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 433
ht-degree: 1%

---

# Outros aprimoramentos na 2020.1

Esta página descreve todas as melhorias feitas nas áreas gerais do Workfront com a versão 2020.1. Esses aprimoramentos estão disponíveis atualmente no ambiente de Pré-visualização e serão disponibilizados no ambiente Produção no final de março ou início de abril de 2020.

Para obter uma lista de todas as alterações disponíveis com a versão 2020.1, consulte a [visão geral da versão 2020.1](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md).

## Alteração necessária para adicionar provas ao incluo na lista de permissões

>[!NOTE]
>
>Este recurso foi removido da versão 2020.1. Ele será disponibilizado posteriormente.

O domínio de comprovação está alterando from proofhq.com para workfront.com.

Se o firewall ou servidor de email estiver configurado para permitir acesso somente a fornecedores específicos, você deverá adicionar o seguinte URL adicional ao incluo na lista de permissões para garantir que os usuários em sua organização possam exibir provas no Workfront tanto no visualizador de provas de navegador quanto no visualizador de provas de desktop:

&#42;.workfront.com

A URL &#42;proofhq.com também é necessária.

Para obter mais informações sobre como atualizar o incluo na lista de permissões, consulte [Configurar o incluo na lista de permissões do firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

>[!NOTE]
>
>Essa atualização se aplica somente à revisão no Workfront; não se aplica ao usar o aplicativo independente do Workfront Proof.

## Comportamento de cookie do Workfront atualizado para manter a compatibilidade com o Chrome

Para manter a compatibilidade com uma atualização futura do Google Chrome (Chrome v80), atualizamos a plataforma do Workfront para garantir que os cookies sejam enviados adequadamente com as solicitações.

Essa atualização do Chrome altera o valor padrão do atributo de cookie SameSite. Se quiser testar como sua instância do Workfront se comportará após a atualização do Google Chrome, ajuste os sinalizadores no Chrome e ative as seguintes opções:

* &quot;Cookies SameSite por padrão&quot;
* &quot;Cookies sem SameSite devem ser seguros&quot;

## Sincronização de comentários do Workfront com o Jira

A integração do Workfront para Jira agora sincroniza seus comentários do Workfront com a sequência de comentários nativa do Jira.

Anteriormente, você podia sincronizar comentários do Jira com o Workfront, mas não do Workfront com o Jira.

Para obter mais informações, consulte [Configurar Adobe Workfront para Jira](../../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## O Flash Portfolio Otimizer foi removido

Removemos a capacidade de alternar entre o novo e o herdado (com base no Flash) Portfolio Otimizer do ambiente Workfront Classic para todos os clientes. O Portfolio Otimizer herdado é um recurso obsoleto e as novas ferramentas fornecem a mesma funcionalidade hoje em dia.

Para obter informações sobre o otimizador de portfólio, consulte https://experience.workfront.com/s/article/Understanding-the-Portfolio-Optimizer-356650079

Para obter informações sobre como descontinuar as ferramentas baseadas em Flash no Workfront, consulte [Substituição de ferramentas baseadas em Flash no Adobe Workfront](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).
