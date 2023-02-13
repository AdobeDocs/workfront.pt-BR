---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visão geral do status de progresso da tarefa
description: O Adobe Workfront determina o Status de progresso de uma tarefa observando a progressão da tarefa em sua linha do tempo. Você pode configurar o Workfront para determinar a Condição de um projeto com base no valor do Status de Andamento das tarefas. Para obter mais informações sobre como configurar a Condição do projeto, consulte o artigo Visão geral da condição do projeto e do tipo de condição.
author: Alina
feature: Work Management
exl-id: 38e5f89e-bdfa-433c-9371-3c3003ada3a3
source-git-commit: 65f25a3b1198f491f7357efef11e2ae075e9721a
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 1%

---

# Visão geral do status de progresso da tarefa

O Adobe Workfront determina o Status de progresso de uma tarefa observando a progressão da tarefa em sua linha do tempo. Você pode configurar o Workfront para determinar a Condição de um projeto com base no valor do Status de Andamento das tarefas. Para obter mais informações sobre como configurar a Condição do projeto, consulte o artigo [Visão geral da condição do projeto e do tipo de condição](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

## Critérios que determinam o status de progresso das tarefas

Para obter informações sobre o Status de Andamento de um projeto, consulte [Visão geral do status de progresso do projeto](../../../manage-work/projects/planning-a-project/project-progress-status.md).

Para obter informações sobre como rastrear o progresso de suas tarefas, consulte [Visão geral do modo de rastreamento de tarefas](../../../manage-work/tasks/task-information/task-tracking-mode.md).

Os seguintes critérios determinam o Status de Andamento de uma tarefa:

<table> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Progresso - Status de Progresso</strong> </p> </th> 
   <th> <p><strong>Determinação dos critérios</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td scope="col"> <p> </p> <p><strong>No Prazo</strong> </p> </td> 
   <td scope="col"> <p>Uma tarefa é considerada <strong>Hora de ligar</strong> quando todas as Datas Planejadas correspondem às Datas Projetadas. Este Status de Andamento também pode significar que o projeto está adiantado do cronograma e as Datas previstas podem estar antes das Datas previstas.</p> <p>Para obter mais informações sobre Datas Projetadas, consulte <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Visão geral da data de conclusão projetada para projetos, tarefas e problemas</a>.</p> <p>Para obter mais informações sobre a Data de Conclusão Planejada da tarefa, consulte os seguintes artigos:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Visão geral da data de início planejada da tarefa</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Visão geral da data de conclusão planejada da tarefa</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><p></p> <p><strong>Em Risco</strong> </p> </td> 
   <td><p>Uma tarefa é considerada <strong>Em Risco</strong> quando a Data de conclusão estimada for posterior à Data de conclusão planejada e posterior à Data de conclusão projetada. Isso pode acontecer quando uma tarefa tem uma restrição de <strong>Deve terminar em</strong> ou <strong>Deve Iniciar em</strong> mas a porcentagem concluída ou as relações antecessoras da tarefa mostram que ela não pode terminar ou iniciar nas datas especificadas. </p><p> Definir a restrição de tarefa como <strong>Deve terminar em</strong> define manualmente a Data de conclusão planejada para uma data específica. A Data de conclusão projetada nesse caso corresponde à Data de conclusão planejada. No caso dessa restrição, o Workfront analisa a tarefa para calcular quando ela terminará com base na porcentagem concluída. Esse cálculo é armazenado como a Data de Vencimento Estimada. Se a Data de Vencimento Estimada for posterior à Data de Conclusão Projetada, a tarefa será considerada com risco de atraso. </p> <p> Definir a restrição de tarefa como <strong>Deve Iniciar em</strong> define manualmente a Data inicial planejada para uma data específica. A Data de início projetada nesse caso corresponde à Data de início planejada. No caso dessa restrição, o Workfront analisa a tarefa para calcular quando ela começará com base em suas relações antecessoras. Esse cálculo é armazenado como a Data inicial estimada. Se houver um antecessor empregado que não permitirá que a tarefa seja iniciada na Data Inicial especificada, a Data Inicial Estimada poderá ser posterior à Data de Conclusão Projetada. A tarefa é considerada em risco de atraso. </p> <p>Observação: Normalmente, as Datas estimadas correspondem às Datas previstas, exceto para quando <strong>Deve Iniciar em</strong> ou <strong>Deve terminar em</strong> são usadas. Nesses casos, as Datas estimadas continuam a ser calculadas com base na porcentagem completa e em outros fatores (relacionamentos do antecessor), enquanto as Datas projetadas são forçadas a corresponder às Datas planejadas que foram definidas manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Fora do Cronograma</strong> </p> </td> 
   <td> <p>Uma tarefa é considerada <strong>Bebehind</strong> quando a Data de conclusão estimada for posterior ou igual à Data de conclusão planejada e anterior à Data de conclusão projetada.</p> <p>A Data de conclusão projetada é uma visualização em tempo real de quando a tarefa será concluída com base em um progresso anterior. Embora a tarefa tenha sido iniciada com atraso, ainda não é considerada tarde, porque as Datas de Conclusão Planejadas e Projetadas ainda estão no futuro, e a tarefa pode ainda ser concluída a tempo.</p> <p>Observação: O <strong>Bebehind</strong> e <strong>Em Risco</strong> Os Status de progresso são quase idênticos. No entanto, <strong>Em Risco</strong> indica que há algumas restrições de tarefa forçada (deve terminar em, deve iniciar em, datas fixas) em uma ou ambas as datas planejadas. Se não houver restrições forçadas na tarefa, as Datas Projetadas serão iguais às Datas Estimadas e refletirão o cálculo do sistema da Data de Conclusão com base no progresso atual da tarefa. A tarefa ainda não é considerada atrasada, pois as Datas de Conclusão Planejada e Projetada ainda estão no futuro e a tarefa ainda pode ser concluída a tempo.<br>Para obter mais informações sobre as Datas projetadas e estimadas, consulte <a href="../../../manage-work/tasks/task-information/differentiate-projected-estimated-dates.md" class="MCXref xref">Diferenciar entre datas projetadas e estimadas </a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Atrasado</strong> </p> </td> 
   <td> <p>Uma tarefa é <strong>Atraso</strong> quando a Data de conclusão planejada for anterior à data de hoje.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

## Como o Status de Andamento da tarefa é atualizado ao longo do tempo

Os diferentes tipos de datas em nossos projetos nos informam como as tarefas estão progredindo ao longo do tempo:

* No Prazo

   ![](assets/on-time-progress-status-350x233.png)

* Em Risco

   ![](assets/at-risk-progress-status-350x233.png)

* Fora do Cronograma

   ![](assets/behind-progress-status-350x233.png)

* Atrasado

   ![](assets/late-progress-status-350x233.png)
