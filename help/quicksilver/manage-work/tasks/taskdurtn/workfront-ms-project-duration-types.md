---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Tipos de duração no Adobe Workfront e Microsoft Project
description: Os Tipos de duração disponíveis no Adobe Workfront são diferentes de seus equivalentes no Microsoft Project, chamados de Tipos de tarefa. Às vezes, isso pode ser confuso ao exportar ou importar projetos entre o Workfront e o Microsoft Project.
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
TQID: https://experienceleague.adobe.com/avh0ZuYJpsf7Ed5HiWuLkxEA-0PD-1iFvzHmWvpDZiI
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 257
ht-degree: 11%

---

# Tipos de duração no Adobe Workfront e Microsoft Project

Os Tipos de duração disponíveis no Adobe Workfront são diferentes de seus equivalentes no Microsoft Project, chamados de Tipos de tarefa. Às vezes, isso pode ser confuso ao exportar ou importar projetos entre o Workfront e o Microsoft Project.

Para obter informações sobre como importar e exportar projetos entre o Workfront e o Microsoft Project, consulte os seguintes artigos:

* [Exportar um projeto para o Projeto do Microsoft](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Importar um projeto do Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)

## Tipos de duração em projetos do Workfront e do Microsoft

O Workfront tem quatro tipos de duração de tarefa:

* Simples
* Controlado pelo empenho
* Trabalho Calculado
* Atribuição Calculada

Para obter informações, consulte [Visão geral da duração e do tipo de duração da tarefa](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Esses tipos de duração não são reconhecidos pelo Microsoft Project. Atualmente, o Microsoft Project tem três tipos de tarefa semelhantes aos tipos de duração no Workfront:

* Unidades Fixas
* Trabalho Fixo
* Duração fixa

## O tipo de duração é alterado ao exportar do Workfront para o MS Project

Ao exportar projetos do Workfront para o Microsoft Project, as tarefas orientadas pelo esforço se tornam Trabalho fixo. O Trabalho Simples, Calculado e a Atribuição Calculada se tornam Unidades Fixas.

## O tipo de duração muda ao importar do MS Project para o Workfront

Ao importar projetos do Microsoft Project para o Workfront, as Unidades fixas se tornam Orientadas pelo esforço. Trabalho fixo e Duração fixa recebem o tipo de duração padrão que o administrador do Workfront selecionou para o sistema. Para obter informações, consulte [Configurar preferências de tarefas e problemas do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--
<note type="warning">
When a task has Calculated Work as the Duration Type and the default Duration Type in Setup is set as Calculated Assignment, then MS Project assignment allocations will be lost during the import.
 
(drafting this because it is misleading)
 
</note>
-->
