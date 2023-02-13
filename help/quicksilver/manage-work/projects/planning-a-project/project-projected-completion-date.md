---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Visão geral da data de conclusão projetada para projetos, tarefas e problemas
description: A Data de Conclusão Projetada é um indicador em tempo real, calculado de quando o projeto, a tarefa ou a emissão será concluída. Quando o projeto, a tarefa ou o problema é marcado como Concluído, a Data de Conclusão Projetada muda para a data da Data de Conclusão Real.
author: Alina
feature: Work Management
exl-id: dde400e6-189f-4431-8f2f-7142ce424826
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---

# Visão geral da data de conclusão projetada para projetos, tarefas e problemas

A Data de Conclusão Projetada é um indicador em tempo real, calculado de quando o projeto, a tarefa ou a emissão será concluída. Quando o projeto, a tarefa ou o problema é marcado como Concluído, a Data de Conclusão Projetada muda para a data da Data de Conclusão Real.

As seções a seguir descrevem como a Data de conclusão projetada é determinada para projetos, tarefas e problemas, e como localizá-la.

## Requisitos de acesso

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   <p>For current licenses: 
   <ul><li><p>Contributor or higher to view the Projected Completion Date in a report</p></li> <li><p>A Standard license to create a report</p></li> </ul>
   
   <p>For legacy licenses: 
   <ul><li><p>Review or higher to view the Projected Completion Date in a report</p></li> 
   <li><p>A Plan license to create a report</p> </li></ul>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>You must have Edit access to Reports, Dashboards, Calendars to create a report</p> <p>You must have Edit access to Filters, Views, Groupings to create a report or modify a list view</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Revise ou superior para exibir a Data de conclusão projetada em um relatório</p> <p>Uma licença do Plan para criar um relatório</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Exibir ou ter acesso superior a Projetos</p> <p>É necessário ter acesso Editar para Relatórios, Painéis, Calendários para criar um relatório</p> <p>Você deve ter o acesso Editar a Filtros, Exibições, Agrupamentos para criar um relatório ou modificar uma exibição de lista</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou permissões superiores a um projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Como o Adobe Workfront determina a data de conclusão projetada

A Data de Conclusão Projetada é um campo calculado e não pode ser alterado manualmente.

Os critérios usados para determinar a Data de conclusão projetada são diferentes, dependendo do objeto que você está visualizando:

* **Projetos:** A Data de conclusão projetada para os projetos equivale à Data de conclusão prevista da última tarefa do projeto.
* **Tarefas:** A Data de Conclusão Projetada para tarefas é determinada com base nos seguintes critérios:

   * **Atualizações de progresso feitas na tarefa pelo destinatário da tarefa:** As atualizações de progresso incluem alterações na porcentagem concluída e alterações do status da tarefa.
   * **Data da confirmação:** Se o destinatário da tarefa especificar uma Data de Confirmação, a Data de Conclusão Projetada será alterada para corresponder à Data de Confirmação.

      Para obter mais informações sobre datas de confirmação, consulte o artigo [Visão geral da data de confirmação](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

   * **Predecessores:** Se não houver atrasos nas tarefas do antecessor, a Data de Conclusão Projetada deverá corresponder à Data de Conclusão Planejada. Conforme ocorrem atrasos, as tarefas dependentes mostram uma Data de Conclusão Projetada maior que a Data de Conclusão Planejada.

      Para obter mais informações sobre a Data de Conclusão Planejada de tarefas, consulte [Visão geral da data de conclusão planejada da tarefa](../../../manage-work/tasks/task-information/task-planned-completion-date.md).
   >[!IMPORTANT]
   >
   >Quando o antecessor de uma tarefa tiver uma Data de conclusão real, as tarefas dependentes receberão uma Data de conclusão projetada, conforme descrito no seguinte cenário:
   >
   >
   >Se o projeto tiver a Tarefa A, a Tarefa B e a Tarefa C e a Tarefa B for a sucessora da Tarefa A, a Tarefa C será a sucessora da Tarefa B e uma Data de Conclusão Real será adicionada à Tarefa A, a Data de Conclusão Projetada será automaticamente recalculada para a Tarefa B (desde que a **Tipo de atualização** do projeto está definido como Automático e On Change), mas não será recalculado para a Tarefa C. Atualmente, o Workfront calcula a Data de Conclusão Projetada para tarefas que estão um nível acima ou abaixo da Tarefa atualizada, por motivos de desempenho. 

* **Problemas:**A data de conclusão projetada é inicialmente definida para corresponder à data de conclusão planejada do problema.

   Se o destinatário da emissão especificar uma data de confirmação, tanto a Data de Conclusão Projetada quanto a Data de Conclusão Planejada serão alteradas para corresponder à Data de Confirmação.

   Para obter mais informações sobre datas de confirmação, consulte o artigo [Visão geral da data de confirmação](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Exibir a data de conclusão projetada

Você pode visualizar a Data de conclusão projetada de projetos, tarefas e problemas em relatórios. Você pode visualizar a Data de conclusão projetada de projetos e tarefas em outras áreas do Workfront. 

* [Exibir a Data de Conclusão Projetada de um projeto](#view-the-projected-completion-date-of-a-project)
* [Exibir a Data de Conclusão Projetada de uma tarefa](#view-the-projected-completion-date-of-a-task)
* [Exibir a Data de Conclusão Projetada de um problema](#view-the-projected-completion-date-of-an-issue)

### Exibir a Data de Conclusão Projetada de um projeto {#view-the-projected-completion-date-of-a-project}

1. Vá para o projeto onde deseja exibir a Data de conclusão projetada.
1. Clique em **Detalhes do projeto** no painel esquerdo.
1. Localize a variável **Data de Conclusão Projetada** no campo **Visão geral** seção.

### Exibir a Data de Conclusão Projetada de uma tarefa {#view-the-projected-completion-date-of-a-task}

1. Vá para a tarefa onde deseja exibir a Data de Conclusão Projetada.
1. Clique em **Detalhes da tarefa** no painel esquerdo.
1. Localize a variável **Data de Conclusão Projetada** no campo **Visão geral** seção.

### Exibir a Data de Conclusão Projetada de um problema {#view-the-projected-completion-date-of-an-issue}

Você pode visualizar a Data de conclusão projetada para problemas somente em um relatório de ocorrência ou exibição de lista. A criação de uma exibição de lista é semelhante à criação da exibição em um relatório.

Para criar um relatório de problema que inclua a Data de conclusão prevista:

1. Crie um relatório de problemas, conforme descrito no artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Selecione o **Colunas (Exibir)** guia .
1. Clique em **Adicionar coluna** e comece a digitar **Data de Conclusão Projetada** no **Mostrar nesta coluna:** campo.

1. Selecione-o quando ele aparecer na lista, em **Problema** objeto. 
1. Clique em **Salvar + Fechar**.

   O **Data de Conclusão Projetada** no relatório é preenchida. 

   ![](assets/issue-projected-completion-date-in-view-nwe-350x148.png)
