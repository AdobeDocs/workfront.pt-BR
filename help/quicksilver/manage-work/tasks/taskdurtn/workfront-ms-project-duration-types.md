---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Tipos de duração em projetos do Adobe Workfront e do Microsoft
description: Os Tipos de duração disponíveis no Adobe Workfront são diferentes de seus equivalentes no Microsoft Project, chamados de Tipos de tarefa. Às vezes, isso pode ser confuso ao exportar ou importar projetos entre o Workfront e o Microsoft Project.
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 2%

---

# Tipos de duração em projetos do Adobe Workfront e do Microsoft

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
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(drafting this because it is misleading)
</MadCap:conditionalText>
</note>
-->
