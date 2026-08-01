---
title: Usar Colaboradores de Tarefas
content-type: reference
description: Saiba como usar Colaboradores de tarefas, Colaboradores de IA que podem ser atribuídos a tarefas do Workfront.
author: Becky
feature: Work Management, Tasks
source-git-commit: f1bdb685cb7974c5c445377e0baa4f4b4e7dfa13
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 6%

---

# Usar Colaboradores de Tarefas

{{highlighted-preview-article-level}}

Os Colaboradores de tarefas são colaboradores de IA que podem ser atribuídos diretamente às tarefas do Workfront, além do Colaborador de IA do tipo Revisor existente usado para revisões de documentos e ativos. Como outros Colaboradores de IA, os Colaboradores de tarefas são configurados na área Configuração e atribuídos a tarefas do como um usuário.

Os Colaboradores de Tarefas conectam-se a agentes configurados por você, como um servidor MCP.

Para obter informações e instruções sobre como criar um Colaborador de Tarefas no Workfront, consulte [Configurar um Colaborador de Tarefas](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-task-collaborator) no artigo Configurar Colaboradores de IA.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacote</td> 
   <td><p>Standard, Prime ou Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licença</td> 
   <td><p>[!UICONTROL Padrão]</p>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>[!UICONTROL Administrador do Sistema]</td> 
  </tr> 
  </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

* Você deve configurar um agente no Copilot, Claude ou Writer.ai antes de usá-lo como um Colaborador de tarefas.

## Visão geral do Colaborador de Tarefas

Colaboradores de tarefas são uma maneira de atribuir agentes MCP a tarefas específicas no Workfront. Você configura o agente em um aplicativo, como o Copilot Studio, o Claude ou o Writer.ai, e depois conecta esse agente ao Workfront como um Colaborador de tarefas. Em seguida, é possível atribuí-la a tarefas como atribuiria a um usuário.

Alguns exemplos de workflows podem incluir:

* Detectar imagens carregadas em uma tarefa, gerar variações com base nos critérios fornecidos ao agente e fazer upload das novas imagens na tarefa.
* Gerar cópia a partir de uma descrição da tarefa, revisar a cópia com base nas diretrizes configuradas no agente e postar a cópia no fluxo de atualização.
* Lendo detalhes de um evento, identificando detalhes ausentes e postando perguntas na sequência de atualização sobre os detalhes ausentes.

>[!NOTE]
>
>* Detalhes específicos sobre as responsabilidades e capacidades de um agente são configurados no aplicativo em que o agente é criado, não no Workfront.
>* Atualmente, os Colaboradores de tarefas oferecem suporte a agentes criados no Copilot Studio, Claude e Writer.ai.
>* Ao configurar um agente no Copilot Studio, defina a segurança como **Sem autenticação**.
>* Para obter informações e instruções sobre como criar um Colaborador de Tarefas no Workfront, consulte [Configurar um Colaborador de Tarefas](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-task-collaborator) no artigo Configurar Colaboradores de IA.

## Atribuir um Colaborador de Tarefas a uma tarefa

Os Colaboradores de Tarefas são atribuídos às tarefas da mesma forma que os usuários são atribuídos.

Para obter instruções, consulte [Atribuir tarefas](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md).
