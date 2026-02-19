---
title: 'Criar a Bridge: conectando intenção estratégica a projetos'
description: Saiba como criar uma "thread estratégica" entre seus planos de alto nível no Adobe Workfront Planning e sua execução diária de workflows no Adobe Workfront.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 567ab223-b282-4b98-9655-7b9766fba869
source-git-commit: 7f3ca12d89a2a5fbebc12b3df8a40edbb17d0ead
workflow-type: tm+mt
source-wordcount: '1156'
ht-degree: 0%

---


# Construir a ponte: conectando intenção estratégica a projetos

>[!IMPORTANT]
>
>As informações neste artigo se referem ao Adobe Workfront Planning, um recurso adicional da Adobe Workfront.
>
>Sua organização deve ter um pacote do Workfront Planning Prime ou superior para oferecer suporte aos recursos recomendados neste artigo.
>
>Para obter uma lista de requisitos para acessar o Workfront Planning, consulte [Visão geral do acesso ao Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).
> 
>Para obter informações gerais sobre o Workfront Planning, consulte [Introdução ao Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

Saiba como criar uma thread estratégica entre seus planos de alto nível no Adobe Workfront Planning e sua execução diária no Workfront. Você pode criar uma ponte entre a estratégia e a execução usando conexões.

Este guia destina-se aos administradores do Workfront e gerentes de espaço de trabalho que estão implementando o Workfront Planning.

## Visão geral do alinhamento da estratégia com a execução

Conectar sua estratégia ao seu trabalho diário transforma a visão em realidade. Quando os planos de alto nível estão sincronizados com a execução, você cria um segmento estratégico que garante que cada projeto e tarefa dê andamento aos negócios.

Alcançar esse alinhamento requer um conjunto de links técnicos e medidas de proteção de processo que conectam os esforços no Workfront aos registros estratégicos no Workfront Planning.

Ao reduzir a distância entre o planejamento e a ação, você garante que a energia de sua equipe esteja sempre focada em suas metas de maior prioridade.

## Estabelecer a base criando uma conexão

Antes de interligar o planejamento e a execução, como um gerenciador de espaço de trabalho, você deve definir quais tipos de registro são elegíveis para uma conexão.

### Visão geral do campo de conexão

A ponte começa com a criação de um campo de conexão.

Um campo de conexão serve como um handshake técnico entre os tipos de registro.

Este tipo de campo é o mecanismo por trás de todos os relacionamentos no Workfront Planning. É uma expressão de intenção, na medida em que estabelece que um tipo de registro específico (como uma Tática de canal) pode ser vinculado a outros tipos de objeto, quer eles vivam no Planning ou no Workfront.

Para obter informações, consulte [Visão geral dos tipos de registros conectados](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

### Definir quando criar uma conexão

Idealmente, você deve decidir se precisa criar conexões antes que qualquer trabalho seja criado.

Ao adicionar um campo de conexão, você está arquitetando seu ambiente para oferecer suporte a um segmento estratégico, independentemente de como os registros individuais são criados no final.

## Definir estratégia e execução em sincronia

Para manter o foco da sua camada estratégica, recomendamos que você concentre seus registros de planejamento em intenções de alto nível ao usar o Workfront para execução tática.

Essa abordagem usa os pontos fortes exclusivos de ambos os módulos das seguintes maneiras:

* **Planejamento do Workfront (a camada estratégica):** Permanece de alto nível. Ele rastreia a Campanha, a Tática do Canal e o Orçamento. Ele não emite ruídos e está pronto para os executivos.

* **Workfront (a camada de execução):** gerencia os detalhes táticos. Você pode gerenciar experiências ou atividades individuais como projetos, tarefas e problemas. Você pode atribuí-los à propriedade e criar aprovações para execução.

## Ir da intenção para a ação ativando a ponte

Depois que a conexão for configurada, você deverá decidir como ativar o link entre um registro estratégico específico e um projeto de execução.

### Usar um caminho com led de tabela

Os estrategistas e usuários avançados geralmente usam a visualização de tabela como bancada para refinar os planos ao longo do tempo.

Por padrão, a criação de um registro em uma tabela não estabelece um link para o Workfront.

A conexão com um projeto de execução é estabelecida quando um usuário decide ativar o link.

Isso pode ser feito das seguintes maneiras:

* Crie manualmente um projeto conectado de downstream diretamente do campo de conexão no Workfront Planning ou de uma página Conexões opcional na exibição detalhada do registro.

  A criação manual resulta em um projeto em branco sem formulários personalizados específicos.

  Para obter informações, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

* Automaticamente, usando as automações do Workfront Planning, para necessidades mais complexas.

  Essas automações estão disponíveis como botões na barra de ações quando você seleciona uma linha em uma tabela.

  Isso permite a supervisão humana ou a criação de espaços reservados, garantindo que os projetos sejam gerados somente em seu ambiente de fluxo de trabalho quando forem realmente necessários.

  Para obter informações, consulte [Criar objetos usando as automações de registro do Adobe Workfront Planning](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md)


### Criar ativações automatizadas

Para organizações com solicitações de alto volume ou necessidades de automação avançada, a ponte pode ser ativada automaticamente com base em eventos específicos ou com base em valores de campo configurados em um formulário de solicitação.

Você precisará de uma licença do Adobe Workfront Fusion para essa abordagem.

Para obter mais informações, consulte [Configurar e gerenciar o Workfront Fusion: índice do artigo](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-workfront-fusion-toc).

* **Usar disparadores de envio:** Como os formulários fornecem um evento de envio único e limpo, eles podem ser usados como disparadores para automações do Fusion. Um cenário de Fusão pode detectar um envio de formulário e gerar imediatamente um projeto vinculado no Workfront.

* **Usar acionadores de valor de campo:** Para uma automação mais profunda, você pode configurar o Fusion para monitorar campos específicos. Por exemplo, uma caixa de seleção simples chamada &quot;Pronto para execução&quot; pode servir como catalisador, estabelecendo a ponte automaticamente no momento em que é marcada.

## Adicionar campos de pesquisa à visibilidade da superfície

Depois que um projeto é vinculado, é possível exibir dados em tempo real do Workfront diretamente no registro do Planning, adicionando campos de pesquisa do projeto.

Como gerente de espaço de trabalho, você pode configurar campos de pesquisa para obter qualquer campo personalizado ou do sistema do projeto vinculado (como Data de Término Efetivo ou Lead Creative) no tipo de registro do Planning. Uma vez capturados, esses dados podem ser acumulados por vários níveis de sua hierarquia estratégica, até o nível da campanha. Isso fornece relatórios agregados avançados para as partes interessadas em todo o ciclo de vida do marketing, mantendo-as informadas sem a necessidade de sair do ambiente de planejamento.

## Alcançar visibilidade conectando estratégia à ação

O valor final da ponte é a visibilidade em tempo real.

Conectando intenção à ação, você pode responder rapidamente a perguntas críticas de negócios. Veja a seguir exemplos dessas perguntas:

* A nossa campanha &quot;Reconhecimento da Marca no Ano Fiscal 26&quot; está gerando resultados ativamente neste momento?

* Onde nossas táticas estratégicas precisam de mais suporte criativo para permanecer no cronograma?

* Como estamos alinhando nossos recursos com nossos pilares estratégicos de maior prioridade?

## Práticas recomendadas e dicas

### Dos:

* **Use a metáfora de &quot;thread estratégico&quot;:** Lembre as equipes de que cada projeto deve ser um &quot;bead&quot; em uma cadeia de caracteres estratégica.

* **Automatizar a entrega:** Use automações para acionar a criação de projetos a fim de economizar tempo e esforço, além de melhorar a conectividade e a governança de dados.

* **Link, não duplicar:** Use campos de pesquisa para exibir dados de execução em tempo real (como status ou datas de conclusão) em seus registros estratégicos. Isso garante que suas visualizações estratégicas sejam sempre precisas, sem precisar de atualizações manuais da equipe.

### Não:

* **Não tratar registros de planejamento como listas de tarefas:** A ponte foi projetada para conectar intenção estratégica a projetos de execução. Mantenha seus registros de planejamento focados no &quot;o que&quot; e no &quot;por quê&quot; e permita que o módulo de fluxo de trabalho lide com o &quot;como&quot; detalhado de tarefas e problemas.

* **Não sincronize em excesso:** Não é necessário sincronizar todos os detalhes do nível de projeto novamente no Planning. Mantenha a camada estratégica de alto nível e sem ruído.

* **Não ignore a ponte:** Se o trabalho começar no módulo de Fluxo de Trabalho sem um link para o Planning, você criou um &quot;Plano Sombra&quot; que é invisível para a liderança.

<!--original content:

# The Bridge: Connecting Strategic Intent to Projects 

 

## Goal 

Learn how to create a "strategic thread" between your high-level plans in Workfront Planning and your daily execution in the Workflow module. 

 

## Overview 

Connecting your strategy to your daily work turns vision into reality. When high-level plans are in sync with execution, you create a **strategic thread** that ensures every project and task moves the business forward. 

 

Achieving this alignment requires a set of technical links and process guardrails that connect efforts in the **Workflow module** with strategic records in **Workfront Planning (WFP)**. By bridging the gap between planning and action, you ensure that your team's energy is always focused on your highest-priority goals. 

 

## The foundation: Establishing the connection 

Before you can bridge planning and execution, a workspace manager must define which record types are eligible for a connection. 

 

### The connection field: The technical handshake 

The bridge begins with a **connection field**. This field type is the engine behind all relationships in WFP. It is an expression of intent, in that it establishes that a specific record type (like a *channel tactic*) is allowed to be linked to other objects, whether they live in the workflow module or within planning itself. 

 

### Deciding to connect 

Establishing this allowance is a configuration-level decision that typically happens before any work is created. By adding a connection field, you are architecting your environment to support a "strategic thread," regardless of how the individual records are eventually created. 

 

## Strategy and execution in sync 

To keep your strategic layer focused, we recommend focusing your planning records on high-level intent while using the Workflow module for tactical execution. This approach uses the unique strengths of both modules: 

 

*   **Workfront Planning (The strategic layer):** Stays high-level. It tracks the *Campaign*, the *Channel Tactic*, and the *Budget*. It is noise-free and executive-ready. 

*   **Workflow module (The execution layer):** Manages the tactical details. Individual "Experiences" or "Activities" are managed here as **projects, tasks, and issues**. 

 

## Activating the bridge: From intent to action 

Once the connection is configured, you must decide how to activate the link between a specific strategic record and an execution project. 

 

### Professional triage: The table-led path 

Strategists and power users often use the **table view** as their "workbench" to refine plans over time.  

*   **Deliberate handoff:** By default, creating a record in a table does not establish a link to the Workflow module. The connection to an execution project is established when a user decides to activate the link. This can be done by manually creating a downstream connected project directly from the connection field in WFP or an optional **connection view page** in the record's detail view. Note that manual creation results in a blank project without specific custom forms; for more complex needs, you can use a **native WFP automation**. These automations are available when you select a row in a table, appearing as buttons in the blue action bar at the bottom of your screen. This allows for human oversight or placeholder creation, ensuring that projects are only generated in your workflow environment when they are truly needed. 

 

### Automated activation 

For organizations with high-volume requests or advanced automation needs, the bridge can be activated automatically based on specific events or field values. 

*   **Submission triggers:** Because forms provide a single, clean "submission event," they can be used as triggers for **Fusion automations**. A scenario can detect a form submission and immediately generate a linked project in the workflow module. 

*   **Field-value triggers:** For deeper automation, you can configure **Fusion** to monitor specific fields. For example, a simple checkbox labeled "ready for execution" can serve as the catalyst, establishing the bridge automatically the moment it is checked. 

 

## Surfacing visibility: Lookup fields 

Once a project is linked, you can surface real-time data from the Workflow module directly within the WFP record. 

 

A workspace manager can set up **lookup fields** to pull any native or custom field from the linked project (such as *actual completion date* or *creative lead*) into the WFP record type. Once captured, this data can be rolled up through multiple levels of your strategic hierarchy—even all the way to the campaign level. This provides powerful aggregate reporting for stakeholders across the entire marketing lifecycle, keeping them informed without needing to leave the planning environment. 

 

## Strategy-to-action visibility 

The ultimate value of the bridge is **real-time visibility**. By connecting intent to action, you can answer critical business questions at a glance: 

 

*   "Is our 'FY26 Brand Awareness' campaign actively delivering results right now?" 

*   "Where do our strategic tactics need more creative support to stay on schedule?" 

*   "How are we aligning our resources with our highest-priority strategic pillars?" 

 

## Best practices & tips 

 

### Do: 

*   **Use the "strategic thread" metaphor.** Remind teams that every project should be a "bead" on a strategic string. 

*   **Automate the handoff.** Use automations to trigger project creation to save time and effort while also improving data connectivity and governance. 

*   **Link, don't duplicate.** Use lookup fields to surface real-time execution data (like status or completion dates) in your strategic records. This ensures your strategic views are always accurate without requiring manual updates from your team. 

 

### Don't: 

*   **Don't treat planning records as task lists.** The bridge is designed to connect strategic intent to execution projects. Keep your planning records focused on the "what" and "why," and let the workflow module handle the granular "how" through tasks and issues. 

*   **Don't over-sync.** You don't need to sync every project-level detail back to Planning. Keep the strategic layer high-level and noise-free. 

*   **Don't bypass the bridge.** If work starts in the Workflow module without a link to Planning, you've created a "Shadow Plan" that is invisible to leadership. 

-->



