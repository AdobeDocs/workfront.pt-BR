---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Usar o servidor MCP do Adobe Workfront
description: Use o servidor MCP do Adobe Workfront para pesquisar, criar, atualizar e gerenciar itens do Workfront por meio de conversas em linguagem natural em um assistente de IA.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 4517d45ecc653d27d435a8192a612241120dd33f
workflow-type: tm+mt
source-wordcount: '1243'
ht-degree: 2%

---


# Usar o servidor MCP do Adobe Workfront

O servidor MCP [!DNL Adobe Workfront] permite localizar, criar, atualizar e gerenciar itens do Workfront solicitando um assistente de IA em inglês simples. O assistente de IA decide quais ações do Workfront chamar e lida com a conversa com o Workfront para você.

No momento, [!DNL Claude] é o único assistente de IA com suporte, mas os exemplos e padrões neste artigo se aplicam a qualquer assistente de IA que ofereça suporte ao servidor MCP do Workfront.

Este artigo supõe que você já configurou a conexão. Para obter informações sobre a instalação, consulte [Configurar o servidor MCP do Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md). Para obter mais informações sobre o servidor Workfront MCP, consulte [Visão geral do servidor Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md).



## Ações disponíveis por meio do servidor MCP do Workfront

O servidor MCP do Workfront abrange ações em aprovações, planejamento e fluxo de trabalho.

<!-- NEEDS DETAIL: Confirm the full inventory of actions exposed through the Workfront MCP server. The five core actions below are confirmed from Hamilton's walkthrough. The approvals, planning, and workflow sections need to be filled in from Jeff's engineering channel post, hands-on access, and the deck Oznur published in the MCP external channel. -->

>[!IMPORTANT]
>
>Um assistente de IA atua no Workfront usando sua conta e permissões do Workfront. Você e o seu provedor de assistente de IA são responsáveis pelas ações que o assistente de IA toma em seu nome. Confirme o que o assistente de IA está prestes a fazer antes de permitir que continue.


## Responsabilidade pelas ações do assistente de IA

Quando você conecta um assistente de IA ao Workfront, ele atua no Workfront usando sua conta e permissões do Workfront. As ações do assistente de IA têm o mesmo efeito que as ações executadas diretamente na interface do Workfront.

Você e o seu provedor de assistente de IA são responsáveis pelas ações que o assistente de IA toma no Workfront. A Adobe não se responsabiliza pelas alterações que o assistente de IA faz nos dados do Workfront.

Antes de permitir que o assistente de IA continue com uma solicitação, confirme se você entende o que ele pretende fazer, especialmente para ações que alteram ou excluem dados.

### Ações principais

O servidor MCP do Workfront inclui as seguintes ações principais:

| Ação | O que faz |
|---|---|
| Criar | Cria novos itens no Workfront. |
| Pesquisar | Localiza e recupera itens do Workfront. |
| Atualização | Altera itens existentes no Workfront. |
| Excluir | Remove itens do Workfront. |
| Resolver nomes de campo | Pesquisa os nomes de campo corretos do Workfront para que o assistente de IA possa criar solicitações precisas com base em seus dados. |

<!-- NEEDS DETAIL: Confirm which Workfront object types are supported across the core actions (projects, tasks, issues, portfolios, programs, custom forms, planning records, approvals, etc.). -->

### Ações de aprovações

<!-- NEEDS DETAIL: List the approval-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request a marketer might make. -->

### Ações de planejamento

<!-- NEEDS DETAIL: List the planning-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request. -->

### Ações de fluxo de trabalho

<!-- NEEDS DETAIL: List the workflow-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request. -->

## Exemplos do que perguntar

Depois de se conectar, digite solicitações em linguagem natural no assistente do AI. O assistente de IA decide quais ações do Workfront são chamadas e retorna os resultados.

<!-- NEEDS DETAIL: Example prompts in this section are adapted from the Workflow Optimization Agent (WOA) examples doc on another branch. Validate each example against a working Claude + Workfront MCP server setup before publication, since WOA and the MCP server may expose different action inventories. -->

### Localize e exiba seu trabalho

