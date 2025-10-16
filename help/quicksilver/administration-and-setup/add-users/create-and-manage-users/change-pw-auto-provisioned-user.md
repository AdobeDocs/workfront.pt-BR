---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Alterar a senha de um usuário provisionado automaticamente
description: Recomendamos que você altere o nome de usuário de um novo usuário para seu endereço de email do Workfront e, em seguida, permita que ele altere a senha.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 14124911-e5e1-4a4f-9b25-8b4fab0329e1
source-git-commit: f8d04790caefd12c9811ea3ed94e1f892311d031
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# Alterar a senha de um usuário autoprovisionado

Quando você cria usuários por meio do provisionamento automático, o Adobe Workfront atribui a eles um GUID (Identificador Global Exclusivo) para um nome de usuário. Uma GUID é uma sequência exclusiva de números e letras aleatórios, por exemplo, *5489cb430012526e1ea635e8c29f377f*.

Geralmente, quando um novo usuário tenta alterar sua senha temporária, ele insere seu endereço de email como nome de usuário e recebe um erro por um nome de usuário incorreto. Para alterar a senha, o usuário deve digitar o nome de usuário atribuído pelo sistema, que é um GUID.

Como os nomes de usuário da GUID podem ser difíceis de usar, recomendamos que você altere primeiro o nome de usuário para o endereço de email do Workfront e, em seguida, permita que eles alterem a senha.

>[!TIP]
>
>Você pode encontrar o GUID de um usuário das seguintes maneiras:
>
>* Vá para o perfil do usuário e copie o GUID do URL no seu navegador.
>
>  Por exemplo, na URL `https://acme.workfront.com/user/61941ab1000af22d7104628efa1c738b/details`, você copiaria a cadeia de caracteres de números e letras entre as duas últimas barras: `61941ab1000af22d7104628efa1c738b`.
>
>  Para obter mais informações, consulte [Editar perfil de usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
>
>* Crie um relatório de usuário com uma coluna Usuário > GUID. Para obter mais informações, consulte [Criar um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).
>
>* Consulte a API do Workfront.
>

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plano</p></td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Administrador de Sistema</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Alterar a senha de um usuário autoprovisionado

1. Determine o nome de usuário GUID de um usuário passando uma solicitação de API, como mostrado no exemplo a seguir:

   https://`<domain>`.my.workfront.com/attask/api/v14.0/USER/search?fields=username&amp;ID=`<ID of User>` Onde *`<domain>`* é o domínio da sua empresa e *`<ID of User>`* é a Workfront ID do usuário.

   Você receberá uma resposta semelhante à seguinte:

   ![Obter GUID](assets/get-guid.png)

   O retorno para &quot;username&quot; é a GUID do usuário.

1. Usando o GUID como nome de usuário, altere a senha do usuário.

   Para obter mais informações sobre como alterar sua senha, consulte [Redefinir sua senha](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md).

   Se sua organização usar um sistema SSO, somente um administrador de sistema da Workfront poderá alterar a senha de um usuário. Para obter mais informações, consulte [Visão geral do logon único na Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)

1. Com o usuário conectado ao Workfront, navegue até:

```
   https://<your domain>.my.workfront.com/login/convertUsername
```

1. Na caixa **Seu endereço de email de logon**, verifique se o endereço de email do usuário está correto e clique em **Atualizar Conta**.

   ![Nome de usuário](assets/guidusername-350x272.png)

   O nome de usuário é alterado para seu endereço de email do Workfront.

>[!TIP]
>
>Para localizar a ID de um usuário:
>
>1. Clique no ícone **Menu principal** ![Ícone do menu principal](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique no ícone **Usuários** ![Usuários](assets/users-icon-in-main-menu.png).
>
>1. Selecione o usuário.
>
>   A página de perfil do usuário é aberta e a ID do usuário é exibida no URL.
>
