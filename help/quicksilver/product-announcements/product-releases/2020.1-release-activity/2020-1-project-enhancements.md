---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: Aprimoramentos no projeto 2020.1
description: Esta página descreve todas as melhorias feitas nos Projetos com a versão 2020.1. Esses aprimoramentos estão disponíveis atualmente no ambiente de Pré-visualização e serão disponibilizados no ambiente Produção no final de março ou início de abril de 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 13b6dd9e-52b9-4c5f-b727-bf32fbb94e8c
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# Aprimoramentos no projeto 2020.1

Esta página descreve todas as melhorias feitas nos Projetos com a versão 2020.1. Esses aprimoramentos estão disponíveis atualmente no ambiente de Pré-visualização e serão disponibilizados no ambiente Produção no final de março ou início de abril de 2020.

Para obter uma lista de todas as alterações disponíveis com a versão 2020.1, consulte [Visão geral da versão 2020.1](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md).

## Veja mais facilmente quem está marcado em uma atualização

Agora ficou mais fácil ver quais usuários estão marcados em uma atualização. Os nomes dos usuários marcados são exibidos em azul e vinculados ao perfil do usuário.

Os usuários marcados também são listados na caixa de comentários.

Antes dessa melhoria, os usuários marcados anteriormente não apareciam na caixa Notificar.

Para obter mais informações, consulte [Marcar outros usuários em atualizações](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Incluir e identificar texto citado em um comentário ou resposta de atualização

Ao digitar um comentário, você pode marcar parte dele como citação para diferenciá-lo do seu próprio comentário. Use o botão Cotação de bloco no editor de HTML.

Para obter mais informações, consulte [Atualizar trabalho](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).


## Citar um comentário anterior em um comentário ou resposta de atualização

Ao comentar em uma thread de atualização, você pode incluir rapidamente o texto de um comentário anterior na thread. Procure a opção Responder à Cotação no menu Mais ao lado do comentário que você deseja citar.

Para obter mais informações, consulte [Atualizar trabalho](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Informações adicionais sobre riscos

Para ajudá-lo a entender melhor os riscos de seus projetos, agora é possível ver quem e quando um risco foi inserido e quando ele foi atualizado em um projeto. É possível acessar essas informações em uma visualização de risco e por meio da API pública do Workfront. Esses campos estarão disponíveis com a API versão 11, que é lançada com a versão de Produção 2020.1.

Para obter informações sobre riscos no Workfront, consulte [Criar e editar riscos em projetos](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

## Campos adicionais foram adicionados às Linhas de Base e Tarefas de Linha de Base

Para ajudá-lo a entender melhor o progresso financeiro de seus projetos, agora é possível incluir informações adicionais de custo e receita em um relatório de Linha de base ou de Tarefa de Linha de base. As informações financeiras adicionais não são adicionadas às linhas de base que você salvou no momento, mas são adicionadas para novas linhas de base.

Para obter informações sobre campos financeiros de projeto e tarefa que podem ser acessados a partir dos objetos de Linha de Base e Tarefa de Linha de Base, consulte [Finanças do projeto incluídas nas linhas de base do projeto](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md).

## Problemas no status &quot;Fechado-Pendente de Aprovação&quot; são considerados incompletos

A maneira como o Workfront lida com problemas em um status &quot;Concluído - Aprovação pendente&quot; foi alterada. Agora, esses problemas são percebidos como Abertos e o projeto não pode ser marcado como Concluído até que a aprovação seja resolvida.

Antes dessa alteração, os problemas em um status &quot;Fechado-Pendente de Aprovação&quot; eram considerados Fechados.

Todos os problemas colocados em um status Fechado - Pendente de Aprovação antes dessa alteração se comportarão da mesma forma que antes, sendo considerados concluídos e permitindo que o projeto também seja concluído. Todos os problemas colocados nesse status após a alteração serem feitos serão considerados incompletos.

Para obter informações sobre status de projetos, consulte [Acessar a lista de status de projeto do sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).