Peça ao assistente de IA para pesquisar no Workfront por itens que correspondam ao que você está procurando. Por exemplo:

* *Mostre-me todos os projetos ativos para a equipe de Marketing da Marca.*
* *Receba todas as tarefas atribuídas a Joan Harris.*
* *Mostre-me todos os problemas no projeto &quot;Redesign de Site&quot; na categoria &quot;Técnico&quot;.*

### Criar novos itens

Peça ao assistente de IA para criar projetos, tarefas ou outros itens do Workfront. Por exemplo:

* *Crie um projeto em branco chamado &quot;Q2 Innovation Sandbox&quot; entre 10 de março e 30 de abril. Defina-me como proprietário.*
* *Adicione uma nova tarefa chamada &quot;Controle de qualidade da página de aterrissagem&quot; ao projeto e agende-a de 22 a 26 de abril.*
* *Crie um novo registro de campanha chamado &quot;Vendas de Verão de 2026&quot;.*

### Atualizar itens existentes

Peça ao assistente de IA para fazer alterações em itens já existentes no Workfront. Por exemplo:

* *Atualize a tarefa &quot;Revisão de Design&quot; para que ela termine em 18 de abril e atribua-a à equipe criativa.*
* *Para o projeto &quot;Lucent AI Launch - NA&quot;, leve o final para meados de abril e aumente o orçamento para US$ 150.000.*
* *Atualize o campo de orçamento no registro &quot;Campanha de Verão&quot; para $75.000.*

### Excluir itens

Peça ao assistente de IA para remover itens do Workfront. Por exemplo:

* *Exclua o projeto chamado &quot;Campanha de Teste Q1&quot;.*
* *Remova a tarefa &quot;Produção de Ativo de Impressão&quot; do projeto.*
* *Exclua o registro de campanha chamado &quot;Promoção Antiga&quot;.*

>[!WARNING]
>
>Excluir itens no Workfront por meio de um assistente de IA é o mesmo que excluí-los na interface do Workfront. Confirme o que o assistente de IA está prestes a excluir antes de permitir que ele continue.

### Trabalhar com aprovações

Solicite ao assistente de IA que gerencie aprovações de documentos e ativos. Por exemplo:

* *Adicione Sarah Chen e Miguel Alvarez como aprovadores no documento atual.*
* *Envie um lembrete para os aprovadores do ativo &quot;Vídeo da Campanha da primavera&quot; que não responderam.*
* *Aplique o modelo de aprovação &quot;Inicialização de marketing&quot; ao ativo &quot;Vídeo da campanha da primavera&quot;.*

<!-- NEEDS DETAIL: Add approvals-specific context from the WOA examples doc, including: content approvals must be enabled for the organization, the AI assistant cannot approve or reject on behalf of humans (except via the Workfront AI Reviewer), and best experience is with the Unified Approvals experience. -->

### Trabalhar com registros do Planning

Peça ao assistente de IA para gerenciar registros de planejamento. Por exemplo:

* *Crie um novo registro de planejamento chamado &quot;Plano de marketing do segundo trimestre&quot; para a equipe de marketing da marca.*
* *Adicione uma nova tarefa chamada &quot;Auditoria de Mídia Social&quot; ao registro de planejamento.*
* *Atualize a tarefa &quot;Auditoria de mídia social&quot; para que seja concluída em 18 de abril e atribua-a à equipe criativa.*

### Trabalhar com fluxo de trabalho

Peça ao assistente de IA para gerenciar o fluxo de trabalho. Por exemplo:

* *Encaminhar o projeto &quot;Q2 Innovation Sandbox&quot; para o Painel de Revisão de Inovação.*
* *Atualize o registro da &quot;Campanha de Verão&quot; para o status &quot;Pronto para Iniciar&quot;.*
* *Aprove o registro da &quot;Campanha de Verão&quot;.*


### Solicitações de encadeamento em uma conversa

Você pode encadear solicitações em uma única conversa. O assistente de IA mantém o contexto, para que cada solicitação possa se basear na anterior. Por exemplo:

1. Peça ao assistente de IA para encontrar um conjunto de itens: *Localizar minhas tarefas vencidas.*
1. Depois que o assistente de IA retornar a lista, peça para ele agir de acordo com os resultados: *Atualize todos eles para a próxima sexta-feira.*

