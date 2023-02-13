---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Visão geral do status de progresso do projeto
description: O Adobe Workfront determina o Status de progresso de um projeto, observando a progressão do projeto na linha do tempo. Você pode configurar o Workfront para determinar a Condição de um projeto com base no valor do Status de Andamento das tarefas. Para obter mais informações sobre como configurar a Condição do projeto, consulte o artigo Visão geral da condição do projeto e do tipo de condição.
author: Alina
feature: Work Management
exl-id: 922ca4cf-c526-4704-9966-de67b0c36a2a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 1%

---

# Visão geral do status de progresso do projeto

O Adobe Workfront determina o Status de progresso de um projeto, observando a progressão do projeto na linha do tempo. Você pode configurar o Workfront para determinar a Condição de um projeto com base no valor do Status de Andamento das tarefas. Para obter mais informações sobre como configurar a Condição do projeto, consulte o artigo [Visão geral da condição do projeto e do tipo de condição](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

Veja a seguir os Status de progresso de projetos no Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Hora de ligar</td> 
   <td> <p>Se as Datas de Conclusão Projetada e Estimada forem anteriores ou iguais à Data de Conclusão Planejada do projeto, o Status de Andamento do projeto será <strong>Hora de ligar</strong>.</p> <p> <img src="assets/project-on-time-progress-status-350x69.png" style="width: 350;height: 69;"> </p> </td> 
  </tr> 
  <tr> 
   <td>Em Risco</td> 
   <td> <p>Quando as Datas de Conclusão Estimada e Projetada estiverem no futuro, mas forem posteriores à Data de Conclusão Planejada do projeto e a Data de Conclusão Estimada for posterior à Data de Conclusão Projetada, o Status de Andamento do projeto será <strong>Em Risco</strong>. </p> <p> <img src="assets/project-at-risk-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>Fora do Cronograma</td> 
   <td> <p>Quando as Datas de Conclusão Estimada e Projetada estiverem no futuro, mas forem posteriores à Data de Conclusão Planejada do projeto, mas a Data de Conclusão Estimada não for posterior à Data de Conclusão Projetada, o Status de Andamento do projeto será <strong>Bebehind</strong>.</p> <p> <img src="assets/project-behind-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>Atrasado</td> 
   <td> 
    <ul> 
     <li> <p>Se o projeto estiver concluído e a Data de Conclusão Real for posterior à Data de Conclusão Planejada, o Status de Andamento do projeto será <strong>Atraso</strong>. </p> <p> <img src="assets/project-late-progress-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
     <li> <p>Se o projeto não estiver concluído e a Data de Conclusão Planejada do projeto estiver no passado, o Status de Andamento do projeto será <strong>Atraso</strong>. </p> <p> <img src="assets/project-late-progress-status-incomplete-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Considere o seguinte:

* A Data de Conclusão Projetada do projeto é impulsionada pela tarefa no Caminho Crítico com a Data de Conclusão Projetada mais recente.
* A Data estimada de conclusão do projeto é impulsionada pela tarefa no Caminho Crítico com a Data mais recente de conclusão estimada.

Para obter informações sobre o Caminho Crítico do projeto, consulte [Visão geral do caminho crítico do projeto](../../../manage-work/tasks/manage-tasks/critical-path.md).

Para obter informações sobre Datas de Conclusão Projetadas, consulte [Visão geral da data de conclusão projetada para projetos, tarefas e problemas](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
