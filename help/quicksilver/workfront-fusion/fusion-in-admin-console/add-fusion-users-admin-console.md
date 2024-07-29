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
source-git-commit: b7ceec2750ded516cae20d12b991b8fec94c6029
workflow-type: tm+mt
source-wordcount: '638'
ht-degree: 1%

---

# Adicionar usuários a [!DNL Adobe Workfront Fusion] através de [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>Os procedimentos descritos nesta página se aplicam apenas às organizações que foram integradas ao [!DNL Adobe Admin Console].
>
>Se sua organização ainda não foi integrada ao [!DNL Adobe Admin Console], consulte [Adicionar um usuário a uma organização em [!DNL Adobe Workfront Fusion]](../organizations/add-user-to-an-organization.md).
>
>Para obter uma lista de procedimentos que diferem se sua organização foi integrada ao [!DNL Adobe Admin Console], consulte [Diferenças de administração baseadas em plataforma ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../fusion-in-admin-console/fusion-adobe-admin-console.md).

Você pode adicionar um usuário ao [!DNL Adobe Admin Console] e atribuí-lo a [!DNL Adobe Workfront Fusion], ou atribuir um usuário existente no [!DNL Adobe Admin Console] a [!DNL Workfront Fusion].

Para um vídeo que descreve [!DNL Workfront Fusion] em [!DNL Adobe Admin Console], incluindo como adicionar usuários, consulte [[!DNL Fusion] no Adobe IMS](https://video.tv.adobe.com/v/3412464/){target=_blank}.

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
   <td>
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr>
   <tr> 
   <td role="rowheader">[!DNL Adobe] direitos de administrador</td> 
   <td>Você deve ser um [!UICONTROL Administrador de Configuração de Produto] de [!DNL Adobe] produtos para sua organização.</td> 
  </tr>
  </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

&#42;&#42;Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md)



## Pré-requisitos

Antes de usar o [!DNL Admin Console] para [!DNL Workfront], você deve receber um email convidando você para o console.

1. Se você é novo no [!DNL Adobe] e recebeu um email informando que agora tem direitos de administrador para gerenciar software e serviços do [!DNL Adobe] para sua organização, clique no botão no email para criar uma conta do [!DNL Adobe] e abrir o [!DNL Admin Console].

   Ou

   Se você já tiver uma conta Adobe, vá para a [[!DNL Adobe Admin Console] página](https://adminconsole.adobe.com/).


## Adicionar um novo usuário ao [!DNL Adobe Admin Console] e [!DNL Workfront Fusion]

1. Na [[!DNL Adobe Admin Console] página](https://adminconsole.adobe.com/), selecione a guia **[!UICONTROL Produtos]** na barra de navegação superior e, em seguida, selecione o bloco de produtos **[!DNL Workfront Fusion]**.

   ![Fusão no Admin Console](assets/fusion-product-admin-console.png)

1. Na lista exibida, selecione a organização à qual deseja adicionar um usuário.

   ![Instância do Fusion no Admin Console](assets/fusion-instances-admin-console.png)

1. Na lista exibida, com a guia **[!UICONTROL Perfis de Produto]** selecionada, clique no nome do link [!DNL Workfront Fusion] [!UICONTROL Perfil de Produto].

   ![Perfil de Produto Workfront Fusion](../../administration-and-setup/add-users/create-and-manage-users/assets/prod-profile-1.png)

   >[!IMPORTANT]
   >
   > Não faça alterações no próprio [!UICONTROL Perfil do Produto].

1. Com a guia **[!UICONTROL Usuários]** selecionada acima da lista, clique em **[!UICONTROL Adicionar usuário]**.

1. Na caixa **[!UICONTROL Adicionar usuários a este perfil de produto]**, digite o endereço de email ou o nome de um usuário que deseja adicionar e selecione o usuário na lista exibida.

1. Clique em **[!UICONTROL Salvar]**.

   O usuário foi criado em [!DNL Workfront Fusion].

   <!--
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    -->

1. (Opcional) Continue para [Alterar o nível de acesso de um usuário em [!DNL Workfront Fusion]](#change-a-users-access-level-in-workfront-fusion)

## Alterar o nível de acesso de um usuário no Workfront Fusion

### Alterar a função de um usuário para Administrador

A atribuição de uma função de Administrador a um usuário deve ser feita no [!DNL Adobe Admin Console].

1. Na página [!DNL Workfront Fusion] [!UICONTROL Perfil de Produto] em que você adicionou o usuário, selecione a guia **[!UICONTROL Administradores]**.

1. Clique em **[!UICONTROL Adicionar administrador]**.

1. Na caixa **[!UICONTROL Adicionar administradores de perfil de produto]**, digite o endereço de email ou o nome de um usuário que deseja adicionar e selecione o usuário na lista exibida.

1. Clique em **[!UICONTROL Salvar]**.

   Este usuário agora é um Administrador em [!DNL Workfront Fusion].

### Altere a função de um usuário para [!UICONTROL Membro], [!UICONTROL Contador] ou [!UICONTROL Desenvolvedor de Aplicativos].

As funções [!UICONTROL Membro], [!UICONTROL Contador] e [!UICONTROL Desenvolvedor de Aplicativos] são tratadas dentro de [!DNL Workfront Fusion].

Para obter instruções, consulte [Exibir ou editar funções de usuário](../organizations/manage-fusion-users.md#view-or-edit-user-roles) no artigo [Gerenciar [!DNL Adobe Workfront Fusion] usuários em sua organização](../organizations/manage-fusion-users.md)

## Atribuir um usuário existente no [!DNL Adobe Admin Console] a [!DNL Workfront Fusion]

É possível adicionar um usuário existente a uma equipe no Fusion. Isso é tratado no Fusion.

Para obter instruções, consulte [Adicionar um usuário a uma equipe](/help/quicksilver/workfront-fusion/organizations/add-user-to-an-organization.md#add-a-user-to-a-team) no artigo Adicionar um usuário a uma organização ou equipe no Adobe Workfront Fusion.
