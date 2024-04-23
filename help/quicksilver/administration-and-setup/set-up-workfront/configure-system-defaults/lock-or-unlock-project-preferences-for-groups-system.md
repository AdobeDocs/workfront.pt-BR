---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Bloquear ou desbloquear as preferências do projeto para todos os grupos no sistema
description: Os grupos em sua organização podem precisar de uma preferência de projeto configurada de forma diferente para seus fluxos de trabalho exclusivos. Você pode desbloquear a preferência para todos os grupos em toda a organização para que eles possam configurá-la por conta própria.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f5a94eaf-ebb8-424b-80ff-ba40cc985a6e
source-git-commit: 3e97df265df83965d094d8723fe76043ff4af80e
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# Bloquear ou desbloquear as preferências do projeto para todos os grupos no sistema

Os grupos em sua organização podem precisar de uma preferência de projeto configurada de forma diferente para seus fluxos de trabalho exclusivos. Você pode desbloquear a preferência para todos os grupos em toda a organização para que eles possam configurá-la por conta própria.

Quando uma preferência é desbloqueada e o administrador do grupo a modifica, os projetos associados ao grupo adquirem a configuração dessa preferência na configuração de nível do grupo, em vez da configuração de nível do sistema.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Plano]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador.</p> <p><b>NOTA</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais no seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Sobre preferências bloqueadas e desbloqueadas

Bloquear uma preferência de projeto, tarefa ou problema configurada no nível do sistema garante que todos estejam usando a mesma configuração para essa preferência. Embora você ainda possa reconfigurar uma preferência bloqueada, os administradores de grupos não podem reconfigurá-la para seus grupos.

Por outro lado, desbloquear uma preferência de projeto, tarefa ou problema permite que os administradores de grupo tenham mais flexibilidade para gerenciar a forma como seus grupos trabalham com esses itens. Quando uma preferência é desbloqueada, os administradores de grupos podem reconfigurá-la para seus grupos.

Se um campo não tiver uma opção de bloquear/desbloquear, ele não poderá ser desbloqueado para que administradores de grupo definam configurações no nível do grupo. A configuração só está disponível no nível do sistema.

Para obter instruções sobre como bloquear ou desbloquear uma preferência de projeto, tarefa ou problema no nível do sistema, consulte [Configurar preferências de tarefas e problemas em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>Depois de um [!DNL Workfront] administrador desbloqueia uma preferência no nível do sistema, qualquer administrador de grupo pode configurá-la e bloqueá-la para garantir que todos no grupo e nos subgrupos abaixo estejam usando a mesma configuração. Isso é paralelo à capacidade de um [!DNL Workfront] o administrador precisa configurar e bloquear uma preferência para todos no sistema. Para obter mais informações, consulte [Configurar as preferências do projeto para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) e [Preferência Bloquear ou desbloquear um projeto, tarefa ou problema para subgrupos](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

## Desbloquear uma preferência de projeto para que grupos possam configurá-la

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront]e, em seguida, clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Preferências do projeto]** e, em seguida, clique em **[!UICONTROL Projetos]**.

1. Siga um destes procedimentos:

   * Se você quiser que os administradores de grupos possam configurar uma preferência para seus grupos, desbloqueie-a ![](assets/unlock-toggle-button.png).
   * Se desejar que todos os grupos usem sua configuração para uma preferência, certifique-se de que ela esteja bloqueada (esse é o padrão).

     >[!IMPORTANT]
     >
     >Recomendamos que você se comunique com os administradores e usuários em grupos em todo o sistema para garantir que todas as necessidades sejam consideradas na maneira como você configura uma preferência bloqueada. Ao bloqueá-lo, sua configuração para ele é herdada por todos os grupos no sistema. E se a preferência tiver sido desbloqueada por qualquer período, sua configuração substituirá aquelas que os administradores de grupo podem ter feito.

1. Clique em **[!UICONTROL Salvar]**.
