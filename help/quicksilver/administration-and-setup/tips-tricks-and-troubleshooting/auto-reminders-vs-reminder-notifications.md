---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Lembretes automáticos vs. Notificações de lembrete
description: Este artigo descreve as diferenças entre lembretes automáticos e notificações de lembrete e fornece cenários para cada um.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 26c6fa2c-5c3a-4f53-bd7e-e49a623ff60d
TQID: https://experienceleague.adobe.com/hSVm-rgiBcbHaCwO1veCLEo-q6U5SWzt58qO6KqC84M
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 249
ht-degree: 3%

---

# Comparação entre lembretes automáticos e notificações de lembrete

Este artigo descreve as diferenças entre lembretes automáticos e notificações de lembrete e fornece cenários para cada um. Para obter mais informações sobre todas as [!DNL Adobe Workfront] notificações, consulte [[!DNL Adobe Workfront] notificações](../../workfront-basics/using-notifications/wf-notifications.md).

## Lembretes automáticos

As seguintes características são específicas para lembretes automáticos:

* Só pode ser ativado e editado por um administrador [!DNL Workfront]
* São acionados em todas as tarefas e problemas quando vencidos, atrasados ou próximos à data planejada de conclusão
* Só podem ser enviados ao responsável, ao gerente do responsável ou ao gerente imediato.
* Não é possível ter um modelo de email anexado a eles.

Cenário: se você quiser que lembretes sejam acionados em todas as tarefas e problemas no sistema, defina as configurações automáticas de lembrete. Para obter mais informações, consulte [Configurar lembretes automáticos](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

## Notificações de lembrete

As seguintes características são específicas para notificações de lembrete:

* Pode ser criado por um administrador ou qualquer usuário com uma licença Standard of Plan e acesso administrativo a Notificações de lembrete
* Só pode ser associado manualmente a um objeto
* Só é possível notificar sobre o objeto anexado
* Pode ser enviado para vários participantes do objeto, como proprietário, criador, aprovador ou destinatário
* Pode usar o email padrão ou usar um modelo de email personalizado anexado

Cenário: se você quiser criar lembretes para projetos, folhas de horas ou personalizar lembretes para tarefas e problemas, configure notificações de lembrete. Para obter mais informações, consulte [Configurar notificações de lembrete](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).
