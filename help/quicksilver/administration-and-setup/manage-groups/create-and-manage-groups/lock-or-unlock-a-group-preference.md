---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Bloquear ou desbloquear um projeto, tarefa ou emitir preferência para subgrupos
description: Como administrador de grupo, você pode configurar e bloquear um projeto, uma tarefa ou uma preferência de emissão se um administrador do Workfront tiver desbloqueado o projeto no nível do sistema.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 05c32b6f-52e1-46a7-9011-633713422f3d
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# Bloquear ou desbloquear um projeto, tarefa ou emitir preferência para subgrupos

Como administrador de grupo, você pode configurar e bloquear um projeto, uma tarefa ou uma preferência de emissão se um administrador do Workfront tiver desbloqueado o projeto no nível do sistema.

Bloquear um projeto, tarefa ou preferência de emissão configurada no nível garante que todos no seu grupo e em seus subgrupos estejam usando a mesma configuração para essa preferência. Embora você ainda possa reconfigurar uma preferência bloqueada para o seu grupo, os administradores de grupo não podem reconfigurá-la para grupos.

Por outro lado, desbloquear um projeto, tarefa ou preferência de emissão permite que os administradores de grupo tenham mais flexibilidade para gerenciar a maneira como seus grupos trabalham com esses itens. Quando uma preferência é desbloqueada, os administradores de grupo podem reconfigurá-la para esses subgrupos.

Isso é paralelo à capacidade de um administrador do Workfront bloquear ou desbloquear uma preferência para todos no sistema.

Para obter informações sobre como um administrador do Workfront pode bloquear ou desbloquear uma preferência para todos os grupos no sistema, consulte [Bloquear ou desbloquear preferências de projeto para todos os grupos no sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
-->

>[!NOTE]
>
>* Configurar uma preferência desbloqueada para um grupo não afeta essa preferência para qualquer subgrupo abaixo do grupo.
>
>  No entanto, quando um novo subgrupo é criado, ele herda as configurações de preferência e o estado bloqueado ou desbloqueado do grupo imediatamente acima dele.
>
>* Se você mover um grupo em um grupo que tenha uma preferência bloqueada, o grupo movido herdará essa preferência e ele será bloqueado para o grupo movido.
>* Se você mover um grupo sob uma preferência desbloqueada, o grupo movido não será afetado por essa preferência.
>
>  Se a preferência no grupo movido estiver bloqueada no momento da movimentação, ela permanecerá bloqueada, mas o administrador do grupo poderá desbloqueá-la agora, pois ela será desbloqueada para o grupo pai.

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Workfront*</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> <p>Você deve ser um administrador de grupo do grupo ou um administrador do Workfront. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores do grupo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Se precisar descobrir qual plano ou tipo de licença você tem, entre em contato com o administrador da Workfront.

## Bloquear ou desbloquear um projeto de grupo, tarefa ou preferência de emissão

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Grupos**.
1. Clique no nome do grupo onde deseja bloquear ou desbloquear uma preferência de projeto.
1. No painel esquerdo, clique em **Preferências do projeto** ou **Preferências de tarefas e problemas**.

1. Na página exibida, execute um dos procedimentos a seguir para obter uma preferência que seja desbloqueada no nível do sistema ou para um grupo acima do seu grupo:

   * Se você quiser que os administradores de grupos abaixo do seu grupo possam configurar uma preferência para seus grupos, desbloqueie-a ![](assets/unlock-toggle-button.png).
   * Se quiser que todos os grupos abaixo da sua usem a sua configuração como preferência, verifique se ela está bloqueada ![](assets/lock-toggle-button.png).

      >[!IMPORTANT]
      >
      >É importante se comunicar com os administradores e usuários nos grupos abaixo da sua, para garantir que todas as necessidades sejam contabilizadas na forma como você configura uma preferência bloqueada. Ao bloqueá-lo, sua configuração é herdada por qualquer subgrupo abaixo. E se a preferência tiver sido desbloqueada por qualquer período de tempo, sua configuração substituirá aquelas que os administradores de grupo em subgrupos inferiores podem ter feito.

1. Clique em **Salvar**.
