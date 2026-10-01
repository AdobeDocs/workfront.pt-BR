---
user-type: administrator
product-area: system-administration;setup
navigation-upperic: configure-locations
title: Configurar colaboradores de IA
description: Como administrador do Adobe Workfront, você pode configurar os Colaboradores de IA e atribuí-los a projetos e tarefas.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c38801ee-9750-4ffb-a912-cdcccfc7c60a
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 3cf7495f827156fabac1214b38a104ed826d558c
workflow-type: tm+mt
source-wordcount: '1577'
ht-degree: 2%
---
# Configurar colaboradores de IA

{{preview-fast-release-general}}

Os Colaboradores de IA são uma maneira de integrar agentes de IA em seus projetos, tarefas e problemas. Você pode configurar um Colaborador de IA e atribuí-lo como faria com um usuário.

Por exemplo, você pode configurar um Colaborador de IA do tipo revisor com diretrizes da marca e, em seguida, atribuir esse colaborador para revisar um documento.

Os tipos disponíveis do AI Collaborator incluem:

* Revisor da IA: crie um colaborador usando marcas ou Adobe Brand Intelligence e, em seguida, atribua o colaborador como um revisor nos ativos.

  Para obter mais informações, consulte [Introdução ao Workfront AI Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).

* Agente de trabalho: crie um colaborador usando uma plataforma de IA padrão, como Claude, OpenAI, Copilot ou Writer e, em seguida, atribua o colaborador a uma tarefa ou problema para concluir os itens de trabalho.

  Para obter mais informações, consulte [Usar Agentes de Trabalho](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).

<!--
* <span class="preview">Project Coordinator: An out-of-the-box collaborator that monitors project status and follows up on overdue tasks automatically, without needing to configure an external agent.</span>

   <span class="preview">For more information, see [Use the Project Coordinator collaborator](/help/quicksilver/manage-work/projects/manage-projects/use-project-coordinator.md).</span>
-->


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
   <td>[!UICONTROL Administrador do Sistema] <span class="preview">ou Administrador de Grupo</span></td> 
  </tr> 
  </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

