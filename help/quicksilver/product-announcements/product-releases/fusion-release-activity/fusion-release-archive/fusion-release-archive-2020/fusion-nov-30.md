---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
keywords: fusão
navigation-topic: fusion-release-activity
title: "Atividade da versão do Workfront Fusion: Semana de 30 de novembro de 2020"
description: Esta página descreve todas as melhorias feitas no Adobe Workfront Fusion na semana de 30 de novembro de 2020.
author: Luke
feature: Product Announcements, Workfront Fusion
exl-id: 9621683b-735d-40a6-8d7c-b5bd167cbdd2
hidefromtoc: true
source-git-commit: e18b23e7d58aced4c95c5df51769a6e959fa3d57
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---

# Atividade de lançamento do Workfront Fusion: semana de 30 de novembro de 2020

Esta página descreve todas as melhorias feitas no Adobe Workfront Fusion na semana de 30 de novembro de 2020.

Para obter uma lista de todas as alterações recentes, consulte [Atividade de versão do Adobe Workfront Fusion](../../../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Para obter uma lista de correções de erros recentes no Workfront Fusion, consulte o [Atualizações de manutenção do Workfront](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350) e verifique se há atualizações rotuladas como Atualização de manutenção do Workfront Fusion.

## Limite de taxa para webhooks do Workfront Fusion 2.0.

Introduzimos uma nova garantia de desempenho para o Workfront Fusion 2.0. Agora, os webhooks têm um limite de taxa de 100 solicitações por segundo. Quando esse limite é atingido, o Workfront Fusion 2.0 envia um status 429 (Muitas solicitações).

Anteriormente, as solicitações de webhook não eram limitadas.

Para obter mais informações, consulte [Medidas de proteção de desempenho do Adobe Workfront Fusion](../../../../../workfront-fusion/get-started/fusion-performance-guardrails.md).

## Adicionar um formulário personalizado a um objeto do Workfront no Workfront Fusion 2.0

Para permitir que você adicione formulários personalizados a objetos é o Workfront Fusion 2.0, adicionamos uma ação AssignCategories à Workfront > Misc. Módulo de ação.

Anteriormente, não era possível usar um módulo do Workfront Fusion 2.0 para adicionar um formulário personalizado a um objeto no Workfront.

Para obter mais informações sobre Workfront > Misc. Módulo de ação, consulte [Módulos Adobe Workfront](../../../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Jira Server connector and modules now available</h2>
<p>We've added a Jira Server connector to Workfront Fusion. The Jira Server connector offers the same functionality as the current Jira Cloud connector. </p>
<p>With Jira Server modules, you can:</p>
<ul>
<li> <p>Trigger a scenario when a record is added, modified, or deleted</p> </li>
<li> <p>Create, read, update, or delete a record</p> </li>
<li> <p>List or search records</p> </li>
<li> <p>Download an attachment</p> </li>
<li> <p>Add an issue to a sprint</p> </li>
<li> <p>Make a custom API call</p> </li>
</ul>
<p>Previously, Jira modules were available only for Jira Cloud.</p>
<p>For more information on available Jira modules, see <a href="../../../../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref" xrefformat="{para}">Jira Software modules</a>.</p>
<h2>Azure DevOps connector and modules now available</h2>
<p>You can now use Workfront Fusion to connect to your Azure DevOps applications. With the Azure DevOps modules, you can:</p>
<ul>
<li> <p>Trigger a scenario when a record is added, updated, or deleted.</p> </li>
<li> <p>Create or update records.</p> </li>
<li> <p>Get data from existing records.</p> </li>
<li> <p>Download or upload attachments.</p> </li>
<li> <p>Link work items together.</p> </li>
<li> <p>Retrieve a list of work items.</p> </li>
<li> <p>Perform a custom API call.</p> </li>
</ul>
<p>For more information see <a href="../../../../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md" class="MCXref xref" xrefformat="{para}">Azure DevOps modules</a>.</p>
<h2>Microsoft Dynamics 365 connector and modules now available</h2>
<p>You can now use Workfront Fusion to connect to your Microsoft Dynamics 365 account. With the Microsoft Dynamics 365 modules, you can:</p>
<ul>
<li> <p>Trigger a scenario when records are added or updated in Microsoft Dynamics 365</p> </li>
<li> <p>Create, read, update, or delete a Microsoft Dynamics 365record</p> </li>
<li> <p>Perform a custom API call</p> </li>
</ul>
<p>For information about available Microsoft Dynamics 365 modules, see <a href="../../../../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md" class="MCXref xref" xrefformat="{para}">Microsoft Dynamics 365 modules</a>.</p>
</div>
-->
