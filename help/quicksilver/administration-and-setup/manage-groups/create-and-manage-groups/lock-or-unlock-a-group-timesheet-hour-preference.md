---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Bloquear ou desbloquear uma planilha de horas de grupo e uma preferência de horas
description: Se você for um administrador de grupo, poderá configurar e bloquear uma folha de horas e uma preferência de horas para seu grupo depois que um administrador do Workfront desbloqueá-lo no nível do sistema.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5b36106f-d521-4cc1-9f1f-647415c282b4
source-git-commit: a42a167447d2f11b5502e4a0953b5e7eec2e67b1
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# Bloquear ou desbloquear uma planilha de horas e uma preferência de horas do grupo

Se você for um administrador de grupo, poderá configurar e bloquear uma folha de horas e uma preferência de horas para seu grupo depois que um administrador do Workfront desbloqueá-lo no nível do sistema.

Bloquear uma preferência de Adobe Workfront garante que todos no seu grupo e em seus subgrupos usem a mesma configuração para essa preferência. Embora ainda seja possível reconfigurar uma preferência que você bloqueie, os administradores de grupo não podem fazer isso para subgrupos inferiores.

Por outro lado, desbloquear uma preferência no nível do grupo permite que os administradores de subgrupos tenham mais flexibilidade para gerenciar a forma como seus grupos trabalham com esses itens. Quando uma preferência é desbloqueada, os administradores de grupo podem reconfigurá-la para esses subgrupos.

Isso é paralelo à capacidade que um administrador do Workfront tem de bloquear ou desbloquear uma preferência para todos no sistema.

Para obter informações sobre como um administrador do Workfront pode bloquear ou desbloquear uma planilha de horas e uma preferência de horas para todos os grupos no sistema, consulte [Configurar preferências de horas e folha de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Para obter informações sobre como configurar uma planilha de horas e a preferência de horas para um grupo, consulte [Configurar preferências de horas e folha de horas para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

<!--
Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
-->

>[!NOTE]
>
>* Configurar uma preferência desbloqueada para um grupo não afeta essa preferência para nenhum subgrupo abaixo do grupo.
>
>  No entanto, quando um novo subgrupo é criado, ele herda as configurações de preferência e o estado bloqueado ou desbloqueado do grupo imediatamente acima dele.
>
>* Se você mover um grupo em um grupo que tenha uma preferência bloqueada, o grupo movido herdará essa preferência e ficará bloqueado para o grupo movido.
>* Se você mover um grupo em um grupo que tenha uma preferência desbloqueada, o grupo movido não será afetado por essa preferência.
>
>  Se a preferência no grupo movido estiver bloqueada no momento da movimentação, ela permanecerá bloqueada, mas o administrador do grupo poderá desbloqueá-la agora porque ela está desbloqueada para o grupo pai.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plano</p></td>
  </tr>
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Você deve ser um administrador de grupo do grupo ou um administrador do sistema.</td>
  </tr>
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Bloquear ou desbloquear uma planilha de horas e uma preferência de horas do grupo

>[!TIP]
>
>Se você for um administrador do Workfront, ignore as etapas 1 a 4. Para isso, acesse Configurar > Folhas de horas e horas > Preferências e, em seguida, procure o nome do grupo na caixa na parte superior da página.

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos**.
1. Clique no nome do grupo no qual você deseja bloquear ou desbloquear a preferência de horas e folhas de horas.
1. No painel esquerdo, clique em **Folhas de horas e Preferências de horas**.

1. Na página exibida, siga um destes procedimentos:

   * Se quiser que os administradores de grupos abaixo do seu grupo possam configurar uma preferência para seus grupos, desbloqueie-a ![Desbloquear a opção](assets/unlock-toggle-button.png).
   * Se quiser que todos os grupos abaixo do seu usem sua configuração como preferência, verifique se ela está bloqueada ![Bloquear alternância](assets/lock-toggle-button.png) (esse é o padrão).

     >[!IMPORTANT]
     >
     >É importante se comunicar com os administradores e usuários em grupos abaixo do seu para garantir que todas as necessidades sejam levadas em conta na maneira como você configura uma preferência bloqueada. Ao bloqueá-la, sua configuração para ela é herdada por qualquer subgrupo abaixo de. E se a preferência tiver sido desbloqueada por qualquer período, a configuração substituirá aquelas que os administradores de grupos em subgrupos inferiores podem ter feito.

1. Clique em **Salvar**.
