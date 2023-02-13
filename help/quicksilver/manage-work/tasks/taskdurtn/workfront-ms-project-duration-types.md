---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Tipos de duração no projeto Adobe Workfront e Microsoft
description: Os Tipos de duração disponíveis no Adobe Workfront são diferentes de suas contrapartes no Projeto Microsoft, que são chamadas Tipos de tarefa. Às vezes, isso pode ser confuso ao exportar ou importar projetos entre o Workfront e o Microsoft Project.
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 2%

---

# Tipos de duração no projeto Adobe Workfront e Microsoft

Os Tipos de duração disponíveis no Adobe Workfront são diferentes de suas contrapartes no Projeto Microsoft, que são chamadas Tipos de tarefa. Às vezes, isso pode ser confuso ao exportar ou importar projetos entre o Workfront e o Microsoft Project.

Para obter informações sobre a importação e exportação de projetos entre o Workfront e o Microsoft Project, consulte os seguintes artigos:

* [Exportar um projeto para o Projeto Microsoft](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Importar um projeto do Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)

## Tipos de duração no projeto Workfront e Microsoft

O Workfront tem quatro tipos de duração de tarefa:

* Simples
* Controlado pelo empenho
* Trabalho Calculado
* Atribuição Calculada

Para obter mais informações, consulte [Visão Geral da Duração da Tarefa e do Tipo de Duração](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Esses tipos de duração não são reconhecidos pelo Microsoft Project. Atualmente, o Projeto do Microsoft tem três Tipos de tarefa semelhantes aos Tipos de duração no Workfront:

* Unidades fixas
* Trabalho Fixo
* Duração fixa

## O Tipo de duração muda ao exportar do Workfront para o Projeto MS

Ao exportar projetos do Workfront para o Microsoft Project, as tarefas orientadas para o esforço tornam-se trabalho fixo. O trabalho simples, calculado e a atribuição calculada tornam-se unidades fixas.

## Alteração do Tipo de Duração ao importar do Projeto MS para o Workfront

Ao importar projetos do Microsoft Project para o Workfront, as unidades fixas se tornam orientadas para o esforço. O Trabalho fixo e a Duração fixa recebem o tipo de duração padrão selecionado pelo administrador do Workfront para o seu sistema. Para obter mais informações, consulte [Configurar preferências de emissão e tarefa em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--
<note type="warning">
When a task has Calculated Work as the Duration Type and the default Duration Type in Setup is set as Calculated Assignment, then MS Project assignment allocations will be lost during the import.
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(drafting this because it is misleading)
</MadCap:conditionalText>
</note>
-->
