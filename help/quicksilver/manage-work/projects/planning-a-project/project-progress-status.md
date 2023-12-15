---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Visão geral do status de progresso do projeto
description: O Adobe Workfront determina o status do progresso de um projeto observando o progresso do projeto na linha do tempo. Você pode configurar o Workfront para determinar a Condição de um projeto com base no valor do Status de progresso das tarefas. Saiba mais sobre o Status de progresso do projeto neste artigo.
author: Alina
feature: Work Management
exl-id: 922ca4cf-c526-4704-9966-de67b0c36a2a
source-git-commit: 4e3cafafb121371249fb73f2f001477bdbad2d77
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 1%

---

# Visão geral do status de progresso do projeto

<!--Audited: 12/2023-->

O Adobe Workfront determina o status do progresso de um projeto observando o progresso do projeto na linha do tempo. Você pode configurar o Workfront para determinar a Condição de um projeto com base no valor do Status de progresso das tarefas. Para obter mais informações sobre como configurar a Condição do projeto, consulte o artigo [Visão geral da condição do projeto e do tipo de condição](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

A seguir estão os status de progresso dos projetos no Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>No Prazo</td> 
   <td> O status do progresso de um projeto é <strong>No Prazo</strong> se:<ul><li>Se as Datas de Término Projetada e Estimada forem anteriores ou iguais à Data de Término Planejada do projeto</li></ul> <p> <img src="assets/project-on-time-progress-status-350x69.png" style="width: 350;height: 69;"> </p> </td> 
  </tr> 
  <tr> 
   <td>Em Risco</td> 
   <td> O status do progresso de um projeto é <strong>Em Risco</strong> se <strong>all</strong> dos seguintes são verdadeiros:<ul><li>As datas de conclusão estimada e projetada estão no futuro</li><li> As Datas de Conclusão Estimada e Projetada são posteriores à Data de Conclusão Planejada</li><li> A data de conclusão estimada é posterior à data de conclusão projetada</li></ul><p> <img src="assets/project-at-risk-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>Fora do Cronograma</td> 
   <td> O status do progresso de um projeto é <strong>Atrás</strong> se <strong>all</strong> dos seguintes são verdadeiros:<ul><li>As datas de conclusão estimada e projetada estão no futuro</li><li> As datas de conclusão estimada e projetada são posteriores à data de conclusão planejada do projeto</li><li> A data de conclusão estimada não é posterior à data de conclusão projetada</li></ul> <p> <img src="assets/project-behind-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>Atrasado</td> 
   <td> 
     O status do progresso de um projeto é <strong>Atrasado</strong> se <strong>ou</strong> dos seguintes são verdadeiros:<ul><li>O projeto estiver concluído e a Data de conclusão efetiva for posterior à Data de conclusão planejada <p> <img src="assets/project-late-progress-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
     <li> <p>O projeto não está concluído e a Data de conclusão planejada do projeto está no passado <p> <img src="assets/project-late-progress-status-incomplete-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Considere o seguinte:

* A Data de conclusão projetada do projeto é orientada pela tarefa no Caminho Crítico com a Data de conclusão projetada mais recente.
* A Data de conclusão estimada do projeto é orientada pela tarefa no Caminho Crítico com a Data de conclusão estimada mais recente.

Para obter informações sobre o Caminho Crítico do projeto, consulte [Visão geral do Caminho crítico do projeto](../../../manage-work/tasks/manage-tasks/critical-path.md).

Para obter informações sobre Datas de Término Projetadas, consulte [Visão geral da Data de conclusão projetada para projetos, tarefas e problemas](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
