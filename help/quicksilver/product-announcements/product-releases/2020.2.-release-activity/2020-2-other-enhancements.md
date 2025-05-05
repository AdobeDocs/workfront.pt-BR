---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: Outras melhorias do 2020.2
description: Esta página descreve todas as outras melhorias feitas com a versão 2020.2 no ambiente de Produção. Essas melhorias foram disponibilizadas no ambiente de Produção na semana de 11 de maio de 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 46ed705e-b966-4ae9-a602-a5a73a3de3aa
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# Outras melhorias do 2020.2

Esta página descreve todas as outras melhorias feitas com a versão 2020.2 no ambiente de Produção. Essas melhorias foram disponibilizadas no ambiente de Produção na semana de 11 de maio de 2020.

Para obter uma lista de todas as alterações disponíveis com a versão 2020.2, consulte a [visão geral da versão 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## Para administradores do Workfront: modelos de layout mais recentes criados no Workfront Classic agora disponíveis na nova experiência do Workfront

Os modelos de layout criados no Workfront Classic após o último trimestre de 2019 agora estão disponíveis na nova experiência do Workfront. É uma boa ideia atualizar esses Modelos de layout na nova experiência do Workfront para aproveitar as novas funcionalidades e torná-las o mais úteis possível para os usuários nesse ambiente.

Para obter mais informações, consulte [Modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

**Disponível nestes ambientes:**

* A nova experiência do Adobe Workfront

## Os Processos de Aprovação específicos do grupo estão disponíveis para todos os objetos

Para utilizar totalmente os processos de aprovação específicos do grupo, agora é possível adicioná-los a tarefas, problemas e projetos ao editar esses objetos.

Você também pode anexar automaticamente um processo de aprovação específico do grupo a uma tarefa na área Tarefas da caixa Editar projeto, bem como a problemas, ao configurar filas de solicitações ou Tópicos da fila em um projeto.

Para obter informações sobre como adicionar processos de aprovação a projetos, tarefas e problemas, consulte os seguintes artigos:

* [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md)
* [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [Editar problemas](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Criar uma Fila de Solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
* [Criar Tópicos de Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)

## Criar processos de aprovação para grupos que usam status personalizados

Para facilitar o gerenciamento de fluxos de trabalho exclusivos por parte dos grupos, agora é possível usar status personalizados específicos dos grupos nos processos de aprovação.

Anteriormente, um grupo não podia usar seus próprios status personalizados com seus processos de aprovação específicos do grupo. Somente os status de todo o sistema estavam disponíveis e nem sempre se encaixavam nos processos de aprovação de grupo.

Os status personalizados agora podem ser usados em processos de aprovação de uso único e de todo o sistema:

* Crie um processo de aprovação de uso único para um objeto (projeto, tarefa ou problema) e baseie-o nos status associados ao grupo que está trabalhando nesse objeto. Isso inclui todos os status personalizados associados ao grupo.
* Crie um processo de aprovação global e o disponibilize somente para o grupo ou para todos no sistema.

Para usuários com acesso administrativo a processos de aprovação, as informações sobre como configurar processos de aprovação estão disponíveis em [Criar um processo de aprovação para itens de trabalho](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) (ou se você estiver usando o Adobe Workfront Classic, consulte [Criação de Processos de Aprovação](https://experienceleague.adobe.com/pt-br/docs/workfront/using/home)).

Para usuários, as informações sobre como associar processos de aprovação a itens de trabalho estão disponíveis em [Associar um processo de aprovação novo ou existente ao trabalho](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) (ou se você estiver usando o Adobe Workfront Classic, consulte [Associando um Processo de Aprovação Novo ou Existente ao Trabalho](https://experienceleague.adobe.com/pt-br/docs/workfront/using/home)).

**Disponível nestes ambientes:**

* Adobe Workfront Classic
* A nova experiência do Adobe Workfront

## Novas páginas de sobreposição para pesquisa

Para permitir que os usuários naveguem mais facilmente entre as páginas de pesquisa e as páginas anteriores na nova experiência do Workfront, adicionamos uma página de sobreposição de pesquisa que cobre parcialmente a tela.

Agora, ao clicar em Pesquisa avançada no menu Pesquisar ou realizar uma pesquisa básica, uma página é aberta a partir do lado direito da tela.

Para obter mais informações, consulte [Pesquisar Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

**Disponível nestes ambientes:**

* A nova experiência do Adobe Workfront

## Atualizações de Assinaturas de Eventos

Para permitir que os usuários testem, solucionem problemas e resolvam problemas, modificamos o comportamento e adicionamos mais dados à API de assinaturas de evento. Também fizemos as seguintes alterações:

* Tecnologias de mensagens subjacentes migradas
* Recriação do serviço para ter dependências menos complexas e, portanto, dimensionar com mais eficiência
* Aprimoramentos no monitoramento e alertas

Para saber mais, consulte [Perguntas frequentes - Assinaturas de Eventos](../../../wf-api/general/event-subs-faq.md) e [Práticas recomendadas de assinatura de eventos](../../../wf-api/general/event-sub-best-practice.md).
