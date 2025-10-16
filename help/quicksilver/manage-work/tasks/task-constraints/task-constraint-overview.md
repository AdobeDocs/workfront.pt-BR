---
content-type: overview
product-area: projects
navigation-topic: task-constraints
title: Visão Geral da Restrição de Tarefa
description: As restrições de tarefa determinam quando uma tarefa deve iniciar e terminar em um projeto.
author: Alina
feature: Work Management
exl-id: 91b0844b-95a3-4d18-9fdb-a907dd42e1bf
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 6%

---

# Visão geral de Restrição de Tarefa

<!-- Audited: 12/2023 -->

As restrições de tarefa determinam quando uma tarefa deve iniciar e terminar em um projeto.

## Visão Geral das Restrições de Tarefa

À medida que você constrói seu plano de projeto, toma decisões sobre a sequência e o período das tarefas no projeto. As tarefas podem funcionar independentemente de qualquer sequência de tarefas, mas podem afetar a linha do tempo do projeto. Restrições de Tarefa permitem que um gerente de projeto planeje quando determinadas tarefas podem ser iniciadas ou concluídas em um projeto.

Dependendo da restrição usada, talvez seja necessário especificar uma Data Inicial Planejada, uma Data de Conclusão Planejada ou ambas para a tarefa.

Os tipos de restrição que exigem datas definidas afetam os relacionamentos de predecessores.

>[!TIP]
>
>Considere usar um tipo de restrição que não exija datas específicas se estiver usando relações de predecessoras entre tarefas.

A tabela a seguir exibe cada restrição e sua abreviação. As abreviações são usadas em listas de tarefas e ao criar arquivos de importação do Kickstart. Clique no título vinculado de cada restrição de tarefa para obter mais informações sobre esse tipo de restrição.

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col>
 <thead> 
  <tr> 
   <th> <p><strong>Nome da Restrição</strong> </p> </th> 
   <th> <p><strong>Abreviação</strong> </p> </th> 
   <th> <p><strong>Descrição</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-soon-as-possible.md" class="MCXref xref">Visão geral da Restrição de Tarefa: O Mais Breve Possível</a> </p> </td> 
   <td scope="col"> <p>OMBP</p> </td>
   <td scope="col"> <p>Coloca a hora de início da tarefa o mais próximo possível do início do projeto.</p> 
   <p>É a restrição padrão se o projeto usar um Modo de Cronograma a partir da Data Inicial e se a data inicial padrão do sistema para uma nova tarefa for definida como Baseado na Data Planejada do Projeto. </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-late-as-possible.md" class="MCXref xref">Visão geral da Restrição da Tarefa: O Mais Tarde Possível </a> </p> </td> 
   <td scope="col"> <p>OMTP</p> </td> 
   <td scope="col"> <p>Coloca a hora de conclusão da tarefa o mais próximo possível do fim do projeto.</p> 
   <p>Essa é a restrição padrão quando o Modo de Programação do projeto começa na Data de conclusão e o padrão do sistema ou grupo para a Data inicial de uma tarefa é definido como Baseado na Data Planejada do Projeto. </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/earliest-available-time.md" class="MCXref xref">Visão geral da Restrição da Tarefa: Primeiro Horário Disponível</a> </p> </td> 
   <td scope="col"> <p>MMCD</p> </td> 
 <td scope="col"> <p>Agenda uma tarefa para começar na hora mais próxima disponível depois de considerar quaisquer relações de predecessoras.</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/latest-available-time.md" class="MCXref xref">Visão geral da Restrição da Tarefa: Último Tempo Disponível</a> </p> </td> 
   <td scope="col"> <p>OMTD</p> </td> 
   <td scope="col"> <p>Agenda uma tarefa para começar no último horário disponível depois de considerar as relações predecessor-sucessor no projeto.</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-earlier-than.md" class="MCXref xref">Visão geral da Restrição de Tarefa: Não Iniciar Antes de</a> </p> </td> 
   <td scope="col"> <p>NIAD</p> </td> 
   <td scope="col"> <p>Agenda uma tarefa para iniciar depois da data que você especificar.</p> 
   <p>Essa é a restrição padrão se o Modo de Cronograma do projeto for a Data Inicial e se a Data Inicial padrão do sistema ou grupo para uma nova tarefa for definida como Hoje.   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-later-than.md" class="MCXref xref">Visão geral da Restrição de Tarefa: Não Iniciar Depois de </a> </p> </td> 
   <td scope="col"> <p>NIDD</p> </td> 
   <td scope="col"> <p>Agenda uma tarefa para iniciar antes da data que você especificar.</p> 
   <p>Essa é a restrição padrão se o Modo de programação do projeto for a partir da Data de conclusão e se o padrão do sistema ou grupo para a Data inicial de uma tarefa for definido como Hoje. 
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-earlier-than.md" class="MCXref xref">Visão geral da Restrição de Tarefa: Não Terminar Antes de</a> </p> </td> 
   <td scope="col"> <p>NTAD</p> </td>
   <td scope="col"> <p>Agenda uma tarefa para ser concluída após a data que você especificar.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-later-than.md" class="MCXref xref">Visão geral da Restrição de Tarefa: Não Terminar Depois de </a> </p> </td> 
   <td scope="col"> <p>NTDD</p> </td> 
   <td scope="col"> <p>Agenda uma tarefa para ser concluída antes da data que você especificar.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-start-on.md" class="MCXref xref">Visão geral da Restrição da Tarefa: Deve Iniciar em </a> </p> </td> 
   <td scope="col"> <p>PIE</p> </td> 
   <td scope="col"> <p>Agenda uma tarefa para iniciar exatamente em uma data específica.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-finish-on.md" class="MCXref xref">Visão geral da Restrição de Tarefa: Deve Terminar em</a> </p> </td> 
   <td scope="col"> <p>PTE</p> </td> 
   <td scope="col"> <p>Agenda uma tarefa para terminar em uma data específica.</p> </td>
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/fixed-dates.md" class="MCXref xref">Visão geral da Restrição da Tarefa: Datas Fixas</a> </p> </td> 
   <td> <p>Dt Fixas</p> </td> 
   <td> <p>Agenda uma tarefa para iniciar e terminar em datas específicas.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Visão geral das restrições padrão

Quando você cria novas tarefas, uma Restrição de tarefa é automaticamente selecionada pelo Workfront.

O Workfront usa duas variáveis para decidir qual Restrição de Tarefa é selecionada por padrão para uma nova tarefa:

* O campo **Cronograma do Projeto De** no projeto.

  Para obter informações sobre o campo Cronograma do Projeto - De, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

* A preferência **Data de Início** configurada pelo seu administrador de grupo ou Workfront na área **Tarefas e Problemas** da **Instalação**.

  Para obter informações sobre Preferências de tarefas e problemas, consulte a seção [Novos padrões de tarefas](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#new-task-defaults) em [Configurar preferências de tarefas e problemas em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

A tabela a seguir mostra a Restrição de Tarefa padrão ao escolher variáveis diferentes para seu projeto e suas novas tarefas:

| Cronograma do Projeto de | Data de Início da Tarefa | Padrão de Restrição de Tarefa |
|---|---|---|
| Data de início | Com base na Data de planejamento de projeto | O Mais Breve Possível |
| Data de início | Hoje | Não Iniciar Antes De |
| Data de término | Com base na Data de planejamento de projeto | O mais tarde possível |
| Data de término | Hoje | Não Iniciar Depois De |
