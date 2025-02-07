---
content-type: release-notes
keywords: notas,trimestral,atualizar,versão
navigation-topic: 2021-2-release-activity
title: 21. 2 Melhorias nos relatórios
description: Esta página descreve todas as melhorias de Relatórios feitas com a versão 21.2 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de Produção na semana de 10 de maio de 2021. Para obter uma lista de todas as alterações disponíveis com a versão 21.2, consulte Visão geral da versão 21.2.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1d5f76ef-bea7-4630-8051-454b0d109341
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# 21. 2 Melhorias nos relatórios

Esta página descreve todas as melhorias de Relatórios feitas com a versão 21.2 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de Produção na semana de 10 de maio de 2021. Para obter uma lista de todas as alterações disponíveis com a versão 21.2, consulte a [Visão geral da versão 21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Restringir a edição de horas em projetos e relatórios

Para fornecer mais controle sobre a edição de horas na guia Horas em um projeto e relatórios de Horas, adicionamos uma configuração que permite aos administradores do Workfront restringir a edição de horas a proprietários de horas e administradores do sistema.

Anteriormente, os usuários com Folhas de horas e horas ativadas no nível de acesso podiam editar horas.

Para obter mais informações, consulte [Configurar preferências de horas e folha de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Nova aparência para o campo Atribuições em listas e relatórios atualizados

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront.

Para corresponder à aparência moderna de outras áreas na nova experiência do Workfront, o estilo foi alterado para o campo Atribuições em listas e relatórios atualizados. Esse novo design inclui:

* Um avatar arredondado para as imagens do perfil do usuário, funções de trabalho e equipes
* Exibição de iniciais para usuários sem imagens de perfil
* Um novo ícone Função
* Um novo ícone Pessoas para atribuições avançadas
* Um novo ícone de Acesso Restrito
* Outras pequenas alterações de design

Para obter mais informações sobre atribuições em listas, consulte [Atribuir tarefas](../../../manage-work/tasks/assign-tasks/assign-tasks.md) ou [Atribuir problemas](../../../manage-work/issues/manage-issues/assign-issues.md).

![Atualizações de atribuições](assets/assignments-updates-350x193.png)

## Nova aparência para campos de digitação antecipada em listas e relatórios atualizados

>[!NOTE]
>
>Removido temporariamente do ambiente de Produção do em 20 de maio de 2021.

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront.

Para corresponder à aparência moderna de outras áreas na nova experiência do Workfront, o estilo foi alterado para campos de digitação antecipada em listas e relatórios atualizados. Essas alterações incluem:

* O ícone Typeahead foi removido do campo.
* Ao clicar em um campo de digitação antecipada, o menu de sugestões agora é exibido antes da inserção do texto.
* O menu de sugestões é mais responsivo ao comprimento dos valores e esses valores agora são truncados no final quando o limite de caracteres é atingido, em vez de no meio do valor.

Para obter informações sobre listas atualizadas, consulte a seção [A diferença entre as listas atualizadas e herdadas](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) no artigo [Introdução a listas no Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

![Campo de digitação antecipada](assets/typeahead-updates-350x336.png)

## Relatório sobre atualizações do sistema

O novo relatório de Lançamento oferece maior capacidade de auditoria, permitindo que você faça drill-in para atualizações do sistema, incluindo:

* Alterações de status em um projeto, tarefa ou problema
* Tarefas ou problemas excluídos
* Valores em campos personalizados
* Datas de Término Planejadas
* Alterações no proprietário do projeto

Por exemplo, você pode configurar esse relatório para mostrar a atividade em torno de um campo personalizado específico, incluindo o projeto do campo personalizado, quando um valor foi inserido pela primeira vez, qual era esse valor, quando o campo foi atualizado, qual era o valor anterior, qual era o valor recém-inserido, quais usuários concluíram essas ações etc.

Anteriormente, só era possível relatar atualizações do sistema por meio da API do Workfront.

Para saber mais sobre este relatório e como você pode usá-lo, consulte [Relatório na área Atualizações com um relatório de Entrada de Diário](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

