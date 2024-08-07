---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: Aprimoramentos do projeto 2019.1
description: Esta página descreve todas as melhorias de projeto incluídas na versão 2019.1. A funcionalidade está disponível atualmente no ambiente de Pré-visualização. Ele será disponibilizado no ambiente de Produção do .
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7b39082a-ab96-4e54-8f28-96629760715a
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1461'
ht-degree: 1%

---

# Aprimoramentos do projeto 2019.1

Esta página descreve todas as melhorias de projeto incluídas na versão 2019.1. A funcionalidade está disponível atualmente no ambiente de Pré-visualização. Ele será disponibilizado no ambiente de Produção do .

>[!IMPORTANT]
>
>A funcionalidade descrita nesta página está sujeita a alterações antes da disponibilidade no ambiente de produção.

Para obter uma lista de todas as alterações feitas na versão 2019.1, consulte &quot;Visão geral da atividade da versão 2019.1&quot;.

**Para administradores**

* [Restaurar Modelos da Lixeira](#restore-templates-from-the-recycle-bin)
* [Mostrar carimbos de data e hora para campos de data na página inicial](#show-timestamps-for-date-fields-in-home)
* [Todos os tipos de duração disponíveis nas Preferências do projeto](#all-duration-types-available-under-project-preferences)

**Para todos os usuários**

* [Melhorias Agile](#agile-improvements)
* [Adicionar Tarefas e Problemas de uma Lista a uma Iteração](#add-tasks-and-issues-from-a-list-to-an-iteration)
* [Novos Tamanhos de Papel para Exportação do Gráfico de Gantt](#new-paper-sizes-for-gantt-chart-export)
* [Remoção do Acesso às Caixas de Diálogo do Gráfico de Gantt no Modo de Edição](#removed-access-to-dialog-boxes-in-the-gantt-chart-while-in-edit-mode)
* [Exibir Informações da Tarefa no Gráfico de Gantt da Lista de Projetos em um Programa ou Portfolio](#view-task-information-in-the-project-list-gantt-chart-in-a-program-or-portfolio)
* [Acessar o Gráfico de Gantt da Lista de Tarefas nos Modelos](#access-the-task-list-gantt-chart-on-templates)
* [Exibição do Projeto renomeada no Gráfico de Gantt](#renamed-the-project-view-on-the-gantt-chart)
* [Cenários de hipóteses no Gráfico de Gantt da Lista de Tarefas](#what-if-scenarios-in-the-task-list-gantt-chart)
* [Melhorias na Lista de Tarefas](#task-list-improvements)
* [Exibir Listas em Tela Inteira](#display-lists-in-full-screen)
* [Novas Listas em Áreas Adicionais](#new-lists-in-additional-areas)
* [Enviar um Relatório Entregue no Formato XLSX](#send-a-delivered-report-in-xlsx-format)
* [Exportar logs de auditoria](#export-audit-logs)

## Restaurar Modelos da Lixeira {#restore-templates-from-the-recycle-bin}

Os administradores do Workfront agora podem restaurar modelos na Lixeira. Assim como em outros itens excluídos, é possível restaurar um modelo até 30 dias a partir do momento em que ele foi excluído.

Para obter mais informações, consulte &quot;Restaurando itens excluídos&quot;.

## Mostrar carimbos de data e hora para campos de data na página inicial {#show-timestamps-for-date-fields-in-home}

Como administrador do Workfront, agora você pode optar por mostrar ou ocultar carimbos de data e hora de datas de vencimento na Lista de trabalho e no Calendário usando Modelos de layout. Por padrão, os carimbos de data e hora estão visíveis para usuários de modelo e não-modelo.

Para obter mais informações, consulte &quot;Personalizar a área inicial&quot; no artigo &quot;Criar e gerenciar modelos de layout&quot;.

## Todos os tipos de duração disponíveis nas Preferências do projeto {#all-duration-types-available-under-project-preferences}

Ao definir o tipo de duração padrão de tarefa e problema em Configurar > Preferências do projeto, você pode usar qualquer uma das seguintes opções:

Simples

Controlado pelo empenho

Atribuição Calculada

Trabalho calculado

Anteriormente, se você definisse Simples ou Controlado pelo Esforço como o tipo de duração padrão, não seria possível escolher Atribuição Calculada e Trabalho Calculado.

Para obter mais informações sobre como definir os padrões do tipo de duração de tarefas e problemas, consulte &quot;Preferências de tarefas e problemas&quot;

## Melhorias Agile {#agile-improvements}

As seguintes melhorias estão disponíveis na ferramenta Agile:

Kanban

Adicionar tarefas e problemas a um Quadro Kanban a partir de qualquer lista de tarefas ou relatório.

Anteriormente, só era possível adicionar tarefas ao quadro Kanban a partir do backlog. Não foi possível adicionar problemas.

Filtrar o quadro Kanban por usuários individuais na equipe.

Para obter mais informações, consulte &quot;Usando o Quadro Kanban&quot;.

Exibir e gerenciar problemas no Backlog Kanban.

Para obter mais informações, consulte &quot;Usando o Quadro Kanban.

Anteriormente, não era possível adicionar ou gerenciar problemas em um quadro Kanban.

Scrum

Filtre o storyboard de iteração por usuários individuais na equipe.

Para obter mais informações, consulte &quot;Usar o Storyboard Scrum Agile&quot;.

Anteriormente, não era possível filtrar por usuário nos quadros Kanban ou scrum.

## Adicionar tarefas e problemas de uma lista a uma iteração {#add-tasks-and-issues-from-a-list-to-an-iteration}

Agora é possível usar uma lista de tarefas ou problemas, um relatório ou um painel para adicionar histórias a uma iteração. Também é possível atribuir histórias a várias equipes em uma iteração.

Anteriormente, só era possível adicionar uma história a uma iteração da página de detalhes de tarefas ou problemas, além de adicionar histórias às iterações criadas pela equipe.

Para obter mais informações, consulte &quot;Criação e gerenciamento de iterações Agile&quot;.

## Enviar um relatório entregue no formato XLSX {#send-a-delivered-report-in-xlsx-format}

Agora é possível agendar um relatório para ser entregue no formato MS Excel (.xlsx), além de todos os outros formatos atuais.

Anteriormente, você podia enviar um relatório somente nos seguintes formatos:

HTML

PDF

MS Excel (.xls)

TSV

Para obter informações sobre a programação de relatórios para entrega, consulte &quot;Configuração de entregas de relatório&quot;.

## Melhorias na lista de tarefas {#task-list-improvements}

[atualizar 18.3 Beta 4 de onde foi removido]

As listas de tarefas recém-reprojetadas foram reativadas após uma breve remoção durante a versão 18.3 beta 4. Também introduzimos os seguintes recursos adicionais nas listas de tarefas que não faziam parte da versão original:

Substituição do menu de clique com o botão direito por um ícone Mais ao editar uma tarefa em linha.

As opções que estavam disponíveis no menu de clique com o botão direito do mouse ao editar várias tarefas em linha agora foram movidas para os ícones exibidos na parte superior da lista de tarefas.

Por padrão, as listas de tarefas exibem 2000 tarefas.

Quando o Workfront recalcula as linhas do tempo, os pontos de interrogação adjacentes às tarefas cujas datas estão sendo atualizadas foram substituídos por áreas cinza.

Para obter informações sobre como editar tarefas em linha, consulte &quot;Copiando e Duplicando Tarefas&quot; e &quot;Criando Relacionamentos de Predecessoras por Encadeamento de Tarefas&quot;.

Para obter informações sobre como recalcular linhas do tempo do projeto, consulte &quot;Recalculando linhas do tempo de projetos&quot;.

## Exibir listas em tela cheia {#display-lists-in-full-screen}

Quando uma lista de projetos ou tarefas é maior do que o tamanho da tela, a lista agora é exibida automaticamente em toda a janela do navegador à medida que você rola a tela. Isso aumenta a quantidade de informações visualizadas ao mesmo tempo e facilita o gerenciamento das listas.

Você pode exibir as seguintes listas em tela cheia:

Uma lista de projetos nas seguintes guias e subguias:

Projetos em que estou trabalhando

Projetos dos quais sou proprietário

Todos os Projetos

Guia Projetos em um Portfolio

Guia Projetos em um programa

Uma lista de tarefas nas seguintes guias:

Guia Tarefas em um projeto

Guia Subtarefas em uma Tarefa

Para obter informações sobre a exibição de objetos em listas, consulte &quot;Exibindo Itens em uma Lista&quot;.

## Novas listas em áreas adicionais {#new-lists-in-additional-areas}

Melhoramos o desempenho e a aparência das listas de projetos e tarefas nas seguintes áreas:

Guias Portfolio e Programas na área Projetos

Guia Subtarefas no nível da tarefa

Antes desse aprimoramento, as novas listas estavam disponíveis apenas nas seguintes áreas:

Guia Projetos na área Projetos

Guia Tarefas no nível do projeto

Para obter informações sobre a exibição de objetos em listas, consulte &quot;Exibindo Itens em uma Lista&quot;.

## Exibir Informações de Tarefa no Gráfico de Gantt da Lista de Projetos em um Programa ou Portfolio {#view-task-information-in-the-project-list-gantt-chart-in-a-program-or-portfolio}

Agora você pode ver as informações sobre as tarefas de um projeto na Lista de projetos Gráfico de Gantt dentro de um programa ou Portfolio.

Anteriormente, só era possível exibir informações sobre tarefas no Gráfico de Gantt da Lista de projetos na guia Projetos.

Para obter mais informações, consulte &quot;Exibindo Informações no Gráfico de Gantt&quot;.

## Cenários de Hipóteses no Gráfico de Gantt da Lista de Tarefas {#what-if-scenarios-in-the-task-list-gantt-chart}

Agora é possível executar as seguintes ações nas tarefas de um projeto quando elas são exibidas no modo de edição do Diagrama de Gantt:

Adicionar tarefas

Remover tarefas

Tarefas de edição em linha

Tarefas Duplicadas

Reorganizar Tarefas

Modificar Subtarefas

Embora você possa ver como as alterações afetam a linha do tempo do projeto, elas não são salvas imediatamente. Você pode salvá-los para atualizar permanentemente a linha do tempo do projeto ou pode cancelá-los.

Anteriormente, não era possível visualizar as alterações da lista de tarefas no Diagrama de Gantt.

Para obter informações sobre a edição de tarefas no Gráfico de Gantt, consulte &quot;Atualizando Informações no Gráfico de Gantt da Lista de Tarefas&quot;.

## Acessar o Diagrama de Gantt da Lista de Tarefas nos Modelos {#access-the-task-list-gantt-chart-on-templates}

Agora você pode acessar o Diagrama de Gantt da Lista de Tarefas em um modelo de projeto.

Anteriormente, não era possível exibir o Gráfico de Gantt na lista de tarefas de um modelo.

Para obter mais informações, consulte &quot;Introdução ao Gráfico de Gantt&quot;.

## Novos Tamanhos de Papel para Exportação de Gráfico de Gantt {#new-paper-sizes-for-gantt-chart-export}

Agora é possível imprimir o gráfico de Gantt nos tamanhos de papel A1 e A2.

Anteriormente, só era possível exportar para Carta, Ofício, Razão, A3 (disponível somente para alguns idiomas) e A4.

Para obter mais informações, consulte &quot;Exportar o Gráfico de Gantt para PDF&quot;.

## Exibição de projeto renomeada no Gráfico de Gantt {#renamed-the-project-view-on-the-gantt-chart}

Renomeamos a opção de exibição &quot;Projeto&quot; no gráfico de Gantt para &quot;Ajustar tudo&quot;. A opção de exibição ainda funciona como antes. O novo nome deve ser mais descritivo quanto ao que você visualiza quando a opção é selecionada.

Para obter mais informações, consulte &quot;Exibindo Informações no Gráfico de Gantt&quot;.

## Remoção do acesso a caixas de diálogo no Gráfico de Gantt durante o modo de edição {#removed-access-to-dialog-boxes-in-the-gantt-chart-while-in-edit-mode}

Não será mais possível acessar a caixa de diálogo Atribuições Avançadas enquanto o gráfico de Gantt estiver no modo de edição. Você só pode fazer edições em linha enquanto o Gráfico de Gantt da lista de tarefas está no modo de edição.

Anteriormente, era possível acessar a caixa de diálogo Atribuições avançadas enquanto o gráfico de Gantt estava no modo de edição, mas as alterações feitas no gráfico de Gantt eram salvas e o modo de edição era fechado.

Para obter mais informações sobre a edição do Diagrama de Gantt da Lista de Tarefas, consulte &quot;Atualizando informações no Diagrama de Gantt da Lista de Tarefas&quot;.

## Exportar logs de auditoria {#export-audit-logs}

Agora você pode exportar entradas de log de auditoria para um arquivo CSV. Você pode exportar até 50.000 entradas de log de auditoria para um arquivo CSV de uma vez.

Para obter mais informações, consulte &quot;Gerenciando logs de auditoria&quot;.
