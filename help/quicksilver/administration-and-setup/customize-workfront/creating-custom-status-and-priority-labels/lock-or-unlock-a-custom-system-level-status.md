---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Status de nível de sistema bloqueados e desbloqueados
description: Bloquear os status personalizados é uma maneira de garantir que as pessoas em toda a organização estejam usando os mesmos processos em seu fluxo de trabalho. Quando um status é bloqueado, ele fica disponível para todos os usuários no sistema. Embora você possa editá-lo ou excluí-lo, os administradores de grupo não podem fazer isso para seus grupos. Por outro lado, desbloquear status personalizados permite que os administradores de grupo tenham mais flexibilidade para gerenciar os fluxos de trabalho exclusivos usados em seus grupos. Eles podem alterar os atributos de um status desbloqueado ou excluí-lo de seus grupos.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0e58a1d6-5e0c-4445-a5ac-400dfd4c4948
source-git-commit: c70a10a920d32ad00a2e833b331c92a598902d21
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Status de nível de sistema bloqueados e desbloqueados

Bloquear os status personalizados é uma maneira de garantir que as pessoas em toda a organização estejam usando os mesmos processos em seu fluxo de trabalho. Quando um status é bloqueado, ele fica disponível para todos os usuários no sistema. Embora seja possível editar ou excluir um status bloqueado, os administradores de grupo não podem fazer isso para seus grupos; eles podem alterar somente sua ordem de exibição na lista Status.

Por outro lado, desbloquear status personalizados permite que os administradores de grupo tenham mais flexibilidade para gerenciar os fluxos de trabalho exclusivos usados em seus grupos. Quando um status é desbloqueado, os administradores de grupo podem alterar seus atributos ou excluí-lo de seus grupos.

>[!IMPORTANT]
>
>Se você bloquear um status personalizado após ele ter sido desbloqueado por qualquer período de tempo, as configurações do sistema para o status substituirão as feitas pelos administradores do grupo. Enquanto o status estiver bloqueado, os administradores de grupo não poderão modificar ou excluir o status de seus grupos.

Para obter instruções sobre como bloquear ou desbloquear um status de nível de sistema, consulte [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Status desbloqueados em processos de aprovação

Você pode usar os status bloqueado e desbloqueado em um processo de aprovação do sistema. Se você criar um processo de aprovação do sistema com um status de sistema desbloqueado, os usuários em todo o sistema poderão anexar o processo de aprovação a qualquer projeto, tarefa ou problema no sistema.

As mensagens de aviso são exibidas nos seguintes cenários para ajudar você e seus usuários a entender os resultados dos seguintes cenários:

* Um administrador desbloqueia um status de nível de sistema usado em um processo de aprovação. Uma mensagem avisa que pode excluir o status desbloqueado de seus grupos, o que impediria que os membros do grupo usassem esse processo de aprovação corretamente para objetos atribuídos ao grupo.

* Um usuário começa a editar um processo de aprovação que usa um status desbloqueado. Uma mensagem alerta o usuário sobre o status desbloqueado para que ele possa avaliar se seria uma boa ideia rebloqueá-lo ou substituí-lo.

* Um processo de aprovação no nível do sistema com um status desbloqueado é anexado em um objeto e o status foi excluído para o grupo atribuído ao objeto. Quando um membro do grupo vai para a seção Aprovações do objeto, uma mensagem explica que o processo de aprovação não pode ser iniciado para o objeto.

Você pode usar os status bloqueado e desbloqueado em um processo de aprovação de grupo. Se você criar um processo de aprovação de grupo com um status de grupo desbloqueado, os usuários poderão anexar o processo de aprovação a qualquer projeto, tarefa ou problema associado ao grupo.