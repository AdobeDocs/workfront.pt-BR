---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Usar o servidor MCP do Adobe Workfront
description: Use o servidor MCP do Adobe Workfront para pesquisar, criar, atualizar e gerenciar itens do Workfront por meio de conversas em linguagem natural em uma plataforma de agente de IA.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 152486b7850e01f3de23f22bbe3729c5cd3d3aa2
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 0%

---


# Usar o servidor MCP do Adobe Workfront

O servidor MCP [!DNL Adobe Workfront] permite localizar, criar, atualizar e gerenciar itens do Workfront solicitando uma plataforma de agente de IA em inglês simples. A plataforma decide quais ações do Workfront chamar e lida com a conversa com o Workfront para você.

[!DNL Claude] é a única plataforma de agente de IA com suporte no momento, mas os exemplos e padrões neste artigo se aplicam a qualquer plataforma de agente de IA com suporte para o servidor MCP do Workfront.

Este artigo supõe que você já configurou a conexão. Para obter informações sobre a instalação, consulte [Configurar o servidor MCP do Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md). Para obter mais informações sobre o servidor Workfront MCP, consulte [Visão geral do servidor Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md).

## Ferramentas disponíveis

O servidor MCP do Workfront expõe um conjunto de ferramentas que a plataforma de agente de IA chama em seu nome — por exemplo, ferramentas para pesquisar no Workfront, criar itens, atualizar campos e gerenciar aprovações. Para obter a lista de referência completa, agrupada por área do Workfront, consulte [Ferramentas de servidor MCP do Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md).

>[!IMPORTANT]
>
>Quando você conecta uma plataforma de agente de IA à Workfront, ela age no Workfront usando sua conta e as permissões da Workfront. As ações da plataforma têm o mesmo efeito que as ações executadas diretamente na interface do Workfront.
>
>Você e seu provedor de plataforma de agente de IA são responsáveis pelas ações que a plataforma realiza no Workfront. A Adobe não se responsabiliza pelas alterações que a plataforma de IA Agent faz nos dados do Workfront.
>
>Antes de permitir que a plataforma de agente de IA continue com uma solicitação, confirme se você entende o que ela pretende fazer, especialmente para ações que alteram ou excluem dados.


## Exemplos do que perguntar

Depois de se conectar, digite solicitações em linguagem natural na plataforma do agente de IA. A plataforma de agente de IA decide quais ações do Workfront serão chamadas e retorna os resultados.

### Localize e exiba seu trabalho

Para pesquisar no Workfront itens que correspondam ao que você está procurando, pergunte:

* *Mostre-me todos os projetos ativos para a equipe de Marketing da Marca.*
* *Receba todas as tarefas atribuídas a Joan Harris.*
* *Mostre-me todos os problemas no projeto &quot;Redesign de Site&quot; na categoria &quot;Técnico&quot;.*

### Criar novos itens

Para criar projetos, tarefas ou outros itens do Workfront, pergunte:

* *Crie um projeto em branco chamado &quot;Q2 Innovation Sandbox&quot; entre 10 de março e 30 de abril. Defina-me como proprietário.*
* *Adicione uma nova tarefa chamada &quot;Controle de qualidade da página de aterrissagem&quot; ao projeto e agende-a de 22 a 26 de abril.*
* *Crie um novo registro de campanha chamado &quot;Vendas de Verão de 2026&quot;.*

### Atualizar itens existentes

Para fazer alterações em itens já no Workfront, pergunte:

* *Atualize a tarefa &quot;Revisão de Design&quot; para que ela termine em 18 de abril e atribua-a à equipe criativa.*
* *Para o projeto &quot;Lucent AI Launch - NA&quot;, leve o final para meados de abril e aumente o orçamento para US$ 150.000.*
* *Atualize o campo de orçamento no registro &quot;Campanha de Verão&quot; para $75.000.*

### Excluir itens

Para remover itens do Workfront, pergunte:

* *Exclua o projeto chamado &quot;Campanha de Teste Q1&quot;.*
* *Remova a tarefa &quot;Produção de Ativo de Impressão&quot; do projeto.*
* *Exclua o registro de campanha chamado &quot;Promoção Antiga&quot;.*

>[!WARNING]
>
>Excluir itens no Workfront por meio de uma plataforma de agente de IA é o mesmo que excluí-los na interface do Workfront. Confirme o que a plataforma de agente de IA está prestes a excluir antes de permitir que continue.

### Trabalhar com aprovações

Para gerenciar aprovações de documentos e ativos, peça:

* *Adicione Sarah Chen e Miguel Alvarez como aprovadores no documento atual.*
* *Envie um lembrete para os aprovadores do ativo &quot;Vídeo da Campanha da primavera&quot; que não responderam.*
* *Aplique o modelo de aprovação &quot;Inicialização de marketing&quot; ao ativo &quot;Vídeo da campanha da primavera&quot;.*


### Trabalhar com registros do Planning

Para gerenciar registros de planejamento, pergunte:

* *Crie um novo registro de planejamento chamado &quot;Plano de marketing do segundo trimestre&quot; para a equipe de marketing da marca.*
* *Adicione uma nova tarefa chamada &quot;Auditoria de Mídia Social&quot; ao registro de planejamento.*
* *Atualize a tarefa &quot;Auditoria de mídia social&quot; para que seja concluída em 18 de abril e atribua-a à equipe criativa.*

