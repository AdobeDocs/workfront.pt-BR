---
title: Solicitações e práticas recomendadas do CX Co-worker
content-type: reference
description: Saiba mais sobre as práticas recomendadas para usar o Coworker no Workfront e exiba uma lista de exemplos de prompts.
author: Becky
feature: Get Started with Workfront
source-git-commit: 01de260893e5bbf7a228479df2f3fc6a1337d31d
workflow-type: tm+mt
source-wordcount: '2247'
ht-degree: 2%

---

# Solicitações e práticas recomendadas do CX Co-worker

&lt;!—NÃO USE ISSO—Em vez disso, vincule-se ao artigo de solicitações de exemplo do MCP, certifique-se de atualizá-lo com as versões recentes para o MCP—>

>[!IMPORTANT]
>
>Atualmente, o CX Coworker não está disponível para organizações de assistência médica, finanças ou alguns outros setores com dados confidenciais. O Assistente de IA está disponível para essas organizações. Para obter mais informações, consulte [Visão geral do Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).

Com o CX Co-worker, você pode usar a linguagem natural para interagir com o Workfront Workflow e o Workfront Planning.

O parceiro faz parte da Adobe Experience Cloud Agent Orchestrator.

Para obter mais informações sobre o Agent Orchestrator, consulte [Adobe Experience Platform Agent Orchestrator](https://experienceleague.adobe.com/pt-br/docs/experience-cloud-ai/experience-cloud-ai/agents/agent-orchestrator).

## Requisitos de acesso

<!--Add info about how to qualify for agent orchestrator stuff-->

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Select, Prime ou Ultimate </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Padrão ou Claro</p>
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td><p>Para qualquer funcionalidade fora das habilidades básicas, sua organização deve ter adquirido o Adobe Agent Orchestrator.</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td><p>Você deve ter as permissões apropriadas para interagir com qualquer objeto por meio do Colaborador.</p> <p>Por exemplo, para receber informações sobre um projeto por meio do Colaborador, você deve ter pelo menos a permissão Exibir para esse projeto.</p></td>
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

* O administrador do Workfront deve ter ativado o Assistente de IA para sua organização.

  Para obter mais informações, consulte [Pré-requisitos do Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant) no artigo Visão geral do Assistente de IA.
* O administrador do Workfront deve ter ativado o Assistente de IA para o seu nível de acesso.

  Para obter mais informações, consulte [Habilitar ou desabilitar o Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

## Considerações

Considere as seguintes restrições ao usar o CX Co-worker:

### Reversibilidade

Algumas ações podem ser revertidas. Por exemplo, se um objeto for criado, essa criação poderá ser revertida.

Entretanto, algumas ações, como exclusão de objeto, podem **não** ser revertidas. Recomendamos ter isso em mente ao executar ações em seus dados por meio do Colaborador.

### Restrições de cobertura de dados/objetos

* A consulta e os relatórios de campos personalizados estão nos estágios iniciais e algumas habilidades (como auxiliares de consulta baseados em API) ainda não lidam com campos personalizados arbitrários para agregação e filtragem.

### Limitações de interação/UX

* Atualmente, o CX Co-worker não &quot;aprende&quot; a longo prazo com o estilo ou as preferências de um usuário individual. Cada chat usa apenas a conversa atual e o conhecimento do produto.
* O contexto da conversa é mantido em uma única sessão de chat. Abrir uma nova página ou fechar o assistente redefine o histórico da conversa.
* Se os procedimentos de aprovação viverem em um aplicativo externo, como Confluence ou SharePoint, e forem vinculados somente por meio de campos de URL, o Colaborador não fará a busca no momento e o raciocínio nessas páginas.

### Armazenamento de dados / chaves gerenciadas pelo cliente

* Como o CX Co-worker faz parte da Adobe Experience Platform Agent Orchestrator, os dados das suas interações com o Co-worker são armazenados no Adobe Experience Platform, não no Workfront. Portanto, esses dados não são cobertos pelos contratos de Chaves gerenciadas pelo cliente da Workfront (BYOK).

## Competências essenciais de IA de uso geral

>[!IMPORTANT]
>
>Esses recursos de uso geral estão disponíveis para todos os usuários cuja organização tenha um Contrato Adobe AI assinado em arquivo.

Para conhecer as práticas recomendadas e os prompts dessas habilidades de uso geral, consulte [prompts e práticas recomendadas do Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/ai-prompts-best-practices.md).

<!--Follow up with Oznur-->

### Conhecimento do produto

O CX Co-worker pode fornecer instruções ou informações de referência extraídas da documentação da Workfront.

Para obter mais informações sobre como obter informações da documentação do Workfront, consulte [Obter ajuda do Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md).

Exemplo: como alterar o tipo de duração da tarefa?

### Resumo de projetos, tarefas e problemas

O CX Co-worker pode resumir projetos, tarefas ou problemas<!--, or documents--> que foram carregados no Workfront.

Para obter mais informações sobre resumos de projetos, tarefas e problemas, consulte [Resumir usando o Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md).

Exemplo: resuma o projeto chamado Campanha do último trimestre de 2026.

<!--

### Locate work items

CX Coworker can find work items like projects, tasks, and issues

Example: Find all tasks assigned to me that are due this week.

For more information on using AI Assistant to locate project, tasks, and issues, see [se AI Assistant to work with projects, tasks, and issues](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).

-->

<!--

Follow up on this to see if it's going away or what

### Catch Me Up 

Catch Me Up summarizes updates, uploaded documents, and other notable changes that have about your projects that have occurred in the last 24 hours, 3 days, or 7 days.  

For more information on Catch me up, see [Catch up on work in Priorities](/help/quicksilver/workfront-basics/priorities/catch-me-up.md).

-->

<!--

### Smart filters

You can use natural language filters in Priorities to replace status, pre-built views to help you filter your work.

For more information on using Smart Filters, see [Filter your work with Smart filters](/help/quicksilver/workfront-basics/priorities/filter-group-work-priorities.md) in the article Filter and group your work with Priorities.

-->

## CX Co-worker no Workfront

* [Informações sobre projetos, tarefas e problemas](#project-task-and-issue-information)
* [Gerenciamento de projetos e trabalhos](#project-and-work-management)
* [Conteúdo e aprovações](#content-and-approvals)

### Informações sobre projetos, tarefas e problemas

O CX Co-worker pode fornecer informações sobre projetos, tarefas e problemas, incluindo resumos e a integridade do projeto.

Consulte exemplos de solicitações para aprovações de documentos e ativos nas seguintes áreas:

* [Localizar informações sobre projetos, tarefas ou problemas](#find-information-about-projects-tasks-or-issues)
* [Resumir projetos, tarefas ou problemas](#summarize-projects-tasks-or-issues)
* [Mostrar Integridade do Projeto para projetos, programas ou portfólios](#show-project-health-for-projects-programs-or-portfolios) <!--remove any mention of project health-->

#### Localizar informações sobre projetos, tarefas ou problemas

* Projetos
  * Mostre-me todos os projetos ativos para a equipe de Marketing da Marca
  * é necessária uma lista de projetos no portfólio Campanhas do quarto trimestre na categoria &quot;Digital&quot;.
  * Mostre-me projetos gerenciados por usuários na empresa de Serviços da Creative que são Gerentes de projeto.
* Tarefas
  * Me consiga todas as tarefas atribuídas a Joan Harris.
  * Mostre-me tarefas na categoria &quot;Design&quot; atribuídas à equipe de UX.
  * Preciso de tarefas atribuídas aos redatores no programa Promoções de Férias.
* Problemas
  * Mostre-me todos os problemas no projeto &quot;Redesign de site&quot; na categoria &quot;Técnico&quot;.
  * Obtenha todos os problemas não resolvidos relatados pelo grupo de controle de qualidade.
  * Preciso de problemas atribuídos aos desenvolvedores na empresa Global Tech.

#### Resumir projetos, tarefas ou problemas

* &quot;Resumir este projeto&quot;
* &quot;Resumir a última semana deste projeto&quot;

#### Mostrar Integridade do Projeto para projetos, programas ou portfólios

>[!NOTE]
>
>Sua organização deve estar inscrita no beta de Integridade do Projeto para usar esse recurso.

* &quot;Mostrar a integridade de meus projetos ativos&quot;
* &quot;Mostrar a integridade deste programa&quot;

### Gerenciamento de projetos e trabalhos

Você pode usar o CX Co-worker para criar e gerenciar projetos, incluindo tarefas e atribuições.

Consulte exemplos de prompts para gerenciamento de projeto e trabalho nas seguintes áreas:

* [Criar, atualizar ou excluir projetos](#create-update-or-delete-projects)
* [Identificar o modelo de projeto correto com base no prompt do usuário](#identify-the-right-project-template-based-on-user-prompt)
* [Adicionar, editar ou personalizar tarefas em um projeto](#add-edit-or-customize-tasks-in-a-project)
  <!--* [Create, update, or delete assignments](#create-update-or-delete-assignments)-->
  <!--* [Recommend best matching user assignments for the task based on users' job role and availability](#recommend-best-matching-user-assignments-for-the-task-based-on-users-job-role-and-availability)-->

#### Criar, atualizar ou excluir projetos

Você pode criar projetos do zero ou de modelos, atualizar projetos e excluí-los.

* Crie um projeto em branco chamado Sandbox de inovação do segundo trimestre, a partir de 10 de março e até 30 de abril. Defina-me como proprietário.
* Crie um projeto chamado Lucent AI Launch - NA usando o modelo Campanha de marketing integrado. Inicie em 5 de fevereiro e defina-o como Current (Atual).
* Crie um projeto chamado Redesign de site - EMEA entre 1º de março e 15 de junho. É de alta prioridade, de propriedade da EMEA Marketing, patrocinada pelo VP de Marketing, orçada em US$ 250 mil com cerca de 1.200 horas planejadas, focada na Europa com o objetivo de melhorar as conversões.
* Para o projeto Lucent AI Launch - NA, transfira-o para o segundo trimestre, altere o objetivo para impulsionar testes gratuitos, empurre o final para meados de abril, aumente o orçamento para US$ 150 mil e marque-o como urgente.
* Mostre-me todos os projetos de marketing atuais que terminam no segundo trimestre, que são de alta prioridade ou prioridade urgente, classificados por data final mais próxima.

#### Adicionar ou editar tarefas

É possível adicionar ou editar tarefas em um projeto e personalizar a lista de tarefas do modelo usado para criar um projeto.

* Adicione uma nova tarefa chamada Controle de qualidade da landing page ao projeto e agende-a de 22 a 26 de abril.
* Atualize a tarefa Revisão de design para que ela termine em 18 de abril e a atribua à equipe criativa.
* Remova a tarefa Produção de ativos impressos do projeto.
* Mostre-me todas as tarefas deste projeto que não estão concluídas e estão agendadas para iniciar entre 1º de abril e 30 de abril.
* Defina a Aprovação legal como predecessora da tarefa de inicialização da campanha.
* Adicione uma nova tarefa chamada Cópia final em polonês agendada de 15 a 16 de abril, mova a tarefa Cópia de revisão para 10 de abril, remova a tarefa Revisão extra em rodada e defina Cópia final em polonês como predecessora da Criação de email.
* Durante o fluxo de criação do projeto, tente fornecer o máximo de informações possível sobre os resultados que devem se tornar tarefas do projeto.

#### Criar, atualizar ou excluir atribuições

Você pode criar, atualizar e excluir atribuições de usuário ou funções de trabalho.

* Para a &quot;Página inicial de design para o lançamento do produto&quot; do projeto, identifique as funções de trabalho apropriadas e as horas planejadas recomendadas para todas as tarefas não atribuídas atualmente.
* Tenho várias tarefas não atribuídas, incluindo &quot;Implementar rastreamento do GA4 para site de campanha&quot;, &quot;Configurar eventos de conversão&quot; e &quot;Validar dados de análise&quot;. Você pode sugerir as funções de trabalho certas e as horas estimadas para cada um?
* Para as tarefas criativas &quot;Criar 3 variantes de banner para anúncios de exibição do EMEA&quot;, &quot;Aplicar revisões&quot; e &quot;Exportar ativos finais&quot;, atribua as melhores funções de trabalho e estime o esforço necessário para cada tarefa.
* Em todos os projetos &quot;Lançamento de produto do segundo trimestre&quot;, &quot;Redesign de site - EMEA&quot; e &quot;Campanha de mídia paga - NA&quot;, identifique todas as tarefas não atribuídas e atribua as funções de trabalho apropriadas com horas planejadas recomendadas para cada uma.

<!--

#### Identify the right project template based on user prompt

* We're launching a new product feature with a landing page, emails, paid ads, and social posts. Which project template should we use?
* Create a project for a global marketing campaign with multiple channels and regional rollouts. (should suggest a template if provided more info)
* For Website Redesign – EMEA project, recommend and attach the correct project template.

-->

<!--

#### Recommend best matching user assignments for the task based on users' job role and availability

* Who is the best available user to assign to 'Design Landing Page Hero', considering who still has capacity today?
* Who should be assigned to 'Backend API integration for campaign reporting', considering engineering role alignment?
* For all unassigned tasks in this project, recommend the best users based on job role match and daily availability.
* Recommend users for the tasks 'QA testing for website launch' and 'Content review', prioritizing users whose job roles match and who are not over-allocated today.

-->

### Conteúdo e aprovações

O CX Co-worker pode ajudar a gerenciar aprovações de documentos e ativos no Workfront.

Considere o seguinte ao trabalhar com aprovações de documentos e ativos:

* As aprovações de conteúdo devem ser habilitadas para sua organização antes que você possa usar essa funcionalidade no Co-worker.
* A IA não pode aprovar ou rejeitar em nome de humanos. As decisões dependem de usuários, com exceção do Revisor da IA do Workfront.

  Para obter mais informações sobre o Workfront AI Reviewer, consulte [Introdução ao Workfront AI Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).
* Essa funcionalidade existe no Workfront e não pode ser usada para interagir com ferramentas externas ou provedores de documentos.
* Para obter a melhor experiência, use essa funcionalidade com a experiência de Aprovações unificadas.

  Para obter mais informações sobre Aprovações unificadas, consulte [Visão geral sobre Aprovações unificadas](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

Consulte exemplos de solicitações para aprovações de documentos e ativos nas seguintes áreas:

* [Adicionar ou remover participantes da aprovação](#add-or-remove-approval-participants)
* [Lembrar as partes interessadas de um único ativo que está aguardando revisão](#remind-stakeholders-of-a-single-asset-waiting-for-review)
* [Adicionar, atualizar ou aplicar modelos de aprovação para um único ativo](#add-update-or-apply-approval-templates-for-a-single-asset)

#### Adicionar ou remover participantes da aprovação

* Adicione Sarah Chen e Miguel Alvarez como aprovadores no documento atual.
* Remova Jennifer Otto desta aprovação.
* Remova qualquer pessoa que não tenha tomado uma decisão de aprovação.
* Adicione um novo estágio ao spring-campaign.pdf chamado &quot;Final review&quot;.
* Adicione Mark e Sarah como aprovadores e Phil como revisor no segundo estágio do winter-campaign.pdf
* Para o winter-campaign.pdf, dê à primeira fase um prazo para hoje às 17h, e a revisão final um prazo para amanhã às 17h
* Adicione um estágio de verificação final ao fall-campaign.png com um prazo para quinta-feira às 17h e inclua Jim e Pam como aprovadores, também Oscar como revisor
* Adicione Mark Jones ao fall-campaign.png para o primeiro e o último estágio como revisor.
* Vamos obter uma aprovação de vários estágios criada para o fall-campaign.png com 3 estágios, 1 Design, 2 Redação de Conteúdo e 3 Legais. Só preciso de uma decisão para cada estágio. Adicione Mike, Sally, Jane ao design, Chris, Richard, Mark à redação e Phil, Tom e Sarah ao Legal.

#### Lembrar as partes interessadas de um único ativo que está aguardando revisão

* Envie um lembrete aos aprovadores no ativo &quot;Vídeo da campanha da primavera&quot; que não responderam.
* Lembre todos que não aprovaram esse ativo de &quot;Vídeo da campanha da primavera&quot;.
* Quem ainda não tomou uma decisão sobre o ativo &quot;Diretrizes da marca PDF&quot;? Lembre-os.

#### Adicionar, atualizar ou aplicar modelos de aprovação para um único ativo

* Aplique o modelo de aprovação &quot;Inicialização de marketing&quot; ao ativo com o nome &quot;Vídeo da campanha da primavera&quot;.
* Crie um novo modelo de aprovação com 3 estágios: Creative Review, Legal e Aprovação Final.
* Adicione Julia Santos e Shane Baker ao estágio 1.
* Edite o modelo &quot;Inicialização do produto&quot; para adicionar Elizabeth Peterson ao estágio de aprovação final.
* Crie um template chamado &quot;Urgent Review&quot; com um estágio e atribua-o a Olivia Kim.
* Atualize o template &quot;Creative Review&quot; removendo Rick Kuvec e adicionando Karen Sterling ao estágio 2.


## CX Co-worker no Workfront Planning

### Trabalhar com registros do Planning

* [Criar, excluir, duplicar ou restaurar registros](#create-delete-duplicate-or-restore-records)
* [Vincular registros a outros registros](#link-records-to-other-records)
* [Editar, atualizar ou anexar um campo a um registro](#edit-update-or-append-a-field-to-a-record)
* [Acessar histórico de alterações de registro](#access-record-change-history)

#### Criar, excluir, duplicar ou restaurar registros

* Crie um novo registro de campanha chamado Vendas de verão 2026
* Adicione um novo registro de produto com o nome Widget Pro e o preço $299
* Você pode criar um novo registro de cliente potencial para João Silva?
* Exclua o registro de campanha chamado Promoção antiga
* Remover o registro de teste que acabei de criar
* É possível excluir a ID de registro Rc123abc456?
* Duplicar o registro de campanha do primeiro trimestre
* É possível copiar esta campanha para criar uma nova?
* Fazer uma cópia da campanha de Promoção de Férias
* Restaurar a campanha que eu excluí acidentalmente
* Você pode recuperar o registro de projeto excluído?
* Excluí acidentalmente um registro. É possível restaurá-lo?

#### Vincular registros a outros registros

* Vincule o registro da Campanha de Verão à iniciativa do segundo trimestre
* É possível conectar este produto às campanhas de marketing relacionadas?
* Preciso associar esses três clientes em potencial ao registro da Conta da Empresa

#### Editar, atualizar ou anexar um campo a um registro

* Atualize o campo de orçamento na Campanha de verão para US$ 75.000
* Você pode alterar o status deste registro de projeto para Concluído?
* Adicionar João da Silva ao campo de membros da equipe desta iniciativa

#### Acessar histórico de alterações de registro

* Mostre-me o histórico de alterações para o registro da Campanha de Verão
* Você pode exibir quem modificou este projeto e o que eles alteraram?
* Preciso ver todas as atualizações feitas neste registro na semana passada

### Uso do System Designer no Workfront Planning

* [Criar e configurar espaços de trabalho](#create-and-configure-workspaces)
* [Definir tipos de registro](#define-record-types)
* [Criar campos e campos de fórmula](#design-fields-and-formula-fields)
* [Criar exibições personalizadas](#build-custom-views)


#### Criar e configurar espaços de trabalho

* Crie um novo espaço de trabalho do Planning chamado Campanhas de marketing de 2026
* Atualizar meu espaço de trabalho de Planejamento de Produto para alterar a cor para azul e adicionar uma descrição
* Mostrar todos os espaços de trabalho do Planning aos quais tenho acesso

#### Definir tipos de registro

* Criar um novo tipo de registro chamado Campanhas no meu espaço de trabalho do Planning
* Atualizar o tipo de registro Iniciativas para alterar seu ícone e descrição
* Mostrar todos os tipos de registro no meu espaço de trabalho de Planejamento de Marketing

#### Criar campos e campos de fórmula

* Adicionar um campo Orçamento ao meu tipo de registro de Campanhas de Planejamento com o tipo de moeda
* Criar um campo de fórmula no Planning que calcula os dias restantes até a data final da campanha
* Atualizar o campo Prioridade no meu espaço de trabalho do Planning para adicionar mais opções suspensas

#### Criar exibições personalizadas

* Criar uma exibição de linha do tempo no Planning para ver minha programação de campanha por datas de início e término
* Adicionar uma nova exibição de tabela às minhas Iniciativas de Planejamento que filtra somente o status ativo
* Duplique minha visualização de Campanhas ativas de planejamento e modifique a classificação.
