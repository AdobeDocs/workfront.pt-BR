---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Fazer atribuições inteligentes
description: Você pode usar atribuições inteligentes para identificar quem é o melhor usuário para concluir o trabalho. As atribuições inteligentes são sugestões para usuários, funções ou equipes que a Adobe Workfront apresenta ao atribuir itens de trabalho a recursos com base em um algoritmo que determina o recurso mais apropriado para o trabalho. Para obter informações sobre atribuições inteligentes, consulte Visão geral das atribuições inteligentes.
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 412645a802bdf9057bb61a5a96df257daa1c3948
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Fazer atribuições inteligentes

<!--Audited: 07/2024-->

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">As informações destacadas nesta página se referem à funcionalidade disponível somente no ambiente de Produção para clientes que habilitaram versões rápidas.</span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview"> Essa funcionalidade será removida do ambiente de Produção para clientes que habilitaram a versão rápida com a versão 25.1 em janeiro de 2025. Para obter informações sobre a versão 25.1, consulte [Visão geral da versão do Primeiro Trimestre de 2025](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md).

Você pode usar atribuições inteligentes para identificar quem é o melhor usuário para concluir o trabalho.

As atribuições inteligentes são sugestões para usuários, funções ou equipes que a Adobe Workfront apresenta quando você atribui itens de trabalho a recursos. O Workfront baseia suas sugestões em um algoritmo que determina o recurso mais apropriado para a tarefa.

<span class="preview">Há dois algoritmos separados no Workfront que calculam atribuições inteligentes que funcionam de forma diferente para tarefas e problemas.</span>

Para obter mais informações sobre os critérios usados na determinação de atribuições inteligentes, consulte [Visão geral das atribuições inteligentes](/help/quicksilver/manage-work/tasks/assign-tasks/smart-assignments.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
   <td> <p>Permissões do Contribute ou superior com a capacidade de fazer atribuições em tarefas e problemas</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Fazer atribuições inteligentes

As atribuições inteligentes estão disponíveis na maioria dos locais onde você pode fazer atribuições no Workfront.

1. Vá para as seguintes áreas e clique no campo **Atribuições** ou **Atribuir a este campo**:

   * Uma lista de tarefas ou problemas ou um relatório
   * Um cabeçalho de tarefa ou problema
   * O painel Resumo de tarefas ou problemas
   * <span class="preview">Caixa Nova Tarefa</span> ou Novo Problema, ao adicionar <span class="preview">uma nova tarefa</span> ou problema a um projeto
   * Uma tarefa ou problema no Balanceador de carga de trabalho

1. Coloque o cursor no campo Assignments e aguarde dois segundos.

   Para problemas, as atribuições inteligentes são exibidas nas seguintes seções:

   * **Usuários e equipes**
   * **Funções de trabalho**

   ![](assets/smart-assignments-issue-header.png)

   Para tarefas, as atribuições inteligentes são exibidas nas seguintes seções, dependendo de qual fase do cálculo do algoritmo identificou as atribuições:

   * <span class="preview">**Atribuições sugeridas**: exibe as atribuições identificadas na primeira fase do algoritmo de atribuição inteligente de tarefa.</span>
   * **Usuários e equipes**, **Funções de trabalho** ou <span class="preview">**Funções de trabalho de cartão de taxa**</span>: atribuições identificadas na segunda fase do cálculo do algoritmo de atribuição inteligente de tarefa.

   <span class="preview">![](assets/smart-assignments-task-list.png)</span>

   Para obter mais informações, consulte [Visão geral das atribuições inteligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

1. Selecione o recurso na lista de recomendações clicando no nome.

1. (Opcional) Clique em **Atribuir a mim** para atribuir o item de trabalho a você mesmo.

   >[!TIP]
   >
   >Se não houver sugestões, a lista de sugestões não será aberta.

1. (Opcional) Se não quiser usar um dos usuários recomendados da lista de atribuições inteligentes, comece digitando o nome do recurso desejado e selecione o nome quando ele aparecer na lista.
1. Clique em **Inserir** para fazer a atribuição.

   O usuário selecionado está atribuído à tarefa ou problema.
