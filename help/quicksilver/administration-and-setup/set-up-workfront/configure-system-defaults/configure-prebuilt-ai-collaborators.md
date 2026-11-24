---
user-type: administrator
product-area: system-administration;setup
title: Configurar colaboradores de IA pré-criados
description: Como administrador do Adobe Workfront, você pode configurar Colaboradores de IA pré-criados da Adobe, como o Coordenador de entrada, como Agentes de trabalho que os usuários podem atribuir a tarefas e problemas.
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: ee344fe88ba7e4fb78a6d80ccbfe5cfa1ecbec47
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 8%
---
# Configurar colaboradores de IA pré-criados

## Visão geral

Os Colaboradores de IA pré-criados são Agentes de trabalho prontos da Adobe configurados para executar um trabalho específico, como verificar solicitações de informações ausentes. Eles estão disponíveis como Agentes de trabalho nativos do Adobe, portanto, você não precisa configurar um agente em uma plataforma externa ou fornecer credenciais de plataforma externa.

Ao configurar um Agente de Trabalho, você seleciona um Colaborador pré-criado como a origem do agente. Em seguida, você pode nomear o Agente de trabalho, definir seu nível de acesso e escolher as ações que ele pode realizar. Os usuários atribuem o Agente de trabalho configurado a tarefas ou problemas da mesma forma que atribuem qualquer outro Agente de trabalho. Os usuários não precisam saber que o agente é um Collaborator pré-criado.

Para obter mais informações sobre os Agentes de trabalho e outros tipos de Colaboradores de IA, consulte [Configurar Colaboradores de IA](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacote</td> 
   <td><p>Select, Prime ou Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licença</td> 
   <td><p>[!UICONTROL Padrão]</p></td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>[!UICONTROL Administrador do Sistema] ou Administrador de Grupo</td> 
  </tr> 
  </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Sua organização deve ter o Adobe CX Coworker habilitado. Para obter mais informações, consulte [Visão geral do CX Enterprise Coworker no Workfront](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md).

## Configurar um colaborador de IA pré-criado

Você configura um Colaborador de IA pré-criado ao configurar um Agente de trabalho. Na área **Escolher origem do agente**, selecione **Adobe Nativo** e selecione o Colaborador pré-criado que deseja usar na lista abaixo.

Para obter as etapas completas, consulte [Configurar um Agente de Trabalho no Workfront](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-work-agent-in-workfront).

Depois que o Collaborator é configurado, os usuários podem atribuí-lo a tarefas ou problemas. Para obter mais informações, consulte [Usar Agentes de Trabalho](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).

## Colaboradores de IA pré-criados disponíveis

### CX Enterprise Coworker {#cx-enterprise-coworker}

Um agente do CX Enterprise Coworker habilitado pela Adobe Agent Orchestrator.

Para obter mais informações, consulte [Visão geral do CX Enterprise Coworker no Workfront](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md).

### Coordenador de entrada {#intake-coordinator}

O Coordenador de entrada verifica os detalhes, formulários personalizados e anexos de solicitações quanto a informações ausentes, confusas ou inconsistentes. Ele publica feedback ou faz alterações com a aprovação do usuário.

<!--
### Context Carrier {#context-carrier}

The Context Carrier keeps brief information flowing downstream so that context doesn't get scattered. It helps campaign managers and project managers keep the project team current without writing reports.

Requirements: A Workfront project and a Workfront Planning project must be connected to a Planning record. The Context Carrier must be triggered to run.

Steps to be added.

### Production Specialist {#production-specialist}

The Production Specialist produces images in every size you need, so designers don't have to resize them manually.

Requirement: Users must assign the Production Specialist to a task or issue.

Steps to be added.

### Version Comparer {#version-comparer}

The Version Comparer compares versions of a document so project teams can move content faster instead of spotting differences by hand.

Requirement: The document must have more than one version.

Steps to be added.

### Metadata Manager {#metadata-manager}

The Metadata Manager helps marketing teams find, tag, and label documents while work is in progress instead of later in the process.

Requirement: The Metadata Manager is available when you upload a document. Users must trigger it from the toolbar.

Steps to be added.

### Resource PTO Detector {#resource-pto-detector}

The Resource PTO Detector helps project teams make sure delivery isn't affected by time off, by identifying tasks assigned to people who are out of office.

Requirements: Tasks must be assigned, and PTO must be logged in Workfront.

Steps to be added.

### Campaign Summarizer {#campaign-summarizer}

Description and steps to be added.
-->
