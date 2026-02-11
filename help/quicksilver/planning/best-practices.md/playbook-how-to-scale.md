---
title: 'Manual: dimensionamento gerenciado, após a primeira vitória'
description: Saiba como implantar o Adobe Workfront Planning após sua primeira implementação bem-sucedida
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
exl-id: 54df36b3-01a3-4fd3-b2d3-64ffb2fe5918
source-git-commit: 52bf41e146a11a4af4fbebfe5bb20a9765f2bc7b
workflow-type: tm+mt
source-wordcount: '2025'
ht-degree: 0%

---

# Manual: dimensionamento gerenciado, após a primeira vitória

{{planning-important-intro}}

**Versão**: 1.0

**Contexto**: &quot;Chegamos ao nosso primeiro caso de uso e agora todos querem entrar.&quot;



## &#x200B;1. A &quot;Armadilha de Sucesso&quot;

Às vezes, pode parecer que a fase mais perigosa da adoção do WFP é imediatamente após o primeiro caso de uso bem-sucedido ou POC. O entusiasmo é grande, mas o medo da &quot;dívida técnica&quot; e da &quot;expansão administrativa excessiva&quot; pode levar a duas respostas igualmente prejudiciais:

1. **Governança excessiva**: bloquear o sistema tão rigorosamente que novas equipes revertem para planilhas.

2. **Governança zero**: permitir que cada equipe crie seus próprios campos e tipos de registro, recriando a subutilização de metadados fragmentados encontrada em ambientes herdados.



## &#x200B;2. A filosofia central: WFP como o &quot;mecanismo de reconciliação&quot;

Em vez de tentar impedir que as equipes sejam diferentes, posicionamos o WFP como o local onde essas diferenças são **tornadas visíveis para que possam ser reconciliadas**.



* **Gerenciamento da adoção Velocity**: é natural ter cautela com a expansão para uma nova ferramenta antes de &quot;limpar&quot; os ambientes existentes. Embora a opção de **Simplificar Primeiro** forneça uma base altamente controlada, ela pode atrasar o tempo de implantação das equipes prontas para alinhamento. Acreditamos que a maneira mais eficaz de conduzir essa alteração é reconhecer que a **visibilidade é a Etapa 1**. O ímpeto em direção a uma ferramenta compartilhada e pronta para a empresa (afastando-se da proliferação de PPTs e planilhas) é o que finalmente desbloqueia objetivos de longo prazo.



  **Recomendação**: em vez de uma exigência de &quot;Limpeza primeiro&quot;, recomendamos alocar uma parte menor dos recursos para a manutenção contínua e uma parte significativamente maior para solucionar necessidades comerciais urgentes. Por exemplo, passar um ano apenas &quot;limpando&quot; taxonomias rende pouco valor incremental. No entanto, oferecer **visibilidade entre equipes** (por exemplo, por meio de um Calendário corporativo unificado ou de um roteiro de GTM consolidado) fornece o valor transformador de que suas partes interessadas precisam, ao mesmo tempo que fornece a estrutura de dados unificada necessária para administrar o ambiente ao longo do tempo.

* **Reconheça a realidade**: as equipes independentes desenvolvem naturalmente seus próprios processos, que geralmente ficam ocultos em planilhas isoladas. A transição para o PAM não cria uma confusão; ela ilumina aquela que já existe. Ao tornar esses processos visíveis em um ambiente compartilhado, você os coloca em um lugar onde eles podem finalmente ser abordados e aprimorados.

* **O sinal de progresso**: quando uma equipe solicita seus próprios campos, não é &quot;subutilização&quot;; é **Adoção**. Significa que eles veem o WFP como seu espaço de trabalho.

* **Gerenciar Dívida, Não Ocultar**: é natural se preocupar com o esforço necessário para limpar taxonomias divergentes posteriormente. No entanto, a alternativa — forçando padrões rigorosos muito cedo — muitas vezes leva as equipes de volta às planilhas onde seus processos (e suas dívidas) permanecem ocultos. Ao permitir que as equipes comecem no WFP com suas classificações atuais, você está movendo essa dívida para um ambiente visível e governado. Isso faz da reconciliação final uma tarefa iterativa em vez de um projeto de migração único e esmagador.



