---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Desbloquear ou bloquear a configuração de notificações de eventos para todos os grupos
description: Se você for um administrador do Adobe Workfront, poderá desbloquear ou rebloquear a capacidade de administradores de grupos configurarem uma notificação de eventos para grupos de nível superior que gerenciam. A configuração de uma notificação de evento consiste em ativá-la ou desativá-la.
author: Lisa, Nolan
feature: System Setup and Administration
role: Admin
exl-id: 056d76c1-7e9b-49b9-974a-75765e53b7fd
source-git-commit: 1c0a656f2603c5decabd2bb4e88da1b9530f9e1c
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# Desbloquear ou bloquear a configuração de notificações de eventos para todos os grupos

Se você for um administrador do Adobe Workfront, poderá desbloquear ou rebloquear a capacidade de administradores de grupos configurarem uma notificação de eventos para grupos de nível superior que gerenciam. A configuração de uma notificação de evento consiste em ativá-la ou desativá-la.

Se houver algum grupo acima do grupo gerenciado por você, os administradores também poderão fazer isso pelo seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

Quando um administrador configura uma notificação de evento para um grupo, a configuração afeta os usuários para os quais esse grupo, ou um de seus subgrupos, é o Grupo padrão. Em seus perfis de usuário, esses usuários veem as notificações de evento ativadas para seu Grupo inicial, em vez das notificações de evento ativadas em todo o sistema. Para obter mais informações, consulte [Exibir e configurar notificações de eventos para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

>[!NOTE]
>
>* Um administrador do Workfront pode desbloquear e rebloquear a configuração de uma notificação de evento no Adobe Workfront Classic e na nova experiência do Adobe Workfront. Mas um administrador de grupo pode configurar essa notificação de evento para um grupo somente na nova experiência do Adobe Workfront. Os administradores de grupo que usam o Adobe Workfront Classic podem alternar para a nova experiência do Adobe Workfront para configurar notificações de eventos desbloqueados para um grupo e, em seguida, alternar de volta para o Adobe Workfront Classic para ver as alterações em vigor.
>* Os subgrupos herdam configurações de notificação de eventos de nível de grupo dos grupos de nível superior acima deles.
>

## Requisitos de acesso

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
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Administrador do sistema</p> </td> 
  </tr> 
 </tbody> 
</table>

## Desbloquear ou bloquear novamente a capacidade de configurar uma notificação de evento

>[!IMPORTANT]
>
>Quando você bloquear novamente uma notificação, todos os grupos no sistema herdarão a notificação exatamente como você a definiu. Isso substitui todas as alterações que os administradores de grupo possam ter feito em seus grupos. Portanto, é uma boa ideia consultar esses grupos primeiro.

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **E-mail** > **Notificação**.

1. Verifique se **Notificações de Eventos** está aberta.
1. Clique no ícone à direita da notificação para alterná-lo para a tag bloqueada ![Ícone Bloquear](assets/lock-toggle-button.png) ou desbloqueado ![Ícone Desbloquear](assets/unlock-toggle-button.png) posição.

   Ou

   Para desbloquear ou bloquear várias notificações de uma só vez, selecione-as e, em seguida, clique no botão Desbloquear ![Ícone Desbloquear](assets/unlock-icon-toolbar.png) ou Bloqueio ![Ícone Bloquear](assets/lock-icon-locked-qs.png) botão que é exibido na barra de ferramentas acima da lista.

1. Clique em **Salvar**.
1. (Opcional) Se quiser configurar a notificação de eventos para um grupo de nível superior, em vez de deixar essa tarefa para o administrador do grupo, você pode executar um dos seguintes procedimentos:

   * Excluir **Notificações de Eventos do Sistema** na caixa pesquisar acima da lista de notificações, procure e selecione o nome do grupo de nível superior para listar suas notificações e, em seguida, ative ou desative as notificações desbloqueadas na lista exibida.
   * Clique em **Grupos** no menu esquerdo, em seguida, clique no nome do grupo de nível superior. Clique em **Notificações de Eventos** no painel esquerdo e configure a notificação de evento desbloqueada, conforme explicado em [Exibir e configurar notificações de eventos para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
