---
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Adicionar um usuário a uma organização no Adobe Workfront Fusion
description: Você pode adicionar usuários a organizações no Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 98248cca-98f5-4eb5-b203-67e261df33f1
source-git-commit: 5cdc438c6757d438b2c09796cf77e59dc19c45d9
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 0%

---

# Adicionar um usuário a uma organização ou equipe no Adobe Workfront Fusion

>[!IMPORTANT]
>
>O procedimento descrito nesta página se aplica apenas a organizações que ainda não foram integradas ao [!DNL Adobe Admin Console]. Se sua organização foi integrada ao [!DNL Adobe Admin Console], você deve executar esta ação através do [!DNL Adobe Admin Console].
>
>Para obter instruções sobre como adicionar um usuário depois que sua organização for movida para a [!DNL  Adobe Admin Console] e a Experiência unificada do Adobe, consulte [Adicionar usuários a [!DNL Adobe Workfront Fusion] por meio de [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md).
>
>Para obter uma lista de procedimentos que diferem com base no fato de sua organização ter sido integrada à Adobe Admin Console, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront Fusion/Adobe Business Platform)](../../../quicksilver/workfront-fusion/fusion-in-admin-console/fusion-in-admin-console.md).

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
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para Automação do Trabalho]</p>
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
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> 
     <p>Você deve ser um administrador do [!DNL Workfront Fusion] para sua organização.</p>
     <p>Você deve ser um administrador [!DNL Workfront Fusion] para sua equipe.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Adicionar usuários a uma organização


<!--
<p>The procedure to add a user to your Fusion organization differs based on whether your organization has been onboarded to the Adobe Business Platform. </p>
<ul>
<li> <p><a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">Add a user to an organization that has been onboarded to the Adobe Business Platform</a> </p> </li>
<li> <p><a href="#add-a-user-to-an-organization-that-has-not-been-onboarded-to-the-adobe-business-console" class="MCXref xref">Add a user to an organization that has not been onboarded to the Adobe Business Console</a> </p> </li>
</ul>
<div>
<p><strong>Add a user to an organization that has been onboarded to the Adobe Business Platform</strong></p>
<p>If your organization has been onboarded to the Adobe Business Platform, you must perform this action through the Adobe Admin Console.</p>
<p>For instructions on adding a user in the Adobe Admin Console:</p>
<ul>
<li> <p>See <a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create" class="MCXref xref">Create users in Workfront with the Adobe Admin Console</a></p> </li>
<li> <p>See the section "Add users" in the article <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li>
<li> <p>Contact your Adobe Admin Console Administrator.</p> </li>
</ul>
<p>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see <a href="../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md" class="MCXref xref">Platform-based administration differences (Adobe Workfront/Adobe Business Platform)</a>.</p>
</div>
<p><strong>Add a user to an organization that has not been onboarded to the Adobe Business Console</strong></p>

-->
>[!NOTE]
>
>Se sua organização estiver migrando para a Adobe Admin Console, não será possível gerenciar usuários na Workfront (adicionar ou excluir usuários). Você poderá executar essas ações no Adobe Admin Console após a conclusão da migração.

Para adicionar usuários à organização, você deve ser um administrador na organização à qual deseja adicionar usuários. Para obter informações sobre funções, consulte [Funções da organização em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/organizations/organization-roles.md).

Para adicionar um usuário à organização:

1. Navegue até **[!UICONTROL Organizações]** no menu e selecione a organização à qual deseja adicionar um usuário.
1. Abra a guia **[!UICONTROL Usuários]** no Painel.
1. Clique em **[!UICONTROL Convidar um novo usuário]**.e envie o convite clicando em **[!UICONTROL Enviar]**.

   >[!NOTE]
   >
   >   
   >Se você não vir o botão [!UICONTROL Convidar um novo usuário], sua organização foi integrada ao [!DNL Adobe Business Platform.]
   >
   >  Para obter instruções sobre como adicionar um usuário a uma organização que foi integrada ao [!DNL Adobe Business Platform], consulte [Adicionar usuários ao [!DNL Adobe Workfront Fusion] por meio do [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md)

1. Preencha o formulário.

   <table style="table-layout:auto">
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Endereço de email]</td>
      <td>
        Insira o endereço de email do usuário
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Nome]</td>
      <td>
        <p>Digite o nome completo do usuário</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Função] </td>
      <td>Selecione a função do usuário. Para obter uma explicação sobre as funções, consulte <a href="/help/quicksilver/workfront-fusion/organizations/organization-roles.md">Organização e funções de equipe.</a></p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">Equipes</td>
      <td>Selecione todas as equipes das quais você deseja que o usuário seja membro.</td>
    </tr>
    <tr>
      <td role="rowheader">Nota</td>
      <td>Insira uma nota para o usuário. Esta nota aparecerá no email de convite do usuário.</td>
    </tr>
  </tbody>
</table>

O usuário recebe um email de convite, no qual pode aceitar o convite.

## Adicionar um usuário a uma equipe

Seus usuários são atribuídos a equipes ao criá-los. Se um usuário existente precisar ser adicionado a uma equipe, você pode adicioná-lo na página Usuários da equipe.

A adição de um usuário a uma equipe é tratada na página da equipe.

1. Vá para a equipe à qual você deseja adicionar o usuário selecionando **Organizações** no painel esquerdo, clicando na guia **Equipes** na página da organização e selecionando a equipe.

   Ou

   Se você estiver na página de outra equipe, clique na lista suspensa de equipes na parte superior da página.

1. Na página Equipe (com o nome da equipe na parte superior da página), selecione a guia **Usuários**.
1. Localize o usuário na página. Os usuários em sua organização aparecem nesta página, mesmo que não sejam membros da equipe.
1. Clique em **Nenhum** à direita do nome do usuário e selecione a função que você deseja que eles tenham na equipe.

O usuário é adicionado à equipe do.