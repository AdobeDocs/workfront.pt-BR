---
content-type: release-notes
navigation-topic: product-releases-archive
title: Atividade da versão 2017.2 do Beta 2
description: Esta página descreve todas as alterações disponíveis no ambiente de Pré-visualização com a versão 2017.2 do Beta 2. A funcionalidade nesta página foi disponibilizada no ambiente de Pré-visualização em 24 de maio de 2017. Ele será disponibilizado no ambiente de Produção entre o final de julho e o início de agosto de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0aa8d61e-cf8c-46a7-b093-a0dbc90d37fd
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---

# Atividade da versão 2017.2 do Beta 2

Esta página descreve todas as alterações disponíveis no ambiente de Pré-visualização com a versão 2017.2 do Beta 2. A funcionalidade nesta página foi disponibilizada no ambiente de Pré-visualização em 24 de maio de 2017. Ele será disponibilizado no ambiente de Produção entre o final de julho e o início de agosto de 2017.

>[!IMPORTANT]
>
>A funcionalidade descrita nesta página está sujeita a alterações antes da disponibilidade no ambiente de produção.

Para obter uma lista de todas as alterações feitas em 2017.2, consulte a [visão geral da atividade da versão 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

A versão 2017.2 do Beta 2 contém melhorias para administradores do Workfront e outros usuários:

**Para Administradores:**

* [Aprimoramento de API: assinaturas de evento](#api-enhancement-event-subscriptions)

**Para Todos Os Usuários:**

* [Assinar Projetos](#subscribe-to-projects)
* [Cancelar Assinatura de Itens de Email](#unsubscribe-from-items-from-email)
* [Configure como os marcos são exibidos no Gráfico de Gantt](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* [Modelos de Conjuntos de Recursos](#resource-pools-templates)
* [Exibir Versões de Documentos Comprovados no Workfront](#view-versions-of-proofed-documents-within-workfront)
* [Novo objeto solicitante no relatório de aprovação de prova](#new-requester-object-in-proof-approval-report)

## Aprimoramento de API: assinaturas de evento {#api-enhancement-event-subscriptions}

Quando ocorre uma ação em um objeto do Workfront que é compatível com assinaturas de evento, agora é possível configurar o Workfront para enviar uma resposta para o endpoint desejado. Ou seja, suas integrações podem interagir com a API do Workfront em tempo real.

Para obter mais informações, consulte [API de Assinatura de Evento](../../../../wf-api/general/event-subs-api.md). 

## Inscrever-se em projetos {#subscribe-to-projects}

Agora é possível assinar novos comentários em projetos para os quais você não faz parte da equipe do projeto. Antes desta versão, você só podia assinar comentários sobre problemas e tarefas.

Para obter mais informações sobre como assinar itens, consulte [Assinar itens no Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Cancelar inscrição nos itens do email {#unsubscribe-from-items-from-email}

Você pode cancelar a inscrição de itens usando o link &quot;Cancelar inscrição&quot; no email de inscrição. Anteriormente, só era possível cancelar a assinatura de um item na interface do Workfront.

Para obter mais informações sobre o cancelamento de inscrição nos emails de inscrição, consulte a seção &quot;Recusa de notificação por email&quot; em [Notificações do Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md) 

## Configure como os marcos são exibidos no Gráfico de Gantt {#configure-how-milestones-are-displayed-on-the-gantt-chart}

***CORREÇÃO &#x200B;**: este recurso não está atualmente no ambiente de Pré-visualização de Sandbox. Seu lançamento está planejado para uma data posterior, durante o mês de junho de 2017.*

Agora há duas opções para exibir informações de etapas em um gráfico de Gantt. Você pode configurar um ou ambos os indicadores de marcos a seguir:

* Diamantes de Etapas (ícone)

  Este ícone é exibido no Gráfico de Gantt depois de qualquer tarefa associada a um marco.

* Linhas de etapas

  Uma linha é exibida depois de qualquer tarefa associada ao marco, em todas as tarefas no gráfico de Gantt.

Antes dessa alteração, havia apenas uma opção para permitir que os Marcos fossem exibidos em um gráfico de Gantt, chamada de &quot;Marcos&quot;. Essa opção ativou o ícone de losango do marco e a linha do marco. Esses indicadores não puderam ser separados. As duas opções agora estão disponíveis em todos os gráficos de Gantt, incluindo todas as listas de projetos e relatórios. 

Para obter mais informações sobre como configurar as informações exibidas no gráfico de Gantt, consulte [Configurar como as informações são exibidas no Gráfico de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Modelos de Conjuntos de Recursos {#resource-pools-templates}

Agora você pode especificar Conjuntos de recursos para modelos. Antes desta versão, você poderia associar Conjuntos de recursos somente a usuários e projetos.

Para obter mais informações sobre Conjuntos de Recursos, consulte [Visão geral sobre conjuntos de recursos](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

## Exibir versões de documentos revisados no Workfront {#view-versions-of-proofed-documents-within-workfront}

Agora você pode exibir provas de todas as versões de um documento revisado na interface do Workfront. 

Antes dessa alteração, você podia exibir somente a versão mais recente do documento comprovado.

Os usuários sem uma licença de prova podem:

* Abrir uma prova em uma versão anterior de um documento comprovado

Os usuários com uma licença de prova podem executar um dos seguintes procedimentos:

* Abrir uma prova em uma versão anterior de um documento comprovado
* Exibir os detalhes da prova em uma versão anterior de um documento comprovado

Para obter mais informações, consulte [Gerenciar versões de documentos](../../../../documents/managing-documents/manage-document-versions.md) em [Gerenciar versões de documentos](../../../../documents/managing-documents/manage-document-versions.md).

## Novo objeto solicitante no relatório de aprovação de prova {#new-requester-object-in-proof-approval-report}

Agora, ao criar um relatório Aprovação de prova, há um novo objeto Solicitante. Esse objeto permite relatar informações sobre o usuário que solicitou a aprovação da prova. 

O novo objeto Solicitante no relatório Aprovação de prova contém todos os campos disponíveis com o objeto Usuário existente em outros tipos de relatórios de objeto.

>[!NOTE]
>
> Essas informações estão disponíveis no relatório somente a partir do momento em que esse recurso foi introduzido nos respectivos ambientes de Pré-visualização ou Produção; as informações nos relatórios sobre o objeto Solicitante antes do momento em que essa funcionalidade foi introduzida não estão disponíveis.

Você acessa o objeto Solicitante ao criar um relatório Aprovação de prova, conforme descrito em [Criar um relatório personalizado](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para obter mais informações sobre o relatório do objeto Aprovações de Provas, consulte a seção [Entender os objetos no Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) em [Entender os objetos no Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).
