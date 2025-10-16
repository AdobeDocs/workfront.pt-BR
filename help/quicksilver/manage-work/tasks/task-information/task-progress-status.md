---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visão Geral do Status de Progresso da Tarefa
description: O Adobe Workfront determina o Status de progresso de uma tarefa observando o progresso da tarefa na linha do tempo. Você pode configurar o Workfront para determinar a Condição de um projeto com base no valor do Status de progresso das tarefas. Para obter mais informações sobre como configurar a Condição do projeto, consulte o artigo Visão geral da condição do projeto e do tipo de condição.
author: Alina
feature: Work Management
exl-id: 38e5f89e-bdfa-433c-9371-3c3003ada3a3
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 0%

---

# Visão geral do status de progresso da tarefa

<!-- Audited: 1/2024 -->

O Adobe Workfront determina o Status de progresso de uma tarefa observando o progresso da tarefa na linha do tempo. Você pode configurar o Workfront para determinar a Condição de um projeto com base no valor do Status de progresso das tarefas. Para obter mais informações sobre como configurar a Condição do projeto, consulte o artigo [Visão Geral da Condição do Projeto e do Tipo de Condição](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

## Critérios que determinam o Status do Progresso de tarefas

Para obter informações sobre o status de progresso de um projeto, consulte [Visão geral do status de progresso do projeto](../../../manage-work/projects/planning-a-project/project-progress-status.md).

Para obter informações sobre o acompanhamento do progresso de suas tarefas, consulte [Visão geral do Modo de Acompanhamento de Tarefas](../../../manage-work/tasks/task-information/task-tracking-mode.md).

Os critérios a seguir determinam o Status do Progresso de uma tarefa:

<table> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Status do Progresso</strong> </p> </th> 
   <th> <p><strong>Determinando Critérios</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td scope="col"> <p> </p> <p><strong>No Prazo</strong> </p> </td> 
   <td scope="col"> <p>Uma tarefa é considerada <strong>No Prazo</strong> quando todas as Datas Planejadas correspondem às Datas Projetadas. Esse status de progresso também pode significar que o projeto está antes do cronograma e as datas projetadas podem ser anteriores às datas planejadas.</p> <p>Para obter mais informações sobre Datas Projetadas, consulte <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Visão Geral da Data de Conclusão Projetada para projetos, tarefas e problemas</a>.</p> <p>Para obter mais informações sobre a Data de Conclusão Planejada da tarefa, consulte os seguintes artigos:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Visão geral da data de início planejada da tarefa</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Visão geral da Data de Término Planejada da tarefa</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><p></p> <p><strong>Em Risco</strong> </p> </td> 
   <td><p>Uma tarefa é considerada <strong>Em Risco</strong> quando a Data de Conclusão Estimada for posterior à Data de Conclusão Planejada e posterior à Data de Conclusão Projetada. Isso pode acontecer quando uma tarefa tem uma restrição de <strong>Deve Terminar Em</strong> ou <strong>Deve Iniciar Em</strong>, mas a porcentagem concluída ou as relações de predecessoras da tarefa mostram que ela não pode terminar ou iniciar nas datas especificadas. </p><p> Definir a Restrição de Tarefa como <strong>Deve Terminar em</strong> define manualmente a Data de Conclusão Planejada como uma data específica. A Data de conclusão projetada nesse caso corresponde à Data de conclusão planejada. No caso dessa restrição, o Workfront analisa a tarefa para calcular quando ela terminará com base no percentual concluído. Esse cálculo é armazenado como a Data de vencimento estimada. Se a Data de Vencimento Estimada for posterior à Data de Conclusão Projetada, a tarefa será considerada com risco de atraso. </p> <p> Definir a Restrição de Tarefa como <strong>Deve Iniciar em</strong> define manualmente a Data de Início Planejada como uma data específica. A Data de Início Projetada nesse caso corresponde à Data de Início Planejada. No caso dessa restrição, o Workfront analisa a tarefa para calcular quando ela iniciará com base em seus relacionamentos predecessores. Esse cálculo é armazenado como a Data de Início Estimada. Se houver um predecessor imposto que não permita que a tarefa inicie na Data Inicial especificada, a Data Inicial Estimada poderá ser posterior à Data de Conclusão Projetada. A tarefa é considerada em risco de atraso. </p> <p>Observação: Normalmente, as Datas Estimadas correspondem às Datas Projetadas, exceto quando <strong>Deve Começar Em</strong> ou <strong>Deve Terminar Em</strong> são usadas. Nesses casos, as Datas estimadas continuam a ser calculadas com base no percentual concluído e em outros fatores (relacionamentos predecessores), enquanto as Datas projetadas são forçadas a corresponder às Datas planejadas que foram definidas manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Atrasado</strong> </p> </td> 
   <td> <p>Uma tarefa será considerada como <strong>atrasada</strong> quando a Data de conclusão estimada for posterior ou igual à Data de conclusão planejada e anterior à Data de conclusão projetada.</p> <p>A Data de conclusão projetada é uma visualização em tempo real de quando a tarefa será concluída com base no progresso anterior. Embora a tarefa tenha sido iniciada com atraso, ela ainda não é considerada atrasada, pois as Datas de Término Planejadas e Projetadas ainda estão no futuro e a tarefa ainda pode ser concluída no prazo.</p> <p>Observação: Os Status de Progresso de <strong>Em Risco</strong> e <strong>Em Risco</strong> são quase idênticos. No entanto, <strong>Em Risco</strong> indica que há algumas Restrições de Tarefa Forçadas (Precisa Terminar Em, Precisa Iniciar Em, Datas Fixas) em uma ou ambas as Datas Planejadas. Se não houver restrições forçadas na tarefa, as Datas Projetadas serão iguais às Datas Estimadas e refletirão o cálculo do sistema da Data de Conclusão com base no andamento atual da tarefa. A tarefa ainda não é considerada atrasada, pois as Datas de Término Planejadas e Projetadas ainda estão no futuro, e a tarefa ainda pode ser concluída no prazo.<br>Para obter mais informações sobre as Datas Projetadas e Estimadas, consulte <a href="../../../manage-work/tasks/task-information/differentiate-projected-estimated-dates.md" class="MCXref xref">Visão Geral das Datas Projetadas e Estimadas </a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Atrasado</strong> </p> </td> 
   <td> <p>Uma tarefa está <strong>atrasada</strong> quando a data de conclusão planejada é anterior à data de hoje.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

<!--hiding this because some users find the images confusing, as they don't really show the dates mentioned in the descriptions above. Keep the pictures though, in case some users will complain that we hid them. 

## How task Progress Status updates over time

The different date types in our projects tell us how tasks are progressing over time:

* On Time

  ![](assets/on-time-progress-status-350x233.png)

* At Risk

  ![](assets/at-risk-progress-status-350x233.png)

* Behind

  ![](assets/behind-progress-status-350x233.png)

* Late

  ![](assets/late-progress-status-350x233.png)

-->
