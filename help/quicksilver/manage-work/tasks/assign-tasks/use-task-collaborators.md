---
title: Usar agentes de trabalho
content-type: reference
description: Saiba como usar agentes de trabalho, colaboradores de IA que podem ser atribuídos a tarefas do Workfront.
author: Becky
feature: Work Management, Tasks
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
    internal-label: Tasks
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: bc354886dc8c2f1dae24513f1d74e800e19fb3ab
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 2%
---
# Usar agentes de trabalho

Os agentes de trabalho são colaboradores de IA que podem ser atribuídos diretamente às tarefas do Workfront, além do Revisor de IA existente usado para revisões de documentos e ativos. Como outros Colaboradores de IA, os Agentes de trabalho são configurados na área Configuração e atribuídos a tarefas como um usuário.

Os Agentes de trabalho conectam-se aos agentes configurados no Copilot Studio, Claude ou Writer.

Para obter informações e instruções sobre como criar um Agente de trabalho no Workfront, consulte [Configurar um Agente de Trabalho](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-work-agent) no artigo Configurar Colaboradores de IA.

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

* Você deve configurar um agente no Copilot, Claude ou Writer.ai antes de usá-lo como um Agente de trabalho.

## Visão geral do agente de trabalho

Os Agentes de trabalho são uma maneira de atribuir agentes MCP a tarefas específicas no Workfront. Você configura o agente em um aplicativo, como o Copilot Studio, o Claude ou o Writer.ai, e depois conecta esse agente ao Workfront como um Agente de trabalho. Em seguida, é possível atribuí-la a tarefas como atribuiria a um usuário.

Alguns exemplos de workflows podem incluir:

* Detectar imagens carregadas em uma tarefa, gerar variações com base nos critérios fornecidos ao agente e fazer upload das novas imagens na tarefa.
* Gerar cópia a partir de uma descrição da tarefa, revisar a cópia com base nas diretrizes configuradas no agente e postar a cópia no fluxo de atualização.
* Lendo detalhes de um evento, identificando detalhes ausentes e postando perguntas na sequência de atualização sobre os detalhes ausentes.

>[!NOTE]
>
>* Detalhes específicos sobre as responsabilidades e capacidades de um agente são configurados no aplicativo em que o agente é criado, não no Workfront.
>* O servidor MCP do Workfront não precisa ser adicionado ao agente usado como um Agente de trabalho e não precisa estar conectado para que o Agente de trabalho funcione.
>* Atualmente, os agentes de trabalho oferecem suporte aos agentes criados no Copilot Studio, Claude e Writer.ai.
>* Ao configurar um agente no Copilot Studio, defina a segurança como **Sem autenticação**.
>* Para obter informações e instruções sobre como criar um Agente de trabalho no Workfront, consulte [Configurar um Agente de Trabalho](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-work-agent) no artigo Configurar Colaboradores de IA.

## Informações lidas por um agente de trabalho

Quando um Agente de trabalho começa a trabalhar em uma tarefa, ele lê automaticamente as seguintes informações da tarefa como contexto:

* Título da tarefa
* Descrição da tarefa
* Comentários no fluxo de atualização da tarefa
* Informações em qualquer formulário personalizado anexado à tarefa

Essas informações são sempre lidas e não podem ser definidas como uma configuração do Workfront.

>[!TIP]
>
>Para obter melhores resultados, recomendamos:
>
>* Incluindo qualquer informação de fundo que você queira que o agente use diretamente na descrição da tarefa ou em um campo de formulário personalizado relevante.
>* Verificando se a tarefa corresponde ao que o agente está instruído a fazer. Por exemplo, se o agente for instruído a traduzir o texto do inglês para o francês, inclua o texto que deseja traduzir na descrição da tarefa.

## Acionadores de início do Agente de Trabalho

Quando um Agente de Trabalho é atribuído a uma tarefa, ele começa a trabalhar quando qualquer uma das seguintes situações é atendida:

* O Agente de Trabalho é atribuído a uma tarefa pronta para ser iniciada. (Por exemplo, se a tarefa tiver predecessoras, elas serão concluídas.)
* O Agente de trabalho e um usuário são atribuídos a uma tarefa, e o Agente de trabalho é atribuído primeiro.
* Uma tarefa para a qual um Agente de Trabalho já foi atribuído torna-se pronta para ser iniciada, e o Agente de Trabalho é o único designado ou principal. (Por exemplo, se a tarefa tiver predecessoras, elas serão concluídas.)
* Uma tarefa para a qual um Agente de trabalho e um usuário já estão atribuídos fica pronta para ser iniciada, e o Agente de trabalho foi atribuído primeiro ou é o designado principal. (Por exemplo, se a tarefa tiver predecessoras, elas serão concluídas.)
* Um usuário e um Agente de trabalho são atribuídos a uma tarefa e o usuário é removido.
* Um usuário e um Agente de trabalho são atribuídos a uma tarefa, e o Agente de trabalho é definido como o Principal Designado para a tarefa.

As seguintes situações não fazem com que o Agente de trabalho comece a trabalhar na tarefa:

* Um Agente de trabalho é atribuído a uma tarefa que já tem um usuário atribuído.
* Um Agente de Trabalho é @mentioned em uma tarefa.
* Um Agente de trabalho é atribuído a uma tarefa que já tem um Agente de trabalho atribuído. Nesse caso, o primeiro Agente de trabalho atribuído já terá iniciado o trabalho e o segundo Agente de trabalho não fará nada.
* Um Agente de Trabalho é atribuído a uma tarefa que não está pronta para ser iniciada. (Por exemplo, se a tarefa tiver predecessoras, elas ainda não estarão concluídas.)

## Atribuir um Agente de Trabalho a uma tarefa

Os agentes de trabalho são atribuídos às tarefas da mesma forma que os usuários são atribuídos.

Quando você está procurando um Agente de trabalho na lista de designados disponíveis, o nome do Agente de trabalho é apenas um nome.

Para obter instruções, consulte [Atribuir tarefas](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md).

>[!NOTE]
>
>Os agentes de trabalho não podem ser designados para revisar ou aprovar um documento.

## Agentes de trabalho de solução de problemas

Se o seu Agente de trabalho não retornar uma resposta ou saída, verifique o seguinte:

* Certifique-se de que seu agente esteja publicado no lado do provedor da plataforma de IA.
* Verifique se você tem créditos de IA suficientes na plataforma do seu agente.
* Certifique-se de que a ação executada na tarefa não exija um nível de acesso específico.
* Se você estiver usando o Copilot como provedor do agente, verifique se está usando a configuração &quot;sem autenticação&quot;.
* Se você estiver usando o Copilot, certifique-se de que seu agente esteja configurado em um ambiente global. No momento, a funcionalidade do Agente de Trabalho não é compatível com versões regionais do Copilot Studio.
* Certifique-se de que o Colaborador seja o principal responsável na tarefa.
* Verifique se a tarefa à qual o Agente de trabalho está atribuído Pode iniciar. Por exemplo, verifique se todas as tarefas predecessoras estão concluídas.

>[!TIP]
>
>Você também pode acessar a plataforma do provedor do agente e solicitar que o agente execute a tarefa na plataforma. Se o agente não puder executar a tarefa na plataforma, o Agente de trabalho também terá problemas no Workfront.
