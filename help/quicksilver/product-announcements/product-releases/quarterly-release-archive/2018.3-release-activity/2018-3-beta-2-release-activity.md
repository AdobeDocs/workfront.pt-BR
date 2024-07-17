---
content-type: release-notes
navigation-topic: product-releases-archive
title: Atividade da versão 2018.3 do Beta 2
description: Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão 2018.3 do Beta 2. A funcionalidade estará disponível no ambiente de Pré-visualização em 1 de agosto de 2018. Os aprimoramentos de revisão lançados com o Beta 2 estarão disponíveis no ambiente de Pré-visualização na quarta-feira, 18 de julho. Ele estará disponível no ambiente de Produção em novembro de 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 97945661-e97d-43c8-b564-624c4388de2f
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# Atividade da versão 2018.3 do Beta 2

Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão 2018.3 do Beta 2. A funcionalidade estará disponível no ambiente de Pré-visualização em 1 de agosto de 2018. Os aprimoramentos de revisão lançados com o Beta 2 estarão disponíveis no ambiente de Pré-visualização na quarta-feira, 18 de julho. Ele estará disponível no ambiente de Produção em novembro de 2018.

>[!NOTE]
>
> A funcionalidade descrita nesta página está sujeita a alterações antes da disponibilidade no ambiente de produção.

Para obter uma lista de todas as alterações feitas em 2018.3, consulte  Visão geral da atividade da versão [2018.3](../../../../product-announcements/product-releases/quarterly-release-archive/2018.3-release-activity/2018-3-release-activity-overview.md).

A versão 2018.3 do Beta 2 contém melhorias para administradores do Workfront e outros usuários:

**Para Administradores**

