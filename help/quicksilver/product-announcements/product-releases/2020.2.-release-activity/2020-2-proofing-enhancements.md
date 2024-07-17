---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: Aprimoramentos de revisão 2020.2
description: Esta página descreve todas as melhorias de Prova feitas com a versão 2020.2 no ambiente de Produção. Essas melhorias foram disponibilizadas no ambiente de Produção na semana de 11 de maio de 2020.
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 021c6e0c-3593-40f7-8eeb-7e016001893e
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 0%

---

# Aprimoramentos de revisão 2020.2

Esta página descreve todas as melhorias de Prova feitas com a versão 2020.2 no ambiente de Produção. Essas melhorias foram disponibilizadas no ambiente de Produção na semana de 11 de maio de 2020.

Para obter uma lista de todas as alterações disponíveis com a versão 2020.2, consulte a [visão geral da versão 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## O domínio de comprovação está sendo alterado de proofhq.com para workfront.com.

>[!NOTE]
>
>Esse recurso foi originalmente comunicado como parte da versão 2020.1, mas foi removido da versão antes de seu lançamento em produção.

Se o firewall ou servidor de email estiver configurado para permitir acesso apenas a fornecedores específicos, você deverá adicionar o seguinte URL adicional ao seu arquivo de inclui na lista de permissões para garantir que os usuários em sua organização possam exibir provas no Workfront tanto no visualizador de prova de navegador quanto no visualizador de prova de desktop:

&#42;.workfront.com

A URL &#42;proofhq.com também é necessária.

Incluir na lista de permissões incluir na lista de permissões Para obter mais informações sobre como atualizar a pesquisa do firewall, consulte [Configurar a pesquisa do firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Essa atualização se aplica somente à revisão no Workfront; não se aplica ao usar o aplicativo independente do Workfront Proof.

## Comentários de revisão feitos por convidados aparecem na área Atualizações

Para simplificar a colaboração em provas, os comentários dos convidados aparecem na área Atualizações.

Anteriormente, os comentários de prova feitos pelos convidados estavam disponíveis somente na prova.
