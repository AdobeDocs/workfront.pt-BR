---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Administradores De Grupos Devem Ter Acesso Maior Do Que Aqueles Que Gerenciam
description: Se um administrador de grupo tiver permissões em seus níveis de acesso inferiores àqueles que gerencia, ele não poderá visualizar, modificar ou atribuir níveis de acesso inferiores.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2b501a1e-fb56-44fa-8518-07537dc90a5b
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 0%

---

# Administradores de grupo devem ter um acesso maior do que aqueles que eles gerenciam

Se um administrador de grupo tiver permissões em seus níveis de acesso inferiores àqueles que gerencia, ele não poderá visualizar, modificar ou atribuir níveis de acesso inferiores.

## Problema

Se um administrador de grupo receber um nível de acesso de Planejador modificado com permissões de Exibição para Equipes, mas determinados usuários receberem um nível de acesso de Trabalhador com permissões de Edição para Equipes, o administrador de grupo não poderá interagir com o nível de acesso de Trabalhador modificado.

![Acesso modificado pelo administrador de grupo](assets/group-admin-modified-access.png)


>[!NOTE]
>
>Essa lógica também se aplica ao menu suspenso Ajustar as configurações. Ambos os níveis de acesso podem ter acesso para Editar, mas as configurações no menu suspenso Ajustar suas configurações devem ser maiores para o administrador de grupo.
> ![Ajuste as configurações](assets/fine-tune-your-settings.png)

## Solução

Os administradores de grupo devem ter permissões mais altas em todas as áreas no nível de acesso do que aqueles que eles gerenciam.
