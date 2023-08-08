---
user-type: administrator
product-area: system-administration
keywords: modificar,email,notificação,configurações,em massa,edição em massa,configurar,vários,usuários
navigation-topic: emails-administration
title: Modificar configurações de notificação por email nos perfis dos usuários
description: Se você for um administrador do Adobe Workfront ou tiver um nível de acesso de Planejador que permita editar as configurações de outros usuários, poderá definir as configurações de notificação para vários usuários de uma vez. Isso inclui especificar se os usuários recebem notificações conforme os eventos ocorrem ou em um email de resumo diário, conforme descrito nas notificações do Adobe Workfront. Para obter informações sobre o nível de acesso necessário para editar usuários, consulte Conceder acesso aos usuários.
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: 91eb8770c07396b5772029e9d2370f0b1f10d4a1
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 0%

---

# Modificar configurações de notificação por email nos perfis dos usuários

Se você for um administrador do Adobe Workfront ou tiver um nível de acesso de Planejador que permita editar as configurações de outros usuários, poderá definir as configurações de notificação para vários usuários de uma vez. Isso inclui especificar se os usuários recebem notificações conforme os eventos ocorrem ou em um email de resumo diário, conforme descrito em [Notificações do Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md). Para obter informações sobre o nível de acesso necessário para editar usuários, consulte [Conceder acesso aos usuários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Ao definir as configurações de notificação em massa, você pode alterar apenas as configurações que os usuários selecionados têm em comum.

>[!NOTE]
>
>Você também pode configurar notificações por email para um usuário por vez, incluindo seu próprio perfil. Para obter mais informações, consulte [Ativar ou desativar suas próprias notificações de eventos](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).


## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td>Plano</td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir o tipo de plano ou licença que você tem, entre em contato com o administrador do Workfront.

## Modificar as configurações de notificação por email de vários usuários em massa

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Usuários** ![](assets/users-icon-in-main-menu.png). Selecione os usuários e clique em **Editar**.
1. No **Editar pessoa** for exibida, clique em **Notificação**.

1. Expanda uma categoria para exibir as configurações de notificação relacionadas a ela.

   Se houver pelo menos um usuário selecionado em que as notificações não correspondam às notificações dos outros usuários selecionados, a caixa de seleção de categoria para essa notificação conterá uma linha horizontal ![](assets/straight-line-instead-of-checkmark.jpg) em vez de uma marca de seleção.

1. Clique em qualquer notificação que você deseja que os usuários recebam diariamente ou instantaneamente, ou desmarque qualquer uma que você deseja que eles parem de receber.

   Para o **Comunicação** você pode selecionar notificações individuais somente para entrega instantânea. Você deve selecionar todas as notificações que serão entregues em um resumo diário.

   Quando você modifica uma configuração de notificação, o rótulo **Editado** é exibida para essa configuração de notificação, para que você saiba que essa configuração de notificação foi modificada.

1. Se você selecionou notificações para serem enviadas como um resumo diário, selecione a hora do dia em que deseja que o resumo seja entregue na parte superior do **Notificação** na seção **Enviar o resumo diário por email depois de** menu.

   Após selecionar um tempo de delivery, a variável **Enviar o resumo diário por email depois de** é exibida com um quadro laranja para indicar que a hora do delivery foi editada.

   O resumo diário inclui eventos que atendem aos critérios das notificações 24 horas antes da hora selecionada. Os usuários recebem um email de resumo diário para cada tipo de notificação.

   O resumo diário pode chegar depois do tempo selecionado, dependendo de quantos emails estão na fila para entrega no sistema. A hora listada é a hora local especificada nas configurações do navegador.
