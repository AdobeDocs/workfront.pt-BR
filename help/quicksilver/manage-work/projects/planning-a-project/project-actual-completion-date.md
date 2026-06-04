---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Visão geral da data de conclusão real do projeto
description: Projetos, tarefas e problemas têm uma Data de conclusão efetiva no Adobe Workfront. Esta é a data em que o projeto, tarefa ou problema foi marcado como concluído.
author: Alina
feature: Work Management
exl-id: 0baba359-a61d-43d7-8336-1f45c7f34374
TQID: https://experienceleague.adobe.com/MoATj74YM1zoW2SsIGrpKY0gc9dHRKjlDvnPfT-kk2s
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 490
ht-degree: 2%

---

# Visão geral da data de conclusão real do projeto

Projetos, tarefas e problemas têm uma Data de conclusão efetiva no Adobe Workfront. Esta é a data em que o projeto, tarefa ou problema foi marcado como concluído.

## Datas de Término Efetivo

A Data de Término Efetivo representa a data e a hora reais quando o trabalho é concluído. Quando uma tarefa ou um problema é marcado como Concluído ou Concluído, o Workfront define automaticamente a data da alteração no status do item como a Data de conclusão real da tarefa ou do problema. Se essa data não for um reflexo preciso de quando a tarefa ou o problema foi realmente concluído, você poderá editar manualmente a Data de conclusão real.

Por exemplo, você pode marcar uma tarefa ou um problema como Concluído na segunda-feira, mas sabe que o trabalho foi concluído na sexta-feira anterior. Depois de marcar a tarefa ou o problema como Concluído, você pode atualizar manualmente a Data de conclusão real da tarefa ou o problema para a data da sexta-feira anterior para refletir a conclusão real.

Não é possível editar manualmente a Data de conclusão efetiva de um projeto, mas você pode alterar manualmente o status de um projeto, o que pode acionar uma alteração na Data de conclusão efetiva.

A Data de conclusão efetiva de um projeto é definida das seguintes formas:

* Ao atualizar manualmente o status do projeto: se o Modo de conclusão do projeto estiver definido como Manual e você alterar manualmente o status do projeto para Concluído, isso acionará a Data de conclusão real do projeto a ser atualizada para a data e a hora da última tarefa concluída.
* Automaticamente, quando a última tarefa do projeto for concluída: se o Modo de conclusão do projeto estiver definido como Automático e você marcar a última tarefa como Concluída ou atualizar a Data de conclusão real da última tarefa, a Data de conclusão real do projeto também será atualizada com essa data.

  Para obter informações sobre como definir o Modo de conclusão de um projeto, consulte o artigo [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

  >[!NOTE]
  >
  >O Workfront usa a Data de Término Efetivo da tarefa do projeto que foi concluída por último como a Data de Término Efetivo de todo o projeto.

Um administrador de Workfront ou de grupo determina se o Workfront usa a data de hoje ou a Data de conclusão planejada de uma tarefa ou um problema quando estes estiverem definidos como Concluído ou Fechado. Para obter informações sobre como definir preferências de tarefas e problemas, consulte [Configurar preferências de tarefas e problemas em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--this statement is confusing, not sure what it is referring to, so I am drafting this for now: The value for the Actual Completion Date is always what is considered the current date and time.-->



## Localizar Datas de Término Efetivo

A Data de conclusão real está localizada nas seguintes áreas do Workfront:

* Áreas de Detalhes de Projetos, Tarefas e Problemas
* Editar caixas Projeto, Tarefa e Problema
* Atualizações de Projeto, Tarefa e Problema como uma Atualização do Sistema.
* Listas ou relatórios de projetos, tarefas ou problemas.

Para obter mais informações sobre como criar relatórios, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
