---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Excluir usuários por meio da Adobe Admin Console
description: Você pode remover um usuário somente do Adobe Workfront Fusion, deixando acesso a qualquer outro perfil de produto do Adobe, ou pode remover o usuário totalmente do Adobe Admin Console.
author: Becky
feature: Workfront Fusion
exl-id: 0d989134-46c0-4637-b465-6fbe04258b8a
source-git-commit: 392eee3c7b1aacf92d7877f07a8154924f3926a0
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# Excluir usuários por meio do [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>A funcionalidade deste artigo só estará disponível se a instância de [!DNL Adobe Workfront Fusion] da sua organização tiver sido integrada ao [!DNL Adobe Business Platform].
>
>Para obter uma lista de procedimentos que diferem se sua organização foi integrada ao [!DNL Adobe Business Platform], consulte [Diferenças de administração baseadas em plataforma ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../../workfront-fusion/fusion-in-admin-console/fusion-adobe-admin-console.md).

Você pode remover um usuário somente do [!DNL Adobe Workfront Fusion], deixando acesso a qualquer outro perfil de produto do [!DNL Adobe], ou pode remover o usuário totalmente do [!DNL Adobe Admin Console].

## Excluir um usuário em [!DNL Adobe Workfront Fusion]

Para excluir um usuário em [!DNL Adobe Workfront Fusion], você deve desativá-lo por meio de [!DNL Adobe Admin Console].

Um usuário é desativado de [!DNL Adobe Admin Console] quando uma das seguintes situações se aplicar:

* O usuário é movido de um produto ou perfil de produto e não está atribuído a nenhum outro produto ou perfil de produto.
* O usuário é removido de um grupo vinculado a um perfil de produto e não está incluído em nenhum outro grupo vinculado a um perfil de produto.
* O usuário é removido de um perfil de produto e não está atribuído a outro perfil de produto.
* O usuário é excluído ou desativado na organização que inclui o Workfront Fusion.

  Para obter instruções, consulte a seção &quot;Remover usuários&quot; em [Gerenciar usuários individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html).

No [!DNL Workfront Fusion], a desativação afeta o usuário de uma das seguintes maneiras:

* Se o usuário estiver em apenas uma organização, ele será desativado.
* Se o usuário estiver em mais de uma organização, ele será removido da organização em que o usuário foi modificado no [!DNL Adobe Admin Console].
* Para outras considerações ao excluir um usuário em [!DNL Workfront Fusion], consulte [Considerações ao excluir um usuário em [!DNL Workfront Fusion]](../../workfront-fusion/organizations/manage-fusion-users.md#consider)
