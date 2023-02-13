---
user-type: administrator
product-area: system-administration
keywords: modificar,email,notificação,configurações,itens em massa,editar em massa,configurar,vários,usuários
navigation-topic: emails-administration
title: Modificar as configurações de notificação de email nos perfis dos usuários
description: Se você for um administrador do Adobe Workfront ou tiver um nível de acesso do Planejador que permita editar as configurações de outros usuários, é possível definir as configurações de notificação para vários usuários de uma só vez. Isso inclui especificar se os usuários recebem notificações como eventos, ou em um email de resumo diário, conforme descrito nas notificações do Adobe Workfront. Para obter informações sobre o nível de acesso necessário para editar usuários, consulte Conceder acesso aos usuários.
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 0%

---

# Modificar as configurações de notificação de email nos perfis dos usuários

Se você for um administrador do Adobe Workfront ou tiver um nível de acesso do Planejador que permita editar as configurações de outros usuários, é possível definir as configurações de notificação para vários usuários de uma só vez. Isso inclui especificar se os usuários recebem notificações como eventos, ou em um email de resumo diário, conforme descrito em [Notificações do Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md). Para obter informações sobre o nível de acesso necessário para editar usuários, consulte [Conceder acesso aos usuários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Ao definir configurações de notificação em massa, é possível alterar apenas as configurações que os usuários selecionados têm em comum.

Você também pode configurar notificações por email para um usuário por vez. Para obter mais informações, consulte [Ativar ou desativar suas próprias notificações de evento](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td>Plano</td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano ou tipo de licença você possui, entre em contato com o administrador da Workfront.

## Modifique as configurações de notificação por email de vários usuários em massa

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Usuários** ![](assets/users-icon-in-main-menu.png). Selecione os usuários e clique em **Editar**.
1. No **Editar Pessoa** for exibida, clique em **Notificações**.

1. Expanda uma categoria para exibir as configurações de notificação relacionadas a ela.

   Se houver pelo menos um usuário selecionado em que as notificações não correspondam às notificações dos outros usuários selecionados, a caixa de seleção categoria para essa notificação conterá uma linha horizontal ![](assets/straight-line-instead-of-checkmark.jpg) em vez de uma marca de verificação.

1. Clique nas notificações que deseja que os usuários recebam diariamente ou instantaneamente ou limpe as notificações que deseja que parem de receber.

   Para o **Comunicação** , você pode selecionar notificações individuais somente para delivery instantâneo. Você deve selecionar todas as notificações a serem entregues em um resumo diário.

   Quando você modifica uma configuração de notificação, o rótulo **Editado** for exibido para essa configuração de notificação, para que você saiba que essa configuração de notificação foi modificada.

1. Se você selecionou notificações para serem enviadas como resumo diário, selecione a hora do dia em que deseja que o resumo seja entregue na parte superior do **Notificações** na seção **Receita diária por email após** menu.

   Após selecionar um tempo de delivery, a variável **Receita diária por email após** é exibida com um quadro laranja para indicar que a hora do delivery foi editada.

   O resumo diário inclui eventos que atendem aos critérios das notificações 24 horas antes do horário selecionado. Os usuários recebem um email de resumo diário para cada tipo de notificação.

   O resumo diário pode chegar após o tempo selecionado, dependendo de quantos emails estão na fila para entrega no sistema. A hora listada é a hora local, conforme especificado nas configurações do navegador.
