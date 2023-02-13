---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Lembretes automáticos e notificações de lembrete
description: Este artigo descreve as diferenças entre lembretes automáticos e notificações de lembrete e fornece cenários para cada um. Para obter mais informações sobre todos [!DNL Adobe Workfront] notificações, consulte Adobe [!DNL Workfront] notificações.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 26c6fa2c-5c3a-4f53-bd7e-e49a623ff60d
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# Lembretes automáticos e notificações de lembrete

Este artigo descreve as diferenças entre lembretes automáticos e notificações de lembrete e fornece cenários para cada um. Para obter mais informações sobre todos [!DNL Adobe Workfront] notificações, consulte [[!DNL Adobe Workfront] notificações](../../workfront-basics/using-notifications/wf-notifications.md).

## Lembretes automáticos

As seguintes características são específicas dos lembretes automáticos:

* Só pode ser ativado e editado por um [!DNL Workfront] administrador
* São acionadas em todas as tarefas e problemas quando estão vencidas, atrasadas ou perto da data de conclusão planejada
* Só podem ser enviadas para o destinatário, o gerente do destinatário ou o gerente do gerente imediato.
* Não é possível ter um modelo de email anexado a eles.

Cenário: Se quiser que os lembretes sejam acionados em todas as tarefas e problemas em todo o sistema, configure as configurações de lembrete automático. Para obter mais informações, consulte [Configurar lembretes automáticos](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

## Notificações de lembrete

As seguintes características são específicas para notificações de lembrete:

* Pode ser criado por um administrador ou qualquer usuário com uma licença do Plano e acesso administrativo às Notificações do Lembrete
* Só pode ser associado manualmente a um objeto
* Só é possível notificar em relação ao objeto anexado
* Pode ser enviado para vários participantes do objeto, como proprietário, criador, aprovador ou destinatário
* Pode usar o email padrão ou usar um modelo de email personalizado anexado

Cenário: Se quiser criar lembretes para projetos, folhas de ponto ou quiser personalizar lembretes para tarefas e problemas, configure as notificações de lembrete. Para obter mais informações, consulte [Configurar notificações de lembrete](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).