## &#x200B;3. O modelo de governação das &quot;vias rodoviárias&quot;

Escale sem dívidas definindo &quot;Pistas Globais&quot; e &quot;Playgrounds Locais&quot;.



### A. As rotas globais

* **Objetos Controlados**: objetos que cada equipe deve usar para os relatórios da empresa (por exemplo, `Strategic Pillar`, `Region`, `Fiscal Quarter`).

* **Gerenciado Por**: O Administrador Central De COE/Operações De Marketing.

* **Regra**: esses campos são &quot;Compartilhados&quot; e obrigatórios.



### B. Os Playgrounds locais (Raios)

* **Objetos experimentais**: campos ou tipos de registro específicos às necessidades táticas de uma equipe (por exemplo, `Influencer Handle` de uma equipe do Social ou `URL Slug` de uma equipe da Web).

* **Gerenciado por**: O Líder da Equipe (com orientação simples).

* **Regra**: as equipes podem inovar aqui. Se um campo &quot;Local&quot; é adotado por >3 equipes, é &quot;Promovido&quot; a uma pista global.



## &#x200B;4. O Paradoxo Da Governança: Equipes Em Primeiro Lugar, Padrões Seguem

Um desafio comum no dimensionamento do WFP é decidir qual vem primeiro: **Governança Empresarial** ou **Alinhamento Operacional da Equipe**.



Acreditamos que a maneira mais eficiente de fazer isso é reconhecer que o valor empresarial é construído em uma rua de mão dupla:

1. **As equipes precisam de relevância**: a empresa só percebe valor quando suas equipes estão em execução ativa. Portanto, a governança deve **atender às equipes**, fornecendo uma estrutura que ofereça suporte às suas necessidades operacionais conhecidas.

2. **A Empresa precisa de visibilidade**: a Liderança só pode tomar decisões informadas quando os dados estiverem limpos o suficiente para serem agregados. Portanto, as equipes devem **atender à empresa** fornecendo os metadados viáveis mínimos necessários para a visibilidade do portfólio.



O objetivo da &quot;escala gerenciada&quot; é encontrar a interseção dessas duas necessidades — padronizar o suficiente para fornecer visibilidade, mas não tanto para interromper a execução da equipe.



### A. Alinhamento de prioridades: dados vs. visualização

Ao dimensionar, reconheça que a definição de &quot;Valor&quot; difere entre as personas:

* **O Proprietário de Admin/Produto**: Valores de **taxonomias e classificações unificadas**. Sua meta é uma arquitetura de dados limpa que ofereça suporte à escalabilidade a longo prazo.

* **A Parte Interessada/Líder**: Valores de **visualização e insight** (por exemplo, um Calendário Global ou uma Linha do Tempo do Portfolio). Seu objetivo é o &quot;Momento Relâmpago&quot; que torna os dados acionáveis.



**A Estratégia**: Use a necessidade de visualização das partes interessadas como o *incentivo* para que a equipe esteja em conformidade com a necessidade de padrões de dados do administrador. Você obtém a taxonomia unificada fornecendo o &quot;Super Calendário&quot; que a liderança exige.



### B. A Fase De Observação &quot;Liderada Por Serviços&quot;

Durante o scale-up inicial, o papel do administrador é facilitar esse intercâmbio entre as equipes e a empresa.

* **Priorizar a Operação em vez da Padronização**: é melhor ter equipes planejando ativamente em espaços de trabalho isolados do que paralisá-las devido à falta de definições globais. Essa atividade são os &quot;dados brutos&quot; necessários para criar padrões saudáveis e reais.

