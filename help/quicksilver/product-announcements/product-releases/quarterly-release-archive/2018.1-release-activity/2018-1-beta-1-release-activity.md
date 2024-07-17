---
content-type: release-notes
navigation-topic: product-releases-archive
title: Atividade da versão 2018.1 do Beta 1
description: Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão 2018.1 do Beta 1. A funcionalidade nesta página foi disponibilizada no ambiente de Pré-visualização em 1 de dezembro de 2017. Ele estará disponível no ambiente de Produção em março de 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: efcc2217-ab69-4ac4-8e9a-f811eba77d49
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1065'
ht-degree: 0%

---

# Atividade da versão 2018.1 do Beta 1

Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão 2018.1 do Beta 1. A funcionalidade nesta página foi disponibilizada no ambiente de Pré-visualização em 1 de dezembro de 2017. Ele estará disponível no ambiente de Produção em março de 2018.

>[!IMPORTANT]
>
> A funcionalidade descrita nesta página está sujeita a alterações antes da disponibilidade no ambiente de produção.

Para obter uma lista de todas as alterações feitas em 2018.1, consulte  Visão geral da atividade da versão [2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

A versão 2018.1 do Beta 1 contém melhorias para administradores do Workfront e outros usuários:

**Para Administradores**

* [Modelo de layout atualizado para oferecer suporte à Área Inicial](#updated-layout-template-to-support-the-home-area)
* [Desabilitar Notificações por Email de Revisão Enviadas pelo Workfront](#disable-proofing-email-notifications-sent-from-workfront)
* [Novos recursos adicionados às assinaturas de evento](#new-resources-added-to-event-subscriptions)

**Para Todos Os Usuários**

* [Área Residencial (Atualizou Minha Área de Trabalho)](#home-area-updated-my-work-area)
* [Exibir Dados do Planejador de Recursos no Business Case e Resumo Atualizado do Business Case](#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary)
* [Exibir a Porcentagem de Alocação de Horas Planejadas no Planejador de Recursos](#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner)
* [Os Tipos de Atualização &quot;Automático e Mediante Alteração&quot; e &quot;Somente Alteração&quot; Atualizam os Objetos Pai ao Mesmo Tempo que as Tarefas São Atualizadas](#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated)
* [Instantâneo da Linha do Tempo Disponível no Gráfico de Gantt](#timeline-snapshot-available-in-the-gantt-chart)

## Área da Página Inicial (Minha Área de Trabalho Atualizada) {#home-area-updated-my-work-area}

A nova área da página inicial oferece uma visualização alternativa e aprimorada dos mesmos dados que estão disponíveis na área Meu trabalho. A área Página inicial oferece os seguintes benefícios na área Meu trabalho:

* Uma interface mais simples e intuitiva
* Desempenho aprimorado
* Atualizar tarefas e problemas com formatação de rich text

## Modelo de layout atualizado para oferecer suporte à área inicial {#updated-layout-template-to-support-the-home-area}

Como administrador do Workfront, você pode determinar se os usuários da sua organização têm acesso à área Página inicial configurando o modelo de layout ao qual estão atribuídos. Os usuários aos quais não é atribuído um modelo de layout podem sempre acessar a área Início.

Para obter mais informações, consulte &quot;Criar e gerenciar modelos de layout&quot;.

## Desative as notificações por email de revisão enviadas pelo Workfront {#disable-proofing-email-notifications-sent-from-workfront}

Agora você pode configurar se os usuários na sua instância do Workfront receberão notificações por email do Workfront quando um comentário for feito em uma prova.

Anteriormente, os emails de prova eram sempre enviados do Workfront quando um comentário era feito em uma prova. Se as notificações também estivessem habilitadas no Workfront Proof, os usuários recebiam notificações duplicadas. 

Para clientes existentes do Workfront, o Workfront é configurado por padrão para enviar emails quando é feito um comentário em uma prova.

Para obter informações sobre como desativar as notificações por email para provas no Workfront para que os emails de prova sejam enviados somente do Workfront Proof, consulte .  

## Exibir Dados do Planejador de Recursos no Business Case e Resumo de Business Case Atualizado {#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary}

A área Orçamento de recursos agora está disponível no Business Case de um projeto. Nesta área, você pode revisar as Horas orçadas estimadas para seus recursos no Planejador de recursos e o Custo de mão de obra orçado associado a eles.

A área Estimativas de recursos do Business Case foi renomeada para Estimativas de recursos legados.

Como parte dessa alteração, o Resumo de business case agora inclui informações financeiras com base nas Estimativas de recursos e no Orçamento de recursos.

Antes desta alteração, você não podia ver as informações do Planejador de recursos no Business Case do projeto. Você só pode ver informações de Estimativas de Recursos especificadas no Planejador de Capacidade dos Conjuntos de Recursos Legados.

Para obter mais informações sobre como criar um Business Case, consulte [Criar um Business Case para um projeto](../../../../manage-work/projects/define-a-business-case/create-business-case.md).

## Exibir a Porcentagem de Alocação de Horas Planejadas no Planejador de Recursos {#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner}

A Visualização de usuário do Planejador de recursos agora inclui uma nova coluna que permite visualizar a Alocação de horas planejadas como uma porcentagem do total de Horas disponíveis para o usuário e a função de trabalho.

Antes dessa alteração, você poderia visualizar o total de Horas planejadas e disponíveis para usuários e funções de trabalho somente em colunas separadas.

Para obter mais informações sobre a coluna Porcentagem de Alocação de Horas Planejadas, consulte a seção &quot;Exibindo a Diferença entre Horas Disponíveis e Planejadas ou FTE no Planejador de Recursos&quot; na [Visão geral do Planejador de Recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Os tipos de atualização &quot;Automático e Mediante alteração&quot; e &quot;Somente alteração&quot; acionam as atualizações dos objetos principais ao mesmo tempo que as tarefas são atualizadas {#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated}

Alteramos a forma como as tarefas principais e o projeto são atualizados quando um objeto de nível inferior é atualizado em um projeto. O horário em que um objeto pai é atualizado é determinado pelo campo Tipo de atualização em um projeto. Você pode selecionar dentre os seguintes Tipos de Atualização:

* Automático e Mediante alteração
* Somente mediante alteração
* Somente automática
* Somente manual

Agora, quando você seleciona os Tipos de Atualização &quot;Automático e Ao Alterar&quot; ou &quot;Somente Alterar&quot;, as alterações aplicadas às tarefas individuais também são aplicadas à tarefa pai e ao projeto imediatamente.

Antes dessa alteração, você tinha que atualizar a página para garantir que os objetos principais e a linha do tempo do projeto também fossem atualizados.

Para obter mais informações sobre o Tipo de Atualização de um projeto, consulte [Selecionar o Tipo de Atualização do projeto](../../../../manage-work/projects/manage-projects/select-project-update-type.md).

## Instantâneo da Linha do Tempo Disponível no Gráfico de Gantt {#timeline-snapshot-available-in-the-gantt-chart}

Agora é possível rolar rapidamente para um determinado ponto na vida útil de um projeto usando o novo instantâneo da linha do tempo no gráfico de Gantt.

Quando você seleciona um intervalo de tempo mais granular para o gráfico de Gantt enquanto visualiza uma lista de tarefas ou de projetos, uma barra de rolagem horizontal é mostrada na parte inferior do gráfico de Gantt. Clicar na barra de rolagem permite ver toda a linha do tempo do projeto em um instantâneo. Você pode clicar em qualquer lugar dentro do instantâneo do Gráfico de Gantt para navegar para um ponto específico na vida útil do projeto.

Antes dessa alteração, você tinha que rolar horizontalmente no gráfico de Gantt inteiro para encontrar um determinado momento no tempo, ou você tinha que afastar o zoom da exibição granular.

Para obter mais informações sobre como as informações são exibidas no Gráfico de Gantt, consulte [Configurar como as informações são exibidas no Gráfico de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Novos recursos adicionados às assinaturas de evento {#new-resources-added-to-event-subscriptions}

Agora é possível criar assinaturas de evento para os seguintes recursos:

* **Despesa:** Notifica quando uma despesa é adicionada ou modificada.
* **Atribuição:** notifica você quando uma atribuição é adicionada ou modificada em uma tarefa ou problema para um usuário, função de trabalho ou equipe.
* **Planilha de horas:** notifica você quando uma planilha de horas é enviada, rejeitada ou aprovada.

Para saber mais sobre assinaturas de evento, consulte [API de Assinatura de Evento](../../../../wf-api/general/event-subs-api.md).
