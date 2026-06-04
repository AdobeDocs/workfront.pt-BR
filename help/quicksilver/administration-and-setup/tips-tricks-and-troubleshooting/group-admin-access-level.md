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
TQID: https://experienceleague.adobe.com/uxZXjgW85JgdyPJA5UEEfIvwU41hLWE-B3XLDh6D89w
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 157
ht-degree: 7%

---

# Admins de grupo devem ter um acesso superior aos usuários que gerenciam

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
