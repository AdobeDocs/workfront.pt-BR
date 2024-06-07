---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Visão geral da Data de Término Efetivo do projeto
description: Projetos, tarefas e problemas têm uma Data de conclusão efetiva no Adobe Workfront. Esta é a data em que o projeto, tarefa ou problema foi marcado como concluído.
author: Alina
feature: Work Management
exl-id: 0baba359-a61d-43d7-8336-1f45c7f34374
source-git-commit: c593eab154a0942995b1f913e7189450913faac0
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# Visão geral da Data de Término Efetivo do projeto

Projetos, tarefas e problemas têm uma Data de conclusão efetiva no Adobe Workfront. Esta é a data em que o projeto, tarefa ou problema foi marcado como concluído.

## Datas de Término Efetivo

A Data de Término Efetivo representa a data e a hora reais quando o trabalho é concluído. Quando uma tarefa ou um problema é marcado como Concluído ou Concluído, o Workfront define automaticamente a data da alteração no status do item como a Data de conclusão real da tarefa ou do problema. Se essa data não for um reflexo preciso de quando a tarefa ou o problema foi realmente concluído, você poderá editar manualmente a Data de conclusão real.

Por exemplo, você pode marcar uma tarefa ou um problema como Concluído na segunda-feira, mas sabe que o trabalho foi concluído na sexta-feira anterior. Depois de marcar a tarefa ou o problema como Concluído, você pode atualizar manualmente a Data de conclusão real da tarefa ou o problema para a data da sexta-feira anterior para refletir a conclusão real.

Não é possível editar manualmente a Data de conclusão efetiva de um projeto, mas você pode alterar manualmente o status de um projeto, o que pode acionar uma alteração na Data de conclusão efetiva.

A Data de conclusão efetiva de um projeto é definida das seguintes formas:

* Ao atualizar manualmente o status do projeto: se o Modo de conclusão do projeto estiver definido como Manual e você alterar manualmente o status do projeto para Concluído, isso acionará a Data de conclusão real do projeto a ser atualizada para a data e a hora da última tarefa concluída.
* Automaticamente, quando a última tarefa do projeto for concluída: se o Modo de conclusão do projeto estiver definido como Automático e você marcar a última tarefa como Concluída ou atualizar a Data de conclusão real da última tarefa, a Data de conclusão real do projeto também será atualizada com essa data.

  Para obter informações sobre como configurar o Modo de conclusão de um projeto, consulte o artigo [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

  >[!NOTE]
  >
  >O Workfront usa a Data de Término Efetivo da tarefa do projeto que foi concluída por último como a Data de Término Efetivo de todo o projeto.

Um administrador de Workfront ou de grupo determina se o Workfront usa a data de hoje ou a Data de conclusão planejada de uma tarefa ou um problema quando estes estiverem definidos como Concluído ou Fechado. Para obter informações sobre como configurar preferências de tarefas e problemas, consulte [Configurar preferências de tarefas e problemas em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--this statement is confusing, not sure what it is referring to, so I am drafting this for now: The value for the Actual Completion Date is always what is considered the current date and time.-->



## Localizar Datas de Término Efetivo

A Data de conclusão real está localizada nas seguintes áreas do Workfront:

* Áreas de Detalhes de Projetos, Tarefas e Problemas
* Editar caixas Projeto, Tarefa e Problema
* Atualizações de Projeto, Tarefa e Problema como uma Atualização do Sistema.
* Listas ou relatórios de projetos, tarefas ou problemas.

Para obter mais informações sobre como criar relatórios, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
