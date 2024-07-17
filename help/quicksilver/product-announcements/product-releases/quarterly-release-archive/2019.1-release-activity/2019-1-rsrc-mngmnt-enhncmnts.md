---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: Aprimoramentos no gerenciamento de recursos 2019.1
description: Esta página descreve todas as melhorias no Gerenciamento de recursos incluídas na versão 2019.1. A funcionalidade agora está disponível no ambiente de Produção do.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6eed6023-96cc-45d7-8dae-a36d45e92068
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 0%

---

# Aprimoramentos no gerenciamento de recursos 2019.1

Esta página descreve todas as melhorias no Gerenciamento de recursos incluídas na versão 2019.1. A funcionalidade agora está disponível no ambiente de Produção do.

Para obter uma lista de todas as alterações feitas em 2019.1, consulte a [visão geral da atividade da versão 2019.1](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md).

## Filtro padrão atualizado no Planejador de recursos

O filtro padrão no Planejador de recursos não filtra mais pelo Grupo do projeto.

Ao visualizar o Planejador de recursos, agora você vê apenas os projetos que são atuais e sensíveis à data por padrão. As informações dos seguintes projetos são incluídas por padrão:

* Com uma Data de conclusão planejada que ocorra após a primeira data do mês de hoje.
* Com uma Data de Início Planejada que ocorre antes da última data do quarto mês a partir de hoje.
* Com Status Atual ou de Planejamento.

Anteriormente, o filtro padrão recuperava as informações dos seguintes projetos adicionais:

* Com uma Data de conclusão planejada que ocorra após a primeira data do mês de hoje.
* Com uma Data de Início Planejada que ocorre antes da última data do quarto mês a partir de hoje.
* Com Status Atual ou de Planejamento.
* Com um Grupo que corresponda ao Grupo inicial do usuário que está conectado.

Para obter informações sobre como aplicar filtros ao Planejador de Recursos, consulte [Informações de filtro no Planejador de Recursos](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

## Uso de curingas para filtros do Planejador de recursos

Agora é possível usar curingas ao criar filtros no Planejador de recursos. Por exemplo, você pode usar $$USER.ID para filtrar informações sobre o usuário que está conectado, ou $$USER.companyID para filtrar informações sobre todos os usuários que pertencem à mesma empresa que o usuário que está conectado. Para obter uma lista completa de variáveis baseadas em usuário, consulte a seção [Variáveis de filtro curinga baseadas em usuário](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md#user-based-variables) em [Variáveis de filtro curinga](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

Anteriormente, os curingas não estavam disponíveis para os filtros do Planejador de recursos.

Para obter informações sobre a filtragem no Planejador de recursos, consulte [Informações de filtro no Planejador de recursos](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

<!--
<iframe class="mt-media" src="assets/290697527?title=0&byline=0&portrait=0" width="640px" height="360px" frameborder="0" allowfullscreen></iframe>
-->

## Compatibilidade com variáveis de filtro curinga baseadas em data no Planejador de recursos

Agora você pode usar qualquer versão da variável de filtro curinga $$TODAY ao criar um filtro no Planejador de recursos.

Antes desse aprimoramento, você poderia usar somente variáveis de filtro curinga baseadas em usuário.

Para obter informações sobre a filtragem no Planejador de recursos, consulte [Informações de filtro no Planejador de recursos](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

Para obter informações sobre variáveis de filtro curinga, consulte [Variáveis de filtro curinga](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Opções de exportação para a visualização Função no Planejador de recursos

Agora você pode selecionar quais níveis de informação serão exportados do Planejador de recursos na visualização Função. É possível exportar qualquer um dos itens a seguir:

* Somente funções
* Funções e projetos
* Funções, projetos e usuários

Antes desse aprimoramento, todos os níveis de informação eram exportados na visualização Função. Essas opções foram introduzidas nas visualizações Projeto e Usuário em uma versão anterior.

Para obter informações sobre como exportar informações do Planejador de recursos, consulte [Exportar informações do Planejador de recursos](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## Opções de Formatação de Dados para Exportação do Planejador de Recursos

Agora você pode selecionar como deseja exibir as informações no arquivo do Excel quando exportado do Planejador de recursos.

Você pode exibir a disponibilidade e a alocação de informações exportadas do Planejador de Recursos das seguintes maneiras:

* Desagrupado pelo nome dos objetos aos quais pertence. Nesse caso, os nomes dos objetos aos quais ele pertence são exibidos em cada linha de dados. (esta é a opção padrão)
* Agrupado pelo nome dos objetos aos quais pertence. Nesse caso, as informações no arquivo exportado aparecem como são exibidas no Workfront.

Antes desse aprimoramento, as informações no arquivo exportado apareciam como aparecem no Workfront.

Para obter informações sobre como exportar informações do Planejador de recursos, consulte [Exportar informações do Planejador de recursos](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## Cronograma persistente

>[!NOTE]
>
>As ferramentas de Agendamento de recursos foram substituídas e removidas do Workfront com a versão 23.1. Para obter informações sobre o agendamento de recursos usando o Balanceador de carga de trabalho, consulte [Visão geral do Balanceador de carga de trabalho](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

As linhas do tempo de agendamento agora mantêm o período selecionado ao atualizar a linha do tempo ou sair da página.

Antes desse aprimoramento, as linhas do tempo de agendamento retornavam ao período padrão quando você atualizava ou saía da página.

Esse aprimoramento está disponível nas seguintes áreas:

* Guia Agendamento na área Pessoas
* Guia Equipe Trabalhando Em
* Subguia Agendamento na guia Equipe de um Projeto

Para obter informações sobre como trabalhar com a linha do tempo nas áreas de Agendamento de recursos, consulte &quot;Introdução ao Agendamento de recursos&quot;.

## Novas opções de exportação no Planejador de recursos

Agora você pode selecionar quais níveis de informação serão exportados do Planejador de recursos. Na visualização Projeto, é possível exportar qualquer um dos seguintes itens:

* Somente projetos
* Projetos e funções
* Projetos, funções e usuários

Na Exibição de usuário, é possível exportar qualquer um dos itens a seguir:

* Somente usuários
* Usuários e projetos
* Usuários, Projetos, Funções, Tarefas e Problemas

Antes desse aprimoramento, todos os níveis de informação eram exportados em todas as visualizações do Planejador de recursos por padrão.

Para obter informações sobre como exportar informações do Planejador de recursos, consulte [Exportar informações do Planejador de recursos](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## Atualizar para a visualização Usuário no Planejador de recursos

Todos os usuários no sistema agora são exibidos na Visualização de usuário do Planejador de recursos, mas somente os usuários associados aos projetos filtrados também mostram informações sobre horas.

Antes desta atualização, somente os usuários atribuídos aos itens de trabalho nos projetos filtrados por você eram exibidos na visualização Usuário do Planejador de recursos.

É possível usar filtros baseados em usuário para reduzir o número de usuários exibidos na Exibição de usuário apenas para aqueles atribuídos aos projetos que você deseja exibir.

Para obter informações sobre filtros no Planejador de recursos, consulte [Informações sobre filtros no Planejador de recursos](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).
