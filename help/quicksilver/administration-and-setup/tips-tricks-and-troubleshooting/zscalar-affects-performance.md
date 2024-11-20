---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Configurações de ZScalar podem causar redução no desempenho
description: Após a criação do usuário, você pode editar o usuário e habilitar "Permitir apenas a autenticação SAML 2.0" para que o usuário e a senha sejam controlados pelo sistema SAML. Com essa opção ativada, o usuário só tem permissão para fazer logon via SAML.
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: 806a4c4835e47da4fbbdb28ec0c35c990f70239e
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Workfront: configurações de ZScalar podem causar redução no desempenho

>[!NOTE]
>
>Esse é um problema com ZScalar e não será corrigido pelo Workfront.

O serviço Web de ZScalar usa `http/1.1` por padrão, o que pode causar redução no desempenho do Workfront.

Para verificar e resolver esse problema, configure seu software ZScalar para usar o `http/2`. Isso não pode ser configurado no Workfront.

Você pode encontrar informações sobre `http/2` na documentação ZScalar.
