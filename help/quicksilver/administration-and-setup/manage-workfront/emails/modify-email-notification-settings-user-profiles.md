---
user-type: administrator
product-area: system-administration
keywords: modificar,email,notificação,configurações,em massa,edição em massa,configurar,vários,usuários
navigation-topic: emails-administration
title: Modificar Configurações de Notificação por Email de Vários Usuários
description: Este artigo fornece informações para a Workfront ou administradores de grupo sobre como eles podem atualizar as notificações por email de outros usuários.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: e34abb5ff1068de99eaba33dc95287164e556742
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# Modificar as configurações de notificação por email de vários usuários

<!-- Audited: 12/2023 -->

Se você for um administrador do Adobe Workfront ou tiver um nível de acesso de Planejador que permita editar as configurações de outros usuários, poderá definir as configurações de notificação para vários usuários de uma vez. Isso inclui especificar se os usuários recebem notificações conforme os eventos ocorrem ou em um email de resumo diário, conforme descrito em [Notificações do Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md). Para obter informações sobre o nível de acesso necessário para editar usuários, consulte [Conceder acesso aos usuários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Você também pode configurar notificações por email para um usuário por vez, incluindo seu próprio perfil. Para obter mais informações, consulte [Modificar suas próprias notificações por email](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
    <p>Standard</p>
    <p>Plano</p>
   </td>
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modificar configurações de notificação por email para vários usuários

Ao definir as configurações de notificação em massa, você pode alterar apenas as configurações que os usuários selecionados têm em comum.

Quando você modifica uma configuração de notificação, o rótulo **Editado** é exibido para essa configuração de notificação, para que você saiba que a configuração de notificação foi modificada.

Para modificar as configurações de notificação por email para vários usuários:

{{step-1-to-users}}

1. Selecione os usuários e clique em **Editar**.
1. Na caixa **Editar Pessoa** exibida, clique em **Notificações**.

1. Expanda uma categoria para exibir as configurações de notificação relacionadas a ela.

   Se houver pelo menos um usuário selecionado em que as notificações não correspondam às notificações dos outros usuários selecionados, a caixa de seleção de categoria dessa notificação conterá uma linha horizontal ![Linha em vez de uma marca de seleção](assets/straight-line-instead-of-checkmark.jpg).


1. Clique em qualquer notificação que você deseja que os usuários recebam diariamente ou instantaneamente, ou desmarque qualquer uma que você deseja que eles parem de receber.

   >[!NOTE]
   >
   >   Na categoria **Comunicação**, você pode selecionar notificações individuais somente para entrega instantânea. Você deve selecionar todas as notificações que serão entregues em um resumo diário.


1. Se você selecionou notificações para serem enviadas como um resumo diário, selecione a hora do dia em que deseja que o resumo seja entregue na parte superior da seção **Notificações** do menu **Resumo diário de emails após**.

   ![Hora de resumo diária](assets/daily-digest-time.png)

   O resumo diário inclui eventos que atendem aos critérios das notificações 24 horas antes da hora selecionada. Os usuários recebem um email de resumo diário para cada tipo de notificação.

   O resumo diário pode chegar depois do tempo selecionado, dependendo de quantos emails estão na fila para entrega no sistema. A hora listada é a hora local especificada nas configurações do navegador.
