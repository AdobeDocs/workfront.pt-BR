---
title: 22.1 Aprimoramentos do projeto
description: 22.1 Aprimoramentos do projeto
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d24f2aae-1c3d-41ed-ad17-6276bef2cf45
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1205'
ht-degree: 0%

---

# 22.1 Aprimoramentos do projeto

Esta página descreve todas as melhorias feitas no Project com a versão 22.1 para o ambiente de Pré-visualização. Esses aprimoramentos serão disponibilizados no ambiente de produção

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

a semana de 17 de janeiro de 2022.

Para obter uma lista de todas as alterações disponíveis com a versão 22.1, consulte [Visão geral da versão 22.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Alterar a opção padrão de predecessores ao copiar ou mover tarefas

Para minimizar o número de etapas manuais ao copiar ou mover tarefas, atualizamos as informações que são copiadas ou movidas com a tarefa por padrão. Agora, todos os predecessores são copiados ou movidos com a tarefa por padrão, já que a opção Todos os predecessores é selecionada por padrão.

Antes desse aprimoramento, a opção Todos os predecessores era desmarcada por padrão ao copiar ou mover uma tarefa.

Para obter mais informações, consulte os artigos:

* [Copiar e duplicar tarefas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)
* [Mover tarefas](../../../manage-work/tasks/manage-tasks/move-tasks.md)

## Barra de ferramentas atualizada na lista de painéis e relatórios nos painéis

A barra de ferramentas em quatro páginas de painel agora tem uma aparência moderna que corresponde a outras listas do Workfront, como projetos, tarefas e problemas. Essa barra de ferramentas intuitiva agora facilita a adição, edição, compartilhamento, cópia e exclusão de painéis.

As páginas com a barra de ferramentas atualizada são:

* Relatórios de tarefas (exibidos em painéis)
* Lista Todos os painéis
* Minha lista de painéis
* Lista de painéis compartilhados

Para obter mais informações, consulte [Criar e gerenciar painéis](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-and-manage-dashboards.md).

## Adicionar e editar o painel Resumo de formulários personalizados para documentos

Agora é possível adicionar e editar formulários personalizados diretamente no painel Resumo do documento.

Com essa alteração, você também verá uma nova aparência no Resumo do documento. Há uma nova seção Visão geral, que contém a miniatura da imagem e os detalhes do documento. Também é possível fazer check-in e check-out de documentos na seção de detalhes do documento.

Anteriormente, era necessário ir até a guia formulários personalizados em Detalhes do documento para fazer edições ou adicionar formulários personalizados.

Para obter mais informações, consulte [Resumo para visão geral de documentos](../../../documents/managing-documents/summary-for-documents.md).

## Nova experiência ao copiar uma ou várias tarefas

Para tornar seu uso do Workfront consistente com a nova experiência do Adobe Workfront, reprojetamos a interface ao copiar uma tarefa. Atualmente, está disponível ao copiar uma tarefa no nível da tarefa ou ao copiar uma ou várias tarefas em uma lista.

Algumas melhorias incluem:

* Todas as informações que você deve atualizar antes de copiar a tarefa são exibidas em uma página contínua.
* O Workfront verifica se você tem acesso ao projeto de destino imediatamente após escolher o projeto. Antes dessa melhoria, uma mensagem de aviso indicando que você não tem o acesso correto era exibida após a confirmação da cópia, o que resultava em etapas extras e na não permissão da cópia.
* Capacidade de solicitar acesso a um projeto em que deseja copiar a tarefa sem sair da caixa Copiar tarefa.

Para obter mais informações, consulte [Copiar e duplicar tarefas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

## Nova experiência ao mover uma ou várias tarefas de uma lista

Para oferecer uma experiência consistente ao executar a mesma tarefa, atualizamos a interface para mover uma ou várias tarefas de uma lista para corresponder à experiência ao mover a tarefa no nível da tarefa. (Atualizamos a experiência para mover uma tarefa no nível da tarefa em uma versão anterior da Pré-visualização.)

Para obter mais informações, consulte [Mover tarefas](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Nova experiência ao mover uma tarefa no nível da tarefa

Para tornar seu uso do Workfront consistente com a nova experiência do Workfront, reprojetamos a interface para mover uma tarefa. Atualmente, está disponível ao mover uma tarefa no nível da tarefa. Em uma versão a seguir, estenderemos esse redesign para mover uma tarefa de uma lista.

Algumas das melhorias dessa interface recém-reprojetada incluem:

* Todas as informações que você deve atualizar antes de mover são exibidas em uma página contínua.
* O Workfront verificará se você tem acesso ao projeto de destino imediatamente após escolher o projeto. Antes dessa melhoria, a Workfront avisou que você não tem o acesso correto depois de confirmar a mudança, o que resultou em etapas extras e na não permissão da mudança.
* Capacidade de solicitar acesso a um projeto em que você deseja mover a tarefa sem sair da caixa Mover tarefa.

Para obter mais informações, consulte [Mover tarefas](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Nova experiência ao converter um problema em um projeto usando um modelo no nível do problema

>[!NOTE]
>
>Esse recurso foi removido temporariamente do ambiente de Produção do em 4 de março de 2022. Mais tarde, foi lançado em uma implantação em fases a partir de 28 de abril de 2022. A implantação foi concluída em 5 de maio de 2022. Agora isso está disponível em Pré-visualização e Produção para todos os clientes. (Para obter as atualizações mais recentes sobre o status desse recurso que está sendo lançado para produção, consulte [Visão geral da versão 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).)

Para tornar seu uso do Workfront consistente com a nova experiência do Workfront, reprojetamos a interface para converter um problema em um projeto ao usar um modelo ao convertê-lo da página de problema.

Agora é possível acessar com mais facilidade sua lista de favoritos imediatamente após selecionar para converter o problema.

A interface reprojetada corresponde à experiência ao criar um projeto a partir de um modelo que também atualizamos recentemente.

Para obter mais informações, consulte [Converter um problema em um projeto no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## Converter problemas em projetos usando um modelo de listas, relatórios e painéis

>[!NOTE]
>
>Esse recurso foi removido temporariamente do ambiente de Produção do em 4 de março de 2022. Mais tarde, foi lançado em uma implantação em fases a partir de 28 de abril de 2022. A implantação foi concluída em 5 de maio de 2022. Agora isso está disponível em Pré-visualização e Produção para todos os clientes. (Para obter as atualizações mais recentes sobre o status desse recurso que está sendo lançado para produção, consulte [Visão geral da versão 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).)

Para aumentar a eficiência do seu trabalho e facilitar a conversão de problemas em um ambiente de ritmo rápido, adicionamos a capacidade de converter um problema em um projeto usando um modelo de uma lista, relatório ou painel.

Antes desse aprimoramento, essa funcionalidade existia somente quando você convertia o problema da página de problemas.

Para obter mais informações, consulte [Converter um problema em um projeto no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## Filtrar por lista de usuários em quadros ágeis mostra os usuários com mais atribuições primeiro

>[!NOTE]
>
>Este recurso não será incluído na versão 22.1. Ele foi removido do ambiente de Pré-visualização.

Agora, o filtro mostra os usuários com mais atribuições primeiro, para que sejam mais fáceis de localizar sem percorrer a lista.

Anteriormente, o filtro por lista de usuários nos quadros Kanban e Scrum era exibido em ordem alfabética.

Para obter mais informações, consulte as seguintes informações

* [Filtrar por usuário no quadro Scrum](../../../agile/use-scrum-in-an-agile-team/scrum-board/filter-by-user-scrum-board.md)
* [Filtrar por usuário no quadro Kanban](../../../agile/use-kanban-in-an-agile-team/filter-by-user.md)

## Limitar a capacidade de adicionar documentos a um modelo que você está compartilhando

Às vezes, as pessoas adicionam documentos a um modelo de projeto pensando que estão adicionando a um projeto. Agora você pode ajudar a evitar isso, ao compartilhar um modelo com acesso de Exibição, é possível desativar a nova configuração avançada Adicionar documentos. Isso desativa a capacidade dos destinatários de adicionar documentos ao modelo.

Para obter instruções sobre como compartilhar um modelo, consulte [Compartilhar modelos de projeto](../../../manage-work/projects/create-and-manage-templates/share-project-template.md).

Para obter informações sobre a nova configuração avançada Adicionar documentos, consulte a seção no artigo [Compartilhamento de um modelo](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

## Compartilhar uma pasta de documentos

Agora é possível compartilhar uma pasta de documentos e seu conteúdo na área Documentos. Anteriormente, isso não era possível. Você tinha que compartilhar cada documento em uma pasta separadamente.

Para obter mais informações, consulte [Compartilhar uma pasta de documentos](../../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