* **Identificar os &quot;Mínimos de visibilidade&quot;**: trabalhe com liderança para identificar os 3 a 5 campos que *deve* limpar para os relatórios da empresa (por exemplo, `Strategic Alignment`, `Start Date`, `Budget`). Concentre sua energia de fiscalização SOMENTE aqui.



### B. Harmonização retroativa (governação como serviço)

Assim que surgir um padrão de &quot;necessidades conhecidas&quot; entre as equipes, a empresa poderá consolidar esses padrões em um serviço global.

1. **Observar padrões bem-sucedidos**: identifique as taxonomias &quot;vencedoras&quot; que as equipes já criaram e adotaram.

2. **O Handshake Colaborativo**: junte os campeões de equipe para refinar os sucessos locais em um padrão corporativo compartilhado.

3. **Implantar como um serviço**: implante as novas faixas globais não como uma &quot;restrição&quot;, mas como uma maneira de simplificar os relatórios e o alinhamento entre equipes para as pessoas que estão fazendo o trabalho.



**Principais argumentos**: a governança deve ser uma resposta ao sucesso operacional, não um pré-requisito para ela.



## &#x200B;5. Mecânica de dimensionamento: o modelo de crescimento baseado em padrões

A aplicação dessa filosofia requer uma abordagem cuidadosa da estrutura de dados. Para evitar a &quot;Subutilização de governança&quot;, resista ao anseio de criar campos globais para cada solicitação individual. Em vez disso, use o **Caminho de maturidade do campo** para permitir que o uso real oriente seus padrões corporativos:



1. **Nível 1: Experimento local**: a Equipe A cria um campo personalizado em seu espaço de trabalho.

2. **Nível 2: Reconhecimento de Padrão**: Os Administradores percebem que as Equipes B e C estão usando ou solicitando um campo semelhante.

3. **Nível 3: Padronização Empresarial**: o Administrador cria uma única versão padronizada desse campo como um tipo de registro na **Workspace de Taxonomia Global** e a associa às equipes.



### A Mecânica da &quot;Aposentadoria Suave&quot;

Como o WFP não tem um recurso nativo de &quot;Arquivamento&quot; para campos, retirar um campo local requer um processo deliberado de &quot;Aposentadoria Temporária&quot; para preservar dados históricos sem desorganizar a interface do usuário:



1. **Migração de Dados**: Use uma exibição de tabela (ou Fusion) para copiar valores em massa do campo &quot;Sombra&quot; local para o novo campo Faixa Global. Verifique se os dados estão validados e limpos durante essa movimentação.

2. **Renomear para descontinuação**: renomeie o campo local com um prefixo como `[DEPRECATED]` ou `z_` (por exemplo, `z_Language (Old)`). Isso empurra o campo para a parte inferior dos seletores de campo e sinaliza aos usuários que ele não é mais a &quot;Source da verdade&quot;.

3. **Remoção de Formulário**: **Esta é a etapa mais crítica.** Remova o campo obsoleto de todos os **Registrar Forms**. Isso evita que novos dados sejam inseridos, mantendo os dados antigos visíveis nas exibições de tabela ou relatórios existentes, se necessário.

4. **Período de &quot;Desativação&quot;**: mantenha o campo obsoleto (prefixado e fora de forma) por 30 a 60 dias para garantir que nenhum dado tenha sido perdido durante a migração. Após esse período, se os dados forem totalmente reconciliados no Caminho global, o campo local poderá ser excluído do espaço de trabalho.



## &#x200B;6. Evitar a &quot;deriva do núcleo&quot; (a regra de abstração)

Para evitar que o Planning se torne tão desorganizado quanto o Principal:

* **A Camada de Abstração**: cada campo no WFP deve responder a uma **Pergunta Estratégica**. Se um campo for usado apenas para rastreamento tático (por exemplo, &quot;Esta prova foi aprovada?&quot;), mantenha-o no Core.

