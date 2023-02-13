---
content-type: o
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Visão geral do botão Trabalhar com isso e Concluir
description: Quando você é atribuído a uma tarefa ou problema, você pode usar um botão contextual que altera nomes e funções dependendo de seu envolvimento com o item de trabalho.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: cfda6702-1a9a-4645-b031-8b2f201ac0af
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 0%

---

# Visão geral do botão Trabalhar com isso e Concluir

Quando você é atribuído a uma tarefa ou problema, você pode usar um botão contextual que altera nomes e funções dependendo de seu envolvimento com o item de trabalho.

Usando o botão contextual para aceitar ou concluir itens de trabalho, você pode permitir que o Adobe Workfront atualize vários campos nos itens sem precisar atualizá-los manualmente.

## Trabalhe com os nomes dos botões Concluir

Dependendo de qual área do Workfront você acessa sua tarefa ou problema, o botão Trabalhar nele ou Concluído pode alterar nomes, conforme descrito nos seguintes cenários: 

* Quando a tarefa ou o problema é atribuído pela primeira vez e o status é New, o botão é exibido como Work on it.

   ![](assets/nwe-work-on-it-button.png)

   >[!TIP]
   >
   >Você pode substituir o botão Trabalhar nele por um botão Iniciar. Para obter informações sobre a substituição do botão Trabalho nele por um botão Iniciar, consulte  [Substitua o botão Trabalho nele por um botão Iniciar](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md) .

* Depois de clicar em Trabalhar nele para aceitar, o botão muda para Marcar como concluído ou Concluído , dependendo de onde no Workfront você acessa a tarefa ou o problema. Para obter informações sobre onde você pode acessar o botão Trabalhar nele, consulte a seção [Localize o botão Trabalho nele e Concluído](#locate-the-work-on-it-and-done-button) neste artigo.

   ![](assets/nwe-mark-as-done-button-350x122.png)

* Se você não for o único atribuído à tarefa ou problema e estiver acessando seu item de trabalho na Lista de trabalho na área Início, o botão será alterado para Concluído com a minha parte.

   ![](assets/home-left-done-with-my-part-button-350x184.png)

## Localize o botão Trabalho nele e Concluído {#locate-the-work-on-it-and-done-button}

Você pode localizar o botão Trabalhar nele e Concluído nas seguintes áreas do Workfront:

* A área Início, tanto na Lista de Trabalho quanto no painel de detalhes

   Para obter informações sobre como marcar um item como Concluído na área inicial, consulte [Marcar um item como Concluído na área inicial](../../workfront-basics/using-home/using-the-home-area/mark-item-done-in-home.md).

* No cabeçalho da tarefa ou do problema

   Para obter informações sobre os cabeçalhos de objetos, consulte [Novos cabeçalhos de objeto](../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

* No painel Resumo de tarefas ou problemas em uma lista ou no Balanceador de Carga de Trabalho

   Para obter informações sobre como usar o painel Resumo, consulte [Visão geral do resumo](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

## Visão geral dos campos que são atualizados automaticamente quando você clica no botão Trabalhar nisso e Concluído

A vantagem de usar os botões Trabalhar com ele e Concluído é que você pode permitir que o Workfront atualize automaticamente as informações sobre o item de trabalho atribuído a você.

* [Botão Trabalhar nele](#work-on-it-button)
* [Botão Iniciar](#start-button)
* [O botão Concluir](#the-done-button)

### Botão Trabalhar nele {#work-on-it-button}

Quando você clica em Trabalhar nele, os seguintes itens também são atualizados:

* Atualizações do Status da Atribuição de Solicitado para Trabalho

   >[!TIP]
   >
   >O campo Status da Atribuição é visível somente em relatórios e listas. Para obter informações sobre o campo Status da Atribuição , consulte o [Glossário da terminologia do Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* Data da confirmação

   Para obter informações sobre a data de confirmação, consulte [Visão geral da data de confirmação](../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

### Botão Iniciar {#start-button}

Se você tiver acesso para editar equipes, poderá substituir o botão Trabalhar nele por um botão Iniciar para uma equipe. Quando os usuários com essa equipe como Equipe inicial clicarem no botão Iniciar nos itens aos quais estão atribuídos, os campos adicionais nos itens de trabalho serão atualizados automaticamente. Para obter informações sobre a substituição do botão Trabalho nele por um botão Iniciar, consulte [Substitua o botão Trabalho nele por um botão Iniciar](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

Além dos campos que são atualizados ao clicar no botão Trabalhar nela, os seguintes campos são atualizados automaticamente em uma tarefa ou problema ao clicar no botão Iniciar:

* Status
* Data de início real

   Para obter informações sobre a Data de Início Real, consulte [Visão geral da data de início real do projeto](../../manage-work/projects/planning-a-project/project-actual-start-date.md).

* Data de conclusão real se o botão Iniciar estiver associado a um status que é igual a Concluído ou Fechado.

   Para obter informações sobre a Data de Conclusão Real, consulte [Visão geral da data de conclusão real do projeto](../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

>[!NOTE]
>
>Clicar no botão Desfazer retorna o item de trabalho ao status original e exclui a Data de início real.
>
>O botão Desfazer não está disponível nas seguintes áreas:
>
>* Solicitações de equipe
>* Cabeçalho da tarefa
>


### O botão Concluir {#the-done-button}

Se você tiver acesso a editar equipes, poderá configurar o botão Concluir para que uma equipe atualize os status da tarefa ou da ocorrência quando marcar um item como concluído. Quando os usuários com essa equipe na Home Team clicam no botão Concluído em seus itens, os seguintes campos são atualizados automaticamente em uma tarefa ou problema:

* Status
* Atualizações do Status da Atribuição de Trabalho para Concluído
* Data de conclusão real

Para obter informações sobre como configurar o botão Concluído para uma equipe, consulte os seguintes artigos:

* [Configurar o botão Concluído para tarefas](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md)
* [Configure o botão Concluído para problemas](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md)
