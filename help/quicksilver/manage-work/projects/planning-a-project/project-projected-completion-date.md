---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Visão geral da Data de conclusão projetada para projetos, tarefas e problemas
description: A Data de conclusão projetada é um indicador calculado em tempo real de quando o projeto, tarefa ou problema será concluído. Quando o projeto, tarefa ou problema é marcado como Concluído, a Data de conclusão projetada muda para a data da Data de conclusão atual.
author: Alina
feature: Work Management
exl-id: dde400e6-189f-4431-8f2f-7142ce424826
source-git-commit: 811d8076a0b344e863b25aa253a0fb1c102f0435
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 0%

---

# Visão geral da Data de conclusão projetada para projetos, tarefas e problemas

<!-- Audited: 1/2024 -->

A Data de conclusão projetada é um indicador calculado em tempo real de quando o projeto, tarefa ou problema será concluído. Quando o projeto, tarefa ou problema é marcado como Concluído, a Data de conclusão projetada muda para a data da Data de conclusão atual.

As seções a seguir descrevem como a Data de conclusão projetada é determinada para projetos, tarefas e problemas, e como localizá-la.

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
   <td> 
   <p>Novo: 
   <ul><li><p>Colaborador ou posterior para exibir a Data de conclusão projetada em um relatório</p></li> <li><p>Uma licença Standard para criar um relatório</p></li> </ul>

<p>Atual: 
   <ul><li><p>Revisar ou posterior para exibir a Data de Término Projetada em um relatório</p></li> 
   <li><p>Uma licença de plano para criar um relatório</p> </li></ul>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nível de acesso</td> 
   <td> <p>Acesso de visualização ou superior aos Projetos</p> <p>É necessário ter acesso de Edição a Relatórios, Painéis e Calendários para criar um relatório</p> <p>É necessário ter acesso para Editar filtros, visualizações e agrupamentos para criar um relatório ou modificar uma visualização de lista</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualizar ou aumentar as permissões de um projeto</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação da Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Como o Adobe Workfront determina a data de conclusão projetada

A Data de conclusão projetada é um campo calculado e não pode ser alterada manualmente.

Os critérios usados para determinar a Data de conclusão projetada diferem, dependendo do objeto que você está visualizando:

* **Projetos:** a Data de Conclusão Projetada para projetos é igual à Data de Conclusão Projetada da tarefa mais recente no projeto.

  Por exemplo, uma porcentagem concluída mais alta move a Data de conclusão projetada da tarefa para mais perto do dia atual. Se o status da tarefa for Novo e a Data de conclusão planejada da tarefa estiver próxima ou tiver passado, a Data de conclusão projetada avançará ainda mais para o futuro.

* **Tarefas:** a Data de Conclusão Projetada para tarefas é determinada com base nos seguintes critérios:

   * **Atualizações de progresso feitas na tarefa pelo destinatário da tarefa:** As atualizações de progresso incluem alterações na porcentagem concluída e alterações no status da tarefa.
   * **Data de confirmação:** se o destinatário da tarefa especificar uma Data de confirmação, a Data de conclusão projetada será alterada para corresponder à Data de confirmação.

     Para obter mais informações sobre Datas de Confirmação, consulte o artigo [Visão geral da Data de Confirmação](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

   * **Predecessores:** Se não houver atrasos nas tarefas predecessoras, a Data de Conclusão Projetada deverá corresponder à Data de Conclusão Planejada. Conforme ocorrem atrasos, as tarefas dependentes mostram uma Data de Conclusão Projetada posterior à Data de Conclusão Planejada.

     Para obter mais informações sobre a Data de conclusão planejada das tarefas, consulte [Visão geral da Data de conclusão planejada da tarefa](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

  >[!IMPORTANT]
  >
  >Quando o antecessor de uma tarefa tiver uma Data de Conclusão Real, as tarefas dependentes receberão uma Data de Conclusão Projetada conforme descrito no seguinte cenário:
  >
  >
  >Se o projeto tiver a Tarefa A, a Tarefa B e a Tarefa C, e a Tarefa B for a sucessora da Tarefa A, a Tarefa C for a sucessora da Tarefa B e uma Data de conclusão real for adicionada à Tarefa A, a Data de conclusão projetada será recalculada automaticamente para a Tarefa B (desde que o **Tipo de atualização** do projeto esteja definido como Automático e Mediante alteração), mas não será recalculada para a Tarefa C. Atualmente, a Workfront calcula a Data de conclusão projetada para tarefas que estejam um nível acima ou abaixo da Tarefa atualizada, por motivos de desempenho.

* **Problemas:** a Data de Conclusão Projetada do problema está inicialmente definida para corresponder à Data de Conclusão Planejada do problema.

  Se o destinatário da ocorrência especificar uma data de confirmação, tanto a Data de conclusão projetada quanto a Data de conclusão planejada serão alteradas para corresponder à Data de confirmação.

  Para obter mais informações sobre Datas de Confirmação, consulte o artigo [Visão geral da Data de Confirmação](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Exibir a Data de Término Projetada

Você pode visualizar a Data de conclusão projetada dos projetos, tarefas e problemas nos relatórios. É possível visualizar a Data de conclusão projetada dos projetos e tarefas em outras áreas do Workfront.

### Exibir a Data de Término Projetada de um projeto {#view-the-projected-completion-date-of-a-project}

1. Vá para o projeto em que deseja exibir a Data de conclusão projetada.
1. Clique em **Detalhes do projeto** no painel esquerdo.
1. Localize o campo **Data de Conclusão Projetada** na seção **Visão geral** > **Datas do projeto**.

### Exibir a Data de Término Projetada de uma tarefa {#view-the-projected-completion-date-of-a-task}

1. Vá para a tarefa em que deseja exibir a Data de Conclusão Projetada.
1. Clique em **Detalhes da tarefa** no painel esquerdo.
1. Localize o campo **Data de Conclusão Projetada** na seção **Visão Geral** > **Datas e restrição de tarefas**.

### Exibir a data de conclusão projetada de um problema {#view-the-projected-completion-date-of-an-issue}

Você pode exibir a Data de conclusão projetada para problemas somente em um relatório de problemas ou em uma exibição em lista. Criar uma visualização de lista é semelhante a criar a visualização em um relatório.

Para criar um relatório de problemas que inclua a Data de conclusão projetada:

1. Crie um relatório de problemas, conforme descrito no artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Selecione a guia **Colunas (Exibição)**.
1. Clique em **Adicionar coluna** e comece a digitar **Data de Término Projetada** no campo **Mostrar nesta coluna:**.

1. Selecione-a quando ela aparecer na lista, sob o objeto **Problema**.
1. Clique em **Salvar + Fechar**.

   A coluna **Data de Conclusão Projetada** no relatório está preenchida.

   ![](assets/issue-projected-completion-date-in-view-nwe-350x148.png)