<!-- NEEDS DETAIL: Test multi-step prompt chaining in a working setup and document the patterns that produce reliable results. -->

## Considerações

Lembre-se das considerações a seguir ao usar o servidor MCP do Workfront.

### O assistente de IA pode usar informações do início da conversa

Às vezes, os assistentes de IA reutilizam dados do início de uma conversa, em vez de solicitar as atualizações mais recentes da Workfront. Se algo mudou no Workfront desde a última pesquisa do assistente de IA, você pode ver informações desatualizadas.

Para forçar o assistente de IA a buscar dados novos, solicite-os explicitamente. Por exemplo:

* *Obtenha os dados mais recentes do Workfront. Não usar resultados em cache.*

### O servidor Workfront MCP é atualizado automaticamente

Quando o Adobe lança uma nova versão do servidor MCP do Workfront, o assistente de IA usa a nova versão automaticamente. Você não precisa reconectar ou alterar nada em seu lado.

## Dados e segurança

<!-- NEEDS DETAIL: Document Adobe's official position on data handling and security when Workfront data is passed through an AI assistant. Cover: what data leaves Workfront, where it goes, whether it is retained or used for training by the AI assistant provider, what happens to it after the conversation ends, and any differences between AI assistants (for example, Anthropic's enterprise data handling policies for Claude). This section needs sign-off from security and legal before publication. -->

### Quais dados saem do Workfront

<!-- NEEDS DETAIL: List the categories of Workfront data that can be sent to the AI assistant (item names, field values, attachments, user identifiers, etc.) and any data that the MCP server explicitly does not expose. -->

### Como os provedores do assistente de IA lidam com os dados do Workfront

<!-- NEEDS DETAIL: For each supported AI assistant, summarize the provider's data handling stance: retention, training opt-out, and enterprise vs. consumer differences. Link to the provider's official documentation. Start with Claude (Anthropic). -->

### Diferenças entre os assistentes de IA

<!-- NEEDS DETAIL: Note any meaningful differences in how each supported AI assistant handles Workfront data once additional AI assistants are supported. -->

## Solução de problemas de uso diário

Para obter mais informações sobre problemas de instalação e autenticação, consulte [Solução de problemas de instalação e autenticação](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication) em [Configurar o servidor MCP do Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

| Problema | Causa provável | Corrigir |
|---|---|---|
| O assistente de IA está fornecendo informações desatualizadas. | O assistente de IA está reutilizando dados do início da conversa. | Solicite ao assistente de IA que busque dados novos do Workfront. |
| O assistente de IA retornou dados de itens incorretos do Workfront. | O assistente de IA escolheu os itens errados com base em termos ambíguos. | Pergunte novamente com nomes, IDs ou filtros mais específicos. |
| Uma atualização ou exclusão não entrou em vigor no Workfront. | O assistente de IA ainda não chamou a ação ou suas permissões não permitem essa ação. | Confirme com o assistente de IA se a ação foi executada e verifique suas permissões do Workfront. |

<!-- NEEDS DETAIL: Add additional day-to-day troubleshooting scenarios discovered during hands-on testing. -->

## Perguntas frequentes

### Com quais itens do Workfront posso trabalhar com um assistente de IA?

Todos os itens aos quais você tem acesso no Workfront por meio de níveis de acesso e permissões de objeto.

<!-- NEEDS DETAIL: List the supported Workfront object types. -->

### Meus dados do Workfront são enviados ao provedor do assistente de IA ou armazenados por ele?

Para obter mais informações, consulte [Dados e segurança](#data-and-security) neste artigo.

### O que acontece quando uma nova versão do servidor MCP do Workfront é lançada?

O servidor MCP é atualizado automaticamente. Você não precisa reconectar ou alterar nada.

### Preciso saber a API do Workfront para usar o servidor MCP do Workfront?

Não. O assistente de IA traduz suas solicitações em linguagem natural para as ações certas do Workfront. Se você já estiver familiarizado com a API do Workfront, as ações serão familiares, mas não é um requisito.
