---
content-type: overview
product-area: timesheets
navigation-topic: timesheets-navigation-topic
title: Noções básicas sobre o layout da folha de horas
description: Este artigo descreve o layout das folhas de horas no Adobe Workfront, permitindo entender melhor como personalizar e utilizar as folhas de horas para gravar tempo.
author: Alina
feature: Timesheets
exl-id: 31c48a50-5235-495c-8e46-0974ed98ede1
source-git-commit: ca552b80e9d78fd09068d72479e1b2bddc596c70
workflow-type: tm+mt
source-wordcount: '1043'
ht-degree: 1%

---

# Noções básicas sobre o layout da folha de horas

Este artigo descreve o layout das folhas de horas no Adobe Workfront, permitindo entender melhor como personalizar e utilizar as folhas de horas para gravar tempo.

A folha de horas e as Preferências de hora controlam o que aparece em uma folha de horas. Este artigo fornece uma visão geral de todas as opções disponíveis. Para obter mais informações, consulte [Configurar preferências de hora e folha de ponto](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Para obter informações sobre como registrar o tempo em uma folha de tempo, consulte [Tempo de registro](../../timesheets/create-and-manage-timesheets/log-time.md).

![Layout da folha de ponto](assets/timesheet-layout-unshimmed.png)

Estas são as áreas de uma folha de ponto:

* [Cabeçalho da folha de ponto](#timesheet-header)
* [O painel esquerdo](#the-left-panel)
* [Itens de trabalho](#work-items)
* [Barra de Ferramentas](#toolbar)
* [Rodapé da folha de ponto](#timesheet-footer)
* [Função](#job-role)
* [Tipo de hora](#hour-type)
* [Área de atualizações no painel esquerdo](#updates-area-in-the-left-panel)
* [Painel Resumo](#summary-panel)
* [Intervalo de tempo e área de entrada de hora](#time-frame-and-hour-entry-area)
* [Comentários de entrada de hora](#hour-entry-comments)
* [Horas](#hours)
* [Totais](#totals)

## Cabeçalho da folha de ponto

![](assets/timesheet-title-unshimmed-redesign.png)

O cabeçalho da folha de ponto inclui as seguintes informações:

* O período da folha de ponto.
* A área Ações que inclui o seguinte:
   * Um ícone de estrela para adicionar as folhas de horas à lista de Favoritos.
   * O ícone Mais com uma opção Excluir, onde você pode excluir a folha de ponto.
* O nome do proprietário da folha de ponto.
* O número Total de horas para horas registradas para itens exibidos na folha de horas.
* O número de horas extras. Esta é uma entrada manual e é visível somente quando a variável **Hora excedente** está ativada em uma folha de ponto. Para obter mais informações, consulte [Editar informações da folha de ponto](../create-and-manage-timesheets/edit-timesheets.md).

>[!TIP]
>
>Não é possível registrar um número maior de horas extras do que o total de horas atual na folha de horas. Por exemplo, se você fez logon por 7 horas na folha de ponto até o momento, não é possível registrar 8 horas extras.


* O status da folha de ponto.

## O painel esquerdo

![](assets/timesheet-left-panel-unshimmed-redesign.png)

Você pode acessar as seguintes seções no painel esquerdo:

* **Folha de Horas**: Exibe a folha de ponto real.
* **Atualizações**: Exibe comentários e atualizações do sistema para a folha de ponto. Para obter mais informações, consulte o [Área de atualizações no painel esquerdo](#updates-area-in-the-left-panel) neste artigo.

## Itens de trabalho

![](assets/timesheet-object-names-unshimmed-redesign.png)

Os itens de trabalho são projetos, tarefas e problemas para os quais você deseja registrar tempo. Clicar na seta para baixo na linha de cabeçalho recolhe os projetos e as tarefas e problemas listados abaixo. Clicar na seta apontando para baixo ao lado do nome de um projeto recolhe os itens de trabalho para esse projeto.

Tarefas, problemas e projetos em que o tempo é registrado fora da folha de ponto ou os itens planejados durante o período da folha de ponto aparecem aqui automaticamente.

## Barra de Ferramentas

![](assets/timesheet-toolbar-unshimmed-redesign.png)

A barra de ferramentas inclui as seguintes opções:

* O botão Adicionar item, onde você pode adicionar projetos, tarefas ou problemas.
* O ícone de filtro rápido para procurar tarefas ou problemas na folha de horas.
* O **Mostrar comentários** configuração que permite exibir ou ocultar comentários de hora que são registrados para entradas de projeto, tarefa ou de hora de emissão.
* Ícone de tela cheia , onde você pode exibir a folha de ponto no modo de tela cheia.
* **Abrir resumo** ou **Fechar resumo**), onde é possível abrir ou fechar o painel Resumo para ver informações adicionais sobre tarefas ou problemas. Isso não está disponível para projetos.

Para obter mais informações, consulte [Tempo de registro](../create-and-manage-timesheets/log-time.md).

## Rodapé da folha de ponto

![](assets/timesheet-footer-unshimmed-redesign.png)

Você pode clicar nos botões Enviar para Aprovação, Fechar, Aprovar e Rejeitar nesta área para fechar ou rejeitar uma aprovação de folha de ponto.

Essa área também contém informações sobre quando a folha de ponto foi salva pela última vez. Todas as alterações feitas nas informações na folha de ponto são salvas automaticamente.

## Função de trabalho

![](assets/timesheet-job-role-area-unshimmed-redesign.png)

Você pode selecionar uma função de cargo diferente para associar às entradas de hora. O administrador da Workfront deve habilitar a configuração Atribuir funções de trabalho a entradas de hora manualmente. A função de trabalho especificada para você quando é atribuída à tarefa ou o problema é exibido por padrão. Se você não tiver uma função de trabalho atribuída na tarefa ou no problema, sua Função primária será exibida como padrão. Para obter mais informações, consulte o artigo [Configurar preferências de hora e folha de ponto](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Você pode registrar entradas de várias horas para o mesmo item de trabalho para diferentes funções. Para obter mais informações, consulte [Tempo de registro](../create-and-manage-timesheets/log-time.md).

## Tipo de hora

![](assets/timesheet-hour-type-unshimmed-redesign.png)

Você pode selecionar tipos de horas diferentes para associar às entradas de hora em cada item. Esse campo é exibido somente quando o administrador do Workfront o habilita para seu ambiente. Para obter informações, consulte o artigo [Configurar preferências de hora e folha de ponto](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Você pode registrar entradas de várias horas para o mesmo item de trabalho para tipos de horas diferentes. Para obter mais informações, consulte [Tempo de registro](../create-and-manage-timesheets/log-time.md).

## Área de atualizações no painel esquerdo

![](assets/timesheet-updates-section-unshimmed-redesign.png)

Você pode fazer comentários em uma folha de ponto para se comunicar com seus aprovadores da folha de ponto ou outros usuários na seção Atualizações no painel esquerdo.

Quaisquer comentários feitos na folha de ponto são exibidos nessa área, na parte inferior da folha de ponto. Essa área é exibida abaixo da folha de ponto e acima do rodapé da folha de ponto. Para obter mais informações, consulte [Exibir e gerenciar comentários em uma folha de ponto](../create-and-manage-timesheets/view-and-manage-comments-timesheets.md).

## Painel Resumo

![](assets/timesheet-summary-panel-for-task-unshimmed-redesign.png)

Você pode acessar o painel Resumo para tarefas ou problemas exibidos em uma folha de ponto. A partir daqui, você pode comentar tarefas e problemas ou atualizar suas informações. Para obter mais informações, consulte [Visão geral do resumo](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

Os comentários inseridos para os itens de trabalho no painel Resumo da folha de ponto são exibidos na área Atualizações da tarefa ou do problema. O painel Resumo não está disponível para projetos.

## Intervalo de tempo e área de entrada de hora

![](assets/timesheet-time-frame-log-time-area.png)

O período da folha de ponto é exibido à direita dos itens de trabalho.

Você pode criar folhas de horas para uma, duas ou quatro semanas.

O intervalo de tempo é exibido em incrementos de semana inteira. Os dias fora do período especificado da folha de ponto estão esmaecidos. Não é possível registrar a hora para dias que estão fora do intervalo de tempo da folha de ponto.

Para obter mais informações, consulte [Criar folha de ponto de uso único](../create-and-manage-timesheets/create-tmshts.md) ou [Criar, editar e atribuir perfis de folha de ponto](../create-and-manage-timesheets/create-timesheet-profiles.md).

<!--drafted for the resize columns in timesheets story - make this blurb a TIP when the story is released: 
You can resize the columns that display different weeks, the time frame, or the work item areas by dragging and dropping the vertical lines that separate them.-->

## Comentários de entrada de hora

![](assets/timesheet-hour-entry-comment-button-unshimmed-redesign.png)

Você pode adicionar um comentário para cada entrada de hora que você adicionar à sua folha de horas.

Os comentários inseridos na caixa de comentário da entrada de hora são exibidos na folha de horas, em cada item de trabalho em que você registrou a hora em que a **Mostrar comentários** está ativada na barra de ferramentas.

![](assets/hour-entry-comment-under-task-in-timesheet-unshimmed-redesign.png)

## Horas

![](assets/timesheet-hours-area-unshimmed-redesign.png)

A folha de ponto fornece campos de entrada para cada item de trabalho e dia do intervalo de folha de ponto para registrar o tempo gasto trabalhando no item. À medida que você registra o tempo, o item em que você registra o tempo para os destaques em azul claro e a caixa de hora é contornado em azul escuro.

## Totais

![](assets/timesheet-totals-column-and-header-unshimmed-redesign.png)

Revise a soma de todas as horas inseridas na folha de ponto, resumida por dia (no cabeçalho da folha de ponto) e por objeto (na última coluna).
