---
content-type: overview
product-area: projects
navigation-topic: task-constraints
title: Visão geral da restrição de tarefa
description: As restrições de tarefa determinam quando uma tarefa deve iniciar e terminar em um projeto.
author: Alina
feature: Work Management
exl-id: 91b0844b-95a3-4d18-9fdb-a907dd42e1bf
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 10%

---

# Visão geral da restrição de tarefa

As restrições de tarefa determinam quando uma tarefa deve iniciar e terminar em um projeto.

## Visão Geral das Restrições de Tarefa

Conforme você cria o plano do projeto, toma decisões sobre a sequência e o período de suas tarefas no projeto. As tarefas podem funcionar independentemente de qualquer sequência de tarefas, mas podem afetar a linha do tempo do projeto. As Restrições de Tarefa permitem que um gerente de projeto planeje quando determinadas tarefas podem ser iniciadas ou concluídas em um projeto.

Dependendo da restrição usada, talvez seja necessário especificar uma Data Inicial Planejada, uma Data de Conclusão Planejada ou ambas para a tarefa.

Os tipos de restrição que exigem datas definidas afetam as relações dos predecessores.

>[!TIP]
>
>Considere usar um tipo de restrição que não requer datas específicas se estiver usando relações do antecessor entre tarefas.

A tabela a seguir exibe cada restrição e sua abreviação. As abreviações são usadas em listas de tarefas e ao criar arquivos de importação de Início Rápido. Clique no título vinculado de cada restrição de tarefa para obter mais informações sobre esse tipo de restrição.

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Nome da restrição</strong> </p> </th> 
   <th> <p><strong>Abreviação</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-soon-as-possible.md" class="MCXref xref">Visão geral da restrição de tarefa: Logo Que Possível</a> </p> </td> 
   <td scope="col"> <p>OMBP</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-late-as-possible.md" class="MCXref xref">Visão geral da restrição de tarefa: O Mais Tarde Possível </a> </p> </td> 
   <td scope="col"> <p>OMTP</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/earliest-available-time.md" class="MCXref xref">Visão geral da restrição de tarefa: Hora Disponível Anterior</a> </p> </td> 
   <td scope="col"> <p>MMCD</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/latest-available-time.md" class="MCXref xref">Visão geral da restrição de tarefa: Hora Disponível Mais Recente</a> </p> </td> 
   <td scope="col"> <p>OMTD</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-earlier-than.md" class="MCXref xref">Visão geral da restrição de tarefa: Iniciar Não Anterior a</a> </p> </td> 
   <td scope="col"> <p>NIAD</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-later-than.md" class="MCXref xref">Visão geral da restrição de tarefa: Iniciar Não Mais Tarde</a> </p> </td> 
   <td scope="col"> <p>NIDD</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-earlier-than.md" class="MCXref xref">Visão geral da restrição de tarefa: Concluir não antes de</a> </p> </td> 
   <td scope="col"> <p>NTAD</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-later-than.md" class="MCXref xref">Visão geral da restrição de tarefa: Concluir O Mais Tarde Que</a> </p> </td> 
   <td scope="col"> <p>NTDD</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-start-on.md" class="MCXref xref">Visão geral da restrição de tarefa: Deve Iniciar em</a> </p> </td> 
   <td scope="col"> <p>PIE</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-finish-on.md" class="MCXref xref">Visão geral da restrição de tarefa: Deve terminar em</a> </p> </td> 
   <td scope="col"> <p>PTE</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/fixed-dates.md" class="MCXref xref">Visão geral da restrição de tarefa: Datas fixas</a> </p> </td> 
   <td> <p>Dt Fixas</p> </td> 
  </tr> 
 </tbody> 
</table>

## Visão geral das restrições padrão

Quando você cria novas tarefas, uma Restrição de tarefa é automaticamente selecionada pelo Workfront.

O Workfront usa duas variáveis para decidir qual Restrição de Tarefa é selecionada por padrão para uma nova tarefa:

* O **Agendamento do projeto a partir de** no projeto.

   Para obter informações sobre o campo Agendar de projeto, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

* O **Data inicial** preferência configurada pelo administrador da Workfront ou do grupo na **Tarefas e problemas** área de **Configuração**.

   Para obter informações sobre as Preferências de Tarefas e Problemas, consulte a seção &quot;Novos Padrões de Tarefas&quot; em [Configurar preferências de emissão e tarefa em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

A tabela a seguir mostra a Restrição de Tarefa padrão ao escolher variáveis diferentes para seu projeto e suas novas tarefas:

| Agendamento do projeto a partir de | Data de início da tarefa | Padrão de Restrição de Tarefa |
|---|---|---|
| Data de início | Com base na Data de planejamento de projeto | O Mais Breve Possível |
| Data de início | Hoje | Não Iniciar Antes De |
| Data de término | Com base na Data de planejamento de projeto | O Mais Tarde Possível |
| Data de término | Hoje | Não Iniciar Depois De |
