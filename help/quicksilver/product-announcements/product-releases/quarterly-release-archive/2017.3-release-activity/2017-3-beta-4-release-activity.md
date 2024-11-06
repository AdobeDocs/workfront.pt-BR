---
content-type: release-notes
navigation-topic: product-releases-archive
title: Atividade da versão 2017.3 do Beta 4
description: Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão 2017.3 do Beta 4. A funcionalidade nesta página foi disponibilizada no ambiente de Pré-visualização na semana de 25 de setembro de 2017. Ele estará disponível no ambiente de Produção no início de novembro de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d6bb889c-a057-453f-8f80-761cfb1ad4a1
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '1676'
ht-degree: 0%

---

# Atividade da versão 2017.3 do Beta 4

Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão 2017.3 do Beta 4. A funcionalidade nesta página foi disponibilizada no ambiente de Pré-visualização na semana de 25 de setembro de 2017. Ele estará disponível no ambiente de Produção no início de novembro de 2017.

>[!IMPORTANT]
>
> A funcionalidade descrita nesta página está sujeita a alterações antes da disponibilidade no ambiente de produção.

Para obter uma lista de todas as alterações feitas em 2017.3, consulte  Visão geral da atividade da versão [2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

A versão 2017.3 do Beta 4 contém melhorias para administradores do Workfront e outros usuários:

**Para Administradores**

* [Nova Área de Preferências de Gerenciamento de Recursos na Área Configuração](#new-resource-management-preferences-area-in-the-setup-area)

**Para Todos Os Usuários**

* [Tarefas Duplicadas](#duplicate-tasks)
* [Automatizar Atribuições Ao Agendar Recursos](#automate-assignments-when-scheduling-resources)
* [Modificar atribuições para várias tarefas ao agendar recursos](#modify-assignments-for-multiple-tasks-when-scheduling-resources)
* [Aplicar Distribuição FTE ao Planejador de Recursos](#apply-fte-distribution-to-the-resource-planner)
* [A Seção Função de Trabalho para Configurações de Usuário Inclui a Porcentagem de Disponibilidade de FTE](#job-role-section-for-user-settings-includes-percentage-of-fte-availability)
* [Salvar e Gerenciar Filtros no Relatório de Utilização em um Projeto](#save-and-manage-filters-in-the-utilization-report-on-a-project)
* [Opções de Filtragem Adicionais no Relatório de Utilização](#additional-filtering-options-in-the-utilization-report)
* [Exibir o Relatório de Utilização por Programa ou Portfolio](#view-the-utilization-report-by-program-or-portfolio)
* [Mostrar Informações do Problema Original nos Relatórios de Projeto e Tarefa](#show-original-issue-information-in-project-and-task-reports)
* [As Atualizações do Sistema de Filtro no Fluxo de Atualização Agora São Persistentes entre Objetos](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects)
* [Relatório sobre Estágios de Prova Ativos no Workfront](#report-on-active-proof-stages-within-workfront)
* [Atribuir Perfis de Permissão Workfront Proof Personalizados a Usuários no Workfront](#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront)
* [Recurso de hora adicionado às assinaturas de evento](#hour-resource-added-to-event-subscriptions)

## Tarefas Duplicadas {#duplicate-tasks}

Agora é possível duplicar rapidamente uma tarefa ou um conjunto de tarefas em um projeto. Essa ação cria uma tarefa idêntica à original. Não há opções adicionais durante o processo de duplicação que permitam fazer alterações na tarefa recém-criada.  

Antes dessa alteração, você poderia copiar uma tarefa para um novo projeto ou para o projeto existente e modificar algumas informações à medida que as copiava.

Para  mais informações sobre duplicação de tarefas, consulte [Copiar e duplicar tarefas](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

## Automatizar Atribuições Ao Agendar Recursos {#automate-assignments-when-scheduling-resources}

>[!NOTE]
>
>As ferramentas de Agendamento de recursos foram substituídas e removidas do Workfront com a versão 23.1. Para obter informações sobre o agendamento de recursos usando o Balanceador de carga de trabalho, consulte [Visão geral do Balanceador de carga de trabalho](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Agora você pode permitir que a Workfront proponha automaticamente atribuições para tarefas e problemas não atribuídos ao agendar recursos para vários projetos (na guia Agendamento) ou ao agendar recursos para um único projeto (na guia Equipe).

O Workfront analisa as atribuições de trabalho atuais entre os usuários disponíveis e propõe atribuições inteligentes e lógicas para quaisquer tarefas ou problemas que ainda não foram atribuídos. Você pode modificar qualquer atribuição proposta ou existente antes de finalizar as atribuições.

Para obter mais informações, consulte &quot;Atribuir manualmente tarefas e problemas não atribuídos nas áreas de Agendamento&quot;.

## Modificar Atribuições para Várias Tarefas ao Agendar Recursos {#modify-assignments-for-multiple-tasks-when-scheduling-resources}

Ao atribuir, trocar ou desatribuir usuários em massa ao agendar recursos (na guia Agendamento ou na guia Equipe), agora é possível modificar atribuições para tarefas específicas que você designar (incluindo todas as subtarefas e problemas associados) em um ou mais projetos.

Antes dessa alteração, você poderia modificar atribuições para tarefas e problemas somente em projetos inteiros (não poderia designar tarefas específicas em um projeto).

Para obter mais informações, consulte &quot;Atribuir manualmente tarefas e problemas não atribuídos nas áreas de Agendamento&quot;.

## Aplicar Distribuição FTE ao Planejador de Recursos {#apply-fte-distribution-to-the-resource-planner}

>[!NOTE]
>
>No momento, essa funcionalidade não está disponível na Pré-visualização em todos os clusters.

Agora você pode exibir a quantidade correta de Horas Disponíveis para cada função do usuário com base no Percentual de Disponibilidade FTE para cada função, quando os usuários tiverem mais de uma função.

Por exemplo, se o cronograma de um usuário indicar que ele está disponível para trabalhar 100 horas em um mês, e seu Percentual de disponibilidade de FTE para a Função principal é de 75% e o Percentual de disponibilidade de FTE de sua Outra Função é de 25%, o Planejador de Recursos listará o usuário com 75 Horas Disponíveis na Função principal e com 25 Horas Disponíveis na Outra Função.

Antes dessa alteração, o nome do usuário exibido no Planejador de recursos somente para a Função principal, e a disponibilidade total do usuário com base em seu agendamento (100 horas) era associada somente à Função principal. A Outra Função do usuário exibida no Planejador de Recursos somente se o usuário foi atribuído a uma tarefa nessa função e as Horas Disponíveis para o usuário na Outra Função eram zero.

Para obter mais informações sobre como Horas Disponíveis e FTEs Disponíveis são calculados para usuários e funções no Planejador de Recursos, consulte [Visão geral do cálculo de horas e FTE para usuários e funções no Planejador de Recursos](../../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

## A Seção Função de Trabalho para Configurações do Usuário Inclui Porcentagem de Disponibilidade de FTE {#job-role-section-for-user-settings-includes-percentage-of-fte-availability}

>[!NOTE]
>
>No momento, essa funcionalidade não está disponível na Pré-visualização em todos os clusters.

Agora, ao atualizar um perfil de usuário, você pode adicionar outras funções de trabalho a um usuário e definir o percentual do FTE alocado para cada função de trabalho.

Antes dessa alteração, não era possível alocar uma quantidade específica de FTE para qualquer uma das funções de trabalho às quais o usuário estava associado.

Para obter mais informações sobre como atualizar a Porcentagem de Disponibilidade de FTE para as funções de trabalho do usuário, consulte [Editar perfil de usuário](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) ou [Configurar minhas configurações](../../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

## Nova Área de Preferências de Gerenciamento de Recursos na Área Configuração {#new-resource-management-preferences-area-in-the-setup-area}

Agora você pode encontrar uma nova área em Configuração chamada Gerenciamento de recursos. Nesta área, introduzimos uma configuração que permite especificar como calcular a disponibilidade de usuários no Planejador de recursos. Você pode calculá-la usando os seguintes métodos:

* Manualmente: A Programação Padrão do sistema, além do FTE individual do usuário, é usada para determinar a disponibilidade de horas do usuário no Planejador de Recursos. O Cronograma do usuário é ignorado.
* Automaticamente: o Agendamento do usuário é usado para determinar a disponibilidade de horas do usuário no Planejador de recursos. A disponibilidade de FTE é calculada com base no Cronograma do usuário e no Cronograma padrão. O valor do FTE do usuário é ignorado. 

Para obter mais informações sobre como configurar preferências de Gerenciamento de Recursos para o seu sistema, consulte [Configurar preferências de Gerenciamento de Recursos](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Salvar e Gerenciar Filtros no Relatório de Utilização em um Projeto {#save-and-manage-filters-in-the-utilization-report-on-a-project}

Agora é possível salvar os filtros criados no relatório de Utilização. Além disso, é possível renomear um filtro salvo, duplicar um filtro salvo, excluir um filtro salvo ou modificar um filtro salvo.

Anteriormente, você tinha que especificar opções de filtro individuais cada vez que filtrava o relatório de Utilização.

Para obter mais informações sobre como salvar e gerenciar filtros no relatório de Utilização, consulte [Visão Geral do Relatório de Utilização de Recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) em [Visão Geral do Relatório de Utilização de Recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Opções de Filtragem Adicionais no Relatório de Utilização {#additional-filtering-options-in-the-utilization-report}

Agora, ao executar o relatório de Utilização, novos campos de filtragem para Portfolio, Programas e Projetos agora estão disponíveis ao criar seu filtro, além dos campos Tarefas, Problemas e Funções que estavam disponíveis anteriormente.

Antes dessa alteração, você só podia filtrar por portfólio, programa e projeto adicionando uma nova regra de filtro.

Para obter mais informações, consulte [Visão Geral do Relatório de Utilização de Recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) em [Visão Geral do Relatório de Utilização de Recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Exibir o Relatório de Utilização por Programa ou Portfolio {#view-the-utilization-report-by-program-or-portfolio}

Agora é possível exibir um relatório de Utilização por programa ou portfólio. Isso permite que você veja informações de vários projetos em um único Relatório de Utilização.

Para facilitar essa alteração, a guia Utilização agora está disponível na área Relatórios no Workfront, bem como em um projeto individual.

Antes dessa alteração, os Relatórios de Utilização podiam ser acessados somente em um projeto.

Para obter mais informações, consulte  [Visão geral do relatório de Utilização de Recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md). 

## Mostrar Informações do Problema Original nos Relatórios de Projeto e Tarefa {#show-original-issue-information-in-project-and-task-reports}

>[!NOTE]
>
>No momento, essa funcionalidade não está disponível na Pré-visualização em todos os clusters.

Agora você pode encontrar as seguintes informações sobre o problema original em um projeto ou relatório de tarefa, para os projetos e tarefas que foram criados pela conversão de um problema:

* Data de entrada do problema original
* Nome Original do Problema
* ID do Originador da Questão Original

Essas informações podem ser exibidas em um relatório ou lista de tarefas ou de projetos, criando uma exibição personalizada no modo de texto.

Antes dessa alteração, você não podia relatar essas informações.

Para obter mais informações sobre como criar a exibição de modo de texto personalizado que captura as informações do problema original, consulte [Exibir: exibir informações do problema original em listas de tarefas ou projetos](../../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

## Filtrar atualizações do sistema no fluxo de atualização agora é persistente entre objetos {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

>[!NOTE]
>
>Essa funcionalidade não foi lançada no ambiente de Pré-visualização com o Beta 4. Ele estará disponível na Pré-visualização na primeira metade de outubro.

A opção Filtrar atualizações do sistema agora é persistente entre objetos no site do Workfront. Isso permite ocultar atualizações do sistema e exibir somente comentários do usuário no fluxo de atualização em um objeto, e fazer com que essa configuração permaneça conforme você navega para outros objetos.

Antes dessa alteração, você tinha que optar por filtrar as atualizações do sistema para cada objeto à medida que navegava pelo site do Workfront.

Para obter mais informações, consulte [Atualizar trabalho](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Relatório sobre Estágios de prova ativos no Workfront {#report-on-active-proof-stages-within-workfront}

Ao criar um relatório de Versão do documento no Workfront, agora há uma coluna chamada &quot;Estágios de prova ativos&quot;. Essa coluna permite visualizar o estágio de prova que está ativo atualmente em cada versão de documento no relatório. O nome do estágio é exibido na coluna &quot;Estágios de prova ativos&quot;. Se nenhum estágio estiver ativo na versão do documento, a coluna ficará em branco.

Para obter mais informações sobre campos disponíveis em exibições e relatórios, consulte [Glossário da terminologia do Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Atribuir perfis de permissão personalizados do Workfront Proof aos usuários no Workfront {#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront}

Agora, ao ativar recursos de prova para um usuário no Workfront, você pode atribuir um perfil de permissão personalizado do Workfront Proof. 

Antes dessa alteração, somente os seguintes perfis de permissão estavam disponíveis: Supervisor, Gerente, Administrador.

## Recurso de hora adicionado às assinaturas de evento {#hour-resource-added-to-event-subscriptions}

Usando o novo recurso Hora, agora é possível criar uma assinatura de evento para manter seu aplicativo de faturamento sincronizado com o Workfront.

Para saber mais sobre assinaturas de evento, consulte [API de Assinatura de Evento](../../../../wf-api/general/event-subs-api.md).
