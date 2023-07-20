---
content-type: o
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Visão geral do botão Trabalhar na tarefa e Concluído
description: Quando estiver atribuído a uma tarefa ou problema, você poderá usar um botão contextual que altera nomes e funções dependendo de seu envolvimento com o item de trabalho.
author: Lisa and Alina
feature: Get Started with Workfront
role: User
exl-id: cfda6702-1a9a-4645-b031-8b2f201ac0af
source-git-commit: a634e29df16d401812fb87ea53521d5028f7fd20
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 0%

---

# Visão geral do botão Trabalhar na tarefa e Concluído

Quando estiver atribuído a uma tarefa ou problema, você poderá usar um botão contextual que altera nomes e funções dependendo de seu envolvimento com o item de trabalho.

Usando o botão contextual para aceitar ou concluir itens de trabalho, você pode permitir que o Adobe Workfront atualize vários campos nos itens sem precisar atualizá-los manualmente.

## Trabalhar nisso e nomes de botão Concluído

Dependendo da área do Workfront na qual você acessa sua tarefa ou problema, o botão Trabalhar na tarefa ou Concluído pode alterar os nomes, conforme descrito nos seguintes cenários: 

* Quando a tarefa ou problema for atribuído a você pela primeira vez e o status for Novo, o botão será exibido como Trabalhar nela.

  ![](assets/nwe-work-on-it-button.png)

  >[!TIP]
  >
  >Você pode substituir o botão Trabalhar nisso por um botão Iniciar. Para obter informações sobre como substituir o botão Trabalhar na tarefa por um botão Iniciar, consulte  [Substitua o botão Trabalhar na tarefa por um botão Iniciar](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md) .

* Depois de clicar em Trabalhar nisto, você aceita, o botão muda para Marcar como concluído ou Concluído , dependendo de onde você acessa a tarefa ou o problema no Workfront. Para obter informações sobre onde você pode acessar o botão Trabalhar na tarefa, consulte a seção [Localize o botão Trabalhar na tarefa e concluído](#locate-the-work-on-it-and-done-button) neste artigo.

  ![](assets/nwe-mark-as-done-button-350x122.png)

* Se você não for o único atribuído à tarefa ou problema e estiver acessando seu item de trabalho a partir da Lista de trabalho na área Página inicial, o botão muda para Concluído com minha parte.

  ![](assets/home-left-done-with-my-part-button-350x184.png)

## Localize o botão Trabalhar na tarefa e concluído {#locate-the-work-on-it-and-done-button}

É possível localizar o botão Trabalhar nisso e Concluído nas seguintes áreas do Workfront:

* A área Início, tanto na Lista de trabalho quanto no painel de detalhes

  Para obter informações sobre como marcar um item como Concluído na área Página inicial, consulte [Marcar um item como Concluído na área Página inicial](../../workfront-basics/using-home/using-the-home-area/mark-item-done-in-home.md).

* No cabeçalho da tarefa ou problema

  Para obter informações sobre os cabeçalhos de objetos, consulte [Novos cabeçalhos de objeto](../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

* No painel Resumo de tarefas ou problemas em uma lista ou no Balanceador de carga de trabalho

  Para obter informações sobre como usar o painel Resumo, consulte [Visão geral do resumo](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

## Visão geral dos campos que são atualizados automaticamente ao clicar no botão Trabalhar nisto e Concluído

A vantagem de usar os botões Trabalhar nisso e Concluído é que você pode permitir que o Workfront atualize automaticamente as informações sobre o item de trabalho atribuído a você.

* [Botão Trabalhar na tarefa](#work-on-it-button)
* [Botão Iniciar](#start-button)
* [O botão Concluído](#the-done-button)

### Botão Trabalhar na tarefa {#work-on-it-button}

Ao clicar em Trabalhar nisso, os seguintes itens também são atualizados:

* Atualizações do Status da Atribuição de Solicitado para Em Execução

  >[!TIP]
  >
  >O campo Status da Atribuição é visível somente em relatórios e listas. Para obter informações sobre o campo Status da Atribuição, consulte [Glossário da terminologia do Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* Data de confirmação

  Para obter informações sobre a data de confirmação, consulte [Visão geral da data de compromisso](../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

### Botão Iniciar {#start-button}

Se você tiver acesso para editar equipes, poderá substituir o botão Trabalhar na equipe por um botão Iniciar para uma equipe. Quando usuários com essa equipe como sua Equipe inicial clicam no botão Iniciar em itens aos quais estão atribuídos, campos adicionais em seus itens de trabalho são atualizados automaticamente. Para obter informações sobre como substituir o botão Trabalhar na tarefa por um botão Iniciar, consulte [Substitua o botão Trabalhar na tarefa por um botão Iniciar](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

Além dos campos que são atualizados quando você clica no botão Trabalhar na tarefa, os seguintes campos são atualizados automaticamente em uma tarefa ou problema quando você clica no botão Iniciar:

* Status
* Data do Início Efetivo

  Para obter informações sobre a Data Inicial Real, consulte [Visão Geral da Data de Início Efetivo do projeto](../../manage-work/projects/planning-a-project/project-actual-start-date.md).

* Data de Término Real se o botão Iniciar estiver associado a um status que equivale a Concluído ou Fechado.

  Para obter informações sobre a Data de Término Efetivo, consulte [Visão geral da Data de Término Efetivo do projeto](../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

>[!NOTE]
>
>Clicar no botão Desfazer retorna o item de trabalho ao status original e exclui a Data Inicial Real.
>
>O botão Desfazer não está disponível nas seguintes áreas:
>
>* Solicitações de equipe
>* Cabeçalho da tarefa
>

### O botão Concluído {#the-done-button}

Se você tiver acesso para editar equipes, poderá configurar o botão Concluído para que uma equipe atualize os status de tarefas ou problemas quando marcar um item como concluído. Quando os usuários com essa equipe como sua Equipe inicial clicarem no botão Concluído em seus itens, os seguintes campos serão atualizados automaticamente em uma tarefa ou problema:

* Status
* Atualizações de Status de Atribuição de Em Execução para Concluído
* Data de término efetivo

Para obter informações sobre como configurar o botão Concluído para uma equipe, consulte os seguintes artigos:

* [Configurar o botão Concluído para tarefas](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md)
* [Configurar o botão Concluído para problemas](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md)
