---
content-type: release-notes
navigation-topic: product-releases-archive
title: Atividade da versão Beta 2 de 2018.2
description: Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão 2018.2 Beta 2. A funcionalidade foi disponibilizada no ambiente de Pré-visualização em 5 de abril de 2018. Ele estará disponível no ambiente de Produção em junho de 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: c8ef68f5-53db-4c3c-af0f-e1c98521ec27
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# Atividade da versão Beta 2 de 2018.2

Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão 2018.2 Beta 2. A funcionalidade foi disponibilizada no ambiente de Pré-visualização em 5 de abril de 2018. Ele estará disponível no ambiente de Produção em junho de 2018.

>[!IMPORTANT]
>
> A funcionalidade descrita nesta página está sujeita a alterações antes da disponibilidade no ambiente de produção.

Para obter uma lista de todas as alterações feitas em 2018.2, consulte  [Visão geral da atividade da versão 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

A versão Beta 2 de 2018.2 contém as seguintes melhorias:

* [Editar campos diretamente da área inicial](#edit-fields-directly-from-the-home-area)
* [Registrar Tempo em Dias](#log-time-in-days)
* [Exibir Relações de Predecessoras entre Projetos no Gráfico de Gantt em uma Lista de Projetos](#view-cross-project-predecessor-relationships-on-the-gantt-chart-in-a-list-of-projects)
* [Usar o custo orçado no Portfolio Otimizer para calcular as finanças do Portfolio](#use-budgeted-cost-in-the-portfolio-optimizer-to-calculate-portfolio-finances)
* [Relatório de Utilização: Preenche Horas Orçadas da Nova Área de Orçamento de Recursos](#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area) (Somente visualização)

* [Relatório de Utilização: Exibir Horas Orçadas por Usuário em um Projeto](#utilization-report-view-budgeted-hours-by-user-on-a-project) (Somente visualização)

* [Progresso da prova na lista de documentos disponível para usuários que não fazem provas](#proof-progress-from-the-document-list-available-to-non-proofing-users)
* [Melhorias na mobilidade](#mobile-improvements)

## Editar campos diretamente da área inicial {#edit-fields-directly-from-the-home-area}

Agora, ao selecionar um objeto na área Página inicial, você pode editar os campos associados a esse objeto diretamente no painel direito da área Página inicial. 

Antes dessa alteração, as informações só podiam ser visualizadas na área da Página inicial, não editadas.

Para obter mais informações, consulte [Atualizar ou editar um item de trabalho na área Página Inicial](../../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md) no artigo  [Atualizar ou editar um item de trabalho na área Página Inicial](../../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).

## Registrar Tempo em Dias {#log-time-in-days}

Agora, os administradores do Workfront podem configurar se os usuários em sua organização registram horas em dias ou horas. Os usuários com uma licença de Planejador podem definir essa configuração para si mesmos.

Antes dessa alteração, os usuários podiam registrar horas somente em horas.

É possível definir essa configuração editando o perfil do usuário. Para obter mais informações, consulte [Configurar se a hora está conectada em horas ou dias](../../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md).

Para obter informações sobre como os usuários podem registrar horas em dias após a atualização dessa configuração, consulte [Registrar tempo](../../../../timesheets/create-and-manage-timesheets/log-time.md).

## Exibir Relações de Predecessoras entre Projetos no Gráfico de Gantt em uma Lista de Projetos {#view-cross-project-predecessor-relationships-on-the-gantt-chart-in-a-list-of-projects}

Agora você pode visualizar as relações de predecessoras entre projetos no gráfico de Gantt nas seguintes listas de projetos:

* A guia Projetos dentro de um portfólio ou programa
* Em um Relatório de Projeto

Antes dessa alteração, você poderia exibir os relacionamentos de predecessores entre projetos somente para tarefas individuais no nível do projeto.

Para obter mais informações, consulte [Configurar como as informações são exibidas no Gráfico de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). 

## Usar o custo orçado no Portfolio Otimizer para calcular as finanças do Portfolio {#use-budgeted-cost-in-the-portfolio-optimizer-to-calculate-portfolio-finances}

O novo Otimizador de Portfolio agora usa o Custo Orçado da nova área de Orçamento de Recursos do Business Case ou do Planejador de Recursos para calcular os seguintes campos:

* Valor líquido
* Retorno sobre o investimento (ROI)
* Custo

Anteriormente, o novo e o Legacy Portfolio Otimizer usavam o Custo orçado herdado. O Otimizador de Portfolio herdado ainda usa o Custo orçado herdado para calcular o Valor líquido, o Retorno sobre o investimento e o Custo.

Também adicionamos dois novos campos aos Campos financeiros Portfolio: ROI herdado e Valor líquido herdado para capturar os novos valores das novas ferramentas de gerenciamento de recursos.

Para obter mais informações, consulte [Visão geral do Portfolio Otimizer](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md) no artigo  [Visão geral do Portfolio Otimizer](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

## Relatório de Utilização: Preenche Horas Orçadas da Nova Área de Orçamento de Recursos {#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area}

>[!NOTE]
>
>Essa funcionalidade não será incluída na versão oficial para o ambiente de Pré-visualização com a versão 2018.2. Ele será reintroduzido durante o período beta da versão 2018.3 e será lançado no ambiente de Produção com a versão 2018.3. 

As horas orçadas no Relatório de utilização agora são preenchidas com base nas informações disponíveis na nova área Orçamento de recursos do Business Case.

Antes dessa alteração, eram usadas informações da área Estimativas de recursos herdada.

Para obter mais informações, consulte [Visão Geral do relatório de Utilização de Recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) no artigo  [Visão Geral do relatório de Utilização de Recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Relatório de Utilização: Exibir Horas Orçadas por Usuário em um Projeto {#utilization-report-view-budgeted-hours-by-user-on-a-project}

>[!NOTE]
>
>Essa funcionalidade não será incluída na versão oficial para o ambiente de Pré-visualização com a versão 2018.2. Ele será reintroduzido durante o período beta da versão 2018.3 e será lançado no ambiente de Produção com a versão 2018.3. 

O relatório de Utilização em um projeto agora exibe Horas orçadas por usuário.

Antes dessa alteração, o relatório de Utilização exibia as Horas Orçadas somente por função de trabalho. 

Para obter mais informações, consulte [Visão Geral do relatório de Utilização de Recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) no artigo [Visão Geral do relatório de Utilização de Recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Progresso da prova na lista de documentos disponível para usuários que não fazem provas {#proof-progress-from-the-document-list-available-to-non-proofing-users}

Indicadores de progresso de prova (Enviado, Aberto, Comentários Feitos e Decisão) agora são exibidos para todos os usuários ao visualizar a lista de documentos. Isso inclui usuários que não podem gerar provas (para obter mais informações sobre como permitir que os usuários gerem provas, consulte a seção .

Antes dessa alteração, os indicadores de progresso de prova estavam disponíveis somente para usuários que podiam gerar provas.

Para obter mais informações, consulte [Visão geral do progresso e do status da prova](../../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md).

## Melhorias na mobilidade {#mobile-improvements}

O aplicativo móvel contém as seguintes melhorias:

* Os links compartilhados com você em outros aplicativos móveis agora são abertos no aplicativo móvel do Workfront.

  Para obter mais informações sobre compartilhamento de links, consulte .

  Essa atualização está disponível no iOS e no Android.

* Atualizamos nossos requisitos de suporte para a plataforma iOS para oferecer suporte ao iPhone X.

  Para obter mais informações sobre dispositivos móveis e sistemas operacionais compatíveis, consulte o . 
