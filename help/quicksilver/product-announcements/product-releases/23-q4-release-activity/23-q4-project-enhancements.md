---
title: Aprimoramentos do projeto do quarto trimestre de 2023
description: Aprimoramentos do projeto do quarto trimestre de 2023
author: Lisa
feature: Product Announcements
source-git-commit: 803c03845b834757b4643d8fd5c88f185ad6c32e
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# Aprimoramentos do projeto do quarto trimestre de 2023

Esta página descreve todas as melhorias de projeto feitas com a versão do quarto trimestre de 2023 para o ambiente de Pré-visualização. Esses aprimoramentos serão disponibilizados no ambiente de produção com a versão 23.10.

Para obter uma lista de todas as alterações disponíveis neste momento do ciclo de lançamento do quarto trimestre de 2023, consulte [Visão geral da versão do quarto trimestre de 2023](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md).

## Novas aprovações de documentos

As aprovações de documentos estão sendo reprojetadas em uma implantação em fases que será disponibilizada para mais usuários com cada versão.

Nesta versão, o processo de aprovação foi simplificado para a criação de aprovações e a aprovação/revisão de documentos, além de novas funcionalidades. As melhorias específicas incluem:

* Interface aprimorada para alterar um usuário entre um revisor e um aprovador
* Processo aprimorado para adicionar um aprovador ou revisor externo
* Experiência de aprovação e revisão aprimorada para aprovadores e revisores externos

Para obter mais informações sobre como usar as novas aprovações de documentos, consulte [Visão geral das novas aprovações de documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

[Veja uma demonstração em vídeo desse recurso.](https://video.tv.adobe.com/v/3424867){target=_blank}

## Design atualizado ao adicionar um novo problema a um projeto

Esta atualização foi anunciada com a versão 23.3 do.

Atualizamos a caixa Novo problema que é exibida ao enviar um novo problema para um projeto. Agora, a interface corresponde à caixa Nova solicitação, que é exibida ao enviar uma nova solicitação para uma fila de solicitações.

Para obter mais informações, consulte [Criar problemas](/help/quicksilver/manage-work/issues/manage-issues/create-issues.md).

## Recálculo dinâmico de campos calculados em formulários

Os campos calculados em um formulário anexado a um objeto agora são recalculados dinamicamente em tempo real quando valores dependentes de qualquer formulário na página são modificados. Isso permite que você veja os resultados atualizados sem salvar o formulário.

A forma como os campos são calculados não foi alterada.

Um pequeno número de campos de formulário não terá recálculo dinâmico, em páginas que não foram modernizadas.

Para obter mais informações, consulte [Editar informações em campos de formulário personalizados](/help/quicksilver/workfront-basics/work-with-custom-forms/edit-custom-forms.md).

[Veja uma demonstração em vídeo desse recurso.](https://video.tv.adobe.com/v/3422678/){target=_blank}

## Definir horas planejadas em tarefas filho recorrentes com tipo de duração Simples sem atribuições

Fizemos uma alteração na maneira como as Horas planejadas são alocadas para tarefas recorrentes sem atribuições e com um tipo de duração Simples. Agora, quando você define Horas Planejadas em uma nova tarefa recorrente com um Tipo de Duração Simples e sem atribuições, as horas também são alocadas para as recorrências individuais. Antes dessa alteração, as horas não eram salvas para recorrências individuais quando as tarefas pai eram desatribuídas.

Para obter informações sobre como criar tarefas recorrentes, consulte [Criar tarefas recorrentes](/help/quicksilver/manage-work/tasks/create-tasks/create-recurring-tasks.md).

## Atualizações em tempo real na lista de tarefas

As listas de tarefas agora são atualizadas em tempo real. As alterações feitas em uma tarefa são atualizadas na lista de tarefas, para que um usuário que esteja visualizando a lista de tarefas possa ver as alterações sem atualizar a página.