* **Consolidação primeiro**: se uma equipe quiser um novo campo de metadados, convide-a para verificar a Taxonomia global primeiro. Isso requer a concessão de **acesso Somente Leitura** aos clientes potenciais da equipe para o espaço de trabalho de Taxonomia Global (consulte a Seção 7). Ao mapear suas necessidades táticas para um campo estratégico existente, você evita duplicações desnecessárias e mantém a integridade dos relatórios.



## &#x200B;7. O modelo de visibilidade &quot;Acesso somente leitura&quot;

Resolva a sensação de &quot;Siloed&quot; sem o barulho do trabalho &quot;Siloed&quot;.

* **O problema**: as equipes em spokes se sentem isoladas porque só veem seus próprios registros.

* **A Correção**: conceder às equipes **acesso Somente Leitura aos espaços de trabalho designados como &#39;Primários&#39; para esses tipos de registros compartilhados**.

* **O Resultado**: eles podem ver o contexto corporativo mais amplo para inspiração e alinhamento, mas seu espaço de trabalho local permanece limpo e focado em suas tarefas específicas.



## &#x200B;8. Gerenciando o crescimento através de workshops

Dimensionar o PAM é tanto um desafio cultural quanto técnico. Use workshops direcionados para preencher a &quot;lacuna de governança&quot;.



### A. Workshop de descoberta da &quot;bagunça necessária&quot;

* **Público-alvo**: líderes regionais de marketing e especialistas em operações.

* **Meta**: documentar a &quot;Realidade Silonizada&quot; atual (os dados operacionais fragmentados).

* **A Mensagem**: &quot;Não estamos aqui para excluir seus campos. Estamos aqui para entender como eles se ligam à estratégia global.&quot;

* **Resultado**: um mapeamento de rascunho de campos táticos locais para rotas estratégicas globais.



### B. A Sessão De Alinhamento &quot;Visibilidade Estratégica&quot;

* **Público-alvo**: partes interessadas de marketing de alto nível (liderança).

* **Objetivo**: redefinir a ansiedade de &quot;Simplificar primeiro&quot;.

* **A Mensagem**: &quot;Não precisamos de uma taxonomia perfeita para iniciar. Estamos usando o WFP como o ambiente para *compilar* a taxonomia perfeita.&quot;

* **Resultado**: aprovação para avançar com o WFP como mecanismo de reconciliação enquanto o Core permanecer em seu estado atual.



### C. A Exibição &quot;Spoke-to-Global&quot;

* **Público-alvo**: novas equipes explorando o WFP.

* **Objetivo**: reduzir a sensação de &quot;siloed&quot;.

* **A Mensagem**: &quot;Veja como o trabalho local da Equipe A alimenta automaticamente a Workspace primária designada? Você pode ter a mesma visibilidade para seu trabalho também.&quot;

* **Resultado**: aceitação de novos departamentos que veem o benefício de serem &quot;conectados&quot; sem perder sua independência local.



### D. Horário comercial do &quot;Suporte contínuo&quot;

* **Público-alvo**: todos os usuários do WFP (atuais e potenciais).

* **Meta**: fornecer um ambiente recorrente e de baixo risco para orientação tática e solução de problemas.

* **A Mensagem**: &quot;Não há perguntas erradas. Estamos aqui para ajudá-lo a resolver seus desafios específicos de planejamento em tempo real.&quot;

* **Resultado**: maior confiança do usuário, resolução mais rápida de atritos técnicos e identificação de novos padrões que possam justificar padronização global.



## &#x200B;9. Equipe de Escala: Funções e Responsabilidades

O sucesso em um modelo de dimensionamento gerenciado requer mais do que apenas a configuração da ferramenta; requer uma distribuição clara das funções entre as equipes Global e Spoke.



### A. O Arquiteto Corporativo (CDE Central/Operações de Marketing)

* **Foco**: integridade da empresa, desempenho do sistema e **taxonomia de dados unificados**.

