---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Reordenar status do grupo
description: Como administrador de grupo, você pode alterar a ordem dos status de projetos, tarefas e problemas de um grupo que gerencia.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 0cdb4d10-7792-4140-8dec-ef805f668f90
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 6%

---

# Reordenar status do grupo

Como administrador de grupo, você pode alterar a ordem dos status de projetos, tarefas e problemas de um grupo que gerencia.

<!--
The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.
-->

![](assets/statuses.png)

Se houver algum grupo acima do grupo gerenciado por você, os administradores também poderão fazer isso pelo seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

>[!NOTE]
>
>* Um administrador do Workfront pode reordenar os status no nível do sistema. Isso não afeta a ordem dos status dentro dos grupos.
>
>  No entanto, os status em um grupo de nível superior recém-criado herdam a ordem dos status de nível do sistema. (Um novo subgrupo herda a ordem dos status no grupo um nível acima.)
>
>* Você pode reordenar os status bloqueados. Para obter informações sobre status bloqueados, consulte [Criar ou editar o status de um grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
>

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront* </td> 
   <td>Qualquer</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConditions-wf-groups.groups"> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> <p>Você deve ser um administrador de grupo do grupo ou um administrador do Workfront. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acesso administrativo total a um usuário</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Se precisar descobrir o tipo de plano ou licença, contate o administrador do Workfront.

## Ordem padrão dos status

Por padrão, os status são exibidos na seguinte ordem:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th width="33.33%">Projeto</th> 
   <th width="33.33%">Tarefa</th> 
   <th width="33.33%">Problema</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
     <p>Em Andamento</p> 
     <p>Parado</p> 
     <p> Em Espera </p> 
     <p> Em Planejamento </p> 
     <p> Completo </p> 
     <p> Solicitado(a) </p> 
     <p> Aprovado </p> 
     <p> Rejeitado </p> 
     <p> Ideia </p> 
   </td> 
   <td> 
     <p>Novo(a)</p> 
     <p>Em andamento</p> 
     <p>Completo</p> 
   </td> 
   <td> 
     <p>Novo(a)</p> 
     <p>Em andamento</p> 
     <p>Reaberta</p> 
     <p>Aguardando Retorno</p> 
     <p>Em Espera</p> 
     <p>Não é Possível Duplicar</p> 
     <p>Fechado</p> 
     <p>Solucionado</p> 
     <p>Verificação Completa</p> 
     <p>Não Será Resolvido</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

## Reordenar status de tarefas e projetos em um grupo gerenciado por você

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu Principal** no canto superior direito do Adobe Workfront e em **Configurar** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Grupos** e, em seguida, clique no nome do grupo.
1. No painel esquerdo, clique em **Status**.
1. Acima da lista de status exibida, clique na guia **Projetos** ou **Tarefas**.

1. Arraste e solte os status na ordem desejada.

   A nova ordem de status é salva automaticamente.

1. Para testar a nova ordem de status, vá para uma tarefa ou projeto associado ao grupo, clique no status no canto superior direito e verifique se os status exibidos estão na ordem configurada.

## Reordenar status de ocorrências

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu Principal** no canto superior direito do Adobe Workfront e em **Configurar** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Grupos** e, em seguida, clique no nome do grupo.
1. No painel esquerdo, clique em **Status**.
1. Clique na guia **Problemas**.
1. (Opcional) Selecione um tipo de problema (**Relatório de Erros**, **Pedido de Alteração**, **Problema** ou **Solicitação**).

   >[!NOTE]
   >
   >* Não é possível personalizar a ordem dos status para a Lista Mestra.
   >* Recomendamos que você ordene os status para cada tipo de ocorrência da mesma maneira. Para obter mais informações sobre tipos de problemas, consulte [Configurar tipos de solicitação](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Arraste e solte os status na ordem desejada.

   A nova ordem de status é salva automaticamente.

1. Para testar a nova ordem de status, vá para um problema associado ao grupo, clique no status no canto superior direito e verifique se os status exibidos estão na ordem configurada.
