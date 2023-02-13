---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adicionar usuários ao Adobe Workfront Fusion por meio da Adobe Admin Console
description: Você pode adicionar um usuário ao Adobe Admin Console e atribuí-lo ao Adobe Workfront Fusion ou atribuir um usuário existente no Adobe Admin Console ao Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: c8924e00-1154-4cf8-84e8-472251b5fc28
hidefromtoc: true
source-git-commit: 6cd6b1433fb56b92872f0ad80bb1a700fc0854cc
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 1%

---

# Adicionar usuários a [!DNL Adobe Workfront Fusion] através da [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>Os procedimentos descritos nesta página se aplicam somente às organizações que foram integradas à variável [!DNL Adobe Admin Console].
>
>Se sua organização ainda não tiver sido integrada à [!DNL Adobe Admin Console], consulte [Adicionar usuário a uma organização em [!DNL Adobe Workfront Fusion]](../organizations/add-user-to-an-organization.md).
>
>Para obter uma lista de procedimentos diferentes com base no fato de sua organização ter sido integrada à [!DNL Adobe Admin Console], consulte [Diferenças de administração baseadas em plataforma ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../fusion-in-admin-console/fusion-adobe-admin-console.md).

Você pode adicionar um usuário ao [!DNL Adobe Admin Console] e atribuí-los a [!DNL Adobe Workfront Fusion]ou atribua um usuário existente no [!DNL Adobe Admin Console] para [!DNL Workfront Fusion].

Para um vídeo descrevendo [!DNL Workfront Fusion] no [!DNL Adobe Admin Console], incluindo como adicionar usuários, consulte [[!DNL Fusion] no Adobe IMS](https://video.tv.adobe.com/v/3412464/){target=_blank}.

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!UICONTROL Pro] ou superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licença**</td> 
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> <p>[!UICONTROL Workfront Fusion for Work Automation] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr>
   <tr> 
   <td role="rowheader">[!DNL Adobe] direitos de administrador</td> 
   <td>Você deve ser um [!UICONTROL Product Configuration Administrator] de [!DNL Adobe] produtos para sua organização.</td> 
  </tr>
  </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

&#42;&#42;Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md)



## Pré-requisitos

Antes de usar o [!DNL Admin Console] para [!DNL Workfront], você deve receber um email convidando você para o console.

1. Se você for novo em [!DNL Adobe] e você recebeu um email informando que agora tem direitos de administrador para gerenciar [!DNL Adobe] software e serviços para sua organização, clique no botão no email para criar um [!DNL Adobe] e abra o [!DNL Admin Console].

   Ou

   Se você já tiver uma conta do Adobe, acesse [[!DNL Adobe Admin Console] página](https://adminconsole.adobe.com/).


## Adicionar um novo usuário ao [!DNL Adobe Admin Console] e [!DNL Workfront Fusion]

1. No [[!DNL Adobe Admin Console] página](https://adminconsole.adobe.com/), selecione o **[!UICONTROL Produtos]** na barra de navegação superior e selecione o **[!DNL Workfront Fusion]** bloco do produto.

   ![Fusão em Admin Console](assets/fusion-product-admin-console.png)

1. Na lista que é exibida, selecione a organização à qual deseja adicionar um usuário.

   ![Instância Fusion no Admin Console](assets/fusion-instances-admin-console.png)

1. Na lista que é exibida, com a variável **[!UICONTROL Perfis de produto]** da guia selecionada, clique no nome da [!DNL Workfront Fusion] [!UICONTROL Perfil de produto] link .

   ![Perfil de produto do Workfront Fusion](../../administration-and-setup/add-users/create-and-manage-users/assets/prod-profile-1.png)

   >[!IMPORTANT]
   >
   > Não faça alterações no [!UICONTROL Perfil de produto] próprio.

1. Com o **[!UICONTROL Usuários]** guia selecionada acima da lista, clique em **[!UICONTROL Adicionar usuário]**.

1. No **[!UICONTROL Adicionar usuários a este perfil de produto]** , digite o endereço de email ou o nome de um usuário que deseja adicionar e selecione o usuário na lista exibida.

1. Clique em **[!UICONTROL Salvar]**.

   O usuário é criado em [!DNL Workfront Fusion].

   <!--
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    -->

1. (Opcional) Continue para [Altere o nível de acesso de um usuário em [!DNL Workfront Fusion]](#change-a-users-access-level-in-workfront-fusion)

## Alterar o nível de acesso de um usuário no Workfront Fusion

### Alterar a função de um usuário para Administrador

A atribuição de uma função de Administrador a um usuário deve ser realizada na função [!DNL Adobe Admin Console].

1. No [!DNL Workfront Fusion] [!UICONTROL Perfil de produto] em que você adicionou o usuário, selecione o **[!UICONTROL Administradores]** guia .

1. Clique em **[!UICONTROL Adicionar administrador]**.

1. No **[!UICONTROL Adicionar administradores de perfil de produto]** , digite o endereço de email ou o nome de um usuário que deseja adicionar e selecione o usuário na lista exibida.

1. Clique em **[!UICONTROL Salvar]**.

   Esse usuário agora é administrador no [!DNL Workfront Fusion].

### Alterar a função de um usuário para [!UICONTROL membro], [!UICONTROL Contador]ou [!UICONTROL Desenvolvedor de aplicativos].

[!UICONTROL membro], [!UICONTROL Contador]e [!UICONTROL Desenvolvedor de aplicativos] as funções são tratadas dentro [!DNL Workfront Fusion].

Para obter instruções, consulte [Exibir ou editar funções de usuário](../organizations/manage-fusion-users.md#view-or-edit-user-roles) no artigo [Gerenciar [!DNL Adobe Workfront Fusion] usuários em sua organização](../organizations/manage-fusion-users.md)

## Atribua um usuário existente na [!DNL Adobe Admin Console] para [!DNL Workfront Fusion]

1. Comece a editar o usuário conforme descrito na seção &quot;Editar detalhes do usuário&quot; do artigo [Gerenciar usuários individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) no [!DNL Adobe Admin Console] documentação.

1. Adicionar **[!DNL Adobe Workfront Fusion]** aos produtos atribuídos ao usuário.
