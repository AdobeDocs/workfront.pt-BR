---
content-type: release-notes
keywords: notas,trimestral,atualização,versão
navigation-topic: 2021-2-release-activity
title: 21. 2 Melhorias dos relatórios
description: Esta página descreve todas as melhorias nos Relatórios feitas com a versão 21.2 para o ambiente de Visualização. Esses aprimoramentos serão disponibilizados no ambiente de produção na semana de 10 de maio de 2021. Para obter uma lista de todas as alterações disponíveis com a versão 21.2, consulte Visão geral da versão 21.2.
author: Luke
feature: Product Announcements
exl-id: 1d5f76ef-bea7-4630-8051-454b0d109341
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---

# 21. 2 Melhorias dos relatórios

Esta página descreve todas as melhorias nos Relatórios feitas com a versão 21.2 para o ambiente de Visualização. Esses aprimoramentos serão disponibilizados no ambiente de produção na semana de 10 de maio de 2021. Para obter uma lista de todas as alterações disponíveis com a versão 21.2, consulte [Visão geral da versão 21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Restringir edição de hora em projetos e relatórios

Para fornecer mais controle sobre a edição por hora na guia Horas em um projeto e relatórios de Hora , adicionamos uma configuração que permite que os administradores do Workfront restrinjam a edição de hora aos proprietários de hora e administradores do sistema.

Anteriormente, os usuários com Folhas de horas e horas ativadas em seu nível de acesso podiam editar horas.

Para obter mais informações, consulte [Configurar preferências de hora e folha de ponto](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Nova aparência para o campo Atribuições em listas e relatórios atualizados

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront.

Para corresponder à aparência moderna de outras áreas na nova experiência do Workfront, o estilo foi alterado para o campo Atribuições em listas e relatórios atualizados. Essa reformulação inclui:

* Um avatar arredondado para imagens de perfil de usuário, funções de trabalho e equipes
* Iniciais exibidas para usuários sem imagens de perfil
* Um novo ícone de função de trabalho
* Um novo ícone de Pessoas para atribuições avançadas
* Um novo ícone de Acesso Restrito
* Outras alterações menores ao projeto

Para obter mais informações sobre atribuições em listas, consulte [Atribuir tarefas](../../../manage-work/tasks/assign-tasks/assign-tasks.md) ou [Atribuir problemas](../../../manage-work/issues/manage-issues/assign-issues.md).

![](assets/assignments-updates-350x193.png)

## Nova aparência para campos de digitação em listas e relatórios atualizados

>[!NOTE]
>
>Removido temporariamente do ambiente de Produção em 20 de maio de 2021.

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront.

Para corresponder à aparência moderna de outras áreas na nova experiência do Workfront, o estilo foi alterado para campos de digitação em listas e relatórios atualizados. Essas alterações incluem:

* O ícone Typeahead foi removido do campo .
* Ao clicar em um campo do tipo , o menu de sugestões agora é exibido antes que você insira texto.
* O menu de sugestões é mais responsivo ao comprimento dos valores e esses valores agora são truncados no final quando o limite de caracteres é atingido, em vez de no meio do valor.

Para obter informações sobre listas atualizadas, consulte o [A diferença entre as listas atualizadas e herdadas](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) no artigo [Introdução a listas no Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

![](assets/typeahead-updates-350x336.png)

## Relatório sobre atualizações do sistema

O novo relatório de Entrada de Lançamento oferece maior capacidade de auditoria, permitindo que você faça drill-in nas atualizações do sistema, incluindo:

* Alterações de status em um projeto, tarefa ou problema
* Tarefas ou problemas excluídos
* Valores em campos personalizados
* Datas de Conclusão Planejadas
* Alterações no proprietário do projeto

Por exemplo, você pode configurar esse relatório para mostrar a atividade em torno de um campo personalizado específico, incluindo o projeto para o campo personalizado, quando um valor foi inserido pela primeira vez, qual foi o valor, quando o campo foi atualizado, qual foi o valor anterior, qual foi o valor inserido recentemente, quais usuários concluíram essas ações etc.

Anteriormente, era possível criar relatórios sobre atualizações de sistema somente por meio da API do Workfront.

Para saber mais sobre esse relatório e para que pode usá-lo, consulte [Relatório sobre a área Atualizações](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

