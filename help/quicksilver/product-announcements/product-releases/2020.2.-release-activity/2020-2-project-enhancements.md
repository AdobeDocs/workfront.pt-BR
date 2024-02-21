---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: Aprimoramentos no projeto 2020.2
description: Esta página descreve todas as melhorias feitas no Project com a versão 2020.2 para o ambiente de Produção. Essas melhorias foram disponibilizadas no ambiente de Produção na semana de 11 de maio de 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 150bc838-d6a5-445a-af77-62c4ed74dd1b
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 0%

---

# Aprimoramentos no projeto 2020.2

Esta página descreve todas as melhorias feitas no Project com a versão 2020.2 para o ambiente de Produção. Essas melhorias foram disponibilizadas no ambiente de Produção na semana de 11 de maio de 2020.

Para obter uma lista de todas as alterações disponíveis com a versão 2020.2, consulte [Visão geral da versão 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## Para administradores do Workfront: novo failsafe quando o status do projeto para novos projetos estiver oculto ou desbloqueado

Na Configuração, você configura uma preferência para garantir que cada novo projeto tenha um determinado status quando o projeto for criado. Isso é importante porque um projeto sempre precisa de um status para funcionar corretamente no Workfront, mesmo quando o projeto é totalmente novo.

Para garantir que novos projetos sempre tenham um status, mesmo que um administrador oculte ou desbloqueie o status configurado para novos projetos, o sistema agora atribui o primeiro status na lista Status a todos os novos projetos até que você configure o novo status para novos projetos novamente.

Para obter informações sobre como configurar a preferência para o status de todos os novos projetos, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) (ou se estiver usando o Adobe Workfront Classic, consulte [Configurando as Preferências do Projeto](https://one.workfront.com/s/article/Setting-Project-Preferences-1883392298)).

**Disponível nestes ambientes:**

* Adobe Workfront Classic
* A nova experiência do Adobe Workfront

## Para administradores do Workfront: design aprimorado nas Preferências do projeto

A experiência de definir as preferências do projeto agora é mais intuitiva e fácil de usar:

* Os títulos são maiores do que os rótulos de opção, para que você possa encontrar o que está procurando com mais rapidez.
* Dividir linhas e espaços em branco extras separam cada seção para que você possa se concentrar mais facilmente no que está fazendo.
* Se você digitar um número inválido para uma opção como &quot;Horas típicas por dia de trabalho&quot;, uma mensagem de aviso será exibida imediatamente em vez de ser exibida depois que você clicar em Salvar.
* Os rótulos de opção correspondem ao texto da interface correspondente em outro lugar no Workfront, como a área Detalhes e os relatórios.

Para obter informações sobre a área Preferências do projeto, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) (ou se estiver usando o Adobe Workfront Classic, consulte [Configurando as Preferências do Projeto](https://one.workfront.com/s/article/Setting-Project-Preferences-1883392298)).

**Disponível nestes ambientes:**

* Adobe Workfront Classic
* A nova experiência do Adobe Workfront

## Filtro, Visualização e Agrupamento selecionados retidos nas listas de Relatórios

Agora, o último Filtro, Exibição ou Agrupamento aplicado a um relatório específico é selecionado, mesmo que o usuário faça logoff e logon novamente no Workfront.

Anteriormente, depois que um usuário aplicava um Filtro, Exibição ou Agrupamento a uma lista de Relatórios e depois navegava para fora dessa página, o Filtro, Exibição ou Agrupamento padrão aparecia na próxima vez que o usuário navegava para esse mesmo relatório.

**Disponível nestes ambientes:**

* A nova experiência do Adobe Workfront
* Adobe Workfront Classic

## Mover e copiar tarefas para outro projeto mantém a restrição da tarefa quando as tarefas podem se ajustar à linha do tempo do projeto

Melhoramos a maneira como o Workfront lida com a Restrição de tarefa específica por data de uma tarefa quando você copia a tarefa ou a move para outro projeto. Exemplos de Restrições de Tarefas específicas por data são: Deve começar em, Deve terminar em, Datas fixas, Não iniciar depois de e assim por diante.

Por exemplo, quando você move ou copia uma tarefa com uma restrição Deve Iniciar Em para outro projeto cuja Data Inicial Planejada é anterior à Data Inicial da tarefa, a tarefa mantém a restrição após ser copiada ou movida. Quando você move ou copia uma tarefa com uma restrição Deve Iniciar Em para um projeto cuja Data Inicial Planejada é posterior à Data Inicial da tarefa, a Restrição da Tarefa muda para O Mais Breve Possível.

Antes dessa alteração, a Restrição da tarefa sempre muda para O mais rápido possível.

Para obter informações sobre como mover tarefas, consulte [Mover tarefas](../../../manage-work/tasks/manage-tasks/move-tasks.md) (ou se estiver usando o Adobe Workfront Classic, consulte [Movendo Tarefas](https://one.workfront.com/s/article/Moving-Tasks-2081996259)).

Para obter informações sobre como copiar tarefas, consulte [Copiar e duplicar tarefas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md) (ou se estiver usando o Adobe Workfront Classic, consulte [Copiar e Duplicar Tarefas](https://one.workfront.com/s/article/Copy-and-Duplicate-Tasks-218695605)).

Para obter uma visão geral de todas as Restrições de Tarefa, consulte [Visão geral de Restrição de Tarefa](../../../manage-work/tasks/task-constraints/task-constraint-overview.md) (ou se estiver usando o Adobe Workfront Classic, consulte [Visão Geral da Restrição de Tarefa](https://one.workfront.com/s/article/Task-Constraint-Overview-453396848)).

**Disponível nestes ambientes:**

* Adobe Workfront Classic
* A nova experiência do Adobe Workfront

## Como evitar a perda de dados enquanto faz alterações na guia Detalhes ou em uma lista de tarefas

Para evitar a perda de dados ao atualizar informações na página Detalhes de um objeto ou de tarefas em uma lista de tarefas no nível do projeto ao salvar as alterações manualmente, uma mensagem de aviso agora é exibida para notificá-lo de que você tem alterações não salvas antes de tentar editar informações no cabeçalho. As únicas ações permitidas antes de salvar suas alterações são a assinatura ou a adição do objeto aos favoritos.

Para obter informações sobre como editar tarefas em uma lista, consulte [Editar tarefas em uma lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)

**Disponível nestes ambientes:**

* A nova experiência do Adobe Workfront

