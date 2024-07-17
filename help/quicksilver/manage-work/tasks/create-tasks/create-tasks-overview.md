---
product-area: projects
navigation-topic: create-tasks
title: Visão geral da criação de tarefas
description: Você só pode criar tarefas em um projeto depois de criá-lo.
author: Alina
feature: Work Management
exl-id: 7bd6578e-9288-4793-ba07-a0c126c479b9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 0%

---

# Visão geral da criação de tarefas

Você só pode criar tarefas em um projeto depois de criá-lo.

Por exemplo, após criar um projeto, você pode adicionar tarefas e modificá-las para organizar o plano do projeto. Para obter mais informações sobre como criar um projeto, consulte [Criar um projeto](../../../manage-work/projects/create-projects/create-project.md). Para obter informações sobre como criar tarefas, consulte [Criar tarefas em um projeto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

Este artigo descreve considerações, limitações e padrões que se aplicam ao criar tarefas.

## Maneiras de criar tarefas em um projeto

Você pode criar tarefas em um projeto das seguintes maneiras:

* Do zero, conforme descrito em [Criar tarefas em um projeto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).
* Copie tarefas para o mesmo projeto ou para um novo projeto ou duplique tarefas no mesmo projeto, conforme descrito em [Copiar e duplicar tarefas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* Mova tarefas de um projeto para outro, conforme descrito em [Mover tarefas](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Limitações na criação de tarefas

Quando você tem o acesso e as permissões corretas, é possível criar tarefas em um projeto. No entanto, os seguintes casos ocorrem quando talvez você não possa criar tarefas:

* O administrador do Adobe Workfront ou um administrador de grupo deve ativar a adição de tarefas a um projeto com status Concluído ou Inativo na área Preferências do projeto. Para obter informações sobre como definir preferências de projeto, consulte [Configurar preferências de projeto do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Não é possível adicionar tarefas a um projeto que está em Aprovação pendente.

## O número máximo de tarefas permitido em um projeto

Um projeto pode conter até 5.000 tarefas. Uma mensagem de aviso é exibida no projeto quando você está se aproximando do limite, quando o limite é atingido e se você tentar exceder o limite.

Dependendo do número de tarefas em seus projetos quando essa limitação foi imposta, a instância do Workfront pode permitir mais de 5.000 tarefas em um único projeto.

Se você conseguir incluir mais de 5.000 tarefas em um único projeto, esteja ciente do seguinte:

* O limite de tarefas do ambiente Workfront é definido como o número atual de tarefas no maior projeto, mais 10% adicionais.

  Por exemplo, se um projeto na instância do Workfront contiver 10.000 tarefas, o limite de cada projeto em toda a instância do Workfront será de 11.000 tarefas.

* Projetos menores melhoram o desempenho e minimizam os desafios de gerenciamento que acompanham projetos grandes.

## Padrões de tarefa ao adicionar tarefas a um projeto

Há dois tipos de informações padrão que o Workfront atualiza automaticamente para tarefas quando você as cria:

* Informações padrão no nível do sistema

  O administrador do Workfront ou um administrador de grupo estabelece os padrões no nível do sistema para tarefas na área Tarefas e problemas das Preferências do projeto. Para obter informações sobre preferências de tarefas e problemas, consulte [Configurar preferências de tarefas e problemas em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) ou [Configurar preferências de tarefas e problemas para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

* Informações padrão no nível do projeto

  O restante desta seção descreve os padrões em nível de projeto que você, como gerente de projeto, pode definir para todas as novas tarefas adicionadas a um projeto

Quando você adiciona uma tarefa a um projeto, dependendo de como o projeto está configurado, o Workfront pode anexar automaticamente um processo de aprovação ou formulários personalizados à tarefa.

Para obter informações sobre como configurar um projeto para adicioná-los por padrão, consulte a seção &quot;Tarefas&quot; no artigo [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

Ao definir as informações padrão a serem associadas com tarefas adicionadas a um projeto no nível do projeto, considere o seguinte:

* Você deve ter permissões de gerenciamento no projeto para definir as configurações padrão para o processo de aprovação de tarefas e formulários personalizados.
* Todas as novas tarefas são criadas com o processo de aprovação e os formulários personalizados definidos ao editar o projeto.
* É possível modificar essas configurações padrão ao adicionar tarefas usando a caixa Editar tarefa, mas não ao adicionar tarefas em edição em linha.
* Você pode definir o processo de aprovação e os formulários personalizados para tarefas em um modelo.

   * Quando um projeto é criado a partir desse modelo, o processo de aprovação e os formulários personalizados são aplicados automaticamente ao projeto.
   * Quando um modelo é anexado a um projeto existente, o projeto preserva o processo de aprovação da tarefa original e as configurações de formulários personalizados, se estiverem definidas. Se não estiverem definidas, as configurações do modelo se tornarão as configurações do projeto.
   * Quando um modelo é anexado a um projeto existente, as tarefas adicionadas ao projeto a partir do modelo preservam o processo de aprovação e as configurações personalizadas de formulários que tinham no modelo, independentemente das configurações da tarefa no projeto.

  Para obter informações sobre como anexar um modelo a um projeto, consulte [Anexar um modelo a um projeto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Ao copiar o projeto, as configurações padrão da tarefa são transferidas para o novo projeto.

  Para obter informações sobre como copiar um projeto, consulte [Copiar um projeto](../../../manage-work/projects/manage-projects/copy-project.md).

* Quando você copia tarefas de um projeto para outro e o projeto de destino tem configurações padrão diferentes para tarefas, as tarefas copiadas preservam as configurações padrão do projeto original, a menos que sejam limpas no processo de cópia.
* Quando você duplica uma tarefa no mesmo projeto, os formulários personalizados e o processo de aprovação são transferidos para a tarefa duplicada.

  Para obter informações sobre como copiar e duplicar tarefas, consulte [ [Copiar e duplicar tarefas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

* Quando você move a tarefa para outro projeto, as configurações padrão da tarefa são salvas nas tarefas do projeto original, independentemente das configurações padrão da tarefa no novo projeto.

  Para obter informações sobre como mover tarefas, consulte [Mover tarefas](../../../manage-work/tasks/manage-tasks/move-tasks.md).
