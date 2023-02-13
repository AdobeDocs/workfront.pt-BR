---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Os administradores de grupo devem ter acesso mais alto do que aqueles que gerenciam
description: Se um administrador de grupo tiver permissões em seu Nível de acesso inferiores àquelas que ele gerencia, ele não poderá visualizar, modificar ou atribuir níveis de acesso mais baixos.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 458149110d71475820dc6f3b27f1e062c3fe66f6
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---


# Os administradores de grupo devem ter acesso mais alto do que aqueles que gerenciam

Se um administrador de grupo tiver permissões em seu Nível de acesso inferiores àquelas que ele gerencia, ele não poderá visualizar, modificar ou atribuir níveis de acesso mais baixos.

## Problema

Se um administrador de grupo receber um nível de acesso modificado do Planejador com permissões de Exibição para Equipes, mas determinados usuários receberem um nível de acesso do Trabalhador com permissões de Edição para Equipes, o administrador de grupo não poderá interagir com o nível de acesso do Trabalhador modificado.

![](assets/group-admin-modified-access.png)


>[!NOTE]
>
>Essa lógica também se aplica ao menu suspenso Ajustar configurações. Ambos os níveis de acesso podem ter acesso ao Editar, mas as configurações no menu suspenso Ajustar configurações devem ser mais altas para o administrador do grupo.
> ![](assets/fine-tune-your-settings.png)

## Solução

Os administradores de grupo devem ter permissões mais altas em todas as áreas no nível de acesso do que aquelas que gerenciam.