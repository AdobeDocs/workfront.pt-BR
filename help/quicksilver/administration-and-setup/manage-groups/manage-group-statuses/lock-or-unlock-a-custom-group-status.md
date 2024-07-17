---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Status de grupos bloqueados e desbloqueados
description: Bloquear os status personalizados de um grupo é uma maneira de garantir que as pessoas no grupo e em seus subgrupos estejam usando os mesmos processos em seu fluxo de trabalho. Quando um status de grupo é bloqueado, ele fica disponível para todos os usuários no grupo e nos grupos inferiores. Embora você (ou um administrador do Workfront) possa editar ou excluir um status bloqueado, os administradores de subgrupos abaixo não podem fazer isso para esses grupos. Por outro lado, desbloquear os status personalizados de um grupo permite que os administradores de subgrupos mais baixos tenham mais flexibilidade para gerenciar seus workflows. Eles podem alterar os atributos de um status desbloqueado ou excluí-lo de seus grupos.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3463e4cb-7336-49b7-b81a-c2acef72f61d
source-git-commit: d67de32fcbe4706cf8a1fc6f5bb8ec9d08b07119
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# Status de grupos bloqueados e desbloqueados

Bloquear os status personalizados de um grupo é uma maneira de garantir que as pessoas no grupo e em seus subgrupos estejam usando os mesmos processos em seu fluxo de trabalho. Quando um status de grupo é bloqueado, ele fica disponível para todos os usuários no grupo e nos grupos inferiores. Embora você (ou um administrador do Workfront) possa editar ou excluir um status bloqueado, os administradores de subgrupos abaixo não podem fazer isso para esses grupos; eles podem alterar apenas sua ordem de exibição na lista Status.

Por outro lado, desbloquear os status personalizados de um grupo permite que os administradores de subgrupos mais baixos tenham mais flexibilidade para gerenciar os workflows exclusivos usados em seus grupos. Quando um status de grupo é desbloqueado, os administradores de subgrupos inferiores podem alterar seus atributos ou excluí-los desses subgrupos.

>[!IMPORTANT]
>
>Se você bloquear um status personalizado depois de desbloqueado por qualquer período, as configurações do status substituirão as feitas pelos administradores de grupo nos subgrupos inferiores. Enquanto o status é bloqueado, esses administradores não podem modificar ou excluir o status de seus grupos.

Para obter instruções sobre como bloquear ou desbloquear um status de grupo, consulte [Criar ou editar um status de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Você pode usar os status bloqueado e desbloqueado em um processo de aprovação de grupo. Se você criar um processo de aprovação de grupo com um status de grupo desbloqueado, os usuários poderão anexar o processo de aprovação a qualquer projeto, tarefa ou problema associado ao grupo.