### Trabalhar com fluxo de trabalho

Para gerenciar o workflow, pergunte:

* *Encaminhar o projeto &quot;Q2 Innovation Sandbox&quot; para o Painel de Revisão de Inovação.*
* *Atualize o registro da &quot;Campanha de Verão&quot; para o status &quot;Pronto para Iniciar&quot;.*
* *Aprove o registro da &quot;Campanha de Verão&quot;.*


### Solicitações de encadeamento em uma conversa

Você pode encadear solicitações em uma única conversa. A plataforma de agente de IA mantém o contexto, para que cada solicitação possa se basear na anterior. Por exemplo:

1. Solicitar um conjunto de itens: *Localizar minhas tarefas vencidas.*
1. Depois de obter a lista, peça uma ação sobre os resultados: *Atualize todos eles para a próxima sexta-feira.*

<!-- NEEDS DETAIL: Test multi-step prompt chaining in a working setup and document the patterns that produce reliable results. -->

## Considerações

Lembre-se das considerações a seguir ao usar o servidor MCP do Workfront.

### A plataforma de agente de IA pode usar informações de versões anteriores da conversa

Às vezes, as plataformas de agentes de IA reutilizam dados do início em uma conversa, em vez de solicitar as atualizações mais recentes da Workfront. Se algo mudou no Workfront desde a última pesquisa da plataforma de agente de IA, você pode ver informações desatualizadas.

Para forçar a plataforma de agente de IA a buscar dados novos, solicite-os explicitamente. Por exemplo:

* *Obtenha os dados mais recentes do Workfront. Não usar resultados em cache.*

### O servidor Workfront MCP é atualizado automaticamente

Quando o Adobe lança uma nova versão do servidor MCP do Workfront, sua plataforma de agente de IA usa a nova versão automaticamente. Você não precisa reconectar ou alterar nada em seu lado.

## Dados e segurança

<!-- NEEDS DETAIL: Document Adobe's official position on data handling and security when Workfront data is passed through an AI agentic platform. Cover: what data leaves Workfront, where it goes, whether it is retained or used for training by the AI agentic platform provider, what happens to it after the conversation ends, and any differences between AI agentic platforms (for example, Anthropic's enterprise data handling policies for Claude). This section needs sign-off from security and legal before publication. -->

### Quais dados saem do Workfront

<!-- NEEDS DETAIL: List the categories of Workfront data that can be sent to the AI agentic platform (item names, field values, attachments, user identifiers, etc.) and any data that the MCP server explicitly does not expose. -->

### Como os provedores da plataforma de IA Agentic lidam com os dados do Workfront

<!-- NEEDS DETAIL: For each supported AI agentic platform, summarize the provider's data handling stance: retention, training opt-out, and enterprise vs. consumer differences. Link to the provider's official documentation. Start with Claude (Anthropic). -->

### Diferenças entre plataformas de agentes de IA

<!-- NEEDS DETAIL: Note any meaningful differences in how each supported AI agentic platform handles Workfront data once additional AI agentic platforms are supported. -->

## Solução de problemas de uso diário

+++ Expanda para exibir dicas de solução de problemas para o uso diário do servidor MCP do Workfront.

| Problema | Causa provável | Corrigir |
|---|---|---|
| A plataforma de agente de IA está fornecendo informações desatualizadas. | A plataforma de agente de IA está reutilizando dados do início da conversa. | Solicite dados novos do Workfront. |
| A plataforma de agente de IA retornou dados dos itens incorretos do Workfront. | A plataforma de agente de IA escolheu os itens errados com base em termos ambíguos. | Pergunte novamente com nomes, IDs ou filtros mais específicos. |
| Uma atualização ou exclusão não entrou em vigor no Workfront. | A plataforma de agente de IA ainda não chamou a ação ou suas permissões não permitem essa ação. | Confirme com a plataforma do agente de IA se a ação foi executada e verifique suas permissões do Workfront. |

Para obter mais informações sobre problemas de instalação e autenticação, consulte [Solução de problemas de instalação e autenticação](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication) em [Configurar o servidor MCP do Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

+++

## Perguntas frequentes

+++ Expanda para exibir as perguntas frequentes sobre o uso do servidor MCP do Workfront.

### Com quais itens do Workfront posso trabalhar por meio de uma plataforma de agente de IA?

Todos os itens aos quais você tem acesso no Workfront por meio de níveis de acesso e permissões de objeto.

<!-- NEEDS DETAIL: List the supported Workfront object types. -->

### Meus dados do Workfront são enviados ao provedor de plataforma do agente de IA ou armazenados por ele?

Para obter mais informações, consulte [Dados e segurança](#data-and-security) neste artigo.

### O que acontece quando uma nova versão do servidor MCP do Workfront é lançada?

O servidor MCP é atualizado automaticamente. Você não precisa reconectar ou alterar nada.

### Preciso saber a API do Workfront para usar o servidor MCP do Workfront?

Não. A plataforma de agente de IA traduz suas solicitações em linguagem natural para as ações certas do Workfront. Se você já estiver familiarizado com a API do Workfront, as ações serão familiares, mas não é um requisito.

+++
