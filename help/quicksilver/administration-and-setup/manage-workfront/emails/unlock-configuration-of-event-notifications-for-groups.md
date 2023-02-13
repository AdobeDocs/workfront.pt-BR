---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Desbloquear ou bloquear a configuração de notificações de eventos para todos os grupos
description: Se você for um administrador do Adobe Workfront, poderá desbloquear ou rebloquear a capacidade de os administradores de grupo configurarem uma notificação de evento para grupos de nível superior que eles gerenciam. A configuração de uma notificação de evento consiste em ativá-la ou desativá-la.
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 056d76c1-7e9b-49b9-974a-75765e53b7fd
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# Desbloquear ou bloquear a configuração de notificações de eventos para todos os grupos

Se você for um administrador do Adobe Workfront, poderá desbloquear ou rebloquear a capacidade de os administradores de grupo configurarem uma notificação de evento para grupos de nível superior que eles gerenciam. A configuração de uma notificação de evento consiste em ativá-la ou desativá-la.

Se houver algum grupo acima do grupo que você gerencia, os administradores também poderão fazer isso para o seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

Quando um administrador configura uma notificação de evento para um grupo, a configuração afeta os usuários para os quais esse grupo, ou um de seus subgrupos, é seu Grupo doméstico. Em seus perfis de usuário, esses usuários visualizam as notificações de eventos ativadas para seu Grupo doméstico, em vez das notificações de eventos ativadas em todo o sistema. Para obter mais informações, consulte [Exibir e configurar notificações de evento para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

>[!NOTE]
>
>* Um administrador do Workfront pode desbloquear e rebloquear a configuração de uma notificação de evento no Adobe Workfront Classic e na nova experiência do Adobe Workfront. Mas um administrador de grupo pode configurar essa notificação de evento para um grupo somente na nova experiência do Adobe Workfront. Os administradores de grupo que usam o Adobe Workfront Classic podem alternar para a nova experiência do Adobe Workfront para configurar notificações de evento desbloqueadas para um grupo e, em seguida, alternar de volta para o Adobe Workfront Classic para ver as alterações em vigor.
>* Os subgrupos herdam as configurações de notificação de eventos no nível do grupo dos grupos de nível superior acima deles.
>


## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Administrador do sistema</p> </td> 
  </tr> 
 </tbody> 
</table>

## Desbloquear ou rebloquear a capacidade de configurar uma notificação de evento

>[!IMPORTANT]
>
>Ao rebloquear uma notificação, todos os grupos no sistema herdam a notificação exatamente como você a definiu. Isso substitui todas as alterações que os administradores de grupo possam ter feito para seus grupos, então é uma boa ideia consultar-se primeiro.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Email** > **Notificações**.

1. Certifique-se de que o **Notificações de evento** está aberta.
1. Clique no ícone à direita da notificação para alterá-lo para o desbloqueado ![](assets/lock-toggle-button.png) ou bloqueado ![](assets/unlock-toggle-button.png) posição.

   Ou

   Se desejar desbloquear ou bloquear várias notificações de uma só vez, selecione-as e clique no botão Desbloquear ![](assets/unlock-icon-toolbar.png) ou Bloquear ![](assets/lock-icon-locked-qs.png) botão que é exibido na barra de ferramentas acima da lista.

1. Clique em **Salvar**.
1. (Opcional) Se você quiser configurar a notificação de evento para um grupo de nível superior em vez de deixar essa tarefa para o administrador do grupo, é possível fazer um dos seguintes procedimentos:

   * Excluir **Notificações de evento do sistema** na caixa de pesquisa acima da lista de notificações, procure e selecione o nome do grupo de nível superior para listar suas notificações e, em seguida, ative ou inative as notificações desbloqueadas na lista exibida.
   * Clique em **Grupos** no menu à esquerda, clique no nome do grupo de nível superior. Clique em **Notificações de evento** no painel esquerdo, em seguida, configure a notificação de evento desbloqueado, como explicado em [Exibir e configurar notificações de evento para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
