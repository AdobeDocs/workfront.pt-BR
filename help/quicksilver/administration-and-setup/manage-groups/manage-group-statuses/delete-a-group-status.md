---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Excluir um status de grupo
description: Como administrador de grupo, você pode deletar um status de um grupo gerenciado se ele não estiver configurado como um status obrigatório ou bloqueado no nível do sistema ou para um grupo superior na hierarquia.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: bfce0325-fe6e-459f-96ca-9a5c94c61ed3
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 0%

---

# Excluir um status de grupo

Como administrador de grupo, você pode deletar um status de um grupo gerenciado se ele não estiver configurado como um status obrigatório ou bloqueado no nível do sistema ou para um grupo superior na hierarquia.

Se houver algum grupo acima do grupo gerenciado por você, os administradores também poderão fazer isso pelo seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

>[!NOTE]
>
>Não é possível excluir o seguinte:
>
>* Os status incorporados Planejamento, Atual e Concluído. É possível atualizar os nomes, editar as cores e bloqueá-las ou desbloqueá-las, mas elas não podem ser excluídas.
>* Status que estão em um estado pendente de aprovação para pelo menos um objeto associado ao grupo ou um de seus subgrupos.

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

## Excluir um status de grupo

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos**.
1. Clique no nome do grupo de nível superior.
1. No painel esquerdo, clique em **Status**.
1. Na lista de status exibida, passe o mouse sobre o status que deseja excluir e clique em **Excluir** quando ele aparecer à direita.

   ![](assets/hover-click-delete.jpg)

1. Na caixa exibida, selecione um status para designar um status de substituição para objetos (projetos, tarefas, problemas e processos de aprovação) que estavam usando o status que você está excluindo.

   Somente os status que correspondem ao status que você está excluindo estão disponíveis. Por exemplo, se você estiver excluindo um status que equivale a Atual, poderá ver apenas os status que correspondem a Atual.

   Além disso, os status exibidos dependem se o status que você está excluindo é desbloqueado ou bloqueado:

   * **Se estiver desbloqueado**: os status bloqueados e desbloqueados não ocultos estão disponíveis.

     Junto com os status que foram criados para o subgrupo, os status herdados dos grupos de nível do sistema e nível superior são incluídos.

   * **Se estiver bloqueado**: uma destas opções é verdadeira:

      * Se houver outros status bloqueados e não ocultos, somente eles estarão disponíveis.
      * Se não houver um status bloqueado não oculto, o status padrão do Workfront estará disponível, mesmo se estiver oculto ou desbloqueado.

        Para obter informações sobre os status padrão do Workfront, consulte [Acessar a lista de status de projetos do sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md), [Acessar a lista de status de tarefas do sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md) e as informações sobre os 4 status de problemas necessários em [Acessar a lista de status de problemas do sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md).

1. Clique em **Excluir status**.

   Se o status excluído for o padrão para esse tipo no grupo, o status de substituição ocupará seu lugar.

   Se o status de excluído foi definido como o status padrão do projeto nas preferências do projeto, a preferência agora é definida como o status de substituição.

## Quando um grupo é excluído

Quando um grupo é excluído e substituído por outro grupo, todos os status exclusivos que o grupo excluído tinha são adicionados aos status do grupo de substituição. Para obter mais informações, consulte [Status personalizados em um grupo movido ou excluído](../../../administration-and-setup/manage-groups/manage-group-statuses/custom-statuses-in-group-moved-or-deleted.md).
