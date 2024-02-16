---
content-type: release-notes
navigation-topic: product-releases-archive
title: Atividade de versão final Beta 2018.1
description: Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão Beta Final 2018.1. A funcionalidade foi disponibilizada no ambiente de Pré-visualização em 31 de janeiro de 2018. Ele estará disponível no ambiente de Produção em março de 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 35bd3604-5452-4b46-afb1-78bc2fbb48ec
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---

# Atividade de versão final Beta 2018.1

Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão Beta Final 2018.1. A funcionalidade foi disponibilizada no ambiente de Pré-visualização em 31 de janeiro de 2018. Ele estará disponível no ambiente de Produção em março de 2018.

>[!IMPORTANT]
>
> A funcionalidade descrita nesta página está sujeita a alterações antes da disponibilidade no ambiente de produção.

Para obter uma lista de todas as alterações feitas em 2018.1, consulte  [Visão geral da atividade da versão 2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

A versão final Beta 2018.1 contém melhorias para administradores do Workfront e outros usuários:

**Para administradores**

* [Configurar Disponibilidade de Recursos e Alocações de Usuários para Calcular com Base no Cronograma do Usuário](#configure-resource-availability-and-user-allocations-to-calculate-based-on-the-user-schedule)

**Para todos os usuários**

* [Aprimoramentos para dispositivos móveis](#mobile-enhancements)
* [Integração com Jira](#jira-integration)
* [Atualização de nomes do visualizador de provas](#update-to-proofing-viewer-names)
* [Alteração na cadência de sincronização ao sincronizar do ambiente de produção de provas para visualização](#change-to-synchronization-cadence-when-synchronizing-from-the-proofing-production-environment-to-preview)
* [A mensagem de aviso é exibida quando o limite de 2.000 itens é atingido no Planejador de recursos](#warning-message-displays-when-the-2-000-item-limit-is-reached-in-the-resource-planner)

## Aprimoramentos para dispositivos móveis {#mobile-enhancements}

A seguinte funcionalidade chegará às lojas de aplicativos móveis no início de março de 2018:

* Nova navegação: a página inicial dos nossos Aplicativos para dispositivos móveis foi reprojetada.
* Página inicial no Mobile: nossa nova funcionalidade Página inicial também foi atualizada em nossos aplicativos móveis.

A nova funcionalidade é compatível com as plataformas iOS e Android.

## Integração com Jira {#jira-integration}

Agora é possível vincular problemas do Jira a tarefas ou problemas do Workfront instalando e configurando o complemento Workfront para Jira. Com essa integração, os gerentes de projeto podem continuar trabalhando no Workfront, enquanto os engenheiros de desenvolvimento podem continuar trabalhando no Jira, enquanto seus itens individuais são vinculados por meio da integração do Workfront com o Jira.

Você pode configurar as seguintes opções por meio dessa integração:

* Estabeleça acionadores para as atribuições do Workfront para criar automaticamente problemas no Jira quando ocorrerem.
* Vincule manualmente problemas do Jira a tarefas do Workfront ou problemas que foram criados anteriormente.
* Especifique os campos que devem ser sincronizados nos itens vinculados assim que um dos itens for atualizado em um dos aplicativos.

O complemento Workfront estará disponível para as versões No local e Sob demanda do Jira. O complemento é gratuito e estará disponível para download no Atlassian Marketplace no início de março de 2018.

Para obter mais informações sobre o complemento Workfront para Jira, incluindo um link para baixá-lo, consulte [Uso do Workfront com Jira.](https://support.workfront.com/hc/en-us/sections/115001130053)

## Atualização de nomes do visualizador de provas {#update-to-proofing-viewer-names}

Os nomes do visualizador de provas baseado em HTML5 e dos visualizadores de provas baseados em Flash foram renomeados em todo o sistema Workfront. Os nomes anteriores e atualizados são os seguintes: 

| **Nome anterior** | **Nome atualizado** |
|---|---|
| Visualizador de provas HTML5 | Novo visualizador de provas |
| Visualizador da prova de Flashes | Visualizador de provas herdadas |

{style="table-layout:auto"}

 Para obter mais informações sobre o uso do novo visualizador de provas, consulte [Revisar provas no visualizador de provas.](https://support.workfront.com/hc/en-us/sections/115000275214)

## Configurar Disponibilidade de Recursos e Alocações de Usuários para Calcular com Base no Cronograma do Usuário {#configure-resource-availability-and-user-allocations-to-calculate-based-on-the-user-schedule}

>[!NOTE]
>
>As ferramentas de Agendamento de recursos foram substituídas e removidas do Workfront com a versão 23.1. Para obter informações sobre como programar recursos usando o Balanceador de carga de trabalho, consulte [Visão geral do Balanceador de carga de trabalho](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

O administrador do Workfront agora pode determinar como o Workfront calcula a disponibilidade de recursos e a alocação de usuários no nível do sistema (considerando horas e a disponibilidade de FTE). O administrador do Workfront pode configurar a disponibilidade de recursos e a alocação de usuários a serem calculadas usando o agendamento padrão ou o agendamento do usuário.

Essa configuração afeta a disponibilidade do usuário nas seguintes circunstâncias ao agendar recursos:

* Ao permitir que o Workfront atribua recursos automaticamente, conforme descrito em &quot;Atribuir manualmente tarefas e problemas não atribuídos nas áreas de Programação&quot;.

* Ao exibir indicadores de alocação, conforme descrito em &quot;Gerenciar alocações de usuários nas áreas de Agendamento&quot;.

Para obter mais informações, consulte &quot;Configurar como o Workfront calcula a hora e a disponibilidade de FTE do recurso para a área de Agendamento&quot;.

>[!NOTE]
>
>As ferramentas de Agendamento de recursos foram substituídas e removidas do Workfront com a versão 23.1. Para obter informações sobre como programar recursos usando o Balanceador de carga de trabalho, consulte [Visão geral do Balanceador de carga de trabalho](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).


## Alteração na cadência de sincronização ao sincronizar do ambiente de produção de provas para visualização {#change-to-synchronization-cadence-when-synchronizing-from-the-proofing-production-environment-to-preview}

>[!NOTE]
>
>Essa alteração entrará em vigor em 11 de fevereiro de 2018.

Os dados do ambiente de produção de prova do Workfront agora são sincronizados ao ambiente de Pré-visualização de prova do Workfront todas as semanas.

Antes dessa alteração, os dados eram sincronizados do ambiente de produção de prova do Workfront para o ambiente de Pré-visualização mensalmente, enquanto os dados do ambiente de produção do Workfront eram sincronizados com o ambiente de Pré-visualização do Workfront semanalmente. Essa discrepância causou alguns erros de sincronização ao usar a funcionalidade de Prova no ambiente de Pré-visualização do Workfront. 

Para obter mais informações, consulte [Visualizar ambiente de teste de sandbox - Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md). 

## A mensagem de aviso é exibida quando o limite de 2.000 itens é atingido no Planejador de recursos {#warning-message-displays-when-the-2-000-item-limit-is-reached-in-the-resource-planner}

Como estamos trabalhando atualmente em uma solução mais permanente para melhorar o desempenho no Planejador de recursos, introduzimos um limite de 2.000 itens para cada exibição que você pode aplicar ao Planejador de recursos:

* A Exibição de usuário exibe apenas 2.000 atribuições
* A Visualização de projetos exibe apenas 2.000 projetos
* A Exibição de funções exibe somente 2.000 funções

Quando o Planejador de recursos tenta carregar mais de 2.000 itens, uma notificação é exibida alertando que somente 2.000 itens podem ser exibidos.

Para obter mais informações sobre esses limites e como eles afetam o Planejador de recursos, consulte [Limitações de exibição do Planejador de recursos](../../../../resource-mgmt/resource-planning/resource-planner-display-limitations.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our beta program for the Resource Planner performance, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref">Resource Planner performance beta </a>.</p>
-->
