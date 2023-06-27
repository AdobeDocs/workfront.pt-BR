---
filename: manage-fusion-users
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Gerenciar [!DNL Adobe Workfront Fusion] usuários em sua organização
description: Gerenciar [!DNL Adobe Workfront Fusion] usuários em sua organização
author: Becky
feature: Workfront Fusion
exl-id: fbb858a6-1230-41b4-892a-4ffeb2711922
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Gerenciar [!DNL Adobe Workfront Fusion] usuários em sua organização

[!DNL Adobe Workfront Fusion] os administradores podem gerenciar funções de usuário dentro do [!DNL Workfront Fusion].

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on adding a user in the Adobe Admin Console:
>
>* See [Add a user to an organization in Adobe Workfront Fusion](../../workfront-fusion/organizations/add-user-to-an-organization.md#create)
>* See the section "Add users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)
>* Contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront Fusion/Adobe Business Platform)](../../workfront-fusion/fusion-in-admin-console/fusion-adobe-admin-console.md).

-->

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!DNL Pro] ou superior</p> </td> 
  </tr> 
   <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
    <td> <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
   </tr>
   <tr> 
   <td role="rowheader">Licença [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Requisito de licença atual: Não [!DNL Workfront Fusion] requisito de licença.</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para automação de trabalho]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o [!UICONTROL Select] ou o [!UICONTROL Prime] [!DNL Adobe Workfront] Planejar, sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no [!UICONTROL Ultimate] [!DNL Workfront] plano.</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> 
     <p>Você deve ser um [!DNL Workfront Fusion] administrador da sua organização.</p>
     <p>Você deve ser um [!DNL Workfront Fusion] administrador da sua equipe.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Exibir ou editar funções de usuário {#view}

[!DNL Adobe Workfront Fusion] os administradores podem exibir e atualizar funções de usuário.

1. Enquanto estiver conectado como um [!DNL Workfront Fusion] administrador, selecione **[!UICONTROL Usuários]** no painel de navegação esquerdo.
1. Clique em **[!UICONTROL Detalhes]** na linha do usuário que deseja exibir.
1. (Opcional) Para atualizar a função do usuário, clique na lista suspensa na **[!DNL Role]** na linha da organização em que deseja alterar a função do usuário e, em seguida, selecione a nova função.

## Exibir ou editar detalhes do usuário {#view2}

[!DNL Adobe Workfront Fusion] administradores podem exibir e atualizar detalhes do usuário.

1. Enquanto estiver conectado como um [!DNL Workfront Fusion] administrador, selecione **[!UICONTROL Usuários]** no painel de navegação esquerdo.
1. Clique em **[!UICONTROL Detalhes]** na linha do usuário que deseja exibir.
1. (Opcional) Para atualizar os detalhes do usuário, clique em **[!UICONTROL Opções]** no canto superior direito da tela, selecione **[!UICONTROL Detalhes da alteração]**.

## Excluir um usuário {#delete}

[!DNL Adobe Workfront Fusion] administradores podem excluir usuários.

1. Enquanto estiver conectado como um [!DNL Workfront Fusion] administrador, selecione [!UICONTROL Usuários] no painel de navegação esquerdo.
1. Clique em **[!UICONTROL Detalhes]** na linha do usuário que deseja exibir.
1. (Opcional) Para atualizar os detalhes do usuário, clique em **[!UICONTROL Opções]** no canto superior direito da tela, selecione **[!UICONTROL Excluir]**.

### Considerações ao excluir um usuário no Workfront Fusion

* Quando um usuário é excluído, as conexões, as chaves e os webhooks do usuário são removidos. Quaisquer cenários pertencentes ao usuário são transferidos para o Proprietário da organização. As conexões nesses cenários devem ser atualizadas, pois as conexões pertencentes ao usuário não são mais válidas.
* Se o usuário excluído possuir quaisquer aplicativos ou modelos públicos, os aplicativos ou modelos públicos serão transferidos para o Proprietário da organização. Se não houver um Proprietário da organização, os aplicativos ou modelos públicos serão transferidos para outro usuário.
