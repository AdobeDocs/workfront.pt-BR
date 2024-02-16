---
content-type: release-notes
navigation-topic: product-releases-archive
title: Atividade da versão Beta 1 2017.3
description: Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão 2017.3. A funcionalidade nesta página foi disponibilizada no ambiente de Pré-visualização em 9 de agosto de 2017. Ele estará disponível no ambiente de Produção no início de novembro de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 33a91c25-98ec-4f08-b444-4e11e05e464b
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1426'
ht-degree: 0%

---

# Atividade da versão Beta 1 2017.3

Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão 2017.3. A funcionalidade nesta página foi disponibilizada no ambiente de Pré-visualização em 9 de agosto de 2017. Ele estará disponível no ambiente de Produção no início de novembro de 2017.

>[!IMPORTANT]
>
> A funcionalidade descrita nesta página está sujeita a alterações antes da disponibilidade no ambiente de produção.

Para obter uma lista de todas as alterações feitas em 2017.3, consulte  [Visão geral da atividade da versão 2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

A versão Beta 1 2017.3 contém melhorias para administradores do Workfront e outros usuários:

**Para administradores:**

* [Evite que tarefas e problemas sejam excluídos quando as horas são registradas](#prevent-tasks-and-issues-from-being-deleted-when-hours-are-logged)
* [Remoção da configuração de &quot;Acesso antecipado&quot; da área de configuração](#removal-of-the-early-access-setting-from-the-setup-area)
* [Alteração de endereço de email padrão do Workfront](#workfront-default-email-address-change)

**Para Todos Os Usuários:**

* [Melhorias no Agendamento de Recursos](#resource-scheduling-improvements)
* [Monitor widescreen](#widescreen-display)
* [Redimensionar e reordenar colunas em relatórios e listas](#resize-and-reorder-columns-in-reports-and-lists)
* [Opção Limpar dados personalizados ao copiar tarefas e problemas](#clear-custom-data-option-when-copying-tasks-and-issues)
* [Criar um projeto diretamente de um modelo](#create-a-project-directly-from-a-template)
* [Notificação no aplicativo para objetos inscritos](#in-app-notification-for-subscribed-objects)
* [@Tagging atualmente não disponível no ambiente de visualização](#tagging-currently-not-available-in-the-preview-environment)
* [Incluir Informações de Alocação de Usuário no Relatório de Utilização em um Projeto](#include-user-allocation-information-in-the-utilization-report-on-a-project)

## Melhorias no Agendamento de Recursos {#resource-scheduling-improvements}

>[!NOTE]
>
>As ferramentas de Agendamento de recursos foram substituídas e removidas do Workfront com a versão 23.1. Para obter informações sobre como programar recursos usando o Balanceador de carga de trabalho, consulte [Visão geral do Balanceador de carga de trabalho](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

As seguintes melhorias no agendamento de recursos estão disponíveis ao agendar recursos para uma equipe, para um projeto ou para vários projetos como gerente de recursos:

* [Exibir área de agendamento no modo de tela cheia](#view-scheduling-area-in-full-screen-mode)
* [Mais Opções de Intervalo de Datas para Exibir a Área de Programação de Recursos](#more-date-range-options-for-viewing-the-resource-scheduling-area)
* [Exibir Datas Projetadas na Linha do Tempo de Agendamento](#view-projected-dates-on-the-scheduling-timeline)

### Exibir área de agendamento no modo de tela cheia {#view-scheduling-area-in-full-screen-mode}

É possível exibir a linha do tempo de agendamento no modo de tela cheia, permitindo ver mais informações em uma única visualização. 

Para obter mais informações, consulte &quot;Introdução ao agendamento de recursos&quot;.

### Mais Opções de Intervalo de Datas para Exibir a Área de Programação de Recursos {#more-date-range-options-for-viewing-the-resource-scheduling-area}

Você pode exibir as seguintes opções adicionais de intervalo de datas ao exibir a linha do tempo de programação:

* Exibição em um dia
* Visualização em 4 semanas
* Visualização de 6 semanas

Antes dessa alteração, você poderia visualizar a linha do tempo do agendamento somente em uma visualização de 1, 2 ou 3 semanas. Esses intervalos de datas ainda estão disponíveis, além dos novos intervalos de datas.

Quando você exibe a linha do tempo do agendamento em uma visualização de um dia, as alocações de usuário (incluindo o total diário de horas) não podem ser exibidas.

Para obter mais informações, consulte &quot;Introdução ao agendamento de recursos&quot;.

### Exibir Datas Projetadas na Linha do Tempo de Agendamento {#view-projected-dates-on-the-scheduling-timeline}

Agora você pode configurar a linha do tempo de agendamento para mostrar as Datas projetadas em vez das Datas planejadas para tarefas e problemas. 

Antes dessa alteração, as tarefas e problemas na linha do tempo do agendamento mostravam apenas Datas planejadas.

Quando você exibe Datas Projetadas na linha do tempo de programação, as alocações de usuário (incluindo o total diário de horas) não podem ser exibidas.

Para obter mais informações, consulte &quot;Introdução ao agendamento de recursos&quot;.

## Monitor widescreen {#widescreen-display}

Ao exibir qualquer um dos seguintes objetos no Workfront, toda a janela do navegador é preenchida automaticamente:

* Projetos
* Tarefas
* Problemas
* Relatórios
* Painéis
* Calendários

Antes dessa alteração, havia duas barras laterais brancas em ambos os lados da área exibida. Agora, a visualização em widescreen se ajusta dinamicamente à largura da tela e da janela do navegador.

## Redimensionar e reordenar colunas em relatórios e listas {#resize-and-reorder-columns-in-reports-and-lists}

Agora é possível reordenar e redimensionar colunas em um relatório ou lista, sem precisar editar o relatório. (Essa funcionalidade foi removida com a desativação do ambiente de Acesso antecipado no início deste ano. Ele agora está sendo reintroduzido.)

Essa funcionalidade não está disponível para listas ou relatórios de painel, pois essas listas foram reprojetadas em uma nova estrutura de grade de dados. Todas as outras listas terão essa funcionalidade ativada nesta versão.

Para obter mais informações sobre como redimensionar e reordenar colunas, consulte [Modificar a largura e a ordem da coluna](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

## Opção Limpar dados personalizados ao copiar tarefas e problemas {#clear-custom-data-option-when-copying-tasks-and-issues}

Ao copiar uma tarefa ou problema, agora é possível selecionar uma opção para apagar dados personalizados. Quando você escolhe limpar os dados personalizados de uma tarefa ou problema, o formulário é copiado para o novo item, mas os dados personalizados no formulário não são. A limpeza de dados personalizados também afeta os formulários personalizados anexados aos documentos anexados aos itens ou os formulários personalizados anexados às despesas na tarefa.

Antes dessa alteração, os dados personalizados incluídos em um formulário personalizado também eram copiados para o novo item quando você copiava a tarefa ou problema. 

Para obter mais informações sobre copiar tarefas, consulte [Copiar e duplicar tarefas](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Para obter mais informações sobre cópia de problemas, consulte [Copiar problemas](../../../../manage-work/issues/manage-issues/copy-issues.md).

## Criar um projeto diretamente de um modelo {#create-a-project-directly-from-a-template}

Agora é possível criar um projeto a partir de um modelo, no nível do modelo.

Antes dessa alteração, você poderia criar um projeto a partir de um modelo somente na guia Projetos na área Projetos do Workfront, usando a **Novo projeto do modelo** opção.

Para obter mais informações sobre como criar um projeto a partir de um modelo, consulte [Criar um projeto usando um modelo](../../../../manage-work/projects/create-projects/create-project-from-template.md).

## Evite que tarefas e problemas sejam excluídos quando as horas são registradas {#prevent-tasks-and-issues-from-being-deleted-when-hours-are-logged}

Agora você pode configurar o Workfront para permitir ou impedir a exclusão de tarefas e problemas que tenham horas registradas.

Antes dessa alteração, quando você excluía uma tarefa ou problema em que as horas eram registradas, as horas eram excluídas com a tarefa ou problema, ou eram movidas para o projeto, dependendo das suas Preferências de Horas e Planilha de Horas.

Para obter mais informações sobre como excluir tarefas, consulte [Excluir tarefas](../../../../manage-work/tasks/manage-tasks/delete-tasks.md).

Para obter mais informações sobre exclusão de problemas, consulte [Excluir problemas](../../../../manage-work/issues/manage-issues/delete-issues.md).

Para obter mais informações sobre como ativar a configuração do sistema para exclusão de tarefas e problemas, consulte [Configurar preferências de tarefas e problemas em todo o sistema](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Remoção da configuração de &quot;Acesso antecipado&quot; da área de configuração {#removal-of-the-early-access-setting-from-the-setup-area}

Estamos removendo a configuração que permitia aos administradores do Workfront inscrever usuários para participar do ambiente de Acesso antecipado. Essa funcionalidade foi descontinuada no final de 2016. Não lançamos nenhuma nova funcionalidade para Acesso antecipado em 2017, e todos os recursos que estavam restantes nesse ambiente foram movidos para Produção.

Antes dessa alteração, os administradores do Workfront ainda podiam adicionar usuários ao ambiente de Acesso antecipado, embora não houvesse novos recursos para acessar.

## Alteração de endereço de email padrão do Workfront {#workfront-default-email-address-change}

O endereço de email padrão para emails de saída do Workfront foi alterado de [noreply@attask.com](mailto:noreply@attask.com) para [noreply@my.workfront.com](mailto:noreply@workfront.com).

Se você filtrar emails enviados do Workfront atualmente, será necessário alterar seu filtro para refletir o novo endereço padrão. 

A alteração no endereço padrão não afeta os endereços de email configurados do Workfront. 

Para obter mais informações, consulte.

## Notificação no aplicativo para objetos inscritos {#in-app-notification-for-subscribed-objects}

Quando um usuário faz um comentário sobre projetos, tarefas e problemas que você assinou, agora você recebe uma notificação no aplicativo. Para saber mais sobre as notificações no aplicativo de assinatura, consulte [Exibir e gerenciar notificações no aplicativo](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

Dependendo dos recursos ativados pelo administrador do Workfront, você também pode receber notificações por email sobre itens inscritos. É possível cancelar facilmente a inscrição de um item por meio de um link em um email de inscrição, conforme descrito em [Notificações do Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).

Antes dessa alteração, você sempre recebia uma notificação por email sobre itens inscritos e não havia opção de receber uma notificação no aplicativo.

Embora você possa desativar o email de subscrição, não pode desativar as notificações no aplicativo para itens subscritos. Para obter mais informações, consulte [Configurar notificações de eventos para todos no sistema](../../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

Para saber mais sobre a assinatura de itens, consulte [Assinar itens no Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md).

## @Tagging atualmente não disponível no ambiente de visualização {#tagging-currently-not-available-in-the-preview-environment}

À medida que trabalhamos para trazer a funcionalidade de formato Rich Text para o fluxo de atualização, você não poderá usar temporariamente o símbolo @ para marcar outros usuários no fluxo de atualização para os seguintes objetos no Ambiente de visualização:

* Projeto
* Tarefa
* Problema
* Planilha de horas

Você ainda pode marcar outras pessoas clicando no link **Incluir outros nesta atualização** ícone.

Para obter mais informações, consulte [Marcar outros usuários em atualizações](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Incluir Informações de Alocação de Usuário no Relatório de Utilização em um Projeto {#include-user-allocation-information-in-the-utilization-report-on-a-project}

>[!NOTE]
>
>As ferramentas de Agendamento de recursos foram substituídas e removidas do Workfront com a versão 23.1. Para obter informações sobre como programar recursos usando o Balanceador de carga de trabalho, consulte [Visão geral do Balanceador de carga de trabalho](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

O Relatório de utilização em um projeto agora considera se as Horas planejadas foram realocadas na duração de uma tarefa. Quando a alocação de horas do usuário tiver sido modificada (conforme descrito em &quot;Gerenciar alocações de usuários nas áreas de Agendamento&quot;), os dados no Relatório de Utilização poderão ser afetados se as datas selecionadas no Relatório de Utilização contiverem apenas uma parte de uma tarefa.

Para obter mais informações, consulte [Visão Geral do relatório de Utilização de Recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).
