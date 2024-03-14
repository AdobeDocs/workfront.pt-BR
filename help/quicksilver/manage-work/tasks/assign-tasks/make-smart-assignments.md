---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Fazer atribuições inteligentes
description: Você pode usar atribuições inteligentes para identificar quem é o melhor usuário para concluir o trabalho. As atribuições inteligentes são sugestões para usuários, funções ou equipes que a Adobe Workfront apresenta ao atribuir itens de trabalho a recursos com base em um algoritmo que determina o recurso mais apropriado para o trabalho. Para obter informações sobre atribuições inteligentes, consulte Visão geral das atribuições inteligentes.
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: c50ff48bbc492199b39db17b8c445207209bb6a5
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 0%

---

# Fazer atribuições inteligentes

<!--Audited: 02/2024-->

{{preview-and-fast-release}}

Você pode usar atribuições inteligentes para identificar quem é o melhor usuário para concluir o trabalho.

As atribuições inteligentes são sugestões para usuários, funções ou equipes que a Adobe Workfront apresenta quando você atribui itens de trabalho a recursos. O Workfront baseia suas sugestões em um algoritmo que determina o recurso mais apropriado para a tarefa.

<span class="preview">Há dois algoritmos separados no Workfront para tarefas e problemas. </span>

Para obter mais informações sobre os critérios usados na determinação de atribuições inteligentes, consulte [Visão geral das atribuições inteligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Novo: Padrão</p>
      Ou
      <p>Atual: trabalho ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a tarefas e problemas</p> <p>Acesso de visualização ou superior aos Projetos</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribuir com permissões ou superiores com a capacidade de fazer atribuições em tarefas e problemas</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront. Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Fazer atribuições inteligentes

As atribuições inteligentes estão disponíveis na maioria dos locais onde você pode fazer atribuições no Workfront.

1. Vá para as seguintes áreas e clique no botão **Atribuições** ou **Atribuir esta para** campo:

   * Uma lista de tarefas ou problemas ou um relatório
   * Um cabeçalho de tarefa ou problema
   * O painel Resumo de tarefas ou problemas
   * <span class="preview">Caixa Nova tarefa ou Novo problema ao adicionar uma nova tarefa ou problema a um projeto</span>
   * O campo Atribuições de um item listado na área Página inicial
   * Uma tarefa ou problema no Balanceador de carga de trabalho

1. Coloque o cursor no campo de atribuição e aguarde dois segundos.

   <span class="preview">A variável **Atribuições sugeridas** é exibida.</span> <!--check the casing for "assignments" should be lower case in task lists??-->

   >[!TIP]
   >
   >   O cabeçalho da lista é exibido **Aqui estão algumas recomendações** em vez de **Atribuições sugeridas** em uma lista de problemas.

   ![](assets/smart-assignments-task-header-nwe-350x302.png)

   Para problemas, as sugestões de atribuição inteligente são exibidas no **Atribuições sugeridas** área.

   Para tarefas, as atribuições inteligentes são exibidas nas seguintes seções, dependendo de qual fase do cálculo do algoritmo identificou as atribuições:

   * **Atribuições sugeridas**: Atribuições identificadas na primeira fase do cálculo do algoritmo de atribuição inteligente de tarefa.
   * <span class="preview">**Outras atribuições**: Atribuições identificadas na segunda fase do cálculo do algoritmo de atribuição inteligente de tarefa. Esta seção não está disponível para problemas. </span> <!--replace this with the new UI: "Other assignments"-->

   ![](assets/smart-assignments-task-list.png)

   Para obter mais informações, consulte [Visão geral das atribuições inteligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

1. Selecione o usuário na lista de recomendações clicando no nome.

1. (Opcional) Clique em **Atribuir a mim** para atribuir o item de trabalho a si mesmo.

   >[!TIP]
   >
   >Se não houver sugestões, a lista de sugestões não será aberta.

1. (Opcional) Se não quiser usar um dos usuários recomendados da lista de atribuições inteligentes, comece digitando o nome do recurso desejado e selecione o nome quando ele aparecer na lista.
1. Clique em **Enter** para fazer a atribuição.

   O usuário selecionado está atribuído à tarefa ou problema.
