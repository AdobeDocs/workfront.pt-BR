---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Usar o servidor MCP do Adobe Workfront
description: Use o servidor MCP do Adobe Workfront para pesquisar, criar, atualizar e gerenciar itens do Workfront por meio de conversas em linguagem natural em uma plataforma de agente de IA.
author: Courtney
feature: Get Started with Workfront
source-git-commit: f96afd17e9f4e726ac545a9cb0c54ace5a4fcffe
workflow-type: tm+mt
source-wordcount: '1642'
ht-degree: 0%

---


# Usar o servidor MCP do Adobe Workfront

{{highlighted-preview-article-level}}

O servidor MCP [!DNL Adobe Workfront] permite localizar, criar, atualizar e gerenciar itens do Workfront solicitando uma plataforma de agente de IA em linguagem natural. A plataforma decide quais ações do Workfront chamar e lida com a conversa com o Workfront para você.

>[!IMPORTANT]
>
>Atualmente, o servidor MCP do Workfront está disponível somente para clientes na região dos EUA que usam o AWS.

## Pré-requisitos

Este artigo supõe que você já configurou a conexão. Para obter informações sobre a instalação, consulte [Configurar o servidor MCP do Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

## Ferramentas disponíveis

O servidor MCP do Workfront expõe um conjunto de ferramentas que a plataforma de agente de IA chama em seu nome. Por exemplo, ferramentas para pesquisar no Workfront, criar itens, atualizar campos e gerenciar aprovações. Para obter a lista de referências completas, consulte [ferramentas de servidor MCP do Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md).

>[!IMPORTANT]
>
>Quando você conecta uma plataforma de agente de IA à Workfront, ela age no Workfront usando sua conta e as permissões da Workfront. As ações da plataforma têm o mesmo efeito que as ações executadas diretamente na interface do Workfront.<br>
>
>Você e seu provedor de plataforma de agente de IA são responsáveis pelas ações que a plataforma realiza no Workfront. A Adobe não se responsabiliza pelas alterações que a plataforma de IA Agent faz nos dados do Workfront.<br>
>
>Antes de permitir que a plataforma de agente de IA continue com uma solicitação, confirme se você entende o que ela pretende fazer, especialmente para ações que alteram ou excluem dados.


## Exemplos do que perguntar

Depois de se conectar, digite solicitações em linguagem natural na plataforma do agente de IA. A plataforma de agente de IA decide quais ações do Workfront serão chamadas e retorna os resultados.

>[!NOTE]
>
>Algumas ações podem não estar disponíveis devido aos controles do administrador na área Configuração do Workfront. Por exemplo, talvez você não consiga criar itens se o administrador do Workfront tiver desativado as ações de gravação para o servidor MCP.


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


## Considerações

Lembre-se das seguintes considerações ao usar o servidor MCP do Workfront:

### A plataforma de agente de IA pode usar informações de versões anteriores da conversa

Às vezes, as plataformas de agentes de IA reutilizam dados do início em uma conversa, em vez de solicitar as atualizações mais recentes da Workfront. Se algo mudou no Workfront desde a última pesquisa da plataforma de agente de IA, você pode ver informações desatualizadas.

Para forçar a plataforma de agente de IA a buscar dados novos, solicite-os explicitamente. Por exemplo:

* *Obtenha os dados mais recentes do Workfront. Não usar resultados em cache.*

### Verificar se há atualizações para o servidor MCP do Workfront

Você pode querer atualizar periodicamente sua conexão com o servidor MCP do Workfront para garantir que você tenha as ferramentas e os recursos mais recentes.

A maioria das atualizações deve ocorrer automaticamente. No entanto, recomendamos verificar as notas de versão do Workfront periodicamente.


## Dados e segurança

As ferramentas do servidor MCP do Workfront são consistentes com o funcionamento das chamadas de API. A Workfront não armazena prompts, respostas ou quaisquer outros dados. Quaisquer dados do Workfront que você solicitar poderão ser acessados na plataforma do Workfront.

Suas permissões de nível de acesso e objeto determinam o que você pode consultar ou gravar no Workfront. O administrador do Workfront tem controle das ações de leitura e gravação do MCP na área Configuração do Workfront.

### Quais dados saem do Workfront

O provedor da plataforma do agente de IA tem acesso aos dados do Workfront com os quais você interage por meio do servidor MCP do Workfront. Consulte seu provedor de plataforma de IA para obter detalhes.


### Como os provedores da plataforma de IA Agentic lidam com os dados do Workfront

A Workfront não tem controle sobre como o provedor da plataforma de agente de IA lida com os dados do Workfront. Consulte seu provedor de plataforma de IA para obter detalhes.

## Solução de problemas de uso diário

+++ Expanda para exibir dicas de solução de problemas para o uso diário do servidor MCP do Workfront.

| Problema | Causa provável | Corrigir |
|---|---|---|
| A plataforma de agente de IA está fornecendo informações desatualizadas. | A plataforma de agente de IA está reutilizando dados do início da conversa. | Solicite dados novos do Workfront. |
| A plataforma de agente de IA retornou dados dos itens incorretos do Workfront. | A plataforma de agente de IA escolheu os itens errados com base em termos ambíguos. | Pergunte novamente com nomes, IDs ou filtros mais específicos. |
| Uma atualização ou exclusão não entrou em vigor no Workfront. | O administrador do Workfront desativou as ações de gravação do servidor MCP do Workfront ou você não tem permissão para executar a ação no item específico. | Confirme com a plataforma do agente de IA se a ação foi executada. Em seguida, verifique se as ações de gravação estão ativadas para o servidor MCP do Workfront e se você tem permissão para alterar o item. |

Para obter mais informações sobre problemas de instalação e autenticação, consulte [Solução de problemas de instalação e autenticação](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication) em [Configurar o servidor MCP do Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

+++

## Perguntas frequentes

+++ Expanda para exibir as perguntas frequentes sobre o uso do servidor MCP do Workfront.

### O que é uma plataforma de agente de IA?

Uma plataforma de agente de IA é uma ferramenta de IA que pode realizar ações em seu nome no
outros sistemas, não apenas responda as perguntas. Ao conectar um ao Workfront
por meio do servidor MCP, é possível localizar, criar, atualizar e excluir o Workfront
itens com base no que você solicita em linguagem natural. Exemplos incluem Claude
Desktop, ChatGPT e outros clientes de IA compatíveis com MCP.


### Preciso ser um administrador do Workfront para usar o servidor MCP do Workfront?

Não. Qualquer usuário do Workfront pode usar o servidor MCP do Workfront por meio de uma conexão
Plataforma de agente de IA. A plataforma de agente de IA atua usando o Workfront
conta, nível de acesso e permissões de objeto, de modo que você só pode fazer o que
O já poderia fazer diretamente no Workfront.

### Por que a plataforma de IA Agent não pode criar, atualizar ou excluir itens para mim?

O administrador do Workfront controla quais ações de MCP são permitidas no
Área de configuração do Workfront. Se as ações de gravação estiverem desativadas, a plataforma de agente IA
O ainda pode localizar e ler itens do Workfront, mas não pode fazer alterações. Você também
precisam do nível de acesso correto e das permissões de objeto para os itens específicos
você está trabalhando com.

### A plataforma de agente de IA perguntará antes de alterar ou excluir os dados do Workfront?

Isso depende da plataforma de agente de IA, não do Workfront. A maioria das plataformas
solicitar que você confirme antes de executarem uma ação, especialmente para exclusões.
Antes de aprovar uma solicitação, leia o que a plataforma diz que está prestes a fazer —
as alterações acontecem no Workfront da mesma forma que aconteceriam se você as fizesse
você mesmo na interface.

<!--

### Can I undo something the AI agentic platform did in Workfront?

Changes the AI agentic platform makes in Workfront work the same way as 
changes you make in the interface. If Workfront supports undoing or 
restoring a particular action (for example, restoring a deleted item from 
the Recycle Bin), the same options apply. If Workfront doesn't normally let 
you undo an action, you can't undo it through the AI agentic platform either.

-->

### Por que a plataforma de agente de IA retornou os itens incorretos do Workfront?

A plataforma de agente IA escolhe itens com base nas palavras usadas. Se o seu
for ambígua — por exemplo, dois projetos têm nomes semelhantes — ela
pode escolher a errada. Pergunte novamente com nomes, IDs, datas e endereços mais específicos
ou filtros para restringir os resultados.


### Com quais itens do Workfront posso trabalhar por meio de uma plataforma de agente de IA?

Todos os itens aos quais você tem acesso no Workfront por meio do seu nível de acesso e
permissões de objeto. Isso inclui projetos, tarefas, problemas, documentos,
aprovações, registros do Planning e muito mais.

### Outras pessoas podem ver minhas conversas com a plataforma de agente de IA?

A Workfront não armazena seus prompts nem as respostas da plataforma de agente de IA.
Quem quer que forneça sua plataforma de agente de IA controla como suas conversas
são armazenados ou compartilhados. Consulte seu provedor de plataforma de IA para obter
detalhes.

### Preciso saber a API do Workfront ou qual ferramenta de MCP usar?

Não. A plataforma de agente de IA traduz sua solicitação em linguagem natural para
as ações certas do Workfront e escolhe as ferramentas certas para você. Se você estiver
já familiarizadas com a API do Workfront, as ações se sentirão familiares,
mas não é um requisito.

### Meus dados do Workfront são enviados ao provedor de plataforma do agente de IA ou armazenados por ele?

Para obter mais informações, consulte [Dados e segurança](#data-and-security) neste
artigo.

### O que acontece quando uma nova versão do servidor MCP do Workfront é lançada?

O servidor MCP geralmente é atualizado automaticamente, mas talvez seja necessário atualizar sua conexão com o servidor MCP algumas vezes para ver as ferramentas e os recursos mais recentes.

+++
