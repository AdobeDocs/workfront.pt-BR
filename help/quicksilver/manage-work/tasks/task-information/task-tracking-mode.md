---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visão geral do modo de rastreamento de tarefas
description: É possível ajustar a configuração do Modo de rastreamento de uma tarefa ao criar ou editar uma tarefa para controlar como e quando os indicadores de Status de Andamento de uma tarefa são exibidos. O Adobe Workfront exibe sinalizadores de Status de Andamento quando você configura determinadas configurações para rastrear o progresso em tarefas.
author: Alina
feature: Work Management
exl-id: 397b5593-ac01-40cf-b683-fcf671a53d26
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 3%

---

# Visão geral do modo de rastreamento de tarefas

É possível ajustar a configuração do Modo de rastreamento de uma tarefa ao criar ou editar uma tarefa para controlar como e quando os indicadores de Status de Andamento de uma tarefa são exibidos. O Adobe Workfront exibe sinalizadores de Status de Andamento quando você configura determinadas configurações para rastrear o progresso em tarefas.

Para obter mais informações sobre o Status de Andamento das tarefas, consulte [Visão geral do status de progresso da tarefa](../../../manage-work/tasks/task-information/task-progress-status.md).

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

Como proprietário de tarefa ou gerente de projeto, você pode selecionar como o Workfront indica o status do progresso em cada tarefa. Para obter informações sobre como definir o Modo de rastreamento em suas tarefas, consulte [Definir modo de rastreamento para tarefas](../../../manage-work/tasks/task-information/set-tracking-mode-for-tasks.md).

Você pode selecionar entre as seguintes opções:

* [Usuário deve atualizar](#user-must-update)
* [Assumir Em Dia](#assume-on-time)
* [Ignorar avisos de atrasos](#ignore-late-warnings)
* [Completar Automaticamente](#auto-complete)
* [Predecessor](#predecessor)

### Usuário deve atualizar {#user-must-update}

Quando essa opção é selecionada, o Workfront usa a porcentagem concluída e as horas reais da tarefa registradas para determinar o status de progresso da tarefa. Esta é a opção padrão.

### Assumir Em Dia {#assume-on-time}

A Workfront supõe que uma tarefa será concluída a tempo, independentemente do status de conclusão atual. Caso contrário, a Workfront assumirá automaticamente uma Data de conclusão planejada do próximo dia útil. Você ainda deve indicar quando a tarefa for concluída. Use essa opção quando os usuários não atualizarem regularmente suas tarefas.

### Ignorar avisos de atrasos {#ignore-late-warnings}

O Status de Andamento de uma tarefa será No Tempo até que se torne Atrasado. Por exemplo, se você agendar uma tarefa para demorar 10 dias e no dia em que ela deve ser concluída, a tarefa mostrará uma porcentagem concluída de 60%, o Workfront atualizará a Data de conclusão projetada adicionando quatro dias e o Status de progresso da tarefa se tornará Atrasado.

### Completar Automaticamente {#auto-complete}

A Workfront parte do princípio que as tarefas serão concluídas como programadas e as marca como concluídas em suas Datas de Vencimento ou de Conclusão Planejada. Até lá, o Workfront usa Porcentagem concluída e Horas reais registradas para determinar o Status de progresso. No entanto, independentemente do Status de progresso antes da data de conclusão agendada, o Workfront ainda marca a tarefa concluída.

As seguintes exceções existem:

* Se a tarefa tiver antecessores incompletos, ela não será automaticamente concluída até que todos os antecessores estejam concluídos.
* Se a tarefa tiver uma restrição de Data fixa, a tarefa sempre será concluída na Data de Conclusão Planejada, independentemente de seus antecessores serem concluídos.

>[!IMPORTANT]
>
>Selecionar para que as tarefas sejam concluídas automaticamente marca a tarefa Concluída quando a hora do projeto é recalculada. Se o Tipo de atualização do projeto for definido como Automático ou Automático e On Change, a linha do tempo do projeto será calculada diariamente. Para obter informações sobre os cálculos de linha do tempo em projetos, consulte [Recalcular linhas do tempo do projeto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).
>
>A hora da Data de conclusão real é a meia-noite do dia em que a linha do tempo é calculada automaticamente. O tempo usado para gerar esse carimbo de data e hora é o Fuso Horário de seu sistema, conforme definido pelo administrador do Workfront na seção Informações do Cliente da Configuração. Para obter informações sobre como configurar o Fuso horário do seu sistema, consulte [Configurar informações básicas para seu sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### Predecessor {#predecessor}

A Workfront estima a Data de conclusão projetada de uma tarefa de acordo com sua relação antecessora. O Status de Andamento de uma tarefa é determinado com base nessa estimativa. Por exemplo, a Tarefa B tem uma Duração de 1 dia e está programada para ser concluída dois dias após o antecessor, a Tarefa A, que deve levar cinco dias. Um usuário então atualiza a Tarefa B para 50% de conclusão, mas o antecessor, Tarefa A, ainda não começou. O Workfront processa a Tarefa dependente B para conclusão seis dias após a data de início da tarefa antecessora, permitindo 5 dias para a Tarefa A e 1 dia para a Tarefa B.
