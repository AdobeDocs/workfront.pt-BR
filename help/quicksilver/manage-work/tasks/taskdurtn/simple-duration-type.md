---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Visão geral do tipo de duração: simples'
description: O Tipo de duração simples é um Tipo de duração que pode ser definido para uma tarefa no Adobe Workfront.
author: Alina
feature: Work Management
exl-id: 9bb472db-1448-467e-93ca-611453e1c00a
TQID: https://experienceleague.adobe.com/-pBdowTzvPA4ubjZsZnaELWkVfmrd48nowdJJm0hhXk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 326
ht-degree: 1%

---

# Visão geral do tipo de duração: simples

<!-- Audited: 5/2025 -->

O Tipo de duração simples é um tipo de duração que pode ser definido para uma tarefa no Adobe Workfront. Para obter mais informações sobre os tipos de duração no Workfront, consulte [Visão Geral da Duração e do Tipo de Duração da Tarefa](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Visão geral do tipo de duração simples

O administrador do Workfront ou do grupo pode definir o tipo de duração padrão do seu sistema ou grupo como Simples. Nesse caso, todas as novas tarefas serão criadas com esse tipo de duração.

Para obter informações sobre como alterar as preferências de tarefas e problemas como parte das preferências de projetos no nível do sistema ou do grupo, consulte [Configurar preferências de tarefas e problemas em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

As seguintes situações ocorrem quando uma tarefa tem um tipo de duração Simples:

* Os gerentes de projeto podem modificar a Duração e as Horas planejadas de uma tarefa ao modificar como essas horas devem ser distribuídas entre os atribuídos.

  Para obter informações, consulte [Atualizar as horas planejadas e a duração de uma tarefa com um tipo de duração simples](../../../manage-work/tasks/taskdurtn/update-planned-hours-duration-for-simple-duration-task.md).

  >[!IMPORTANT]
  >
  >Quando você cria uma tarefa pela primeira vez e a atribui ao tipo de duração Simples, mas não especifica uma Duração, o Workfront calcula a duração da tarefa com base na quantidade de Horas planejadas especificada para a tarefa. Se você modificar manualmente a duração de uma tarefa Duração simples, o Workfront interromperá a correspondência das Horas planejadas com a duração, pois presume que você deseja defini-las manualmente.
  >
  >O Workfront calcula a duração das tarefas cuja duração não foi modificada manualmente usando a seguinte fórmula:
  >
  > `Task Duration = Task Planned Hours / Typical hours per work day`
  >
  >O administrador do Workfront define `Typical hours per work day` na área Preferências do projeto da instalação da sua instância.

* A porcentagem de alocação está oculta, mas as horas de alocação estão disponíveis para edição.
* Todos os novos clientes têm o Tipo de duração no nível do sistema definido como Simples.

## Alterar o tipo de duração de uma tarefa para Simples

Para obter informações sobre como alterar o Tipo de Duração de uma tarefa, consulte [Atualizar o Tipo de Duração de uma tarefa](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3"> <p>Select <strong>Simple</strong> from the drop-down menu.</p> </li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong><strong>.</strong></li>
</ol>
-->
