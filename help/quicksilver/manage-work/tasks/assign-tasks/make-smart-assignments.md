---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Fazer atribuições inteligentes
description: Você pode usar atribuições inteligentes para identificar quem é o melhor usuário para concluir o trabalho. As atribuições inteligentes são sugestões para usuários que o Adobe Workfront apresenta quando você atribui itens de trabalho a recursos com base em um algoritmo que determina o recurso mais apropriado para a tarefa. Para obter informações sobre atribuições inteligentes, consulte Visão geral das atribuições inteligentes.
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 03894773e61fc0706148695572a164a2e778da9b
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Fazer atribuições inteligentes

<!--update "Results" to "Other assignments" with Prod-->

<span class="preview">As informações destacadas nesta página se referem a funcionalidades ainda não disponíveis no geral. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes.</span>

<span class="preview">Para obter informações sobre a programação de lançamento atual, consulte [Visão geral da versão do primeiro trimestre de 2024](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span>

Você pode usar atribuições inteligentes para identificar quem é o melhor usuário para concluir o trabalho.

As atribuições inteligentes são sugestões para usuários que o Adobe Workfront apresenta quando você atribui itens de trabalho a recursos com base em um algoritmo que determina o recurso mais apropriado para a tarefa.

<span class="preview">Há dois algoritmos separados no Workfront para tarefas e problemas. </span>
Para obter informações sobre atribuições inteligentes, consulte [Visão geral das atribuições inteligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Novo: Padrão</p>
      Ou
      <p>Atual: trabalho ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a tarefas e problemas</p> <p>Acesso de visualização ou superior aos Projetos</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribuir com permissões ou superiores com a capacidade de fazer atribuições em tarefas e problemas</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Fazer atribuições inteligentes

As atribuições inteligentes estão disponíveis na maioria dos locais onde você pode fazer atribuições no Workfront.

1. Vá para as seguintes áreas e clique no botão **Atribuições** ou **Atribuir esta para** campo:

   * Uma lista de tarefas ou problemas ou um relatório
   * Um cabeçalho de tarefa ou problema
   * O painel Resumo de tarefas ou problemas
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
   * <span class="preview">**Resultados**: Atribuições identificadas na segunda fase do cálculo do algoritmo de atribuição inteligente de tarefa. Esta seção não está disponível para problemas. </span> <!--replace this with the new UI: "Other assignments"-->

   ![](assets/smart-assignments-task-list.png)

   Para obter mais informações, consulte [Visão geral das atribuições inteligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md) .

1. Selecione o usuário na lista de recomendações clicando no nome.

1. (Opcional) Clique em **Atribuir a mim** para atribuir o item de trabalho a si mesmo.

   >[!TIP]
   >
   >Se não houver sugestões, a lista de sugestões não será aberta.

1. (Opcional) Se você não quiser usar um dos usuários recomendados na lista de atribuições inteligentes, comece digitando o nome do usuário desejado e selecione o nome quando ele aparecer na lista.
1. Clique em **Enter** para fazer a atribuição.

   O usuário selecionado está atribuído à tarefa ou problema.
