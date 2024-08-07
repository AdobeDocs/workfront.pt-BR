---
content-type: release-notes
navigation-topic: 2019-2-release-activity
title: Aprimoramentos do projeto 2019.2
description: Esta página descreve todas as melhorias de projeto incluídas na versão 2019.2. A funcionalidade está planejada para estar disponível no ambiente de Produção na semana de 20 de maio de 2019.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 76292f90-af1a-4740-9b8e-b02a6303625c
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 1%

---

# Aprimoramentos do projeto 2019.2

Esta página descreve todas as melhorias de projeto incluídas na versão 2019.2. A funcionalidade está planejada para estar disponível no ambiente de Produção na semana de 20 de maio de 2019.

Para obter uma lista de todas as alterações feitas em 2019.2, consulte a [Visão Geral da Atividade da Versão 2019.2](../../../../product-announcements/product-releases/quarterly-release-archive/2019.2-release-activity/2019-2-release-activity-overview.md).

## Encontre Grupos Com Mais Rapidez Ao Personalizar Status

O menu suspenso na guia Status na área Configuração agora é um menu de digitação antecipada. Isso permite pesquisar e encontrar rapidamente qualquer grupo no sistema, facilitando a personalização dos status.

Anteriormente, o menu suspenso exibia um número limitado de grupos. Se o grupo desejado não fosse exibido, você teria que navegar até Configuração > Grupos e encontrar o grupo específico para personalizar os status do grupo.

Para obter mais informações, consulte [Criar ou editar um status](../../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Anexar processos padrão personalizados de Forms e aprovação a tarefas

Agora é possível configurar formulários personalizados padrão e processos de aprovação para anexar a tarefas ao adicionar tarefas a um projeto. Você pode definir as configurações padrão no nível do projeto.

Para obter informações sobre como configurar formulários personalizados padrão e processos de aprovação para tarefas no nível do projeto, consulte a seção &quot;Tarefas&quot; no artigo [Editar projetos](../../../../manage-work/projects/manage-projects/edit-projects.md).

## Exibir a Linha Inteira de uma Tarefa Pai em Negrito em uma Lista de Tarefas

Em uma lista de tarefas, a linha que contém uma tarefa pai é exibida em negrito. Essa alteração fica visível quando a lista é classificada pela estrutura de Detalhamento de trabalho ou pelo Número da tarefa em ordem crescente.

## Reverter Alterações nas Listas de Tarefas

Um novo botão Salvamento Automático na lista de tarefas permite que você selecione se deseja que as alterações feitas sejam salvas automaticamente ou se deseja ver os efeitos das alterações antes de salvá-las. Esta configuração se aplica à lista de tarefas e ao gráfico de Gantt.

Antes desse aprimoramento, todas as alterações eram sempre salvas automaticamente.

Para obter informações sobre como editar tarefas em uma lista de tarefas, consulte [Editar tarefas](../../../../manage-work/tasks/manage-tasks/edit-tasks.md).

Para obter informações sobre como editar tarefas no Gráfico de Gantt, consulte [Atualizar informações na lista de tarefas Gráfico de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Novos Padrões de Largura de Coluna em Novas Listas

Agora, o Workfront ajusta automaticamente a largura das colunas de acordo com as informações de formato do valor em cada coluna. Por exemplo, as colunas que exibem um número são mais largas que as que exibem o campo Descrição.

Antes dessa melhoria, as larguras de coluna nas novas visualizações de projeto e tarefa eram definidas como 100 pixels, a menos que especificado de outra forma.

Para obter informações sobre larguras de coluna, consulte [Modificar largura e ordem da coluna](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

## Desativar objetos não utilizados

>[!NOTE]
>
>Esse recurso foi lançado diretamente no ambiente de Produção durante o período de Visualização 2019.2.

Se você tiver objetos que não são mais usados, poderá desativá-los para ocultá-los das listas para impedir que os usuários os associem a outros objetos.

Agora, ao editar qualquer um dos objetos abaixo, você pode indicar se eles devem estar ativos. Os objetos definidos como Ativos aparecem em menus suspensos e campos de digitação antecipada e podem ser anexados a outros objetos. Objetos não definidos como Ativos não são visíveis em menus suspensos e campos de digitação antecipada para anexar a outros objetos.

* Processos de Aprovação
* Empresas
* Formulários personalizados
* Caminhos de Etapas
* Portfólios
* Programas
* Modelos

Tudo o que você desativar for usado atualmente continuará a funcionar como sempre funcionou, e não será removido ou bloqueado.

>[!IMPORTANT]
>
>Ao criar esses objetos por meio da API do Workfront, o valor padrão do parâmetro &quot;isActive&quot; é true. Este é um novo campo para todos os objetos e não está disponível para edição antes da versão 11 da API. Esse campo existia anteriormente para Portfolio, exceto que o valor padrão era false; ele será alterado para um valor padrão de true, começando com a versão 11 da API.

## Exibir o BCWS (Custo Orçado do Trabalho Agendado) e o BCWP (Custo Orçado do Trabalho Realizado) nas Exibições

Agora é possível exibir o BCWS (Custo Orçado do Trabalho Agendado) e o BCWP (Custo Orçado do Trabalho Executado) nas visualizações de projeto e tarefa.

Embora essas métricas de desempenho do projeto tenham sido usadas em cálculos financeiros no Workfront antes, elas não estavam visíveis no sistema antes desse aprimoramento.

Para obter informações sobre como calcular o BCWS, consulte [Calcular o BCWS (Custo do Trabalho Agendado)](../../../../manage-work/projects/project-finances/calculate-bcws.md).

Para obter informações sobre como calcular o COTR, consulte [Calcular o COTR (Custo Orçado do Trabalho Realizado)](../../../../manage-work/projects/project-finances/calculate-bcwp.md).

