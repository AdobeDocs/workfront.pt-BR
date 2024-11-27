---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: As configurações do ZScaler podem causar redução no desempenho
description: Após a criação do usuário, você pode editar o usuário e habilitar "Permitir apenas a autenticação SAML 2.0" para que o usuário e a senha sejam controlados pelo sistema SAML. Com essa opção ativada, o usuário só tem permissão para fazer logon via SAML.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 2752a9e2-44fe-49b5-a7ab-4021d91ed37b
source-git-commit: f66b219e9fd203f108844ad397bcfa848b8f1134
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Workfront: as configurações do ZScaler podem causar redução no desempenho

>[!NOTE]
>
>Esse é um problema com o ZScaler e não será corrigido pelo Workfront.

O serviço Web do ZScaler usa `http/1.1` por padrão, o que pode causar redução de desempenho no Workfront.

Para verificar e resolver esse problema, configure seu software ZScaler para usar o `http/2`. Isso não pode ser configurado no Workfront.

Você pode encontrar informações sobre `http/2` na documentação do ZScaler.
