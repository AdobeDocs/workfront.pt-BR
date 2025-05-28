---
title: Efetuar login como outro usuário
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Como administrador do Adobe Workfront, às vezes pode ser necessário acessar o Workfront em nome de outro usuário.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2f8dd132-1086-4980-9b56-993a68231e96
source-git-commit: 6068c9c53568d3ebec9fae294bfee1cbd365714b
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 0%

---

# Fazer logon como outro usuário

<!--Audited: 5/2025-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all users only in the Preview environment.</span> -->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. Also linked to other articles: Creating and Managing Groups, etc.</p>
-->

Como administrador do Adobe Workfront, às vezes pode ser necessário acessar o Workfront em nome de outro usuário. Ou, como administrador de grupo, talvez seja necessário acessar o Workfront em nome de um usuário que seja membro de um grupo que você gerencia.

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
>Para obter mais informações sobre integrações de documentos, consulte [Configurar integrações de documentos](../../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Novo: Padrão</p>
   <p>Ou</p>
   <p>Atual: Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Com o nível de acesso de Administrador do sistema, você pode fazer logon como qualquer pessoa.</p> <p>Com um nível de acesso Padrão ou Planejador, você pode fazer logon como um usuário com um nível de licença inferior se a configuração Usuários no nível de acesso estiver definida como Acesso de edição, com as opções Criar e pelo menos uma das duas opções de Administrador de usuários habilitadas em Ajustar suas configurações <img src="assets/gear-icon-in-access-levels.png">. </p> 
   <p>OBSERVAÇÃO: dessas duas opções, se o Administrador de Usuários (Usuários de Grupo) estiver ativado, você deverá ser um administrador de grupo de um grupo do qual o usuário seja membro.</p></td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Fazer logon e executar ações como outro usuário

1. Faça logon no Workfront como administrador do Workfront ou administrador de grupo.

   >[!NOTE]
   >
   >* Se você for um administrador de grupo, poderá efetuar login somente como usuários nos grupos que gerencia. Além disso, a permissão Administrador de usuários (usuários de grupo) deve estar ativada em seu nível de acesso:
   >   
   >  ![Usuário administrador de grupo](assets/group-admin-user.png)
   >   
   >  Essa configuração é desativada por padrão. Para obter mais informações, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   >   
   >* Não é possível redefinir a senha de um administrador do Workfront.

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Fazer logon como**.

1. Na caixa **Comece a digitar o nome...** da guia **Fazer Logon Como**, comece a digitar o nome do usuário e clique nele quando ele aparecer na lista suspensa.


   >[!NOTE]
   >* O usuário selecionado deve ter um nível de acesso definido no Workfront. Não é possível fazer logon no sistema Workfront como um usuário que não tem direitos para fazer logon.
   >* Os administradores de grupo podem fazer logon somente como usuários membros dos grupos que gerenciam. Eles não podem fazer logon como administrador do Workfront.

1. Clique Em **Fazer Logon**. Você está conectado como outro usuário e uma notificação é exibida na parte superior da tela indicando isso.

   <!--
   <p> Might come in a future story:</p>
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



1. Depois de executar as ações necessárias como usuário, clique em **Logout** na parte superior da tela.

## Atividade de rastreamento e auditoria enquanto um administrador está conectado como outro usuário

O Workfront fornece mecanismos para rastrear e auditar atividades que ocorrem enquanto o administrador está conectado como outro usuário.

Quando você efetua login como outro usuário, a última data de login para esse usuário é modificada para a data em que o administrador do sistema ou do grupo efetuar login como esse usuário.

* [Exibir indicadores em itens](#view-indicators-on-items)
* [Exibir informações de auditoria](#view-audit-information)

### Exibir indicadores em itens {#view-indicators-on-items}

Ao fazer logon no Workfront como outro usuário e executar uma ação, o Workfront indica claramente que qualquer ação executada é feita por você em nome do usuário com o qual você está conectado.

Por exemplo, se você comentar em um item enquanto estiver conectado como outro usuário, uma instrução indicará que o comentário foi feito por você em nome do usuário ao visualizar a seção Atualizações de um objeto.

### Exibir informações de auditoria {#view-audit-information}

1. Faça logon no Workfront como administrador do Workfront ou administrador de grupo.
   {{step-1-to-setup}}
   <!--1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).-->

1. No painel esquerdo, clique em **Fazer Logon como** e na guia **Log de Acesso**.

   >[!NOTE]
   >
   >Sempre que um administrador de sistema ou de grupo fizer logon no Workfront como outro usuário, o evento será conectado na trilha de auditoria. Além disso, todas as ações auditáveis que ocorrem enquanto o administrador está conectado como outro usuário são conectadas na trilha de auditoria.

1. (Opcional) Você pode filtrar os resultados exibidos na trilha de auditoria das seguintes maneiras:

   * Por usuário que fez logon
   * Por usuário que fez logon como
   * Por data e hora
