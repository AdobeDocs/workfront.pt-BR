---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Várias abas do navegador fazem com que o Workfront faça logout
description: Quando uma pessoa tem várias guias do navegador abertas, o Workfront pode fazer logout automaticamente.
feature: Get Started with Workfront
author: Becky
exl-id: 1cc8bf6c-0eda-41ef-8efd-bba3a5f33b08
TQID: 'https://experienceleague.adobe.com/Zof7zbTOm-w1vyBTchiXJv2QrNYbOxw9O4DYIjYQ6Ss'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: c042179c-157b-516d-b27c-e3bf303e8567
    internal-label: Get Started with Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 41%
---
# Várias abas do navegador fazem com que o Workfront faça logout

## Problema

Quando um usuário tem várias guias de navegador abertas e clica em uma guia que ficou inativa por algum tempo, a sessão da guia expirou. O usuário não pode ver a página que abrira e, em vez disso, vê a seguinte mensagem:

```
Tab session expired
This tab session has been halted due to inactivity. Refresh the tab to continue where you left off.
```

## Motivo

Esse comportamento é devido à Autenticação baseada em política (PBA), uma medida de segurança configurada pela sua organização. Quando uma guia fica inativa por mais tempo do que o limite definido na configuração PBA da organização, a sessão da guia expira.

## Solução

A solução depende de você ter estado ativo em outra guia que está conectada no Workfront.

* Se você tiver uma guia ativa do Workfront aberta, recarregue a guia expirada. Ele retornará à página que você abriu antes de expirar.

* Se você não tiver uma guia ativa do Workfront aberta, faça logon no Workfront novamente.
