---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visão geral do modo de rastreamento de tarefas
description: É possível ajustar a configuração do Modo de rastreamento de uma tarefa ao criar ou editar uma tarefa para controlar como e quando os indicadores de Status de progresso de uma tarefa são exibidos. O Adobe Workfront exibe sinalizadores de Status do Progresso quando você define determinadas configurações para rastrear o progresso em tarefas.
author: Alina
feature: Work Management
exl-id: 397b5593-ac01-40cf-b683-fcf671a53d26
source-git-commit: d2836549ee3c615201ce5f3454258e9af31efa42
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 2%

---

# Visão geral do modo de rastreamento de tarefas

<!-- Audited: 01/2024 -->

É possível ajustar a configuração do Modo de rastreamento de uma tarefa ao criar ou editar uma tarefa para controlar como e quando os indicadores de Status de progresso de uma tarefa são exibidos. O Adobe Workfront exibe sinalizadores de Status do Progresso quando você define determinadas configurações para rastrear o progresso em tarefas.

Para obter mais informações sobre o Status de Progresso das tarefas, consulte [Visão geral do Status de Progresso da Tarefa](../../../manage-work/tasks/task-information/task-progress-status.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Set Tracking Mode for tasks</h2>
<p>(NOTE: drafted, because we created a new article and linked it below. Left this article as a "Overview" article only.) </p>
<p>To set the tracking mode:</p>
<ol>
<li value="1">Go to the task you want to set the tracking mode for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png">next to the name of the task, then click&nbsp;<strong>Edit</strong>.</p> <p>The Edit Task dialog box opens. </p> </li>
<li value="3"> <p>In the&nbsp;<strong>Settings</strong> section, use the&nbsp;<strong>Tracking Mode</strong> drop-down menu to select the Tracking Mode for the task.</p> <p>For more information about the tracking mode options, see the <a href="#tracking-mode-options" class="MCXref xref" xrefformat="{para}">Tracking Mode options</a> section in this article. </p> </li>
<li value="4">Click&nbsp;<strong>Save Changes.</strong></li>
</ol>
</div>
-->

## Opções do modo de rastreamento {#tracking-mode-options}

Como proprietário de tarefa ou gerente de projeto, você pode selecionar como o Workfront indica o status do progresso em cada tarefa. Para obter informações sobre como definir o Modo de Acompanhamento em suas tarefas, consulte [Definir Modo de Acompanhamento para tarefas](../../../manage-work/tasks/task-information/set-tracking-mode-for-tasks.md).

Você pode selecionar entre as seguintes opções:

* [O Usuário Deve Atualizar](#user-must-update)
* [Assumir Em Dia](#assume-on-time)
* [Ignorar avisos de atrasos](#ignore-late-warnings)
* [Preenchimento Automático](#auto-complete)
* [Predecessor](#predecessor)

### Usuário deve atualizar {#user-must-update}

Quando essa opção é selecionada, o Workfront usa o Percentual concluído da tarefa e as Horas efetivas registradas para determinar o Status de progresso da tarefa. Esta é a opção padrão.

### Assumir Em Dia {#assume-on-time}

A Workfront presume que uma tarefa será concluída a tempo, independentemente do status de conclusão atual. Se a tarefa não for concluída no prazo (na Data de conclusão planejada), o Workfront assumirá automaticamente uma Data de conclusão planejada para o próximo dia útil. Você ainda deve indicar quando a tarefa é concluída. Use essa opção quando os usuários não atualizarem regularmente suas tarefas.

### Ignorar avisos de atrasos {#ignore-late-warnings}

O Status do Progresso de uma tarefa será No Prazo até ela se tornar Late. Por exemplo, se você programar uma tarefa para durar 10 dias e no dia em que ela deve ser concluída, a tarefa mostrará um Percentual concluído de 60%. Em seguida, o Workfront atualizará a Data de conclusão projetada adicionando quatro dias e o Status do Andamento da tarefa se tornará Atrasado.

### Completar Automaticamente {#auto-complete}

A Workfront presume que as tarefas serão concluídas conforme agendado e as marca como concluídas em suas Datas de Término Previstas ou Vencidas. Até lá, o Workfront usa o Percentual concluído e as Horas efetivas registradas para determinar o status do progresso. No entanto, independentemente do Status do progresso antes da data de conclusão agendada, o Workfront ainda marca a tarefa como concluída.

As seguintes exceções existem:

* Se a tarefa tiver predecessoras incompletas, ela não será automaticamente concluída até que todas as predecessoras sejam concluídas. Os predecessores devem ser aplicados.
* Se a tarefa tiver uma restrição de Data Fixa, a tarefa sempre será concluída na Data de Conclusão Planejada, independentemente de seus predecessores estarem concluídos.

>[!IMPORTANT]
>
>Selecionar a opção de conclusão automática das tarefas marca a tarefa como Concluída quando o horário do projeto for recalculado. Se o Tipo de atualização do projeto estiver definido como Automático ou Automático e Mediante alteração, a linha do tempo do projeto será calculada diariamente. Para obter informações sobre os recálculos de linha de tempo em projetos, consulte [Recalcular linhas de tempo do projeto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).
>
>A hora da Data de conclusão real é a meia-noite do dia em que a linha do tempo é calculada automaticamente. O horário usado para gerar esse carimbo de data e hora é o fuso horário do seu sistema, conforme definido pelo administrador do Workfront na seção Informações do cliente da Configuração. Para obter informações sobre como definir o fuso horário do sistema, consulte [Configurar informações básicas do sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### Predecessor {#predecessor}

A Workfront estima a Data de conclusão projetada de uma tarefa de acordo com seu relacionamento antecessor. O Progress Status de uma tarefa é determinado com base nessa estimativa. Por exemplo, a Tarefa B tem uma Duração de 1 dia e está programada para ser concluída dois dias após sua antecessora, a Tarefa A, que deve levar cinco dias. Um usuário atualiza a Tarefa B para 50% concluída, mas a predecessora, a Tarefa A, ainda não foi iniciada. O Workfront programa a Tarefa B dependente para conclusão seis dias após a data de início da tarefa predecessora, permitindo 5 dias para a Tarefa A e 1 dia para a Tarefa B.
