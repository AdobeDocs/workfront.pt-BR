---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Várias guias do navegador fazem com que o Workfront faça logout
description: Quando uma pessoa tem várias guias do navegador abertas, o Workfront pode fazer logout automaticamente.
feature: Get Started with Workfront
source-git-commit: ef85b267b3417dddd0c9cc4a2b916b83dc416e14
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 7%

---

# Várias guias do navegador fazem com que o Workfront faça logout

>[!IMPORTANT]
>
>Esse problema está presente somente para organizações que foram integradas ao Adobe IMS.

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