* [Para Revisores de IA](#for-ai-reviewers)
* [Para agentes de trabalho](#for-work-agents)

### Para Revisores de IA:

* Sua organização deve ter um Contrato de IA de geração da Adobe assinado em arquivo.

  Para obter mais informações, consulte [Assinar o contrato da Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) no artigo Assistente de IA na Workfront.
* Você deve ter configurado uma marca no Workfront antes de usá-la para um Revisor de IA.

  Para obter instruções, consulte [Criar e gerenciar marcas para o Revisor da IA](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).
* Para usar o Adobe Brand Intelligence para um Revisor de IA, sua organização deve usar a experiência unificada de revisão e aprovação no Workfront.

  Para obter mais informações, consulte [Introdução à revisão e aprovação unificadas](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md).

### Para agentes de trabalho

Você deve configurar um agente no Claude, Copilot Studio, Writer, OpenAI ou IBM antes de usá-lo como um Agente de trabalho.

>[!NOTE]
>
>Nosso objetivo é conectar-se com qualquer provedor de agente; portanto, se o provedor que você está usando não for compatível com Agentes de trabalho, entre em contato com a equipe de conta para obter assistência.

## Criar um novo Revisor de IA

Os Revisores de IA podem ser configurados para usar marcas da Workfront ou Adobe Brand Intelligence.

* **Marcas**: as marcas são criadas no Workfront. Você pode criar marcas no Workfront fazendo upload de arquivos PDF que contêm as diretrizes da marca ou inserindo manualmente os elementos da marca.
* **Adobe Brand Intelligence**: quando um Colaborador de IA revisa um ativo usando o Adobe Brand Intelligence, você pode exibir comentários feitos pelo Revisor de IA no Frame.io.


{{step-1-to-setup}}

1. Na navegação à esquerda, clique em **Colaboradores de IA**.
1. Clique em **Novo Colaborador** no canto superior direito da tela.
1. Clique em **Revisor** e em **Continuar**.
1. No campo Nome do Colaborador, informe um nome para o colaborador. Esse é o nome que aparece na lista de responsáveis disponíveis em uma tarefa.
1. Selecione se o colaborador usará uma marca ou Adobe Brand Intelligence para suas análises.
1. (Condicional) Se o Colaborador de IA usar uma Marca, selecione a marca e a diretriz da marca que ele usará.
1. Clique em **Salvar**.

## Configurar um agente de trabalho

Agentes de trabalho são agentes que podem ser atribuídos a tarefas ou problemas no Workfront. Você configura o Agente de trabalho com um nome, nível de acesso e outros detalhes e o atribui a uma tarefa da mesma forma que atribuiria a um usuário.

Como os Agentes de trabalho são agentes, suas ações e habilidades são configuradas onde você configura os agentes. Atualmente, os agentes usados como Agentes de trabalho podem ser criados no Copilot Studio, Claude ou Writer, OpenAI e IBM.

Os agentes de trabalho podem ser atribuídos a tarefas ou problemas.

Para obter uma lista de práticas recomendadas ao criar um agente para trabalhar como Agente de Trabalho, consulte [Práticas recomendadas para criar um agente para um Agente de Trabalho](#best-practices-for-creating-an-agent-for-a-work-agent).

* [Configurar um agente de trabalho no Workfront](#configure-a-work-agent-in-workfront)
* [Práticas recomendadas para criar um agente para um Agente de trabalho](#best-practices-for-creating-an-agent-for-a-work-agent)

### Configurar um agente de trabalho no Workfront

{{step-1-to-setup}}

1. Na navegação à esquerda, clique em **Colaboradores de IA**.
1. Clique em **Novo Colaborador** no canto superior direito da tela.
1. Selecione **Agentes de trabalho** e clique em **Continuar**.
1. No campo Nome do Colaborador de IA, digite um nome para o colaborador. Esse é o nome que aparece na lista de responsáveis disponíveis em uma tarefa.
1. No campo Descrição do Colaborador de IA, informe uma descrição da finalidade do colaborador ou das ações que ele executa.
1. No campo Nível de Acesso, selecione um nível de acesso para este colaborador. Esse nível de acesso controla o que o colaborador pode fazer, da mesma forma que um nível de acesso controla o que um usuário pode fazer.
1. (Opcional) No campo Grupos, selecione os grupos aos quais o Agente de trabalho será associado.

   >[!NOTE]
   >
   ><span class="preview">Se você for um administrador de grupo, este campo exibirá somente os grupos para os quais é um administrador. Os administradores de grupo devem selecionar pelo menos um grupo.</span>

1. Na área **Escolher origem do agente**, selecione se deseja conectar um agente criado em uma plataforma comum, como Copilot ou Writer, ou usar um agente personalizado.
1. (Condicional) Se você estiver usando um agente de uma plataforma comum, insira os detalhes de autenticação da plataforma do agente:

   | Plataforma | Autenticação necessária |
   |---|---|
   | Copilot Studio | Segredo do canal da web |
   | Agentes gerenciados do Claude | Chave da API antropica<br>ID do agente<br>ID do ambiente |
   | Agente Gravador | Chave de API<br>ID do Aplicativo |
   | <span class="preview">Agentes OpenAI</span> | <span class="preview">Chave da API <br>ID do Agente</span> |
   | <span class="preview">Orquestração watsonx da IBM</span> | <span class="preview">URL do Serviço<br>Chave da API<br> ID do Agente</span> |

1. Clique em **Testar conexão**. Isso permite saber se a conexão foi configurada corretamente.
1. No **Depois que o Colaborador terminar o trabalho, ele poderá** alternar a área e as ações que você deseja que o colaborador execute.

   * <span class="preview">Enviar notificação: o Agente faz um comentário no fluxo de atualização, marcando o usuário que solicitou o trabalho, atribuiu o Agente ou que é proprietário do projeto. </span>
   * <span class="preview">Carregar um documento</span>
   * <span class="preview">Marcar tarefa como concluída</span>
   * Gravar campos de tarefa: selecione os formulários e campos nos quais o Agente pode gravar.

1. Clique em **Salvar**.

Para obter mais informações sobre Agentes de Trabalho, incluindo como atribuí-los a tarefas, consulte [Usar Agentes de Trabalho](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).

### Práticas recomendadas para criar um agente para um Agente de trabalho

As práticas recomendadas a seguir podem ser úteis ao criar um agente para usar como um Agente de trabalho no Workfront. Para ver as práticas recomendadas, clique na seção do aplicativo em que você está criando o agente.

+++ Claude

1. Navegue até o Claude Console em [platform.claude.com](https://platform.claude.com/).
1. Crie uma chave de API.
   1. Em Chaves de API, clique em **Criar chave** no canto superior direito.
   1. Forneça um nome e uma data de expiração.
   1. Copie a chave e salve-a em um local seguro. Você precisará dessa chave para configurar o Agente de trabalho no Workfront.

1. Criar um ambiente.
   1. Em **Agentes gerenciados** > **Ambientes**, clique em **Criar ambiente** no canto superior direito.
   1. Forneça um nome e tipo de hospedagem conforme aplicável.
   1. Configure pacotes compartilhados e metadados conforme necessário. Os ambientes podem ser reutilizados em vários agentes e permitem pacotes e metadados compartilhados.
      A ID de ambiente aparece abaixo do nome do ambiente no canto superior esquerdo.

1. Crie um agente.
   1. Em Agentes gerenciados > Agentes, clique em **Criar agente** no canto superior direito.
   1. Forneça nome, modelo, prompt do sistema, habilidades e ferramentas, conforme aplicável. Seja descritivo, pois os Agentes de trabalho passam o contexto da tarefa para esse agente, que então executa o trabalho.
      A ID do agente aparece abaixo do nome do agente no canto superior esquerdo.

1. Configure o Agente de trabalho no Workfront.
   1. Insira sua chave de API, ID do ambiente e ID do agente
   1. Clique em **Testar Conexão** para verificar.

1. Atribua o Agente de trabalho a uma tarefa do Workfront.
   1. O agente de trabalho é acionado depois que todas as tarefas predecessoras são concluídas.

+++
<!--
+++ Copilot Studio



+++
-->
+++ Gravador

>[!NOTE]
>
> Você pode usar um agente Escritor como um Agente de trabalho, mas os manuais do Escritor não podem ser usados como Agentes de trabalho.

Ao criar um agente para usar como um Agente de trabalho no Writer, recomendamos o seguinte fluxo de trabalho.

Informações mais detalhadas sobre a criação de agentes podem ser encontradas na [Documentação do autor](https://dev.writer.com/no-code/introduction).

1. Crie um aplicativo sem código no Writer AI Studio.
1. Adicione um único campo de entrada Text. Você pode usar o nome padrão &quot;Entrada de texto&quot;.
1. Adicione `@TextInput` ao seu prompt. Na seção Prompts da configuração do aplicativo, verifique se o modelo de prompt faz referência à variável de entrada. Sem isso, o modelo nunca vê os dados da tarefa.
1. Ajuste o Prompt para gerar a saída imediatamente. Remova quaisquer instruções que solicitem esclarecimentos ou contexto adicional ao usuário antes de responder. Por exemplo: &quot;Ao receber entrada, trate-a como uma solicitação de geração de conteúdo e produza a saída imediatamente. Não peça esclarecimentos.&quot;
1. Copie a chave da API e a ID do aplicativo. Você precisará deles para configurar o Agente de trabalho no Workfront.

   * Para obter instruções sobre como configurar uma chave de API no Writer, consulte [Quickstart](https://dev.writer.com/home/quickstart) na documentação do Writer.
   * Para obter instruções sobre como configurar uma ID de aplicativo no Writer, consulte [Invocar agentes sem código por meio da API](https://dev.writer.com/home/applications) na documentação do Writer.

1. Configure o Agente de trabalho no Workfront. Como parte da configuração, insira sua chave de API e ID do Aplicativo, depois clique em **Testar conexão** para verificar.
1. Atribua o Agente de trabalho a uma tarefa do Workfront. O Agente de Trabalho inicia o trabalho quando todas as tarefas predecessoras da tarefa são concluídas.

+++

<div class="preview">

<!--
## Configure a Project Coordinator

The Project Coordinator is an out-of-the-box collaborator that monitors project status and helps keep work on track. Unlike Work Agents, the Project Coordinator does not require you to configure an external agent.

{{step-1-to-setup}}

1. In the left navigation, click **AI Collaborators**.
1. Click **New Collaborator** in the upper-right corner of the screen.
1. Select **Project Coordinator**.
1. In the **AI Collaborator name** field, enter a name for the Project Coordinator. This is the name that appears as the collaborator in your project.
1. In the **AI Collaborator description** field, enter a description of what the Project Coordinator does or its purpose.
1. In the **Access level** field, select an access level for the Project Coordinator. This access level controls what the collaborator can do on projects.
1. (Optional) In the **Send project updates** section, toggle **Allow** to enable project update notifications, then specify update details.
   * In the **Cadence** field, select whether the Coordinator sends updates daily or weekly.
   * If the Coordinator sends updates weekly, in the **Day of week** field, select the day of the week that updates are sent.
   * In the **Time (MST)** field, select the time to send updates.
   * In the **How to send** field, select whether the Coordinator sends updates as an update on the project, or as an email
   * In the **Who gets the update** field, select whether the update is sent only to the project owner, or to all project stakeholders.
   * (Optional) Check **Send additional update immediately when coordinator is assigned** to notify on assignment.
   * (Optional) Check **Send additional update when a date is missed** to send notifications when dates are missed.
1. (Optional) In the **Notify task assignees** section, toggle **Allow** to enable task notifications, then check the boxes for the situations that you want to notify assignees about.
1. (Optional) In the **Remind reviewers and approvers** section, toggle **Allow** to enable reminders for reviewers, then check the boxes for the situations that you want to remind reviewers and approvers about.
1. (Optional) In the **Update the content of project and task fields** section, toggle **Allow** to enable the coordinator to update project and task field values.
1. Click **Save**.

For more information on the Project Coordinator, including how to assign it to projects, see [Use the Project Coordinator collaborator](/help/quicksilver/manage-work/projects/manage-projects/use-project-coordinator.md).
-->

</div>

## Gerenciar colaboradores de IA

Você pode editar, copiar e excluir os colaboradores de IA existentes.

>[!NOTE]
>
><span class="preview">Os administradores de grupo podem exibir e interagir somente com os Colaboradores de IA associados aos grupos para os quais são administradores. Se outros grupos também estiverem associados a um determinado Colaborador de IA, um administrador de grupo poderá exibi-lo, mas não editá-lo.</span>

{{step-1-to-setup}}

1. Na navegação à esquerda, clique em **Colaboradores de IA**.
1. (Condicional) Para editar um Collaborator, clique no nome do Collaborator que deseja editar, faça qualquer edição na janela Editar Collaborator e clique em **Salvar**.
1. (Condicional) Para excluir um Colaborador, clique no ícone Excluir ![ícone Excluir](assets/delete-collaborator-icon.png) na linha do Colaborador de IA que você deseja excluir e clique em **Excluir**.
