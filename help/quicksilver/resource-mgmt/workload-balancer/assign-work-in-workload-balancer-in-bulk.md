---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Atribuir trabalho em massa usando o Balanceador de carga de trabalho
description: Você pode atribuir recursos a várias tarefas e problemas em massa usando o Balanceador de carga de trabalho do Adobe Workfront.
author: Lisa
feature: Resource Management
exl-id: fb0f80d3-7da4-4f5f-857d-3fb518ba12e2
TQID: https://experienceleague.adobe.com/6QlIfRh94tpLTZF6x5LU2BueTjShzNsaKxb45CEylqA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: c33d85a1-be85-4290-854c-87408c10aa80
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 73c78912e15a03bfd09c127e39d94bf5af42b8e2
workflow-type: tm+mt
source-wordcount: 1242
ht-degree: 5%

---

# Atribuir trabalho em massa usando o Balanceador de carga de trabalho

<!--Audited: 07/2024-->

Você pode atribuir recursos a várias tarefas e problemas em massa usando o Balanceador de carga de trabalho do Adobe Workfront.

Para obter informações gerais sobre como atribuir trabalho a usuários usando o Balanceador de carga de trabalho, consulte [Visão geral da atribuição de trabalho no Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

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
   <td><p>Padrão</p>
       <p>Planejar, ao usar o Balanceador de carga de trabalho na área Recursos; Trabalhar, ao usar o Balanceador de carga de trabalho de uma equipe ou projeto</p></td>
  </tr>
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Editar acesso ao seguinte:</p> 
    <ul> 
     <li>Gerenciamento de recursos</li> 
     <li>Projetos</li> 
     <li>Tarefas</li> 
     <li>Problemas</li> 
    </ul>
   </td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td>Contribuir com permissões ou mais altas para projetos, tarefas e problemas que incluem Fazer atribuições</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações para fazer atribuições em massa no Balanceador de carga de trabalho

* Você pode gerenciar rapidamente atribuições de recursos para várias tarefas e problemas em um ou mais projetos. As alterações nas atribuições ficam visíveis no Balanceador de carga de trabalho imediatamente.
* Não é possível atribuir recursos a itens de trabalho que estão concluídos ou a itens que estão em um projeto concluído.
* Você pode fazer o seguinte ao atribuir funções de trabalho e usuários em massa:

   * Substitua as atribuições entre usuários e funções em todas as combinações válidas.
   * Cancele a atribuição de um usuário de todos os seus itens de trabalho.

**EXEMPLOS**

* Você é responsável por fazer atribuições de usuários em vários projetos novos. Os projetos foram originalmente criados a partir de modelos e as funções de trabalho já estão atribuídas a várias tarefas nos projetos. Você deseja atribuir um usuário específico, Jackie Simms, a todas as tarefas atualmente atribuídas a uma função de trabalho. Você pode usar a função Substituir para atribuir essas tarefas a Jackie Simms.
* 45 tarefas em 3 projetos diferentes são atribuídas a Jackie Simms. Jackie deixa a organização, e agora você precisa reatribuir suas tarefas para outro usuário. Você pode usar a função Substituir para atribuir essas tarefas à nova pessoa.
* Dez tarefas em dois projetos diferentes são atribuídas a outro usuário, Rick Kuvec. Você percebe que Rick foi designado para essas tarefas por engano, mas você não tem certeza de a quem eles precisam ser atribuídos neste momento. Você precisa desatribuir Rick para todas as tarefas ao mesmo tempo. Você pode usar a função Cancelar atribuição para remover Rick dessas tarefas.

## Atribuir trabalho em massa no Balanceador de carga de trabalho

1. Vá para o Balanceador de carga de trabalho onde deseja atribuir trabalho.

   Você pode atribuir trabalho aos usuários usando o Balanceador de carga de trabalho na área Recursos, no projeto ou no nível da equipe. Para obter mais informações sobre onde o Balanceador de carga de trabalho está localizado na Workfront, consulte [Localizar o Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).


1. Clique em **Atribuições em massa** ![Atribuições em massa](assets/bulk-assignments-wb.png) na parte superior do Balanceador de carga de trabalho.

   O painel Atribuições em massa é aberto à direita do Balanceador de carga de trabalho.

1. (Condicional) Se você estiver acessando o Balanceador de carga de trabalho da área de Recursos ou de uma equipe, expanda o menu suspenso **Projeto: Nome** e use os modificadores de filtro para selecionar o projeto ou projetos para os quais deseja fazer atribuições. Você pode selecionar projetos por Nome (esta é a opção padrão) ou por Status.

   Para obter informações sobre modificadores de filtro Workfront, consulte [Filtros e modificadores de condição](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >O Nome do projeto é selecionado por padrão quando você acessa o Balanceador de carga de trabalho de um projeto.

   ![Nome do projeto em atribuições em massa](assets/project-name-status-dropdown-bulk-assignments-wb.png)

1. (Opcional) Clique em **Selecionar tarefas do projeto** para selecionar a(s) tarefa(s) para a(s) qual(is) você deseja fazer atribuições. Em seguida, no menu suspenso **Tarefa: Nome**, selecione as tarefas por Nome (esta é a opção padrão) ou Status e use os modificadores de filtro para procurar tarefas específicas.

   Para obter informações sobre modificadores de filtro Workfront, consulte [Filtros e modificadores de condição](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >Não é possível selecionar tarefas com o status Concluído.

   ![Status da tarefa em atribuições em massa](assets/task-name-status-dropdown-bulk-assignments-wb.png)

   >[!TIP]
   >
   >Deixe essa seleção em branco se quiser fazer atribuições em massa para problemas e tarefas.

1. (Opcional) Clique no ícone **Excluir** ![Excluir ícone](assets/delete.png) ao lado de um dos critérios selecionados

   Ou

   Clique em **Limpar tudo** no canto superior direito do painel Atribuições em massa para remover todas as seleções.

1. Selecione uma das seguintes opções e continue com as etapas descritas abaixo:

   * [Substituir recurso](#replace-user)
   * [Cancelar atribuição de recurso](#unassign-user)

   >[!TIP]
   >
   >Se nenhum item corresponder aos filtros selecionados, essas opções estarão esmaecidas.

<!--

### Assign user {#assign-user}

When you assign a user using Bulk Assignments in the Workload Balancer, the following things occur:

* A user is assigned to all work items currently assigned to a specified role within the selected projects.
* The user is not assigned to the following types of work items:

   * Items that are already assigned to a user.
   * Completed items.

* If the user you selected is not associated with the specified role, the role is replaced by the user in the user's Primary Role.

To assign a user to work items previously assigned to job roles:

1. Start assigning work items using Bulk Assignments in the Workload Balancer as described above and select **Assign**. 

1. In the **Role assignment** field, click the drop-down arrow to choose from a list of roles. Only roles currently assigned within the specified projects are displayed. This is a required field. 

   ![Role assignment](assets/bulk-assignments-workload-balancer-assign-selected.png)

1. In the **User to assign** field, click the drop-down arrow to choose from a list of suggested users or to type another user's name.

   Select users from the following areas:

   * **Suggested Assignments**: Users who can fulfill the selected role and who match the criteria for Smart Assignments. For more information, see [Smart assignments overview](../../manage-work/tasks/assign-tasks/smart-assignments.md).
   * **Other Assignments**: All users in the system who can fulfill the selected role. 
   
      >[!TIP]
      >
      >Only the first 50 users are listed in the Other Assignments area.


   After selecting a user, Workfront displays a note about the number of items where the user you specified will be assigned and what job role they will replace.

   >[!TIP]
   >
   >All the roles of the user display in the list, under the user's name.


1. Click **Assign**.

   The specified roles are replaced with the users that you selected.

   You receive a confirmation about how many work items have had the selected role replaced with the selected user.

   ![Bulk assignment confirmation](assets/bulk-assign-user-confirmation-before-assigning-nwe-350x83.png)

-->

### Substituir recurso {#replace-user}

Você pode substituir um recurso que já está atribuído a itens de trabalho por outro recurso nos projetos selecionados.

A substituição do recurso pode ser:

* Função com função
* Usuário com usuário
* Usuário com função
* Função com usuário

Quando você substitui um recurso por outro usando Atribuições em massa no Balanceador de carga de trabalho, as seguintes situações ocorrem:

* O recurso de substituição é atribuído a todos os itens de trabalho atualmente atribuídos ao recurso original dentro dos projetos selecionados.
* O novo recurso não está atribuído a nenhum item de trabalho já marcado como Concluído.
* Para substituição de usuário por usuário, se a função associada ao primeiro usuário não corresponder a nenhuma função do segundo usuário, o segundo usuário será atribuído em sua Função principal.

Para substituir um recurso por outro recurso:

1. Selecione os itens de trabalho na área de atribuições em massa do Balanceador de carga de trabalho conforme descrito acima e selecione **Substituir recurso**.
1. No campo **Recurso atribuído no momento**, clique na seta suspensa para escolher em uma lista de recursos. Somente os recursos atualmente atribuídos a itens de trabalho incompletos dentro dos projetos especificados são exibidos. Este campo é obrigatório.

   ![Substituir recurso](assets/bulk-assignments-workload-balancer-replace-selected.png)

1. No campo **Recurso a ser atribuído**, clique na seta suspensa para escolher de uma lista de recursos sugeridos ou para digitar outra função de trabalho ou nome de usuário. Por padrão, os recursos listados primeiro correspondem aos critérios das Atribuições inteligentes. Para obter mais informações, consulte [Visão geral das atribuições inteligentes](../../manage-work/tasks/assign-tasks/smart-assignments.md).

   O Workfront exibe uma observação sobre o número de itens em que o recurso atribuído atualmente substituirá o segundo recurso.

1. Clique em **Substituir**.

   O primeiro recurso é substituído pelo segundo em todos os itens de trabalho do projeto ou tarefa selecionada.

   Você receberá uma confirmação sobre quantos itens de trabalho tiveram a atribuição original substituída pelo segundo recurso selecionado.

### Cancelar atribuição de recurso {#unassign-user}

Você pode desatribuir um recurso de todos os itens de trabalho aos quais ele está atribuído nos projetos selecionados.

Quando você cancela a atribuição de um usuário de todas as atribuições usando Atribuições em massa no Balanceador de carga de trabalho, as seguintes situações ocorrem:

* O usuário especificado é removido de todos os itens de trabalho aos quais está atribuído.
* Se o usuário não atribuído estiver associado a funções de trabalho, as funções de trabalho permanecerão atribuídas aos itens de trabalho quando o usuário for removido.

* Se o usuário especificado for atribuído a itens de trabalho concluídos, o usuário permanecerá atribuído a esses itens de trabalho.

Para obter mais informações sobre atribuições de usuários e funções de trabalho, consulte [Visão geral da atribuição de trabalho no Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Para desatribuir um usuário dos itens de trabalho nos projetos selecionados ou para as tarefas ou problemas selecionados nas quais ele está atribuído:

1. Selecione os itens de trabalho na área de atribuições em massa do Balanceador de carga de trabalho conforme descrito acima e selecione **Cancelar atribuição do recurso**.

1. No campo **Usuário a ser desatribuído**, clique na seta suspensa para escolher em uma lista de usuários. Somente os usuários atualmente atribuídos a itens de trabalho incompleto nos projetos especificados são exibidos. Este campo é obrigatório.

   ![Cancelar atribuição de usuário](assets/bulk-assignments-workload-balancer-unassign-selected.png)

   O Workfront exibe uma observação sobre o número de itens para os quais o usuário atribuído no momento terá a atribuição cancelada.

1. Clique em **Cancelar atribuição**.\
   Você recebe uma confirmação sobre o número de itens de trabalho dos quais o usuário especificado foi removido.




