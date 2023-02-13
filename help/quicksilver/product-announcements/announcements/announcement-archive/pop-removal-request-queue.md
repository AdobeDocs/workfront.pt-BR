---
content-type: reference
navigation-topic: announcements
title: Novo sistema gerenciado pela Adobe Workfront para substituir o email POP para filas de solicitações por 21.1
description: Estamos substituindo a opção de email POP para filas de solicitação por um novo sistema gerenciado pela Adobe Workfront. Você ainda poderá enviar solicitações por email, mas precisará configurar um novo endereço de email gerenciado pelo Workfront na área Fila de solicitações .
author: Luke
feature: Product Announcements
exl-id: d7147641-ba36-422b-a9b2-3c2f4ab609d8
source-git-commit: f05b462ff596ccc19215ca684802a9820a98211a
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# Novo sistema gerenciado pela Adobe Workfront para substituir o email POP para filas de solicitações por 21.1

Estamos substituindo a opção de email POP para filas de solicitação por um novo sistema gerenciado pela Adobe Workfront. Você ainda poderá enviar solicitações por email, mas precisará configurar um novo endereço de email gerenciado pelo Workfront na área Fila de solicitações .

## Por que você está removendo a opção de email POP?

A tecnologia POP é uma opção de email não confiável e menos segura. Além disso, vemos muitos problemas do cliente relacionados especificamente ao email POP. Fazer a alteração em um sistema gerenciado pela Workfront resultará em uma experiência mais confiável.

## Que ação preciso tomar?

Você precisa configurar um novo endereço de email para cada fila de solicitações que tenha configurado com o email POP no ambiente Produção e distribuir o novo endereço de email conforme necessário. Para obter mais informações, consulte [Permitir que os usuários enviem um problema por email para um projeto da Fila de solicitações](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

## Qual é o plano de transição?

A partir do lançamento da versão 21.1 no começo de fevereiro, você terá 60 dias para migrar os usuários para o novo *@AM.workfront.com* endereço de email que você criar. Durante o período de 60 dias, o email POP usado anteriormente continuará funcionando.

## Como posso testar isso na Visualização?

Para testar essa alteração na visualização, você precisa ativar emails no ambiente de visualização. Para fazer isso, siga as instruções na seção Managing emails in preview em [Ativar a entrega de emails do ambiente Preview Sandbox](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!IMPORTANT]
>
>O que você definir aqui não será transferido para seu ambiente de produção. Você precisará passar por esse processo novamente depois que a funcionalidade for lançada para produção.
