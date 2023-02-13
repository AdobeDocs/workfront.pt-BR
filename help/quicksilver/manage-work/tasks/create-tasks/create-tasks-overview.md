---
product-area: projects
navigation-topic: create-tasks
title: Criar visão geral de tarefas
description: Você pode criar tarefas em um projeto somente depois de criá-lo.
author: Alina
feature: Work Management
exl-id: 7bd6578e-9288-4793-ba07-a0c126c479b9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---

# Criar visão geral de tarefas

Você pode criar tarefas em um projeto somente depois de criá-lo.

Por exemplo, depois de criar um projeto, você pode querer adicionar tarefas e modificá-las para organizar o plano do projeto. Para obter mais informações sobre como criar um projeto, consulte [Criar um projeto](../../../manage-work/projects/create-projects/create-project.md). Para obter informações sobre como criar tarefas, consulte [Criar tarefas em um projeto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

Este artigo descreve considerações, limitações e padrões que se aplicam ao criar tarefas.

## Maneiras de criar tarefas em um projeto

Você pode criar tarefas em um projeto das seguintes maneiras:

* Do zero, conforme descrito em [Criar tarefas em um projeto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).
* Copie tarefas para o mesmo projeto ou para um novo projeto ou duplique tarefas no mesmo projeto, conforme descrito em [Copiar e duplicar tarefas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* Mover tarefas de um projeto para outro, conforme descrito em [Mover tarefas](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Limitações na criação de tarefas

Quando tiver o acesso e as permissões corretas, você poderá criar tarefas em um projeto. No entanto, os seguintes são casos em que talvez você não consiga criar tarefas:

* O administrador do Adobe Workfront ou um administrador de grupo deve habilitar a adição de tarefas a um projeto que esteja em um status Concluído ou Inativo na área Preferências do projeto . Para obter informações sobre como definir preferências de projeto, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Não é possível adicionar tarefas a um projeto que esteja em Aprovação pendente.

## O número máximo de tarefas permitidas em um projeto

Um projeto pode conter até 5.000 tarefas. Uma mensagem de aviso é exibida no projeto quando você estiver se aproximando do limite, quando atingir o limite e tentar exceder o limite.

Dependendo do número de tarefas em seus projetos quando essa limitação foi imposta, a instância do Workfront pode permitir mais de 5.000 tarefas em um único projeto.

Se você conseguir incluir mais de 5.000 tarefas em um único projeto, esteja ciente do seguinte:

* O limite de tarefas para seu ambiente Workfront é definido para o número atual de tarefas em seu maior projeto, mais um 10% adicional.

   Por exemplo, se um projeto na instância do Workfront contiver 10.000 tarefas, o limite para cada projeto na instância do Workfront será de 11.000 tarefas.

* Projetos menores melhoram o desempenho e minimizam os desafios de gerenciamento que acompanham grandes projetos.

## Padrões de tarefa ao adicionar tarefas a um projeto

Há dois tipos de informações padrão que o Workfront atualiza automaticamente para tarefas quando você as cria:

* Informações padrão de nível de sistema

   O administrador do Workfront ou um administrador de grupo estabelece os padrões do sistema para tarefas na área Tarefas e problemas das Preferências do projeto. Para obter informações sobre as preferências de tarefa e emissão, consulte [Configurar preferências de emissão e tarefa em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) ou [Configurar preferências de tarefa e emissão para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

* Informações padrão de nível de projeto

   O restante desta seção descreve os padrões do nível do projeto que você, como gerente de projeto, pode definir para todas as novas tarefas adicionadas a um projeto

Ao adicionar uma tarefa a um projeto, dependendo de como o projeto é configurado, o Workfront pode anexar automaticamente um processo de aprovação ou formulários personalizados à tarefa.

Para obter informações sobre como configurar um projeto para adicioná-las por padrão, consulte a seção &quot;Tarefas&quot; no [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md) artigo 10. o

Ao definir informações padrão a serem associadas a tarefas adicionadas a um projeto no nível do projeto, considere o seguinte:

* É necessário ter permissões de gerenciamento no projeto para definir as configurações padrão para o processo de aprovação de tarefas e formulários personalizados.
* Todas as novas tarefas são criadas com o processo de aprovação e os formulários personalizados definidos ao editar o projeto.
* Você pode modificar essas configurações padrão ao adicionar tarefas usando a caixa Editar tarefa, mas não ao adicionar tarefas na edição em linha.
* Você pode definir o processo de aprovação e os formulários personalizados para tarefas em um modelo.

   * Quando um projeto é criado a partir desse modelo, o processo de aprovação e os formulários personalizados são automaticamente aplicados ao projeto.
   * Quando um modelo é anexado a um projeto existente, o projeto preserva o processo de aprovação da tarefa original e as configurações de formulários personalizados, se estiverem definidas. Se não estiverem definidas, as configurações do modelo se tornarão as configurações do projeto.
   * Quando um modelo é anexado a um projeto existente, as tarefas adicionadas ao projeto a partir do modelo preservam o processo de aprovação e as configurações de formulários personalizados que tinham no modelo, independentemente das configurações de tarefa no projeto.

   Para obter informações sobre como anexar um modelo a um projeto, consulte [Anexar um modelo a um projeto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Ao copiar o projeto, as configurações padrão da tarefa são transferidas para o novo projeto.

   Para obter informações sobre cópia de um projeto, consulte [Copiar um projeto](../../../manage-work/projects/manage-projects/copy-project.md).

* Ao copiar tarefas de um projeto para outro e o projeto de destino tiver configurações padrão diferentes para tarefas, as tarefas copiadas preservarão as configurações padrão do projeto original, a menos que sejam apagadas no processo de cópia.
* Ao duplicar uma tarefa no mesmo projeto, os formulários personalizados e o processo de aprovação são transferidos para a tarefa duplicada.

   Para obter informações sobre cópia e duplicação de tarefas, consulte [ [Copiar e duplicar tarefas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

* Quando você move a tarefa para outro projeto, as configurações padrão da tarefa são salvas nas tarefas do projeto original, independentemente das configurações padrão da tarefa no novo projeto.

   Para obter informações sobre como mover tarefas, consulte [Mover tarefas](../../../manage-work/tasks/manage-tasks/move-tasks.md).
