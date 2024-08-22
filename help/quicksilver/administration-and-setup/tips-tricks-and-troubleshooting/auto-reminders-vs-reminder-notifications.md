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
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# Lembretes automáticos vs. notificações de lembrete

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

* Pode ser criado por um administrador ou qualquer usuário com uma licença de Plano e acesso administrativo a Notificações de lembrete
* Só pode ser associado manualmente a um objeto
* Só é possível notificar sobre o objeto anexado
* Pode ser enviado para vários participantes do objeto, como proprietário, criador, aprovador ou destinatário
* Pode usar o email padrão ou usar um modelo de email personalizado anexado

Cenário: se você quiser criar lembretes para projetos, folhas de horas ou personalizar lembretes para tarefas e problemas, configure notificações de lembrete. Para obter mais informações, consulte [Configurar notificações de lembrete](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).
