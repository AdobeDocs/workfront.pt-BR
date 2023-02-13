---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Bloquear ou desbloquear uma folha de horas e uma preferência de hora do grupo
description: Se você for um administrador de grupo, poderá configurar e bloquear uma folha de ponto e uma preferência de hora para seu grupo depois que um administrador do Workfront desbloqueá-la no nível do sistema.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5b36106f-d521-4cc1-9f1f-647415c282b4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

# Bloquear ou desbloquear uma folha de horas e uma preferência de hora do grupo

Se você for um administrador de grupo, poderá configurar e bloquear uma folha de ponto e uma preferência de hora para seu grupo depois que um administrador do Workfront desbloqueá-la no nível do sistema.

Bloquear uma preferência do Adobe Workfront garante que todos no seu grupo e em seus subgrupos estejam usando a mesma configuração para essa preferência. Embora ainda seja possível reconfigurar uma preferência bloqueada, os administradores de grupo não podem fazer isso para subgrupos inferiores.

Por outro lado, desbloquear uma preferência no nível do grupo permite que os administradores de subgrupo tenham mais flexibilidade para gerenciar a maneira como seus grupos trabalham com esses itens. Quando uma preferência é desbloqueada, os administradores de grupo podem reconfigurá-la para esses subgrupos.

Isso é paralelo à capacidade de um administrador do Workfront bloquear ou desbloquear uma preferência para todos no sistema.

Para obter informações sobre como um administrador do Workfront pode bloquear ou desbloquear uma folha de ponto e uma preferência de hora para todos os grupos no sistema, consulte [Configurar preferências de hora e folha de ponto](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Para obter informações sobre como configurar uma folha de ponto e a preferência de hora para um grupo, consulte [Configurar as preferências de hora e folha de ponto para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

<!--
Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
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

## Bloquear ou desbloquear uma folha de horas e uma preferência de hora do grupo

>[!TIP]
>
>Se você for um administrador do Workfront, é possível ignorar as etapas 1 a 4, acessando Configurar > Folha de Horas e Horas > Preferências e, em seguida, pesquisando o nome do grupo na caixa na parte superior da página.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Grupos**.
1. Clique no nome do grupo onde deseja bloquear ou desbloquear uma folha de ponto e uma preferência de horas.
1. No painel esquerdo, clique em **Folhas de Horas e Preferências de Horas**.

1. Na página exibida, execute um dos seguintes procedimentos:

   * Se você quiser que os administradores de grupos abaixo do seu grupo possam configurar uma preferência para seus grupos, desbloqueie-a ![](assets/unlock-toggle-button.png).
   * Se quiser que todos os grupos abaixo da sua usem a sua configuração como preferência, verifique se ela está bloqueada ![](assets/lock-toggle-button.png) (esse é o padrão).

      >[!IMPORTANT]
      >
      >É importante se comunicar com os administradores e usuários nos grupos abaixo da sua, para garantir que todas as necessidades sejam contabilizadas na forma como você configura uma preferência bloqueada. Ao bloqueá-lo, sua configuração é herdada por qualquer subgrupo abaixo. E se a preferência tiver sido desbloqueada por qualquer período de tempo, sua configuração substituirá aquelas que os administradores de grupo em subgrupos inferiores podem ter feito.

1. Clique em **Salvar**.
