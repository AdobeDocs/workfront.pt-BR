---
product-area: projects
navigation-topic: update-work-in-a-project
title: Exibir e Atualizar o Percentual Concluído das Tarefas
description: Você pode atualizar o percentual concluído de uma tarefa para indicar o progresso feito na tarefa em sua conclusão. Atualizar o percentual concluído de ocorrências é semelhante a atualizá-lo para uma tarefa. Este artigo descreve como atualizar o percentual concluído de uma tarefa.
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: 66fc75ed9a7fca4b44ac776c314a6e08a6fbd450
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---

# Exibir e atualizar o Percentual Concluído das tarefas

<!--Audited: 05/2025-->

Você pode atualizar o percentual concluído de uma tarefa para indicar o progresso feito na tarefa em sua conclusão.

Atualizar o percentual concluído de ocorrências é semelhante a atualizá-lo para uma tarefa. Este artigo descreve como atualizar o percentual concluído de uma tarefa.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso.

Você deve ter o seguinte acesso para atualizar tarefas manualmente:

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
   <td> <p>Nova licença: Standard</p> 
   Ou
   <p>Licença atual: Comercial ou superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a tarefas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para a tarefa</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Áreas em que é possível atualizar o percentual concluído de uma tarefa

Você pode atualizar o percentual concluído de uma tarefa em qualquer uma das seguintes áreas:

* **Em uma lista de tarefas**: você pode atualizar o percentual concluído de uma tarefa quando a coluna Percentual concluído for exibida.

  Para obter mais informações sobre edição em linha, consulte [itens de edição em linha em uma lista no Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

* **No modo de exibição Marco**: Você pode atualizar o percentual concluído de uma tarefa ao usar o modo de exibição Marco em uma lista de projetos ou em um relatório de projeto.

  >[!TIP]
  >
  >  Não é possível atualizar o percentual concluído de problemas na exibição de Marco.


  Para obter mais informações, consulte [Usar a exibição de Marco](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **No cabeçalho da tarefa**: você pode atualizar o percentual concluído de uma tarefa no cabeçalho da tarefa.

  ![](assets/nwe-updatetaskpercentinheader-350x54.png)

* **No painel Resumo de uma tarefa**: você pode atualizar a porcentagem concluída de uma tarefa na parte superior do painel Resumo ao visualizar a tarefa nas seguintes áreas:

   * Lista de tarefas ou relatório
   * Planilha de horas
   * Balanceador de carga de trabalho

  ![](assets/update-percent-complete-in-task-summary-highlighted.png)

  Para obter mais informações, consulte [Resumo geral](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)

* **Página inicial**: você pode atualizar a porcentagem concluída de uma tarefa ou problema no painel Resumo na área Página inicial ou no widget Meu trabalho.

  Para obter informações, consulte [Introdução à Página Inicial](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

## Considerações sobre a atualização do percentual concluído de uma tarefa

* Quando você marca uma tarefa como 100% concluída, o Status da tarefa é atualizado para Concluído. O status de um problema é atualizado para Fechado.
* Concluir uma tarefa também atualiza o percentual concluído do pai e do projeto.
* Existem os seguintes cenários para tarefas e projetos principais:
   * Não é possível atualizar o percentual concluído de uma tarefa pai para 100% quando o Modo de Conclusão em Resumo do projeto está definido como Automático e as subtarefas não estão concluídas.
   * Você pode atualizar o percentual concluído de uma tarefa pai ou de um projeto para 100% quando o Modo de Conclusão em Resumo do projeto estiver definido como Manual e as subtarefas estiverem concluídas ou incompletas.

  Para obter mais informações, consulte [Editar projetos](../manage-projects/edit-projects.md).

## Atualizar o percentual concluído de uma tarefa

1. Vá para qualquer uma das áreas em que deseja atualizar o percentual concluído de uma tarefa.

   Para obter informações, consulte a seção [Áreas em que você pode atualizar a porcentagem concluída de uma tarefa](#areas-where-you-can-update-the-percent-complete-of-a-task) neste artigo.

1. Localize o campo **Percentual concluído** da tarefa cuja porcentagem concluída você deseja atualizar.

   >[!TIP]
   >
   >O campo Percentual concluído sempre é exibido na parte superior do painel Resumo.

1. Clique dentro do campo **Percentual concluído** e digite um número entre 0 e 100

   Ou

   Clique e arraste a bolha azul **Percentual concluído** para o número necessário para indicar quanto da tarefa você concluiu, quando disponível.

   >[!NOTE]
   >
   >    * Não é possível inserir um número decimal ao clicar dentro da bolha Percentual concluído.
   >    * Quando você arrasta e solta a bolha azul no painel Resumo, a Porcentagem concluída é atualizada em um ponto.
   >
   >    * Quando você arrasta e solta a bolha azul no cabeçalho da tarefa, a Porcentagem concluída é atualizada em incrementos de 5 pontos.

1. Pressione Enter no teclado para salvar a porcentagem concluída.

   A Porcentagem concluída do projeto ou qualquer tarefa pai também pode ser atualizada automaticamente.

   O status da tarefa ou do problema também é atualizado.

