---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Bloquear ou desbloquear uma preferência de projeto, tarefa ou problema para subgrupos
description: Como administrador de grupo, você pode configurar e bloquear uma preferência de projeto, tarefa ou problema se um administrador do Workfront a tiver desbloqueado no nível do sistema.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 05c32b6f-52e1-46a7-9011-633713422f3d
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%

---

# Preferência Bloquear ou desbloquear um projeto, tarefa ou problema para subgrupos

Como administrador de grupo, você pode configurar e bloquear uma preferência de projeto, tarefa ou problema se um administrador do Workfront a tiver desbloqueado no nível do sistema.

Bloquear uma preferência de projeto, tarefa ou problema configurada no nível garante que todos no seu grupo e em seus subgrupos usem a mesma configuração para essa preferência. Embora você ainda possa reconfigurar uma preferência bloqueada para seu grupo, os administradores de grupo não podem reconfigurá-la para grupos.

Por outro lado, desbloquear uma preferência de projeto, tarefa ou problema permite que os administradores de grupo tenham mais flexibilidade para gerenciar a forma como seus grupos trabalham com esses itens. Quando uma preferência é desbloqueada, os administradores de grupo podem reconfigurá-la para esses subgrupos.

Isso é paralelo à capacidade que um administrador do Workfront tem de bloquear ou desbloquear uma preferência para todos no sistema.

Para obter informações sobre como um administrador do Workfront pode bloquear ou desbloquear uma preferência para todos os grupos no sistema, consulte [Bloquear ou desbloquear preferências do projeto para todos os grupos no sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
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
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Novo: Padrão</p>
       <p>Ou</p>
       <p>Atual: Plano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>Você deve ser um administrador de grupo do grupo ou um administrador do sistema.</td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Preferência Bloquear ou desbloquear um projeto, tarefa ou problema de grupo

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos**.
1. Clique no nome do grupo em que deseja bloquear ou desbloquear uma preferência de projeto.
1. No painel esquerdo, clique em **Preferências do projeto** ou **Preferências de tarefas e problemas**.

1. Na página exibida, siga um destes procedimentos para obter uma preferência desbloqueada no nível do sistema ou para um grupo acima do seu grupo:

   * Se quiser que os administradores de grupos abaixo do seu grupo possam configurar uma preferência para seus grupos, desbloqueie-a ![Desbloquear a opção](assets/unlock-toggle-button.png).
   * Se quiser que todos os grupos abaixo do seu usem sua configuração como preferência, verifique se ela está bloqueada ![Bloquear alternância](assets/lock-toggle-button.png).

     >[!IMPORTANT]
     >
     >É importante se comunicar com os administradores e usuários em grupos abaixo do seu para garantir que todas as necessidades sejam levadas em conta na maneira como você configura uma preferência bloqueada. Ao bloqueá-la, sua configuração para ela é herdada por qualquer subgrupo abaixo de. E se a preferência tiver sido desbloqueada por qualquer período, a configuração substituirá aquelas que os administradores de grupos em subgrupos inferiores podem ter feito.

1. Clique em **Salvar**.
