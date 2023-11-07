---
content-type: api
product-area: user-management
navigation-topic: general-api
title: Desativar um usuário por meio da API
description: Desativar um usuário por meio da API
author: Becky
feature: Workfront API
role: Developer
exl-id: 45b06cce-4622-4739-b9f3-2edb9101c099
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---


# Desativar um usuário por meio da API

Quando um usuário deixa a organização, você pode desativá-lo, disponibilizando sua licença do Adobe Workfront para outro usuário e evitando que seja atribuído um trabalho inadvertidamente. Ao desativar um usuário, você preserva seu histórico de trabalho, incluindo suas atribuições de trabalho e sua associação com notas, horas e documentos.

Para saber mais sobre como desativar um usuário, consulte &quot; [Desativar ou reativar um usuário](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

Para obter informações sobre como usar a API principal, consulte [Noções básicas sobre API](../../wf-api/general/api-basics.md).

Para desativar um usuário por meio da API:

1. Gere uma chave de API usando a seguinte solicitação de API:

```
<domain>.my.workfront.com/attask/api/v15.0/user?action=generateApiKey&username=`username`&password=`password`&method=PUT`
```

1. Localize o GUID do usuário que deseja desativar.

   1. Use a solicitação de API a seguir para recuperar o GUID para todos os usuários em seu sistema. Observe que **isActive** mostra o campo **true** para usuários que estão ativos no momento e **false** para usuários que foram desativados:

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/search?fields=isActive
```

1. Localize o GUID do usuário que deseja desativar, use o seguinte **PUT** solicitação para alterar o **isActive** valor do campo para **false**:

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/`<user's GUID>`?updates={"isActive":"false"}&method=put&apiKey=`<apiKey>`&fields=isActive
```

1. A resposta demonstrará que a **isActive** o valor do campo foi alterado de **true** para **false** indicando que o usuário foi desativado:

<!-- [Copy](javascript:void(0);) -->
<pre><code>{<br>&nbsp;&nbsp;&nbsp;&nbsp;data:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ID:&nbsp;"592125e60089b88fae8b51c08383e144",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;name:&nbsp;"Tyler Reid",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;objCode:&nbsp;"USER",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;isActive:&nbsp;false&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>}<br></code></pre>
