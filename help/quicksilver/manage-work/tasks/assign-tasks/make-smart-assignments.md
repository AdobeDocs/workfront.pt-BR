---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Faça atribuições inteligentes
description: Você pode usar atribuições inteligentes para identificar quem é o melhor usuário para concluir o trabalho. As atribuições inteligentes são sugestões para usuários, funções ou equipes que a Adobe Workfront apresenta ao atribuir itens de trabalho a recursos com base em um algoritmo que determina o recurso mais apropriado para o trabalho. Para obter informações sobre atribuições inteligentes, consulte Visão geral das atribuições inteligentes.
author: Lisa
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/0EhPmb9Y3Vus-62FzgaPy-gtb4ioBmtVwt6bf3axWXU
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 380
ht-degree: 11%

---

# Fazer atribuições inteligentes

<!--Audited: 07/2024-->

Você pode usar atribuições inteligentes para identificar quem é o melhor usuário para concluir o trabalho.

As atribuições inteligentes são sugestões para usuários, funções ou equipes que a Adobe Workfront apresenta quando você atribui itens de trabalho a recursos. O Workfront baseia suas sugestões em um algoritmo que determina o recurso mais apropriado para a tarefa.

<!--<span class="preview">There are two separate algorithms in Workfront that calculate smart assignments that work differently for tasks and for issues.</span> -->

Para obter mais informações sobre os critérios usados na determinação de atribuições inteligentes, consulte [Visão geral das atribuições inteligentes](/help/quicksilver/manage-work/tasks/assign-tasks/smart-assignments.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td> <p>Padrão</p>
   <p>Trabalho ou maior</p>
   </td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a tarefas e problemas</p> <p>Acesso de visualização ou superior aos Projetos</p> </td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td>
   <td>Contribuir com permissões ou superiores com a capacidade de fazer atribuições em tarefas e problemas</td>
  </tr>
 </tbody>
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Fazer atribuições inteligentes

As atribuições inteligentes estão disponíveis na maioria dos locais onde você pode fazer atribuições no Workfront.

1. Vá para as seguintes áreas e clique no campo **Atribuições** ou **Atribuir a este campo**:

   * Uma lista de tarefas ou problemas ou um relatório
   * Um cabeçalho de tarefa ou problema
   * O painel Resumo de tarefas ou problemas
   * Uma tarefa ou problema no Balanceador de carga de trabalho
     <!--* <span class="preview">A New Task</span> or New Issue box, as you add <span class="preview">a new task</span> or issue to a project-->

1. Coloque o cursor no campo Assignments e aguarde dois segundos.

   <!--
   For issues, the smart assignments display in the following sections: 
      * **Users and teams**
      * **Job roles**
        ![Smart assignments issue header](assets/smart-assignments-issue-header.png)
        -->

   As atribuições inteligentes são exibidas nas seguintes seções<!--, depending on which phase of the algorithm's calculation identified the assignments-->:

   <!--* <span class="preview">**Suggested assignments**: Displays assignments identified in the first phase of the task smart assignment algorithm.</span> -->
   * **Usuários e equipes** ou **Funções de trabalho** <!--or **Rate card job roles**: Assignments identified in the second phase of the task smart assignment's algorithm calculation.-->

   ![Exemplo de atribuições inteligentes na lista de tarefas](assets/smart-assignments-task-list.png)

   Para obter mais informações, consulte [Visão geral das atribuições inteligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

1. Selecione o recurso na lista de recomendações clicando no nome.

1. (Opcional) Clique em **Atribuir a mim** para atribuir o item de trabalho a você mesmo.

   >[!TIP]
   >
   >Se não houver sugestões, a lista de sugestões não será aberta.

1. (Opcional) Se não quiser usar um dos usuários recomendados da lista de atribuições inteligentes, comece digitando o nome do recurso desejado e selecione o nome quando ele aparecer na lista.
1. Clique em **Inserir** para fazer a atribuição.

   O usuário selecionado está atribuído à tarefa ou problema.
