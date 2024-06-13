---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Fazer atribuições inteligentes
description: Você pode usar atribuições inteligentes para identificar quem é o melhor usuário para concluir o trabalho. As atribuições inteligentes são sugestões para usuários, funções ou equipes que a Adobe Workfront apresenta ao atribuir itens de trabalho a recursos com base em um algoritmo que determina o recurso mais apropriado para o trabalho. Para obter informações sobre atribuições inteligentes, consulte Visão geral das atribuições inteligentes.
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: ac5e56a2881d589c9a737d5e7115d82ee5c11ea6
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---

# Fazer atribuições inteligentes

<span class="preview">As informações destacadas nesta página se referem a funcionalidades ainda não disponíveis no geral. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes ou no ambiente Produção para clientes que ativaram versões rápidas.</span>

<span class="preview">Para obter informações sobre lançamentos rápidos, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Para obter informações sobre a versão atual, consulte [Visão geral da versão do terceiro trimestre de 2024](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

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

   <div class="preview">
   Uma ou várias das seguintes seções com sugestões de atribuição inteligente são exibidas:

   * **Atribuições sugeridas**: exibido para tarefas.

     >[!TIP]
     >
     >   O cabeçalho da lista é exibido **Aqui estão algumas recomendações** em vez de **Atribuições sugeridas** no ambiente de Produção.
     >
   * **Outras atribuições**: exibido para tarefas e problemas.
   * **Usuários e equipes**: exibido para tarefas e problemas.
   * **Funções de trabalho**: exibe tarefas e problemas.
   </div>

   <span class="preview">![](assets/smart-assignments-task-header-nwe-350x302.png)</span>


   Para tarefas, as atribuições inteligentes são exibidas nas seguintes seções, dependendo de qual fase do cálculo do algoritmo identificou as atribuições:

   * **Atribuições sugeridas**: Atribuições identificadas na primeira fase do cálculo do algoritmo de atribuição inteligente de tarefa. <span class="preview">Esta seção não está disponível para problemas.</span>
   * <span class="preview">**Outras atribuições**, **Usuários e equipes** ou **Funções de trabalho**: Atribuições identificadas na segunda fase do cálculo do algoritmo de atribuição inteligente de tarefa. <!--no longer valid: This section is not available for issues. --></span> <!--replace this with the new UI: "Other assignments"-->

   <span class="preview">![](assets/smart-assignments-task-list.png)</span>

   Para obter mais informações, consulte [Visão geral das atribuições inteligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

1. Selecione o usuário na lista de recomendações clicando no nome.

1. (Opcional) Clique em **Atribuir a mim** para atribuir o item de trabalho a si mesmo.

   >[!TIP]
   >
   >Se não houver sugestões, a lista de sugestões não será aberta.

1. (Opcional) Se não quiser usar um dos usuários recomendados da lista de atribuições inteligentes, comece digitando o nome do recurso desejado e selecione o nome quando ele aparecer na lista.
1. Clique em **Enter** para fazer a atribuição.

   O usuário selecionado está atribuído à tarefa ou problema.
