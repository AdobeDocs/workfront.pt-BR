---
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Sincronização de usuários entre o Adobe Workfront e o Workfront Proof
description: As informações do usuário são sincronizadas do Adobe Workfront para o Workfront Proof; elas não são sincronizadas do Workfront Proof para o Workfront. Por esse motivo, sempre que você criar ou modificar usuários, deverá fazer essas alterações no Workfront. Não é possível fazer alterações em usuários no Workfront Proof.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 4c88a249-b156-45c9-a44c-32f906bfa8a2
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Sincronização do usuário entre o Adobe Workfront e o Workfront Proof

As informações do usuário são sincronizadas do Adobe Workfront para o Workfront Proof; elas não são sincronizadas do Workfront Proof para o Workfront. Por esse motivo, sempre que você criar ou modificar usuários, deverá fazer essas alterações no Workfront. Não é possível fazer alterações em usuários no Workfront Proof.

As seções a seguir fornecem informações sobre a sincronização de usuários do Workfront com o Workfront Proof:

## Informações sincronizadas

O Workfront sincroniza as seguintes informações do usuário com o Workfront Proof:

* Nome (nome e sobrenome do usuário)
* Endereço de email

## Quando a sincronização ocorrer

As informações do usuário são sincronizadas do Workfront para o Workfront Proof nas seguintes circunstâncias:

* As informações de um usuário são atualizadas no Workfront
* Um usuário é criado no Workfront

Dependendo de um usuário com o mesmo endereço de email existir no Workfront Proof, uma das situações a seguir ocorrerá:

* **Se não existir nenhum usuário com um email correspondente no Workfront Proof e**

   * **A revisão de texto está habilitada para o usuário:** O usuário foi criado como um usuário no Workfront Proof.
   * **A revisão de texto não está habilitada para o usuário:** O usuário foi criado como um Contato no Workfront Proof.

* **Se existir um usuário com um email correspondente no Workfront Proof:** A revisão está habilitada para esse usuário no Workfront (se ainda não tiver sido habilitada) e as informações são sincronizadas entre os dois usuários.

  Para obter mais informações, consulte [Configurar o acesso à prova de um usuário](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md) em [Configurar o acesso à prova de um usuário](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

  >[!IMPORTANT]
  >
  >Quando existe um usuário com um email correspondente, em si mesmo ou em outro ambiente de prova, o Workfront cria um endereço de email de alias adicionando a ID da conta do usuário como sufixo ao email. Por exemplo, *username+accountid@domain.com*. Os usuários ainda receberão notificações de prova caso um email de alias seja criado.