* **Responsabilidades**:

   * Gerencia a **Workspace de Taxonomia Global**.

   * Facilita o **Caminho de maturidade do campo** (promovendo sucessos locais para padrões globais).

   * Mantém as exibições **Principais do Workspace** para relatórios executivos.

   * Lidera a **Auditoria Semântica** mensal entre espaços de trabalho.



### B. O Spoke Champion (Proprietário do Processo de Equipe)

* **Foco**: relevância da equipe e velocidade de adoção.

* **Responsabilidades**:

   * Atua como ponto único de contato da equipe funcional.

   * É o proprietário da estrutura do espaço de trabalho local e dos experimentos de campo personalizado.

   * Garante que a equipe use o **Gateway Controlado** (Forms) para entrada de dados.

   * Participa do **Handshake Colaborativo** durante a harmonização.



### C. O Patrocinador Executivo (Liderança de Marketing)

* **Foco**: alinhamento estratégico, visibilidade de OKR e **visualização de portfólio (por exemplo, Calendário global)**.

* **Responsabilidades**:

   * Define os **OKRs de marketing** da empresa no espaço de trabalho de Taxonomia global.

   * Defende o valor de &quot;Etapa de visibilidade 1&quot; para outros líderes.

   * Reforça a alocação de recursos 80/20 (Valor sobre limpeza).



### D. O líder de ativação (gerenciamento de alterações)

* **Foco**: mudança cultural e desenvolvimento de habilidades.

* **Responsabilidades**:

   * Hospeda recorrentes **Office Hours** e **Workshops de Descobertas**.

   * Mantém a exibição interna de &quot;História de sucesso&quot;.

   * Identifica pontos de atrito técnico que o Arquiteto Empresarial deve resolver.



## &#x200B;10. Lista de verificação para dimensionar a próxima equipe

* [ ] **Identifique o Campeão**: quem é o &quot;Proprietário do Processo&quot; ou o &quot;Campeão&quot; desta nova equipe?

* [ ] **Definir o &quot;Delta Local&quot;**: de quais 2 a 3 campos essa equipe precisa que o padrão Global não fornece atualmente?

* [ ] **Mapear para rotas globais**: quais campos globais existentes podem atender a 80% de suas necessidades?

* [ ] **Conceder Visibilidade Global**: Conceder a eles acesso Somente Leitura aos Espaços de Trabalho Primários relevantes e ao espaço de trabalho de Taxonomia Global no Dia 1.

* [ ] **Estabelecer a Transferência**: como seu trabalho &quot;alimenta&quot; os Espaços de Trabalho Principais relevantes? (por exemplo, por meio de um Tipo de registro global ou uma pesquisa específica).

<!--original content: 

**Version**: 1.0 

**Context**: "We've landed our first use case, and now everyone wants in." 

 

## 1. The "Success Trap" 

Sometimes it can feel like the most dangerous phase of WFP adoption is immediately after the first successful use case or POC. Enthusiasm is high, but the fear of "technical debt" and "administrative sprawl" can lead to two equally damaging responses: 

1.  **Over-Governance**: Locking down the system so tightly that new teams revert to spreadsheets. 

2.  **Zero-Governance**: Letting every team create their own fields and record types, recreating the fragmented metadata sprawl found in legacy environments. 

 

## 2. The Core Philosophy: WFP as the "Reconciliation Engine" 

Instead of trying to stop teams from being different, we position WFP as the place where those differences are **made visible so they can be reconciled**. 

 

*   **Managing Adoption Velocity**: It is natural to feel cautious about expanding into a new tool before "cleaning up" existing environments. While choosing to **Simplify First** provides a highly governed foundation, it can delay time-to-value for teams ready to align. We believe the most effective way to lead through this change is to recognize that **visibility is Step 1**. Momentum toward a shared, enterprise-ready tool (moving away from the sprawl of PPTs and spreadsheets) is what ultimately unblocks long-term goals.  

 

    **Recommendation**: Instead of a "Clean Up First" mandate, we recommend allocating a smaller portion of resources to ongoing maintenance and a significantly larger portion to solving pressing business needs. For example, spending a year solely on "cleaning up" taxonomies yields little incremental value. However, delivering **cross-team visibility** (e.g., through a Unified Enterprise Calendar or a consolidated GTM roadmap) provides the transformative value your stakeholders need, while providing the unified data structure you need to govern the environment over time. 

