---
title: Usar Colaboradores de Tarefas
content-type: reference
description: Saiba como usar Colaboradores de tarefas, Colaboradores de IA que podem ser atribuídos a tarefas do Workfront.
author: Becky
feature: Work Management, Tasks
source-git-commit: 1894bbb5ec7f44f93468c202fb9c07fa656a83cf
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 2%

---

# Usar Colaboradores de Tarefas

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Após o lançamento para Pré-visualização, os mesmos recursos também estarão disponíveis mensalmente no ambiente de Produção para clientes que ativaram versões rápidas. </span>

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
   <td><p>Select, Prime ou Ultimate</p></td> 
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

## Acionadores de início do Colaborador de Tarefas

Quando um Colaborador de Tarefas é atribuído a uma tarefa, ele começa a trabalhar quando qualquer uma das seguintes situações é atendida:

* O Colaborador de Tarefas é atribuído a uma tarefa que está pronta para ser iniciada. (Por exemplo, se a tarefa tiver predecessoras, elas serão concluídas.)
* O Colaborador de Tarefas e um usuário são atribuídos a uma tarefa, e o Colaborador de Tarefas é atribuído primeiro.
* Uma tarefa para a qual um Colaborador de Tarefas já foi atribuído como pronta para ser iniciada, e o Colaborador de Tarefas é o único designado ou o principal designado. (Por exemplo, se a tarefa tiver predecessoras, elas serão concluídas.)
* Uma tarefa para a qual um Colaborador de Tarefas e um usuário já estão atribuídos fica pronta para ser iniciada, e o Colaborador de Tarefas foi atribuído primeiro ou é o designado principal. (Por exemplo, se a tarefa tiver predecessoras, elas serão concluídas.)
* Um usuário e um Colaborador de Tarefas são atribuídos a uma tarefa e o usuário é removido.
* Um usuário e um Colaborador de Tarefas são atribuídos a uma tarefa, e o Colaborador de Tarefas é definido como o Principal Designado para a tarefa.

As seguintes situações não fazem com que o Colaborador de Tarefas comece a trabalhar na tarefa:

* Um Colaborador de Tarefas é atribuído a uma tarefa que já tem um usuário atribuído.
* Um Colaborador de Tarefas é @mentioned em uma tarefa.
* Um Colaborador de Tarefas é atribuído a uma tarefa que já tem um Colaborador de Tarefas atribuído. Nesse caso, o primeiro Colaborador de Tarefas atribuído já terá iniciado o trabalho, e o segundo Colaborador de Tarefas não fará nada.
* Um Colaborador de Tarefas é atribuído a uma tarefa que não está pronta para ser iniciada. (Por exemplo, se a tarefa tiver predecessoras, elas ainda não estarão concluídas.)

## Atribuir um Colaborador de Tarefas a uma tarefa

Os Colaboradores de Tarefas são atribuídos às tarefas da mesma forma que os usuários são atribuídos.

Quando você está procurando por um Colaborador de Tarefas na lista de designados disponíveis, o nome do Colaborador de Tarefas é apenas o nome.

Para obter instruções, consulte [Atribuir tarefas](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md).

>[!NOTE]
>
>Colaboradores de Tarefas não podem ser atribuídos para revisar ou aprovar um documento.

## Colaboradores de tarefas de solução de problemas

Se o Colaborador de Tarefas não retornar uma resposta ou saída, verifique o seguinte:

* Certifique-se de que seu agente esteja publicado no lado do provedor da plataforma de IA.
* Verifique se você tem créditos de IA suficientes na plataforma do seu agente.
* Certifique-se de que a ação executada na tarefa não exija um nível de acesso específico.
* Se você estiver usando o Copilot como provedor do agente, verifique se está usando a configuração &quot;sem autenticação&quot;.
* Se você estiver usando o Copilot, certifique-se de que seu agente esteja configurado em um ambiente global. Atualmente, a funcionalidade do Colaborador de Tarefas não oferece suporte a versões regionais do Copilot Studio.
* Certifique-se de que o Colaborador seja o principal responsável na tarefa.
* Verifique se a tarefa à qual o Colaborador de Tarefas está atribuído Pode Iniciar. Por exemplo, verifique se todas as tarefas predecessoras estão concluídas.

>[!TIP]
>
>Você também pode acessar a plataforma do provedor do agente e solicitar que o agente execute a tarefa na plataforma. Se o agente não puder executar a tarefa na plataforma, o Colaborador de tarefas também terá problemas no Workfront.
