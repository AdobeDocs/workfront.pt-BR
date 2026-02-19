---
title: 'Construir O Seu Sucesso: Modelagem Da Hierarquia Da Campanha'
description: Saiba como traduzir seus complexos processos de negócios em uma hierarquia de campanha escalável e controlada usando "Centros de gravidade" e uma arquitetura com vários espaços de trabalho.
feature: Workfront Planning
role: Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 02e3b55f-9188-42bf-8d0b-c9fed86c63c4
source-git-commit: 7f3ca12d89a2a5fbebc12b3df8a40edbb17d0ead
workflow-type: tm+mt
source-wordcount: '1537'
ht-degree: 0%

---

# Arquiteto do seu sucesso: modelagem da hierarquia de campanhas

<!--see the file again for additional comments from Seth and others-->

>[!IMPORTANT]
>
>As informações neste artigo se referem ao Adobe Workfront Planning, um recurso adicional da Adobe Workfront.
>
>Sua organização deve ter um pacote do Workfront Planning Prime ou superior para oferecer suporte aos recursos recomendados neste artigo.
>
>Para obter uma lista de requisitos para acessar o Workfront Planning, consulte [Visão geral do acesso ao Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).
> 
>Para obter informações gerais sobre o Workfront Planning, consulte [Introdução ao Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

Saiba como traduzir processos comerciais complexos em uma hierarquia de campanha escalável e controlada usando centros de gravidade e uma arquitetura de vários espaços de trabalho no Adobe Workfront Planning.

Este guia destina-se aos administradores do Workfront e usuários avançados que estão implementando e projetando a arquitetura de seu ambiente no Workfront Planning.

## Visão geral da arquitetura de sucesso

À medida que suas operações de marketing amadurecem, a complexidade dos dados também amadurece. Sem um blueprint claro, seu Sistema de registro de marketing pode se tornar rapidamente uma gaveta de lixo de registros desconectados, terminologia conflitante e silos de relatórios.

Ao criar uma arquitetura de sucesso, você estabelece uma estrutura para modelar sua hierarquia de campanha no Workfront Planning. Ela leva você do caos nas planilhas para um modelo governado e orientado a objetos que garante que cada equipe fale a mesma linguagem, mantendo a agilidade que precisa executar.

## Crie uma hierarquia para definir seus níveis de intenção

Para manter a clareza e a escalabilidade, recomendamos começar com um caminho principal comprovado ao projetar seu fluxo de trabalho no Workfront Planning.

A partir daí, você pode expandir sua estratégia adicionando mais níveis à sua arquitetura.

### O caminho principal: como passar da estratégia para a ação

Embora as organizações possam expandir essa hierarquia à medida que suas necessidades operacionais evoluem, começar pelos três níveis descritos nas seções abaixo garante uma forte ponte entre a estratégia e a execução.

Com base em nossas descobertas, notamos que a maioria das implementações bem-sucedidas do Workfront Planning prospera em um modelo limpo de três níveis que abrange o Planning e o Workfront.

A seguir estão os níveis de uma implementação bem-sucedida do Planning e os artefatos que você pode considerar criar para lhe dar suporte no processo:

* **Nível 1: Campanhas (Workfront Planning)**

   * **Foco:** Defina os pilares estratégicos de longo prazo e as iniciativas anuais. Por exemplo, defina uma iniciativa para sua organização chamada &quot;Reconhecimento global da marca no ano fiscal de 2026&quot;. Este é o seu foco por um determinado período. Crie campanhas para apoiar esta iniciativa.

   * **Pessoas:** As partes interessadas neste nível podem ser Diretoras de Marketing, vice-presidentes de Marketing ou outros líderes estratégicos.

  Para obter informações, consulte [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

* **Nível 2: Táticas de Canal (Workfront Planning)**

   * **Foco:** Defina os resumos operacionais que descrevem o &quot;quê&quot; de canais específicos. Esta é a camada final de intenção estratégica antes do início do trabalho. Por exemplo, crie uma tática &quot;Q1 Social Media Blitz&quot;. Em seguida, você pode emparelhá-lo com suas campanhas.

   * **Personalidades:** os principais interessados são um líder de operações de marketing, líderes de canal ou gerentes de campanha.

* **Nível 3: Projetos (Planning e Workfront)**

   * **Foco:** Execute as experiências ou atividades exatas que eventualmente realizarão sua iniciativa. Alguns dos resultados são específicos, como publicações sociais, emails, páginas da Web.

   * **Implementação:** você pode criar Táticas no Planning e vinculá-las diretamente aos **Projetos** no Workfront, onde os resultados individuais são gerenciados como tarefas e problemas.

   * **Pessoa:** os principais interessados aqui são pessoas criativas, colaboradores individuais e qualquer pessoa responsável por fazer o trabalho de apoio à iniciativa.

### Expansão estratégica: como adicionar mais níveis

Depois de estabelecer o caminho principal, você pode optar por adicionar camadas adicionais após uma consideração cuidadosa de sua complexidade de negócios específica.

Talvez seja útil criar os seguintes itens adicionais:

* **Planos de canal:** uma camada entre Campanhas e Táticas para agrupar estratégias multifuncionais. Por exemplo, um plano chamado &quot;Estratégia digital&quot;.

* **Atividades:** se você trabalhar em um ambiente de volume mais baixo (você pode ter 5.000 entregas ou menos por ano), algumas equipes podem preferir rastrear experiências individuais como registros do Workfront Planning antes que elas se tornem projetos do Workfront.

>[!IMPORTANT]
>
>Se sua organização produzir mais de 5.000 atividades por ano, você deverá mover o rastreamento de entrega individual para o Workfront.
>
>O gerenciamento de registros de experiência de alto volume no Planning pode levar a um acúmulo de dados que obscurece sua visibilidade estratégica.
>Recomendamos esta orientação ampla para obter o máximo de eficiência:
>
>* Use o Planning para &quot;por que&quot; e &quot;o que&quot;
>* Use o Workfront para o &quot;como&quot; de alto volume.

## Entenda os centros de gravidade para criar sua arquitetura

Um Sistema de Registro de Marketing de nível empresarial não é construído em um único espaço de trabalho. Ele usa uma arquitetura &quot;hub-and-spoke&quot; onde os tipos de registros são gerenciados em seus centros de gravidade naturais.

Para obter mais informações, consulte [Implante sua página inicial estratégica: uma barra inicial de 30 dias](/help/quicksilver/planning/best-practices.md/30-day-launchpad.md).

Para construir sua arquitetura usando a abordagem hub-and-spoke, você deve criar o seguinte:

* Um hub de taxonomia
* Um espaço de trabalho de planejamento estratégico
* Raios funcionais

### Criar o hub de taxonomia como suas classificações

Primeiro, você deve estabelecer um espaço de trabalho centralizado para suas classificações globais a fim de definir os principais conceitos que todos na organização devem entender. Por exemplo, crie os seguintes tipos de registros em um espaço de trabalho central: Marcas, Regiões, Produtos, Personas.

Para obter informações, consulte [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

Estabeleça o seguinte ao criar suas classificações:

* **Local primário:** Escolha um espaço de trabalho primário. Esse espaço de trabalho deve ser a fonte da verdade para os tipos de registro criados.

* **O benefício:** ao agregar essas definições ao restante da empresa, você esclarece que conceitos como &quot;Região: EMEA&quot; significam a mesma coisa para todas as equipes.

### Crie o espaço de trabalho estratégico do Planning como seu centro executivo

O centro executivo é onde as Campanhas de alto nível (e quaisquer Planos de canal) residem.

* **Local principal:** este é o centro de gravidade executivo, proporcionando um ambiente sem ruídos para a tomada de decisões estratégicas.

* **O benefício:** A liderança pode gerenciar o portfólio de campanhas sem ouvir o ruído tático diário.

### Defina os spokes funcionais como espaços de trabalho de suas equipes

As unidades funcionais (Social, Creative, Email) têm seus próprios espaços de trabalho para gerenciar suas Táticas.

* **Local principal:** esses espaços de trabalho são os centros de gravidade individuais para a execução da equipe local.

* **O benefício:** as equipes consomem as campanhas e classificações globais dos hubs, enquanto mantêm seus próprios objetos locais.

  Por exemplo, a equipe pode adicionar o tipo de registro Campanha do espaço de trabalho central no espaço de trabalho da equipe, mas criar campanhas relevantes somente para o espaço de trabalho. Exemplos de campanhas são &quot;Meios de comunicação&quot; ou &quot;Direitos de uso&quot;.

## Usar uma abordagem de governança baseada em substantivos

Para garantir que sua arquitetura se mantenha sob pressão, siga o princípio da governança baseada em substantivos.

Recomendamos o seguinte ao criar suas entidades no Workfront Planning:

* **Use substantivos, não verbos:** Nomeie os tipos de registro conforme as coisas que você está rastreando (nomeie-os como &quot;Campanha&quot; ou &quot;Tático&quot;), e não as ações a serem executadas (não nomeie-os como &quot;Campanha&quot; ou &quot;Planejamento&quot;).

* **Padronizar nomenclatura:** Use os mesmos nomes em todos os espaços de trabalho. Isso permite agregar dados em todo o portfólio para a geração de relatórios executivos.

## E os portfólios e programas existentes?

Uma pergunta comum para organizações maduras é como lidar com os portfólios e programas que já criaram no Workfront. No passado, esses objetos eram frequentemente usados para imitar o planejamento estratégico.

Agora, recomendamos que você mude essa abordagem para o Workfront Planning, que naturalmente se encaixa na abordagem estratégica do planejamento.

### Substituir portfólios e programas por tipos de registro

Em muitas organizações, os portfólios são usados para representar marcas ou unidades de negócios de alto nível, enquanto os programas representam temas estratégicos.

No Workfront Planning, eles são melhor modelados como Tipos de registro no hub de taxonomia.

Tratando uma Marca ou Unidade de Negócios como um tipo de registro, é possível vinculá-los a uma Campanha ou Tática em toda a empresa, fornecendo relatórios muito mais flexíveis do que uma estrutura estática Portfolio - Programa.

### Usar uma estratégia de ponte de relatórios

Embora o Workfront Planning seja o futuro da intenção estratégica, seus relatórios nativos por meio do Canvas Dashboard ainda estão amadurecendo.

Muitas organizações ainda dependem dos recursos robustos de relatórios vinculados às estruturas herdadas do Portfolio e do Programa no Workfront.

Recomendamos o seguinte:

* Não exclua seus portfólios e programas.
* Use as automações do Planning para criar uma ponte entre os tipos de registro e os portfólios e programas.

  Quando uma Tática ou Campanha é criada no Workfront Planning, esse registro pode gerar uma Portfolio ou Programa correspondente no Workfront.

  Para obter informações, consulte [Criar objetos usando as automações de registro do Adobe Workfront Planning](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).

Isso permite:

* Aproveite a visualização estratégica superior do Workfront Planning usando linhas do tempo e calendários.

* Mantenha seus relatórios herdados no Workfront para as partes interessadas que ainda não estão prontas para mudar para o Canvas.

## Práticas recomendadas e dicas

### Dos

* **Mantenha a abordagem principal de primeiro caminho:** Estabeleça o fluxo de Campanha para Tática para Projeto antes de adicionar mais complexidade.

* **Designar espaços de trabalho primários:** Verifique se cada tipo de registro tem um espaço de trabalho doméstico (considere que seu centro de gravidade) que atue como agregador para relatórios.

* **Priorizar formulários de solicitação para o processo de entrada:** Use formulários de registro para grupos com menos sofisticação no Workfront Planning para garantir a integridade dos metadados.

  >[!CAUTION]
  >
  >Embora os usuários avançados possam se beneficiar da entrada direta de dados nas visualizações de tabela, isso deve ser abordado com cuidado.
  >Alterações em massa em uma tabela podem facilmente criar problemas de dados para outras partes interessadas.

### Não

* **Não use generalizações:** Por exemplo, em vez de falar sobre um ambiente &quot;central&quot;, consulte especificamente o Workfront e o objeto Project ao falar sobre execução.

* **Não torne mais complicado:** cada nível adicional de hierarquia adiciona um imposto de gerenciamento. Adicione apenas níveis que respondam a uma pergunta comercial que não possa ser respondida no momento.

* **Não criar silos:** verifique se os tipos de registros estão compartilhados entre espaços de trabalho para que as equipes não redigitem os mesmos dados.


<!--original content:


## Goal 

Learn how to translate your complex business processes into a scalable, governed campaign hierarchy using "Centers of Gravity" and a multi-workspace architecture. 

 

## Overview 

As your marketing operations scale, so does the complexity of your data. Without a clear blueprint, your Marketing System of Record (MSOR) can quickly become a "junk drawer" of disconnected records, conflicting terminology, and reporting silos. 

 

The "Blueprint of Success" is a framework for modeling your campaign hierarchy in Workfront Planning. It moves you from "spreadsheet chaos" to a governed, object-oriented model that ensures every team speaks the same language while maintaining the agility they need to execute. 

 

## The Hierarchy: Finding Your Levels of Intent 

To maintain clarity and scalability, we recommend starting with a proven **Core Path**. While organizations can expand this hierarchy as their operational needs evolve, beginning with these three levels ensures a strong bridge between strategy and execution. 

 

### The Core Path: Strategy to Action 

Most successful implementations thrive on a clean, three-tier model that spans both Planning and Workflow: 

 

1. **Level 1: Campaigns (Planning Module)** 

    * **Focus:** Long-term strategic pillars and annual initiatives (e.g., "FY26 Global Brand Awareness").  

    * **Persona:** CMO, VP of Marketing, Strategic Leads. 

2. **Level 2: Channel Tactics (Planning Module)** 

    * **Focus:** The operational briefs defining the "what" for specific channels (e.g., "Q1 Social Media Blitz"). This is the final layer of strategic intent before work begins. 

    * **Persona:** Marketing Ops, Channel Leads, Campaign Managers. 

3. **Level 3: Workflow Projects (Workflow Module)** 

    * **Focus:** The actual execution of "Experiences" or "Activities" (e.g., specific social posts, emails, web pages).  

    * **Implementation:** Tactics in Planning link directly to **Projects** in the Workflow module, where individual deliverables are managed as tasks and issues. 

    * **Persona:** Creatives, Individual Contributors. 

 

### Strategic Expansion: Adding More Levels 

Once the core path is established, organizations may choose to add additional layers after careful consideration of their specific business complexity: 

 

* **Channel Plans:** A layer between *Campaigns* and *Tactics* to group cross-functional strategies (e.g., "Digital Strategy"). 

* **Workfront Planning Activities:** In lower-volume environments (typically <5,000 deliverables/year), some teams prefer to track individual "Experiences" as Workfront Planning records before they become projects. 


>[!TIP]
>
>**Crucial Tip: The 5,000 Deliverable Threshold** 
>
>If your organization produces more than 5,000 activities per year, you should **always** offload individual deliverable tracking to the **Workflow module**. Managing high-volume "Experience" records in Planning can lead to data accumulation that obscures your strategic visibility. Use Planning for the "Why" and "What," and the Workflow module for the high-volume "How." 

 

## Architecture: Centers of Gravity 

An enterprise-grade MSOR isn't built in a single workspace. It uses a "Hub-and-Spoke" architecture where record types are managed in their natural **Centers of Gravity**. 

 

### 1. The Taxonomy Hub (Classifications) 

Establish one centralized workspace for your "Global Classifications" (e.g., Brands, Regions, Products, Personas). 

* **Primary Location:** This workspace is the "Source of Truth" for these objects. 

* **The Benefit:** By syndicating these definitions to the rest of the business, you solve "Semantic Drift"—ensuring that "Region: EMEA" means the same thing to every team. 

 

### 2. The Strategic Planning Workspace (Executive Center) 

This is where high-level **Campaigns** (and any **Channel Plans**) live.  

* **Primary Location:** This is the executive center of gravity, providing a noise-free environment for strategic decision-making. 

* **The Benefit:** Leadership can manage the portfolio without seeing the day-to-day tactical mess. 

 

### 3. Functional Spokes (Team Workspaces) 

Functional units (Social, Creative, Email) have their own workspaces to manage their **Tactics**. 

* **Primary Location:** These workspaces are the center of gravity for local team execution.  

* **The Benefit:** Teams "consume" the global campaigns and classifications from the hubs, while maintaining their own local objects (like *Media Outlets* or *Usage Rights*). 

 

## Noun-Based Governance: Speak One Language 

To ensure your blueprint holds up under pressure, follow the principle of **Noun-Based Governance**.  

 

* **Use Nouns, Not Verbs:** Name your record types after the "things" you are tracking (`Campaign`, `Tactic`), not the "actions" (`Campaigning`, `Planning`). 

* **Standardize Nomenclature:** Use the same names across all workspaces. This allows you to aggregate data across the entire portfolio for executive reporting. 

 

## What About Existing Portfolios and Programs? 

A common question for mature organizations is how to handle the Portfolios and Programs they've already built in the **Workflow module**. In the past, these objects were often used to mimic strategic planning. 

 

### 1. Portfolios & Programs → Record Types 

In many organizations, **Portfolios** are used to represent high-level Brands or Business Units (BUs), while **Programs** represent strategic themes. 

* **The Shift:** These are best modeled as **Record Types** in your **Taxonomy Hub**. By treating "Brand" or "Business Unit" as a record type, you can link them to any campaign or tactic across the entire enterprise, providing much more flexible reporting than a static Portfolio/Program structure. 

 

### 2. The "Reporting Bridge" Strategy 

While Workfront Planning is the future of strategic intent, its native reporting via **Canvas Dashboards** is still maturing. Many organizations still rely on the robust reporting capabilities tied to their legacy Portfolio and Program structures in the Workflow module. 

* **The Recommendation:** Don't delete your Portfolios and Programs yet. Instead, use **Fusion automations** to create a bridge.  

* **How it Works:** When a Tactic or Campaign is created in Workfront Planning, Fusion can automatically mirror that record into a corresponding Portfolio or Program in the Workflow module. This allows you to: 

    1. Enjoy Workfront Planning's superior **strategic visualization** (Timelines/Calendars). 

    2. Maintain your **legacy reporting** in the Workflow module for stakeholders who aren't yet ready to move to Canvas. 

## Best Practices & Tips 

### Do: 

* **Stick to the Core Path first.** Establish your Campaign-to-Tactic-to-Project flow before adding more complexity. 

* **Designate Primary Workspaces.** Ensure each record type has one "home" workspace (its center of gravity) that acts as the aggregator for reporting. 

* **Prioritize Forms for Intake.** Use record forms for groups with less sophistication in Workfront Planning to ensure metadata integrity. While Power Users may benefit from direct data entry in Table views, this should be approached with caution—bulk changes in a table can easily create data headaches for other stakeholders. 
 

### Don't: 

* **Don't say "Core".** Refer specifically to the **Workflow module** and the **Project** objects when talking about execution. 

* **Don't over-complicate.** Every additional level of hierarchy adds a "management tax." Only add levels that answer a business question you can't currently answer. 

* **Don't create silos.** Ensure your record types are shared across workspaces so teams aren't re-typing the same data.
-->