*   **Acknowledge the Reality**: Independent teams naturally develop their own processes, which often stay hidden in siloed spreadsheets. Transitioning to WFP doesn't create a mess; it shines a light on the one that already exists. By making these processes visible in a shared environment, you put them in the one place where they can finally be addressed and improved. 

*   **The Progress Signal**: When a team asks for their own fields, it's not "sprawl"—it's **Adoption**. It means they see WFP as their workspace. 

*   **Manage Debt, Don't Hide It**: It is natural to be concerned about the effort required to clean up divergent taxonomies later. However, the alternative—forcing strict standards too early—often drives teams back to spreadsheets where their processes (and their debt) remain hidden. By allowing teams to begin in WFP with their current classifications, you are moving that debt into a visible, governed environment. This makes the eventual reconciliation an iterative task rather than a single, overwhelming migration project. 

 

## 3. The "Lanes on a Road" Governance Model 

Scale without debt by defining "Global Lanes" and "Local Playgrounds." 

 

### A. The Global Lanes 

*   **Controlled Objects**: Objects that every team must use for enterprise reporting (e.g., `Strategic Pillar`, `Region`, `Fiscal Quarter`). 

*   **Managed By**: The Central COE/Marketing Ops Admin. 

*   **Rule**: These fields are "Shared" and mandatory. 

 

### B. The Local Playgrounds (Spokes) 

*   **Experimental Objects**: Fields or record types specific to a team's tactical needs (e.g., a Social team's `Influencer Handle` or a Web team's `URL Slug`). 

*   **Managed By**: The Team Lead (with light guidance). 

*   **Rule**: Teams can innovate here. If a "Local" field is adopted by >3 teams, it is "Promoted" to a Global Lane. 

 

## 4. The Governance Paradox: Teams First, Standards Follow 

A common challenge in scaling WFP is deciding which comes first: **Enterprise Governance** or **Team Operational Alignment**.  

 

We believe the most effective way to navigate this is to recognize that enterprise value is built on a two-way street: 

1.  **Teams need relevance**: The enterprise only realizes value when its teams are actively executing. Therefore, governance must **serve the teams** by providing structure that supports their known operational needs. 

2.  **The Enterprise needs visibility**: Leadership can only make informed decisions when data is clean enough to aggregate. Therefore, the teams must **serve the enterprise** by providing the minimum viable metadata required for portfolio visibility. 

 

The goal of "Managed Scaling" is to find the intersection of these two needs—standardizing enough to provide visibility, but not so much that you stall team execution. 

 

### A. Aligning Priorities: Data vs. Visualization 

When scaling, recognize that the definition of "Value" differs between personas: 

*   **The Admin/Product Owner**: Values **unified taxonomies and classifications**. Their goal is a clean data architecture that supports long-term scalability. 

*   **The Stakeholder/Leader**: Values **visualization and insight** (e.g., a Global Calendar or a Portfolio Timeline). Their goal is the "Lightning Moment" that makes the data actionable. 

 

**The Strategy**: Use the stakeholder's need for visualization as the *incentive* for the team's compliance with the admin's need for data standards. You get the unified taxonomy by delivering the "Super Calendar" that leadership demands. 

 

### B. The "Service-Led" Observation Phase 

During early scale-up, the Admin's role is to facilitate this exchange between teams and the enterprise. 

*   **Prioritize Operation over Standardization**: It is better to have teams actively planning in siloed workspaces than to have them stalled by a lack of global definitions. This activity is the "raw data" required to build healthy, real-world standards. 

*   **Identify the "Visibility Minimums"**: Work with leadership to identify the 3-5 fields that *must* be clean for enterprise reporting (e.g., `Strategic Alignment`, `Start Date`, `Budget`). Focus your enforcement energy ONLY here. 

 

