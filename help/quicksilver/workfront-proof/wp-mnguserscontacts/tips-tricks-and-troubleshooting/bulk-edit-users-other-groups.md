---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-users-and-contacts
title: Outros grupos do usuário de edição em massa
description: Ao editar em massa, tentei adicionar um único Outro grupo a vários usuários. Depois de Salvar as alterações, todos os Outros grupos existentes foram removidos e somente o novo Outro grupo permaneceu.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f2402830-3263-4204-ba8a-9028ef937577
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 0%

---

# Outros grupos do usuário de edição em massa

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

## Problema:

Ao editar em massa, tentei adicionar um único Outro grupo a vários usuários.
Depois de Salvar as alterações, todos os Outros grupos existentes foram removidos e somente o novo Outro grupo permaneceu.

## Resposta:

O comportamento resultante depende da associação de grupo atual dos usuários selecionados:

* Se todas as associações de Outros grupos dos usuários selecionados corresponderem exatamente...
Depois de selecionar os usuários e selecionar [!UICONTROL editar], o campo [!UICONTROL Outros grupos] mostrará a lista completa
de todos os grupos aos quais esses usuários pertencem.

* Se os usuários selecionados tiverem diferentes associações de Outro Grupo...
Após selecionar os usuários e clicar em [!UICONTROL Editar], o campo [!UICONTROL Outros grupos] ficará em branco.

Ao clicar em **[!UICONTROL Salvar alterações]**, tudo o que for exibido no campo Outros grupos será salvo.

O conteúdo anterior do campo é substituído.
