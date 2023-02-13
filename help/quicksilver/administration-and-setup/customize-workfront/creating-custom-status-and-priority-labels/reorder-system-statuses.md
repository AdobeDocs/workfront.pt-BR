---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Reordenar os status do sistema e do grupo
description: Como administrador do Workfront, você pode alterar a ordem do projeto, da tarefa e dos status de emissão para todos no sistema ou para um único grupo.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6fee45a6-1a55-4351-8b08-88244c742ed5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 6%

---

# Reordenar os status do sistema e do grupo

Como administrador do Workfront, você pode alterar a ordem do projeto, da tarefa e dos status de emissão para todos no sistema ou para um único grupo.

<!--The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.-->

![](assets/statuses.png)

>[!NOTE]
>
>* Reordenar os status no nível do sistema não afeta a ordem dos status nos grupos.
>
>  No entanto, os status em um grupo de nível superior recém-criado herdam a ordem dos status de nível de sistema. (Um novo subgrupo herda a ordem dos status no grupo um nível acima.)
>
>* Você pode reordenar os status bloqueados. Para obter informações sobre status bloqueados, consulte [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
>* Os administradores de grupo também podem reorganizar os status usados em seus grupos. Para obter mais informações, consulte [Reordenar os status do grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/reorder-group-statuses-from-groups-area.md).
>


## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront* </td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> <p>Você deve ser um administrador do Workfront. Para obter informações sobre administradores do Workfront, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Se precisar descobrir qual plano ou tipo de licença você tem, entre em contato com o administrador da Workfront.

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
    <ul> 
     <li>Em Andamento</li> 
     <li>Parado</li> 
     <li> Em Espera </li> 
     <li> Em Planejamento </li> 
     <li> Completo </li> 
     <li> Solicitado(a) </li> 
     <li> Aprovado </li> 
     <li> Rejeitado </li> 
     <li> Ideia </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>Novo(a)</li> 
     <li>Em andamento</li> 
     <li>Completo</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>Novo(a)</li> 
     <li>Em andamento</li> 
     <li>Reaberta</li> 
     <li>Aguardando Retorno</li> 
     <li>Em Espera</li> 
     <li>Não é Possível Duplicar</li> 
     <li>Fechado</li> 
     <li>Solucionado</li> 
     <li>Verificação Completa</li> 
     <li>Não Será Resolvido</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Reordenar status para tarefas e projetos em todo o sistema ou para um grupo

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Preferências do projeto > Status**.
1. (Condicional) Se estiver reorganizando status para um grupo, comece a digitar o nome do grupo na caixa no canto superior direito e clique no nome quando ele for exibido.

   ![](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. Acima da lista Status que é exibida, clique no botão **Projetos** ou **Tarefas** guia .

1. Arraste e solte os status na ordem desejada.

   A nova ordem de status é salva automaticamente.

1. Para testar a nova ordem de status, vá para uma tarefa ou projeto, clique no status no canto superior direito e verifique se os status exibidos estão na ordem configurada.

## Reordenar status para problemas

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Preferências do projeto > Status.**
1. (Condicional) Se estiver reorganizando status para um grupo, comece a digitar o nome do grupo na caixa no canto superior direito e clique no nome quando ele for exibido.

   ![](assets/issue-statuses-group-name.png)

1. Clique no botão **Problemas** guia .
1. (Opcional) Selecione um tipo de problema (**Relatório de erros**, **Alterar ordem**, **Problema** ou **Solicitação**).

   >[!NOTE]
   >
   >* Não é possível personalizar a ordem dos status da Lista Principal.
   >* Recomendamos que você ordene os status de cada tipo de edição da mesma maneira. Para obter mais informações sobre tipos de problemas, consulte [Configurar tipos de solicitação](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).


1. Arraste e solte os status na ordem desejada.

   A nova ordem de status é salva automaticamente.

1. Para testar a nova ordem de status, vá para uma ocorrência, clique no status no canto superior direito e verifique se os status exibidos estão na ordem configurada.