### B. Retroactive Harmonization (Governance as a Service) 

Once a pattern of "known needs" emerges across teams, the enterprise can move to consolidate those patterns into a global service. 

1.  **Observe Successful Patterns**: Identify the "winning" taxonomies that teams have already built and adopted. 

2.  **The Collaborative Handshake**: Bring team champions together to refine their local successes into a shared enterprise standard. 

3.  **Deploy as a Service**: Roll out the new global lanes not as a "restriction," but as a way to simplify reporting and cross-team alignment for the people doing the work. 

 

**Key Takeaway**: Governance should be a response to operational success, not a prerequisite for it.  

 

## 5. Scaling Mechanics: The Pattern-Based Growth Model 

Applying this philosophy requires a thoughtful approach to data structure. To avoid "Governance Sprawl," resist the urge to build global fields for every individual request. Instead, use the **Field Maturity Path** to let real-world usage guide your enterprise standards: 

 

1.  **Level 1: Local Experiment**: Team A creates a custom field in their workspace. 

2.  **Level 2: Pattern Recognition**: The Admin notices Teams B and C are using or asking for a similar field. 

3.  **Level 3: Enterprise Standardization**: The Admin creates a single, standardized version of that field as a record type in the **Global Taxonomy Workspace** and syndicates it to teams. 

 

### The Mechanics of "Soft Retirement" 

Because WFP does not currently have a native "Archive" feature for fields, retiring a local field requires a deliberate "Soft Retirement" process to preserve historical data without cluttering the UI: 

 

1.  **Data Migration**: Use a table view (or Fusion) to bulk-copy values from the local "Shadow" field into the new Global Lane field. Ensure the data is validated and cleaned during this move. 

2.  **Rename for Deprecation**: Rename the local field with a prefix like `[DEPRECATED]` or `z_` (e.g., `z_Language (Old)`). This pushes the field to the bottom of field pickers and signals to users that it is no longer the "Source of Truth." 

3.  **Form Removal**: **This is the most critical step.** Remove the deprecated field from all **Record Forms**. This prevents new data from being entered while keeping the old data visible in existing table views or reports if needed. 

4.  **The "Sunset" Period**: Keep the deprecated field (prefixed and off-form) for 30-60 days to ensure no data was missed during migration. After this period, if the data is fully reconciled in the Global Lane, the local field can be deleted from the workspace. 

 

## 6. Avoiding the "Core Drift" (The Abstraction Rule) 

To prevent Planning from becoming as cluttered as Core: 

*   **The Abstraction Layer**: Every field in WFP should answer a **Strategic Question**. If a field is only used for tactical tracking (e.g., "Was this proof approved?"), keep it in Core. 

*   **Consolidation First**: If a team wants a new metadata field, invite them to check the Global Taxonomy first. This requires granting team leads **Read-Only access** to the Global Taxonomy workspace (see Section 7). By mapping their tactical needs to an existing strategic field, you prevent unnecessary duplication and maintain reporting integrity. 

 

## 7. The "Read-Only Access" Visibility Model 

Solve the "Siloed" feeling without the noise of "Siloed" work. 

*   **The Problem**: Teams in spokes feel isolated because they only see their own records. 

*   **The Fix**: Grant teams **Read-Only access to the workspaces designated as 'Primary' for those shared record types**.  

*   **The Result**: They can see the broader enterprise context for inspiration and alignment, but their local workspace remains clean and focused on their specific tasks. 

 

## 8. Managing Growth through Workshops 

Scaling WFP is as much a cultural challenge as a technical one. Use targeted workshops to bridge the "Governance Gap." 

 

### A. The "Necessary Mess" Discovery Workshop 

*   **Audience**: Regional Marketing Leads and Ops Champions. 

*   **Goal**: Document the current "Siloed Reality" (the fragmented operational data). 

*   **The Message**: "We aren't here to delete your fields. We're here to understand how they link to the global strategy." 