* [Atualize o endereço de email no Perfil de usuário como um administrador de grupo](#update-the-email-address-in-the-user-profile-as-a-group-administrator)

**Para Todos Os Usuários**

* [Exibir aprovações delegadas a mim na área da página inicial](#view-approvals-delegated-to-me-in-the-home-area)
* [Exportar dados para um determinado período no Planejador de recursos](#export-data-for-a-given-period-in-the-resource-planner)
* [Os totais diários agora são exibidos em vermelho quando o usuário está superalocado](#daily-totals-now-display-in-red-when-the-user-is-overallocated)
* [Tarefas e problemas estão ocultos na linha de tempo do agendamento quando minimizados](#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized)
* [Filtrar Comentários e Respostas por Usuário no visualizador de provas](#filter-comments-and-replies-by-user-in-the-proofing-viewer)
* [Comentar em um intervalo de imagens em uma prova de vídeo](#comment-on-a-range-of-footage-in-a-video-proof)
* [Nova Ferramenta de Polilinha para Marcação de Comentários no visualizador de provas](#new-polyline-tool-for-comment-markup-in-the-proofing-viewer)
* [Remoção de Flashes para relatórios, calendários e compartilhamento de documentos](#flash-removal-for-report-calendar-and-document-sharing)

## Atualize o endereço de email no Perfil de usuário como um administrador de grupo {#update-the-email-address-in-the-user-profile-as-a-group-administrator}

Agora você pode atualizar endereços de email de usuários que pertencem a um grupo que você administra. 

Anteriormente, somente os administradores do Workfront podiam atualizar endereços de email de outros usuários. 

Para obter mais informações, consulte [Administradores de grupo](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

## Exibir aprovações delegadas a mim na área da página inicial {#view-approvals-delegated-to-me-in-the-home-area}

Agora você pode usar a área da página inicial para exibir aprovações de projetos, tarefas e problemas que foram delegados a você.

Antes dessa alteração, você poderia visualizar aprovações delegadas somente na área Meu trabalho.

Para obter mais informações, consulte [Delegar solicitação de aprovação](../../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

## Exportar dados para um determinado período no Planejador de recursos {#export-data-for-a-given-period-in-the-resource-planner}

Uma nova janela agora é exibida ao exportar as informações no Planejador de recursos que permite selecionar um período específico para seu arquivo exportado.

Antes dessa melhoria, você poderia exportar apenas as informações exibidas na tela.

Para obter mais informações sobre como exportar dados do Planejador de recursos, consulte [Visão geral da navegação do Planejador de recursos](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md) no artigo [Visão geral da navegação do Planejador de recursos](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Os totais diários agora são exibidos em vermelho quando o usuário está superalocado {#daily-totals-now-display-in-red-when-the-user-is-overallocated}

>[!NOTE]
>
>As ferramentas de Agendamento de recursos foram substituídas e removidas do Workfront com a versão 23.1. Para obter informações sobre o agendamento de recursos usando o Balanceador de carga de trabalho, consulte [Visão geral do Balanceador de carga de trabalho](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Quando um usuário está superalocado, os totais diários dos dias em que o usuário está superalocado agora são exibidos em vermelho. Esta opção é exibida somente quando a opção Mostrar os totais das horas planejadas diárias está habilitada nas configurações de cronograma do cronograma. Antes desse aprimoramento, havia um indicador de barra vermelha para os dias em que o usuário estava superalocado, mas os totais diários eram exibidos sem um destaque vermelho.

Para obter mais informações sobre alocações de usuários, consulte &quot;Gerenciar alocações de usuários nas áreas de Agendamento&quot;.

## Tarefas e problemas são ocultados na linha de tempo do agendamento quando minimizados {#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized}

Ao minimizar tarefas e problemas na linha do tempo do agendamento, eles agora ficam ocultos para usuários e funções se a opção Mostrar totais de horas planejadas diárias estiver habilitada nas configurações. Tarefas e problemas na área Não atribuído são exibidos em uma exibição compactada.

Anteriormente, ao minimizar tarefas e problemas, as tarefas e problemas permaneceriam na linha do tempo de agendamento para usuários e funções, mas seriam exibidos em uma exibição compactada.

Para obter mais informações sobre como minimizar tarefas e problemas na linha do tempo do agendamento, consulte  &quot;Introdução ao Agendamento de recursos&quot;.

## Filtrar comentários e respostas por usuário no visualizador de provas {#filter-comments-and-replies-by-user-in-the-proofing-viewer}

Agora é possível incluir respostas ao filtrar comentários feitos por usuários especificados. Isso é útil quando você deseja se concentrar em todos os comentários feitos por um revisor importante, como um cliente ou gerente de projeto.

Anteriormente, a filtragem por usuário estava limitada apenas aos comentários criados (iniciados) pelos revisores especificados.

## Comentar em uma variedade de imagens em uma prova de vídeo {#comment-on-a-range-of-footage-in-a-video-proof}

É possível criar um comentário para uma variedade de sequências filmadas em uma prova de vídeo. Isso é útil, por exemplo, quando é necessário indicar que um segmento de filmagem precisa ser refeito ou removido.

Anteriormente, só era possível criar um comentário para um único ponto em uma linha do tempo do vídeo.

## Nova ferramenta de polilinha para marcação de comentários no visualizador de provas {#new-polyline-tool-for-comment-markup-in-the-proofing-viewer}

Agora é possível usar a marcação de polilinha para desenhar linhas e formas segmentadas ao adicionar um comentário a uma prova. Você pode criar uma linha segmentada aberta ou uma forma fechada. Essa ferramenta é especialmente útil ao trabalhar com imagens complexas, como imagens técnicas ou arquitetônicas.

Anteriormente, ao marcar uma prova para adicionar um comentário, você podia desenhar um retângulo, uma linha reta, uma linha ou forma à mão livre ou uma seta.

## Remoção de Flashes para relatórios, calendários e compartilhamento de documentos {#flash-removal-for-report-calendar-and-document-sharing}

Removemos o Flash das seguintes caixas de diálogo de Compartilhamento no Workfront:

* Relatórios
* Calendários
* Documentos

Você ainda pode compartilhar esses objetos como fazia anteriormente, mas agora a experiência não depende mais do Flash.
