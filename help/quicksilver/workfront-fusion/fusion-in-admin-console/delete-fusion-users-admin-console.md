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
source-wordcount: '288'
ht-degree: 0%

---

# Excluir usuários por meio da [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>A funcionalidade deste artigo só estará disponível se a instância de [!DNL Adobe Workfront Fusion] foi integrado na [!DNL Adobe Business Platform].
>
>Para obter uma lista de procedimentos que diferem com base no fato de sua organização ter sido integrada à [!DNL Adobe Business Platform], consulte [Diferenças de administração baseadas em plataforma ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../../workfront-fusion/fusion-in-admin-console/fusion-adobe-admin-console.md).

Você pode remover um usuário do [!DNL Adobe Workfront Fusion] apenas, deixando o acesso a qualquer outro [!DNL Adobe] perfis de produto, ou você pode remover o usuário do [!DNL Adobe Admin Console] completamente.

## Excluir um usuário no [!DNL Adobe Workfront Fusion]

Para excluir um usuário em [!DNL Adobe Workfront Fusion], você deve desativar o usuário por meio da variável [!DNL Adobe Admin Console].

Um usuário é desativado na variável [!DNL Adobe Admin Console] quando se aplicar uma das seguintes condições:

* O usuário é movido de um produto ou perfil de produto e não está atribuído a nenhum outro produto ou perfil de produto.
* O usuário é removido de um grupo vinculado a um perfil de produto e não está incluído em nenhum outro grupo vinculado a um perfil de produto.
* O usuário é removido de um perfil de produto e não está atribuído a outro perfil de produto.
* O usuário é excluído ou desativado na organização que inclui o Workfront Fusion.

  Para obter instruções, consulte a seção &quot;Remover usuários&quot; em [Gerenciar usuários individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html).

Entrada [!DNL Workfront Fusion], a desativação afeta o usuário de uma das seguintes maneiras:

* Se o usuário estiver em apenas uma organização, ele será desativado.
* Se o usuário estiver em mais de uma organização, ele será removido da organização em que foi modificado na [!DNL Adobe Admin Console].
* Por outras considerações, ao excluir um usuário no [!DNL Workfront Fusion], consulte [Considerações ao excluir um usuário no [!DNL Workfront Fusion]](../../workfront-fusion/organizations/manage-fusion-users.md#consider)
