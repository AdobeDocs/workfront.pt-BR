---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: A decisão do aprovador mostra um hífen no relatório Aprovação de prova
description: Um hífen no campo Decisão do aprovador do relatório Aprovação de prova indica que um recipient não está mais em uma função de tomada de decisão na prova.
author: Courtney
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 25d403b9266c31a39c1dce6c1c45ad96ee90af28
workflow-type: tm+mt
source-wordcount: 287
ht-degree: 0%

---

# A decisão do aprovador mostra um hífen no relatório Aprovação de prova

## Problema

No relatório Aprovação de prova, o campo Decisão do aprovador de um recipient mostra um hífen (-), embora o campo Data da decisão mostre uma data e Aguardar decisão seja Falso.

![A decisão do aprovador mostra um hífen no relatório Aprovação de prova](assets/approver-decision-hyphen.png)

## Causa

Um hífen no campo Decisão do aprovador significa que o recipient não está mais em uma função de tomada de decisão na prova. Isso pode acontecer quando:

* O recipient foi adicionado à prova, tomou uma decisão e, posteriormente, foi removido do workflow. Se o recipient revisar a prova, o sistema de prova registrará a visita como uma alteração de decisão. Como o recipient não é mais um aprovador, o sistema registra a nova decisão como um hífen.
* A função de prova do destinatário foi alterada para uma que não inclui direitos de aprovação, como Revisor. Para obter informações sobre as ações que cada função pode realizar em uma prova, consulte [Visão geral das Funções de Prova](../../../review-and-approve-work/proofing/proofing-overview/proof-roles.md).
* O perfil de permissão de prova do recipient foi rebaixado após serem tomados a decisão.

## O que isso significa em seus relatórios

O hífen é intencional. Ele informa que o sistema não está aguardando o recipient aprovar a prova e que o recipient não tem mais uma função de tomada de decisão na prova.

O campo Data da decisão ainda mostra a data da atividade de decisão mais recente do recipient, mas a decisão do recipient não é mais contada no relatório.

Para obter informações sobre como criar e usar o relatório Aprovação de prova, consulte [Usar o relatório de aprovação de prova](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/proof-approval-report.md).
