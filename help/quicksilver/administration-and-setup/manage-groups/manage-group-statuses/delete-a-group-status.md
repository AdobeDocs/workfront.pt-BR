---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Excluir um status de grupo
description: Como administrador de grupo, é possível excluir um status de um grupo que você gerencia se ele não estiver configurado como um status obrigatório ou bloqueado no nível do sistema ou para um grupo superior na hierarquia.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: bfce0325-fe6e-459f-96ca-9a5c94c61ed3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---

# Excluir um status de grupo

Como administrador de grupo, é possível excluir um status de um grupo que você gerencia se ele não estiver configurado como um status obrigatório ou bloqueado no nível do sistema ou para um grupo superior na hierarquia.

Se houver algum grupo acima do grupo que você gerencia, os administradores também poderão fazer isso para o seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

>[!NOTE]
>
>Não é possível excluir o seguinte:
>
>* Os status integrados Planejamento, Atual e Concluído. Você pode atualizar seus nomes, editar suas cores e bloqueá-las ou desbloqueá-las, mas elas não podem ser excluídas.
>* Status que estão em um estado pendente de aprovação para pelo menos um objeto associado ao grupo ou a um de seus subgrupos.


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

## Excluir um status de grupo

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Grupos**.
1. Clique no nome do grupo de nível superior.
1. No painel esquerdo, clique em **Status**.
1. Na lista de status que é exibida, passe o mouse sobre o status que deseja excluir, depois clique em **Excluir** quando parece à extrema direita.

   ![](assets/hover-click-delete.jpg)

1. Na caixa exibida, selecione um status para designar um status de substituição para objetos (projetos, tarefas, problemas e processos de aprovação) que estavam usando o status que você está excluindo.

   Somente os status que correspondem ao status que você está excluindo estão disponíveis. Por exemplo, se você estiver excluindo um status que seja igual a Atual, poderá ver somente status que sejam iguais a Atual.

   Além disso, os status que são exibidos dependem se o status que você está excluindo está desbloqueado ou bloqueado:

   * **Se estiver desbloqueado**: Status não ocultos bloqueados e desbloqueados estão disponíveis.

      Juntamente com os status que foram criados para o subgrupo, os status herdados dos grupos de nível do sistema e nível superior são incluídos.

   * **Se estiver bloqueado**: Um dos seguintes é verdadeiro:

      * Se houver outros status bloqueados e não ocultos, somente eles estarão disponíveis.
      * Se não houver um status bloqueado não oculto, o status padrão do Workfront estará disponível, mesmo que esteja oculto ou desbloqueado.

         Para obter informações sobre os status padrão do Workfront, consulte [Acessar a lista de status de projeto do sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md), [Acessar a lista de status de tarefas do sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)e as informações sobre os 4 status de emissão necessários em [Acesse a lista de status de problemas do sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md).

1. Clique em **Excluir status**.

   Se o status excluído for o status padrão desse tipo no grupo, o status de substituição ocorrerá em seu lugar.

   Se o status excluído foi definido como o status padrão do projeto nas preferências do projeto, a preferência agora é definida como o status de substituição.

## Quando um grupo é excluído

Quando um grupo é excluído e substituído por outro grupo, todos os status exclusivos que o grupo excluído teve são adicionados aos status do grupo de substituição. Para obter mais informações, consulte [Status personalizados em um grupo que é movido ou excluído](../../../administration-and-setup/manage-groups/manage-group-statuses/custom-statuses-in-group-moved-or-deleted.md).
