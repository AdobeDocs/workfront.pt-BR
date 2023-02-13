---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Visão geral da data de conclusão real do projeto
description: Projetos, tarefas e problemas têm uma Data de conclusão real na Adobe Workfront. Esta é a data em que o projeto, a tarefa ou o problema foi marcado como concluído.
author: Alina
feature: Work Management
exl-id: 0baba359-a61d-43d7-8336-1f45c7f34374
source-git-commit: 3a3dc541219706e3f6a4700889db344c110838bb
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# Visão geral da data de conclusão real do projeto

Projetos, tarefas e problemas têm uma Data de conclusão real na Adobe Workfront. Esta é a data em que o projeto, a tarefa ou o problema foi marcado como concluído.

## Datas reais de conclusão

A Data de conclusão real representa a data e a hora reais em que o trabalho é concluído. Quando uma tarefa ou um problema é marcado como Concluído ou Concluído, o Workfront define automaticamente a data da alteração no status do item como a Data de conclusão real da tarefa ou do problema. Se essa data não for um reflexo preciso de quando a tarefa ou o problema foi realmente concluído, é possível editar manualmente a Data de conclusão real.

Por exemplo, você pode marcar uma tarefa ou um problema Concluído na segunda-feira, mas sabe que o trabalho foi concluído na sexta-feira anterior. Depois de marcar a tarefa ou o problema como Concluído, você pode atualizar manualmente a Data de conclusão real da tarefa ou emitir para a data da sexta-feira anterior para refletir a conclusão real.

Não é possível editar manualmente a Data de conclusão real de um projeto, mas é possível alterar manualmente o status de um projeto, o que pode acionar uma alteração na Data de conclusão real.

A Data de conclusão real de um projeto é definida das seguintes maneiras:

* Atualizando manualmente o status do projeto: se o Modo de conclusão do projeto estiver definido como Manual e você alterar manualmente o status do projeto para Concluído, isso acionará a Data de conclusão real do projeto a ser atualizado para a data e hora em que você alterar o status.
* Automaticamente, quando a última tarefa do projeto for concluída: se o Modo de conclusão do projeto estiver definido como Automático e você marcar a última tarefa como Concluído ou atualizar a Data de conclusão real da última tarefa, a Data de conclusão real do projeto também será atualizada com essa data.

   Para obter informações sobre como configurar o Modo de conclusão de um projeto, consulte o artigo [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

   >[!NOTE]
   >
   >O Workfront usa a Data de conclusão real da tarefa do projeto que foi concluída por último como a Data de conclusão real para todo o projeto.

Um administrador de grupo ou Workfront determina se o Workfront usa a data de hoje ou a Data de conclusão planejada de uma tarefa ou um problema quando estão definidos como Concluído ou Fechado. Para obter informações sobre como configurar as preferências de tarefa e emissão, consulte [Configurar preferências de emissão e tarefa em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--this statement is confusing, not sure what it is referring to, so I am drafting this for now: The value for the Actual Completion Date is always what is considered the current date and time.-->



## Localizar Datas de Conclusão Reais

A Data de conclusão real está localizada nas seguintes áreas do Workfront:

* Áreas Projeto, Tarefa e Detalhes da Emissão
* Editar caixas Projeto, Tarefa e Emissão
* Área de Atualizações de Projeto, Tarefa e Edição como uma Atualização do Sistema.
* Projeto, tarefa ou listas ou relatórios de problemas.

Para obter mais informações sobre como criar relatórios, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