*   **Outcome**: A draft mapping of local tactical fields to global strategic lanes. 

 

### B. The "Strategic Visibility" Alignment Session 

*   **Audience**: High-level Marketing Stakeholders (leadership). 

*   **Goal**: Reframe the "Simplify First" anxiety. 

*   **The Message**: "We don't need a perfect taxonomy to start. We are using WFP as the environment to *build* the perfect taxonomy." 

*   **Outcome**: Approval to move forward with WFP as the reconciliation engine while Core remains in its current state. 

 

### C. The "Spoke-to-Global" Showcase 

*   **Audience**: New teams exploring WFP. 

*   **Goal**: Reduce the "siloed" feeling. 

*   **The Message**: "See how Team A's local work automatically feeds the designated Primary Workspace? You can have that same visibility for your work too." 

*   **Outcome**: Opt-in from new departments who see the benefit of being "connected" without losing their local independence. 

 

### D. The "Ongoing Support" Office Hours 

*   **Audience**: All WFP users (current and prospective). 

*   **Goal**: Provide a recurring, low-stakes environment for troubleshooting and tactical guidance. 

*   **The Message**: "There are no wrong questions. We are here to help you solve your specific planning challenges in real-time." 

*   **Outcome**: Increased user confidence, faster resolution of technical friction, and the identification of new patterns that might warrant global standardization. 

 

## 9. Staffing for Scale: Roles and Responsibilities 

Success in a managed scaling model requires more than just tool configuration; it requires a clear distribution of roles across the Global and Spoke teams. 

 

### A. The Enterprise Architect (Central COE/Marketing Ops) 

*   **Focus**: Enterprise integrity, system performance, and **unified data taxonomy**. 

*   **Responsibilities**: 

    *   Manages the **Global Taxonomy Workspace**. 

    *   Facilitates the **Field Maturity Path** (promoting local successes to global standards). 

    *   Maintains the **Primary Workspace** views for executive reporting. 

    *   Leads the monthly **Semantic Audit** across workspaces. 

 

### B. The Spoke Champion (Team Process Owner) 

*   **Focus**: Team relevance and adoption velocity. 

*   **Responsibilities**: 

    *   Acts as the single point of contact for the functional team. 

    *   Owns the local workspace structure and custom field experiments. 

    *   Ensures the team uses the **Governed Gateway** (Forms) for data entry. 

    *   Participates in the **Collaborative Handshake** during harmonization. 

 

### C. The Executive Sponsor (Marketing Leadership) 

*   **Focus**: Strategic alignment, OKR visibility, and **portfolio visualization (e.g., Global Calendaring)**. 

*   **Responsibilities**: 

    *   Defines the enterprise **Marketing OKRs** in the Global Taxonomy workspace. 

    *   Champions the value of "Visibility Step 1" to other leaders. 

    *   Reinforces the 80/20 resource allocation (Value over Cleanup). 

 

### D. The Enablement Lead (Change Management) 

*   **Focus**: Cultural shift and skill development. 

*   **Responsibilities**: 

    *   Hosts recurring **Office Hours** and **Discovery Workshops**. 

    *   Maintains the internal "Success Story" showcase. 

    *   Identifies technical friction points for the Enterprise Architect to resolve. 

 

## 10. Checklist for Scaling the Next Team 

* [ ] **Identify the Champion**: Who is the "Process Owner" or "Champion" of this new team? 

* [ ] **Define the "Local Delta"**: What 2-3 fields does this team need that the Global standard doesn't currently provide? 

* [ ] **Map to Global Lanes**: Which existing Global fields can satisfy 80% of their needs? 

* [ ] **Grant Global Visibility**: Give them Read-Only access to the relevant Primary Workspaces and the Global Taxonomy workspace on Day 1. 

* [ ] **Establish the Handoff**: How does their work "feed" the relevant Primary Workspaces? (e.g., via a Global Record Type or a specific lookup).

-->