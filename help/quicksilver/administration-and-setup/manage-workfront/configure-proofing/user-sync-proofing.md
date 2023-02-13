---
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Sincronização de usuários entre o Adobe Workfront e a Workfront Proof
description: As informações do usuário são sincronizadas do Adobe Workfront para o Workfront Proof; ela não é sincronizada do Workfront Proof para o Workfront. Por causa disso, sempre que você criar ou modificar usuários, deverá fazer essas alterações no Workfront. Não é possível fazer alterações nos usuários na Workfront Proof.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 4c88a249-b156-45c9-a44c-32f906bfa8a2
source-git-commit: b310e36c9eb148db631e7a3552a35dcccc652d60
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Sincronização de usuários entre o Adobe Workfront e a Workfront Proof

As informações do usuário são sincronizadas do Adobe Workfront para o Workfront Proof; ela não é sincronizada do Workfront Proof para o Workfront. Por causa disso, sempre que você criar ou modificar usuários, deverá fazer essas alterações no Workfront. Não é possível fazer alterações nos usuários na Workfront Proof.

As seções a seguir fornecem informações sobre a sincronização de usuários do Workfront para o Workfront Proof:

## Informações sincronizadas

O Workfront sincroniza as seguintes informações do usuário na Workfront Proof:

* Nome (o nome e sobrenome do usuário)
* Endereço de email

## Quando a sincronização ocorre

As informações do usuário são sincronizadas do Workfront para o Workfront Proof nas seguintes circunstâncias:

* As informações de um usuário são atualizadas no Workfront
* Um usuário é criado no Workfront

Dependendo de um usuário com o mesmo endereço de email existir no Workfront Proof, uma das seguintes situações ocorrerá:

* **Se nenhum usuário com um email correspondente existir na Workfront Proof e**

   * **A revisão de texto está ativada para o usuário:** O usuário é criado como um usuário na Workfront Proof.
   * **A revisão de texto não está ativada para o usuário:** O usuário é criado como um Contato na Workfront Proof.

* **Se um usuário com um email correspondente existir na Workfront Proof:** A revisão de texto está ativada para esse usuário no Workfront (se ainda não estiver ativada) e as informações são sincronizadas entre os dois usuários.

   Para obter mais informações, consulte [Configurar o acesso à prova de um usuário](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md) em [Configurar o acesso à prova de um usuário](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

   >[!IMPORTANT]
   >
   >Quando um usuário com um email correspondente existe, em seu próprio ou em outro ambiente de prova, o Workfront cria um endereço de email de alias adicionando a ID da conta do usuário como um sufixo ao email. Por exemplo, *username+accountid@domain.com*. Os usuários ainda receberão notificações de prova no caso de um email alias ser criado.
