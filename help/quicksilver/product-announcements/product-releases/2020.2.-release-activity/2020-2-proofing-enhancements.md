---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: Aprimoramentos na revisão na 2020.2
description: Esta página descreve todas as melhorias de Prova feitas com a versão 2020.2 no ambiente de Produção. Essas melhorias foram disponibilizadas no ambiente de Produção na semana de 11 de maio de 2020.
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 021c6e0c-3593-40f7-8eeb-7e016001893e
TQID: https://experienceleague.adobe.com/Z86GWBBVdj1DPENzHS7wKI1ViRGFzov8L3sNtss4iJU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b18b693b-6d59-4359-95fd-a386b7a615fe
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 235
ht-degree: 2%

---

# Aprimoramentos na revisão na 2020.2

Esta página descreve todas as melhorias de Prova feitas com a versão 2020.2 no ambiente de Produção. Essas melhorias foram disponibilizadas no ambiente de Produção na semana de 11 de maio de 2020.

Para obter uma lista de todas as alterações disponíveis com a versão 2020.2, consulte a [visão geral da versão 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## O domínio de comprovação está sendo alterado de proofhq.com para workfront.com.

>[!NOTE]
>
>Esse recurso foi originalmente comunicado como parte da versão 2020.1, mas foi removido da versão antes de seu lançamento em produção.

Se o firewall ou servidor de email estiver configurado para permitir acesso somente a fornecedores específicos, você deverá adicionar o seguinte URL adicional ao incluo na lista de permissões para garantir que os usuários em sua organização possam exibir provas no Workfront tanto no visualizador de provas de navegador quanto no visualizador de provas de desktop:

&#42;.workfront.com

A URL &#42;proofhq.com também é necessária.

Para obter mais informações sobre como atualizar o incluo na lista de permissões, consulte [Configurar o incluo na lista de permissões do firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Essa atualização se aplica somente à revisão no Workfront; não se aplica ao usar o aplicativo independente do Workfront Proof.

## Comentários de revisão feitos por convidados aparecem na área Atualizações

Para simplificar a colaboração em provas, os comentários dos convidados aparecem na área Atualizações.

Anteriormente, os comentários de prova feitos pelos convidados estavam disponíveis somente na prova.
