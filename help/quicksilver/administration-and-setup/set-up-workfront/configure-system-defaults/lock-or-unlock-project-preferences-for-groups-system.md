---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Bloquear ou desbloquear preferências de projeto para todos os grupos no sistema
description: Os grupos em sua organização podem precisar de uma preferência de projeto configurada de forma diferente para seus fluxos de trabalho exclusivos. Você pode desbloquear a preferência para todos os grupos em toda a organização para que eles possam configurá-la sozinhos.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f5a94eaf-ebb8-424b-80ff-ba40cc985a6e
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---

# Bloquear ou desbloquear preferências de projeto para todos os grupos no sistema

Os grupos em sua organização podem precisar de uma preferência de projeto configurada de forma diferente para seus fluxos de trabalho exclusivos. Você pode desbloquear a preferência para todos os grupos em toda a organização para que eles possam configurá-la sozinhos.

Quando uma preferência é desbloqueada e o administrador do grupo a modifica, os projetos associados ao grupo adquirem a configuração dessa preferência a partir da configuração de nível de grupo, em vez da configuração de nível de sistema.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador.</p> <p><b>OBSERVAÇÃO</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Sobre preferências bloqueadas e desbloqueadas

Bloquear um projeto, tarefa ou preferência de emissão que você tenha configurado no nível do sistema garante que todos estejam usando a mesma configuração para essa preferência. Embora você ainda possa reconfigurar uma preferência bloqueada, os administradores de grupo não podem reconfigurá-la para seus grupos.

Por outro lado, desbloquear um projeto, tarefa ou preferência de emissão permite que os administradores de grupo tenham mais flexibilidade para gerenciar a maneira como seus grupos trabalham com esses itens. Quando uma preferência é desbloqueada, os administradores de grupo podem reconfigurá-la para seus grupos.

Para obter instruções sobre como bloquear ou desbloquear um projeto, tarefa ou preferência de emissão em nível de sistema, consulte [Configurar preferências de emissão e tarefa em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>Depois de um [!DNL Workfront] O administrador desbloqueia uma preferência no nível do sistema, qualquer administrador de grupo pode configurá-la e bloqueá-la para garantir que todos no grupo e nos subgrupos abaixo estejam usando a mesma configuração. Isso é paralelo à capacidade de uma [!DNL Workfront] o administrador precisa configurar e bloquear uma preferência para todos no sistema. Para obter mais informações, consulte [Configurar preferências de projeto para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) e [Bloquear ou desbloquear um projeto, tarefa ou emitir preferência para subgrupos](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

## Desbloquear uma preferência de projeto para que os grupos possam configurá-la

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Preferências do projeto]**, depois clique em **[!UICONTROL Projetos]**.

1. Siga um destes procedimentos:

   * Se quiser que os administradores de grupo possam configurar uma preferência para seus grupos, desbloqueie-a ![](assets/unlock-toggle-button.png).
   * Se quiser que todos os grupos usem sua configuração como preferência, verifique se ela está bloqueada (esse é o padrão).

      >[!IMPORTANT]
      >
      >Recomendamos que você se comunique com os administradores e usuários em grupos em todo o sistema para garantir que todas as necessidades sejam contabilizadas na forma como você configura uma preferência bloqueada. Ao bloqueá-lo, sua configuração é herdada por todos os grupos no sistema. E se a preferência tiver sido desbloqueada por algum período de tempo, sua configuração substituirá aquelas que os administradores de grupo podem ter feito.

1. Clique em **[!UICONTROL Salvar]**.
