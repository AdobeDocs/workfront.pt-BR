---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: "Atividade da versão do Workfront Fusion: Semana de 3 de maio de 2021"
description: Esta página descreve todas as melhorias feitas no Adobe Workfront Fusion na semana de 3 de maio de 2021.
author: Luke
feature: Product Announcements, Workfront Fusion
exl-id: af3312c5-3416-4c03-8528-6a2c0240110e
hidefromtoc: true
source-git-commit: 9c2321794c5ba773bfda1d6e9dfda6b8de1a1449
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---

# Atividade de lançamento do Workfront Fusion: semana de 3 de maio de 2021

Esta página descreve todas as melhorias feitas no Adobe Workfront Fusion na semana de 3 de maio de 2021.

Para obter uma lista de todas as alterações recentes, consulte [Atividade de versão do Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Para obter uma lista de correções de erros recentes no Workfront Fusion, consulte o [Atualizações de manutenção do Workfront](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350) e verifique se há atualizações rotuladas como Atualização de manutenção do Workfront Fusion.

## O conector Salesforce agora pode pesquisar usando o SOQL

O módulo Salesforce > Search for records agora tem a opção de pesquisar usando o SOQL (Salesforce Object Query Language). Também é possível pesquisar usando as opções disponíveis anteriormente (SOSL e pesquisas simples).

Para obter mais informações, consulte [Módulos Salesforce](../../../workfront-fusion/apps-and-their-modules/salesforce-modules.md).

## O novo tipo de conexão no conector DevOps do Azure requer menos escopos

Para melhorar a segurança, adicionamos um novo tipo de conector ao Conector DevOps do Workfront Fusion Azure. Agora, ao criar uma conexão em um módulo DevOps do Azure, você pode selecionar de dois tipos de conexões:

* Azure DevOps

   Esse novo tipo de conexão limita escopos àqueles especificamente necessários para o Workfront Fusion.

* Azure DevOps (Solicitar todos os escopos)

   Este é o tipo de conexão herdada, que solicita todos os escopos disponíveis em uma conexão com o Azure DevOps.

Recomendamos que você use o tipo de conexão Azure DevOps em todos os novos cenários que usam o Azure DevOps. Recomendamos também que você altere os módulos do Azure DevOps em seus cenários existentes para usar o novo tipo de conexão. O tipo de conexão herdado Azure DevOps (Solicitar todos os escopos) será descontinuado em breve.

Para obter mais informações, consulte [Módulos do Azure DevOps](../../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md).
