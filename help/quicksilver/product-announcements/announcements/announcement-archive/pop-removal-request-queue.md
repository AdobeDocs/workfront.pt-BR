---
content-type: reference
navigation-topic: announcements
title: Novo sistema gerenciado pela Adobe Workfront para substituir o email POP em Filas de solicitações pela versão 21.1
description: Estamos substituindo a opção de email POP para filas de solicitações por um novo sistema gerenciado pela Adobe Workfront. Você ainda poderá enviar solicitações por email, mas precisará configurar um novo endereço de email gerenciado pela Workfront na área Fila de solicitações.
author: Luke
feature: Product Announcements
exl-id: d7147641-ba36-422b-a9b2-3c2f4ab609d8
source-git-commit: f05b462ff596ccc19215ca684802a9820a98211a
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# Novo sistema gerenciado pela Adobe Workfront para substituir o email POP em Filas de solicitações pela versão 21.1

Estamos substituindo a opção de email POP para filas de solicitações por um novo sistema gerenciado pela Adobe Workfront. Você ainda poderá enviar solicitações por email, mas precisará configurar um novo endereço de email gerenciado pela Workfront na área Fila de solicitações.

## Por que você está removendo a opção de email POP?

A tecnologia POP é uma opção de email não confiável e menos segura. Além disso, vemos muitos problemas do cliente relacionados especificamente ao email POP. Fazer a alteração em um sistema gerenciado pela Workfront resultará em uma experiência mais confiável.

## Que ação preciso executar?

Você precisa configurar um novo endereço de e-mail para cada fila de solicitações que tiver configurado com e-mail POP no ambiente de produção e distribuir o novo endereço de e-mail conforme necessário. Para obter mais informações, consulte [Habilitar usuários a enviar um problema por email para um projeto da Fila de Solicitações](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

## Qual é o plano de transição?

A partir da versão 21.1, no início de fevereiro, você terá 60 dias para fazer a transição dos usuários para o novo endereço de email *@intake.workfront.com* que criar. Durante o período de 60 dias, o email POP usado anteriormente continuará a funcionar.

## Como posso testar isso na Pré-visualização?

Para testar essa alteração na pré-visualização, é necessário habilitar os emails no ambiente de Pré-visualização. Para fazer isso, siga as instruções na seção Managing emails in preview em [Enable delivery of emails from the Preview Sandbox environment](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!IMPORTANT]
>
>O que você definir aqui não será transferido para o ambiente de Produção. Você precisará passar por esse processo novamente depois que a funcionalidade for lançada na produção.
