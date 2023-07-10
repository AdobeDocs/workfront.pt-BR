---
title: Fazer logon como outro usuário
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Como administrador do Adobe Workfront, às vezes pode ser necessário acessar o Workfront em nome de outro usuário.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2f8dd132-1086-4980-9b56-993a68231e96
source-git-commit: 82f42d81970c7572f43519423ec3a8c0889aaff4
workflow-type: tm+mt
source-wordcount: '895'
ht-degree: 0%

---

# Fazer logon como outro usuário


<span class="preview">As informações destacadas nesta página se referem a funcionalidades ainda não disponíveis no geral. Ele está disponível para todos os usuários somente no ambiente de Pré-visualização.</span>
<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. Also linked to other articles: Creating and Managing Groups, etc.</p>
-->

>[!IMPORTANT]
>
>O procedimento descrito nesta página se aplica apenas a organizações que ainda não foram integradas à Adobe Admin Console. Se sua organização tiver sido integrada à Adobe Admin Console, essa ação não estará disponível.
>
>Para obter uma lista de procedimentos que diferem dependendo de sua organização ter sido integrada à Adobe Admin Console, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Como administrador do Adobe Workfront, às vezes pode ser necessário acessar o Workfront em nome de outro usuário.

Ou, como administrador de grupo, talvez seja necessário acessar o Workfront em nome de um usuário que seja membro de um grupo que você gerencia.

Por exemplo, se uma tarefa não puder progredir até que um usuário de férias execute uma determinada ação, você poderá fazer logon como esse usuário e executar a ação.

<!--
<note type="note">
Some users, such as executives, need to be able to control which administrators can log in to their accounts, and for how long. Working with your organization, Workfront configures settings that allow this control for these users. When a Workfront administrator or group administrator (associated with one of the user's groups) tries to log in as one of these users, an on-screen message prompts the administrator to contact the user for access. From the user profile area, the user can then grant access to the administrator and specify an expiration time for it. For more information on how the user does this, see
<a href="../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md#access" class="MCXref xref">Access</a> in
<a href="../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configure My Settings</a>.
<span class="PinkDraftNote">[Add a note about this being only for the Enterprise package if they decide to do it that way]</span>
</note>
-->

>[!NOTE]
>
>Como uma integração de documentos pode se conectar a arquivos pessoais privados, os administradores não podem acessar integrações de documentos enquanto estiverem conectados como outro usuário.
>
>Para obter mais informações sobre integrações de documentos, consulte [Configurar integrações de documentos](../../../administration-and-setup/configure-integrations/configure-document-integrations.md)

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Com o nível de acesso de Administrador do sistema, você pode fazer logon como qualquer pessoa. Para obter informações sobre esse nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acesso administrativo total a um usuário</a>. </p> <p>Com um nível de acesso de Planejador, você pode fazer logon como um usuário com um nível de licença mais baixo se a <b>Usuários</b> no nível de acesso estiver definida como <b>Editar</b> acesso, com <b>Criar</b> e pelo menos um dos dois <b>Administrador de Usuários</b> opções ativadas em <b>Ajuste as configurações</b> <img src="assets/gear-icon-in-access-levels.png">. </p> 
   <p><b>NOTA</b>: dessas duas opções, se o Usuário <b>Administrador (Usuários de grupo)</b> estiver ativado, você deve ser um administrador de grupo de um grupo do qual o usuário seja membro.</p> 
   <p>Para obter mais informações sobre o <b>Usuários</b> em um nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Fazer logon e executar ações como outro usuário

1. Faça logon no Workfront como administrador do Workfront ou administrador de grupo.

   >[!NOTE]
   >
   >* Se você for um administrador de grupo, poderá efetuar login somente como usuários nos grupos que gerencia. Além disso, a permissão Administrador de usuários (usuários de grupo) deve estar ativada em seu nível de acesso:
   >   
   >  ![](assets/group-admin-user.png)
   >   
   >  Essa configuração é desativada por padrão. Para obter mais informações, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   >   
   >* Não é possível redefinir a senha de um administrador do Workfront.

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Fazer logon como**.

1. No **Usuários** na caixa **Fazer logon como** comece digitando o nome do usuário e clique no nome quando ele aparecer na lista suspensa.

   O usuário deve ter um nível de acesso definido no Workfront. Não é possível fazer logon no sistema Workfront como um usuário que não tem direitos para fazer logon.

   >[!NOTE]
   >
   >Os administradores de grupo podem fazer logon somente como usuários membros dos grupos que gerenciam. Eles não podem fazer logon como administrador do Workfront.

1. Clique em **Fazer logon.**

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Might come in a future story:</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">click an Access period and then click Request to ask the user for access to log as him or her for the specified period of time. Continue these steps after the user grants access. Specify somewhere here that this is only for the Enterprise package if they decide on that</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Or </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">If a prompt appears indicating that the user has restricted access to their account, contact the user to request access.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The user can then can grant you "Log in as" access in their user profile. They can also specify an expiration date and time for the access period. </p>
   -->

   <!--
   This triggers an email to let you know that you have access to log in as the user, depending on how your event notifications are enabled. For more information, see <a href="../../../workfront-basics/using-notifications/event-notifications.md" class="MCXref xref">Event notifications</a>.
   </div>
   -->

   Quando você estiver conectado como outro usuário, uma notificação será exibida na parte superior da tela para indicar isso.

1. Depois de executar as ações necessárias como usuário, clique em **Fazer logoff.**

## Atividade de rastreamento e auditoria enquanto um administrador está conectado como outro usuário

O Workfront fornece mecanismos para rastrear e auditar atividades que ocorrem enquanto o administrador está conectado como outro usuário.

Quando você efetua login como outro usuário, a última data de login é modificada para esse usuário para a data em que o administrador do sistema ou do grupo efetuar login como esse usuário.

* [Exibir indicadores em itens](#view-indicators-on-items)
* [Exibir informações de auditoria](#view-audit-information)

### Exibir indicadores em itens {#view-indicators-on-items}

Ao fazer logon no Workfront como outro usuário e executar uma ação, o Workfront indica claramente que qualquer ação executada é feita por você em nome do usuário com o qual você está conectado.

Por exemplo, se você comentar em um item enquanto estiver conectado como outro usuário, uma instrução indicará que o comentário foi feito por você em nome do usuário.

>[!NOTE]
>
><span class="preview">Ao usar a nova experiência de comentários, o comentário é adicionado como o usuário que fez logon como outro usuário e não há indicação de que ele esteja adicionando um comentário em nome de outra pessoa.
>
>Por exemplo, se um administrador do Workfront fizer logon como outro usuário, o usuário associado ao comentário será o administrador do Workfront. Para obter mais informações, consulte [Nova experiência de comentários](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). </span>


### Exibir informações de auditoria {#view-audit-information}

1. Faça logon no Workfront como administrador do Workfront ou administrador de grupo.
1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Fazer logon como,** em seguida, clique no link **Log de acesso** guia.

   Sempre que um administrador de sistema ou de grupo fizer logon no Workfront como outro usuário, o evento será conectado na trilha de auditoria. Além disso, todas as ações auditáveis que ocorrem enquanto o administrador está conectado como outro usuário são conectadas na trilha de auditoria.

1. (Opcional) Você pode filtrar os resultados exibidos na trilha de auditoria das seguintes maneiras:

   * Por usuário que fez logon
   * Por usuário que fez logon como
   * Por data
