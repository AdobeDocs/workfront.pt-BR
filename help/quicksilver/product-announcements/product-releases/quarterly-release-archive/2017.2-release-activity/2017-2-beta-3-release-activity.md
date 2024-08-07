---
content-type: release-notes
navigation-topic: product-releases-archive
title: Atividade da versão 2017.2 do Beta 3
description: Esta página descreve todas as alterações disponíveis no ambiente de Pré-visualização com a versão 2017.2 do Beta 2. A funcionalidade nesta página foi disponibilizada no ambiente de Pré-visualização em 24 de maio de 2017. Ele será disponibilizado no ambiente de Produção entre o final de julho e o início de agosto de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9647f3c6-f287-426c-a5e7-eb33b8b22a34
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 0%

---

# Atividade da versão 2017.2 do Beta 3

Esta página descreve todas as alterações disponíveis no ambiente de Pré-visualização com a versão 2017.2 do Beta 2. A funcionalidade nesta página foi disponibilizada no ambiente de Pré-visualização em 24 de maio de 2017. Ele será disponibilizado no ambiente de Produção entre o final de julho e o início de agosto de 2017.

>[!IMPORTANT]
>
>A funcionalidade descrita nesta página está sujeita a alterações antes da disponibilidade no ambiente de produção.

Para obter uma lista de todas as alterações feitas em 2017.2, consulte a [visão geral da atividade da versão 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

A versão 2017.2 do Beta 2 contém melhorias para administradores do Workfront e outros usuários:

**Para Administradores:**

* [Restaurando Itens em Massa da Lixeira](#restoring-items-in-bulk-from-the-recycle-bin)
* [As informações do usuário são sincronizadas do Workfront para o ProofHQ (ProofHQ e Workfront)](#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront)

**Para Todos Os Usuários:** 

* [Exibir Usuários Inscritos](#view-subscribed-users)
* [Configure como os marcos são exibidos no Gráfico de Gantt](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* [Incluir a Legenda do Gráfico de Gantt ao exportar para PDF](#include-the-gantt-chart-legend-when-exporting-to-pdf)
* [Exibir aprovações de provas na área Meu trabalho (Workfront)](#view-proof-approvals-in-the-my-work-area-workfront)
* [Exibir nomes de usuários ao tratar de solicitações de aprovação de revisão da área Meu Trabalho (Workfront)](#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront)
* [Visualizador de provas aprimorado para provas de vídeo (ProofHQ e Workfront)](#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront)
* [Exibir Provas de Mídia Avançada em Resoluções Alternativas (ProofHQ e Workfront)](#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront)
* [Novo objeto &quot;Criador de prova&quot; no Relatório de Versão do Documento (Workfront)](#new-proof-creator-object-in-document-version-report-workfront)
* [Nova funcionalidade de conjunto de recursos removida temporariamente da visualização](#new-resource-pool-functionality-temporarily-removed-from-preview)

## Restaurando itens em massa da Lixeira {#restoring-items-in-bulk-from-the-recycle-bin}

Agora é possível restaurar até 10 projetos, tarefas, problemas ou documentos excluídos de cada vez.

Antes dessa alteração, você poderia restaurar apenas um item excluído de cada vez.

Para obter mais informações sobre como restaurar itens, consulte [Restaurar itens excluídos](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Exibir Usuários Assinados {#view-subscribed-users}

Agora é possível ver quem assina um item ao expandir o número de assinantes que é exibido ao lado do link de assinatura.

Antes desse aprimoramento, você não tinha visibilidade de quem está inscrito em nenhum item.

Para obter mais informações sobre como assinar itens, consulte [Assinar itens no Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md). 

## Configure como os marcos são exibidos no Gráfico de Gantt {#configure-how-milestones-are-displayed-on-the-gantt-chart}

Agora há duas opções para exibir informações de etapas em um gráfico de Gantt. Você pode configurar um ou ambos os indicadores de marcos a seguir:

* Diamantes de Etapas (ícone)

  Este ícone é exibido no Gráfico de Gantt depois de qualquer tarefa associada a um marco.

* Linhas de etapas

  Uma linha é exibida depois de qualquer tarefa associada ao marco, abrangendo todas as tarefas no gráfico de Gantt.

Antes dessa alteração, havia apenas uma opção para permitir que os Marcos fossem exibidos em um gráfico de Gantt, chamada de &quot;Marcos&quot;. Essa opção ativou o ícone de losango do marco e a linha do marco. Esses indicadores não puderam ser separados.

Para obter mais informações sobre como configurar as informações exibidas no gráfico de Gantt, consulte [Configurar como as informações são exibidas no Gráfico de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Incluir a legenda do gráfico de Gantt ao exportar para PDF {#include-the-gantt-chart-legend-when-exporting-to-pdf}

Ao exportar o gráfico de Gantt para um PDF, agora é possível selecionar se também deseja exportar a legenda do gráfico junto com o próprio gráfico. Os itens incluídos na legenda são apenas as opções que você ativou para serem exibidas no Gráfico de Gantt na interface do usuário. Essas opções são incluídas na legenda se existirem nas tarefas do projeto. Por exemplo, se você permitir a exibição de Etapas no gráfico de Gantt, a legenda também os exibirá, mas somente se houver pelo menos uma tarefa associada a uma etapa.

Antes dessa alteração, não era possível excluir a legenda do PDF exportado, e a legenda incluía todas as opções e marcadores possíveis do Gantt, independentemente de estarem ativados ou existentes na interface do usuário.

Para obter mais informações sobre como exportar o Gráfico de Gantt, consulte [Exportar o Gráfico de Gantt para PDF](../../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

## As informações do usuário são sincronizadas do Workfront para o ProofHQ (ProofHQ e Workfront) {#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront}

As informações do usuário (nome e email) agora são sincronizadas do Workfront para o ProofHQ quando os usuários são criados ou atualizados no Workfront. 

Para obter mais informações sobre a sincronização de usuários do Workfront para o ProofHQ, consulte .

## Novo objeto &quot;Criador de prova&quot; no Relatório de versão do documento (Workfront)

{#new-proof-creator-object-in-document-version-report-workfront}

Agora, ao criar um relatório de Versão do documento, há um novo objeto Criador de prova. Esse objeto permite relatar informações sobre o usuário que criou a prova. 

O novo objeto Criador de prova no relatório Versão do documento contém todos os campos disponíveis com o objeto do usuário existente em outros tipos de relatórios de objeto.

>[!NOTE]
>
> Essas informações estão disponíveis no relatório somente a partir do momento em que esse recurso foi introduzido nos respectivos ambientes de Pré-visualização ou Produção; as informações nos relatórios sobre o objeto Solicitante antes do momento em que essa funcionalidade foi introduzida não estão disponíveis.

Você acessa o objeto Criador de provas ao criar um relatório de Versão do documento, conforme descrito em [Criar um relatório personalizado](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para obter mais informações sobre o relatório de objetos Versão do Documento, consulte a seção [Entender objetos no Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) em [Entender objetos no Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Exibir aprovações de provas na área Meu trabalho (Workfront) {#view-proof-approvals-in-the-my-work-area-workfront}

Todas as aprovações de prova que você enviou para aprovação agora são exibidas na área Meu Trabalho, na guia **Trabalho que enviei para aprovação**.

Antes desta alteração, a guia **Trabalho que enviei para aprovação** não incluía aprovações de prova.

Aprovações de provas são exibidas somente quando os seguintes critérios são atendidos:

* A aprovação está pendente de aprovação no momento
* O processo de aprovação é atribuído a um usuário licenciado do Workfront (os processos de aprovação atribuídos a usuários não licenciados do Workfront não são exibidos)
* Os processos de aprovação foram instigados após a liberação dessa funcionalidade (os processos de aprovação instigados antes dessa funcionalidade serem liberados não são exibidos)

Para obter mais informações, consulte [Exibir aprovações](../../../../review-and-approve-work/manage-approvals/view-approvals.md) em [Exibir aprovações](../../../../review-and-approve-work/manage-approvals/view-approvals.md).

## Exibir nomes de usuários ao tratar solicitações de aprovação de provas da área Meu trabalho (Workfront) {#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront}

Agora, ao aprovar aprovações de aprovações na área Meu trabalho, o nome do usuário que solicitou a aprovação agora é exibido.

Para obter mais informações, consulte [Aprovando trabalho](../../../../review-and-approve-work/manage-approvals/approving-work.md) em [Aprovando trabalho](../../../../review-and-approve-work/manage-approvals/approving-work.md). 

## Visualizador de provas aprimorado para provas de vídeo (ProofHQ e Workfront) {#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront}

O revisor de provas no Workfront e no ProofHQ está sendo atualizado com uma nova aparência, arquitetura HTML5 para melhor desempenho e suporte para novas funcionalidades.

O novo visualizador de provas contém as seguintes melhorias:

* Prova quadro a quadro
* Buffering de vídeo
* Funcionalidade de pesquisa na Lista de comentários
* As ações definidas no comentário são exibidas em cada comentário na Lista de comentários
* Modo de tela cheia
* Revisar o conteúdo de forma mais rápida ou mais lenta
* Verificador ortográfico ao adicionar comentários e respostas

### Visualização

O novo visualizador de provas está disponível para teste nos seguintes ambientes de Visualização:

* Ambiente de visualização do ProofHQ

  Para obter mais informações sobre o ambiente de Visualização do ProofHQ, consulte [Visualizar Ambiente de Teste de Sandbox - Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).

* Ambiente de visualização do Workfront, quando sua conta está habilitada com comprovação

  Para obter mais informações sobre o ambiente de Visualização do Workfront, consulte  [O Ambiente De Sandbox De Visualização Do Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

Nesta versão, o novo visualizador de provas suporta apenas provas em vídeo. Isso significa que todas as provas de vídeo usam o novo visualizador de provas, enquanto todas as provas de mídia estática e avançada continuam a usar o visualizador de provas existente.

### Produção

Quando lançado para o ambiente de Produção com a versão 17.2 do, os administradores podem escolher se o visualizador de provas novo ou herdado é adequado para os usuários em sua organização. Por padrão, o visualizador de provas herdadas será usado.

Para obter informações sobre como usar o novo visualizador de prova de vídeo, consulte  

## Exibir provas de mídia avançada em resoluções alternativas (ProofHQ e Workfront) {#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront}

Agora é possível ajustar a resolução das provas de Rich Media especificando uma resolução personalizada ou arrastando a imagem para a resolução desejada.

Antes dessa alteração, você podia revisar as provas usando somente a resolução inerente à tela ou ao dispositivo no qual estava revisando o conteúdo.

Você pode usar o modo Comparar para comparar diferentes resoluções de provas.

Para obter mais informações, consulte [Abrir provas no Desktop Proofing Viewer](../../../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/open-proofs-in-dpv.md). 

## Nova funcionalidade de conjunto de recursos removida temporariamente da visualização {#new-resource-pool-functionality-temporarily-removed-from-preview}

Devido a desafios de desenvolvimento, decidimos remover a nova guia Planejamento de recursos e renomear a guia Planejamento de recursos herdados de volta para o nome original de &quot;Planejamento de recursos&quot;.

A nova funcionalidade Conjuntos de recursos também foi removida com essa alteração. A nova guia Planejamento de recursos e a funcionalidade dos Conjuntos de recursos retornarão ao ambiente de Pré-visualização de sandbox no final de junho de 2017.
