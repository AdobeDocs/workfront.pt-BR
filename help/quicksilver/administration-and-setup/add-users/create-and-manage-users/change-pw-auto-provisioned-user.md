---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Alterar a senha de um usuário provisionado automaticamente
description: Geralmente, quando um novo usuário tenta alterar sua senha temporária, ele digita seu endereço de email e recebe um erro para um nome de usuário incorreto. Eles devem inserir o nome de usuário atribuído pelo sistema, que é o GUID (Identificador Exclusivo Global). Como é difícil lembrar e usar um GUID, recomendamos que você altere o nome de usuário de um novo usuário para o endereço de email do Workfront e, em seguida, permita que ele altere a senha.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 14124911-e5e1-4a4f-9b25-8b4fab0329e1
source-git-commit: 7bd3d2252b124a07a112aaa2b7798063087e7cab
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# Alterar a senha de um usuário provisionado automaticamente

Ao criar usuários por meio do provisionamento automático, a Adobe Workfront atribui a eles um GUID (Identificador exclusivo global) para um nome de usuário. Um GUID é uma string exclusiva de números e letras aleatórios, por exemplo, *5489cb430012526e1ea635e8c29f377f*.

Geralmente, quando um novo usuário tenta alterar sua senha temporária, ele digita seu endereço de email para o nome de usuário e recebe um erro para um nome de usuário incorreto. Para que o usuário altere sua senha, ele deve digitar o nome de usuário atribuído pelo sistema, que é um GUID.

Como os nomes de usuário do GUID podem ser difíceis de usar, recomendamos que você altere primeiro o nome de usuário para seu endereço de email do Workfront e, em seguida, permita que ele altere sua senha.

>[!TIP]
>
>Você pode encontrar o GUID de um usuário das seguintes maneiras:
>
>* Vá para o perfil do usuário e copie o GUID do URL no navegador.
>
>  Por exemplo, no URL `https://acme.workfront.com/user/61941ab1000af22d7104628efa1c738b/details`, você copiaria a string de números e letras entre as duas últimas barras: `61941ab1000af22d7104628efa1c738b`.
>
>  Para obter mais informações, consulte [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
>
>* Crie um relatório de usuário com uma coluna Usuário > GUID . Para obter mais informações, consulte [Criar um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).
>
>* Consulte a API do Workfront.
>


## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Alterar a senha de um usuário provisionado automaticamente

1. Determine o nome de usuário do GUID de usuário transmitindo uma solicitação de API, como mostrado no exemplo a seguir:

   https://`<domain>`.my.workfront.com/attask/api/v14.0/USER/search?fields=username&amp;ID=`<ID of User>` Onde *`<domain>`* é o domínio de sua empresa e *`<ID of User>`* é a Workfront ID do usuário.

   Você recebe uma resposta semelhante à seguinte:

   ![](assets/get-guid.png)

   O retorno para &quot;nome de usuário&quot; é o GUID do usuário.

1. Usando o GUID como nome de usuário, altere a senha do usuário.

   Para obter mais informações sobre como alterar sua senha, consulte [Redefinir senha](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md).

   Se sua organização usar um sistema SSO, somente um administrador de sistema da Workfront poderá alterar a senha de um usuário. Para obter mais informações, consulte [Visão geral do logon único no Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)

1. Com o usuário conectado ao Workfront, navegue até:

```
   https://<your domain>.my.workfront.com/login/convertUsername
```

1. No **Seu endereço de email de logon** , verifique se o endereço de email do usuário está correto e clique em **Atualizar conta**.

   ![](assets/guidusername-350x272.png)

   O nome de usuário do usuário é alterado para seu endereço de email do Workfront.

>[!TIP]
>
>Para localizar a ID de um usuário:
>
>1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Usuários** ![](assets/users-icon-in-main-menu.png).
>
>1. Selecione o usuário.
>
>   A página de perfil do usuário é aberta e sua ID de usuário é exibida no URL.
