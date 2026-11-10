---
title: Introdução ao Espaço de ideação para planejamento do Adobe Workfront
description: O Adobe Workfront Planning agora oferece um recurso adicional para identificar antes de você iniciar suas campanhas. Aproveite o potencial da IA para transformar dados e direcionar entradas em planos tangíveis e dar às equipes um ponto de partida informado, em vez de uma página em branco.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: eb361af2-3e4f-4a79-b5f3-7a344ac5794c
    internal-label: Workfront Planning
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 215b8f1bf28e8df2b95c4f0519ffebcbcaa8df16
workflow-type: tm+mt
source-wordcount: '1311'
ht-degree: 0%
---

# Introdução ao espaço de ideação para o Adobe Workfront Planning

<!--
Should we add a new Feature to ExL for "Strategic Ideation"?
-->

<!--
information in this article come from this document, in addition to my notes for this project up to August 31, 2026:
https://adobe-my.sharepoint.com/:w:/r/personal/alinaw_adobe_com/_layouts/15/Doc.aspx?sourcedoc=%7B513DE769-B70B-4040-8C9E-6A9B8E3167BB%7D&file=getting-started-catalyze.docx&action=default&mobileredirect=true
-->

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ele está disponível somente como parte do programa **Espaço de ideação Beta**. </span>\
</span>

>[!IMPORTANT]
>
>As informações neste artigo se referem ao Adobe Workfront Planning. Sua empresa deve adquirir um pacote adicional do Planning para acessar o Workfront Planning.
>
>A funcionalidade descrita aqui não estará disponível se sua organização tiver adquirido o Workfront Planning como um produto independente.
>
>Para obter informações gerais sobre o Workfront Planning, consulte [Introdução ao Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).
> 
>

<!--
Future - when they make it available in Planning: replace the above with this OR ... insert the snippet:

>[!IMPORTANT]
>
>The information in this article refers to Adobe Workfront Planning which your organization can purchase either as an Adobe Workfront package or a standalone product. 
>
>Not all capabilities included in the Planning package are available to Workfront Planning when it is purchased as a standalone product. 
>
>For general information about Workfront Planning, see [Get started with Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).
> 
>For information about Workfront Planning as a standalone product, see [Get started with Adobe Workfront Planning as a standalone product](/help/quicksilver/planning/planning-sta/planning-sta-overview.md). 
>
-->

O espaço Adobe Ideation é o recurso de ideação estratégica alimentado por IA da Adobe, integrado diretamente ao Workfront Planning. Ele oferece às equipes de marketing um ponto de partida estruturado e informado por dados para a estratégia de campanha, substituindo a pesquisa e a adivinhação manuais por resumos gerados por IA com base no histórico de desempenho real de uma organização.

Acessível somente pelo Workfront Planning ou pelo Menu principal do Workfront, o espaço de ideação está localizado na parte frontal do ciclo de vida da campanha, antes do planejamento, da produção e do delivery, e se alimenta diretamente no espaço de trabalho do Workfront Planning, onde as equipes planejam e executam seu trabalho.

Os espaços de ideação usam o Adobe Enterprise CX Coworker para gerar resumos que podem ser convertidos posteriormente em registros do Planning ou baixados como PDFs.

## Disponibilidade do produto

A linha do tempo de lançamento planejada para o espaço de ideação que está sujeito a alterações inclui os seguintes marcos:

* **Beta fechado:** lançado em julho de 2026, para um pequeno número de clientes.

  O espaço de ideação está disponível no ambiente de Produção para clientes participantes.
* **Abrir Beta:** Direcionado para 12 de novembro de 2026. Essa é uma oferta de aceitação, em que você deve ativar ativamente a opção, em vez de recusá-la ativamente.

  O espaço de ideação está disponível nos ambientes de produção, pré-visualização e sandbox para todos os clientes que atendem a todos os outros requisitos.

* **Disponibilidade geral:** programada para 1º de fevereiro de 2027.

## Requisitos do produto

<!--section duplicated here: help/quicksilver/planning/ideation/access-needed-to-use-ideation-space.md-->

>[!NOTE]
>
>Não é necessário um logon separado para acessar o espaço de ideação. Ela estará disponível imediatamente se você puder fazer logon no Workfront se também tiver o Workfront Planning.
>
>Para obter mais informações sobre o acesso necessário para usar o espaço de ideação, consulte [Acesso necessário para usar o espaço de ideação](/help/quicksilver/planning/ideation/access-needed-to-use-ideation-space.md).

É possível acessar o espaço de ideação se sua organização e você tiverem acesso ao seguinte:

* Provedores de nuvem:

  * AWS

    Os provedores Azure e GCP não são compatíveis.

* Produtos:

  * Adobe Workfront com o Workfront Planning
  * Adobe Enterprise CX Coworker para Workfront

    >[!IMPORTANT]
    >
    >No momento, o Adobe CX Enterprise Coworker não está disponível para organizações nos setores de assistência médica, financeiro ou de alguns outros setores com dados confidenciais. O Assistente de IA está disponível para essas organizações, mas o espaço de ideação não está disponível para clientes do Workfront que não têm Colaborador.

* Pacotes do Adobe:

  * Durante a versão do Open Beta (a partir de 12 de novembro de 2026), você deve ter o seguinte:

    * Um pacote de fluxo de trabalho do Adobe Workfront com um pacote do Workfront Planning

  * Após a versão de Disponibilidade geral (prevista para 1º de fevereiro de 2027), você poderá ter um dos seguintes itens:

    * Um pacote de fluxo de trabalho do Adobe Workfront com um pacote do Workfront Planning
    * Um produto Adobe Workfront Planning como independente




<!--not required anymore: * Adobe GenStudio for Performance Marketing-->

<!-- only required for closed beta, see below: * Adobe Customer Journey Analytics-->

<!--
No longer required or recommended, per Et:

In addition to above requirements, you must also meet the following criteria to participate in the Closed Beta program: 

* Have an active Adobe Customer Journey Analytics (CJA) account with campaign tracking in place
* Have multi-channel campaigns with a repeatable planning process
* Actively use Workfront Planning for marketing operations
* Have at least one identified strategist or ideation user who will be the primary Ideation space user
-->

## Público-alvo e casos de uso

O espaço de ideação foi projetado para profissionais de marketing de produtos e marcas responsáveis por definir a estratégia da campanha e produzir resumos da campanha.

<!--
Too much: 

| Role | Primary job to be done |
|---|---|
| Brand Marketer | Identify messaging, trends, and cultural shifts that resonate with target audiences |
| Product Marketer | Launch insight-driven, culturally relevant campaigns that deliver business impact |
| Collaborators | Internal creative studios, external agencies, media planners/managers, and executives who need visibility into strategic direction |
-->

Como um gerenciador de espaço de trabalho, você pode usar o Espaço de ideação para criar registros no Workfront Planning seguindo as seguintes etapas:

* Crie um breve no espaço Ideação depois de iniciá-lo no Planning, conforme você começa a criar ou editar registros.
* Use os prompts de IA para coletar detalhes de outros registros no seu sistema ou da Web e finalizar a criação de resumos de ideação.
* Crie tipos de registro do Planning a partir dos resumos.
* Refine seus resumos de ideação e atualize os tipos de registro existentes no Planning.

Veja a seguir casos de uso para saber como usar o Espaço de ideação:

* **Atualizar uma campanha anterior usando o desempenho histórico**

  * Por exemplo, você pode atualizar campanhas existentes para um novo trimestre, temporada ou momento do produto.
  * Isso produz um &quot;resumo delta&quot; com base em um desempenho anterior, descrevendo o que permanece, quais alterações e por quê.

* **Criar uma nova campanha usando o desempenho histórico**

  * Por exemplo, você pode criar uma campanha ao iniciar um novo produto, segmento ou iniciativa sem um histórico de campanha direto.
  * Isso produz um resumo novo por meio da ideação guiada, uma combinação de canais recomendada e o conceito inicial ou as direções da mensagem.

## Espaço de ideação e a Adobe CX Enterprise Coworker

O espaço de ideação usa o Adobe CX Enterprise Coworker como sua interface de prompt.

Os usuários podem fazer perguntas de acompanhamento e refinar um breve diálogo em vez de obter um único resultado instantâneo.

Quando um resumo é vinculado a um registro ativo do Workfront Planning, o Colaborador impede a substituição dele para que o plano subjacente permaneça intacto. O registro é sobreposto somente quando você exporta o resumo para o Workfront Planning.

<!--
Previous intro but oped for the more direct one above: 
The Ideation space is a collaborative strategic marketing ideation tool for brand and product marketers to build stronger campaigns faster and with better team alignment. It grounds AI suggestions in real-marketing context — past briefs, performance data, audience insights, brand guidelines, and existing campaign assets — so results are relevant, not generic.

Ideation space works exclusively with the CX Enterprise Coworker for Workfront as the prompting agent for all its capabilities. 
-->

A seguir estão alguns dos recursos do Colaborador quando usados no espaço de ideação:

* Fazer upload de documentos ou insights sociais
* Acessar o conteúdo da Web pertinente ao resumo que você está criando
* Definir uma meta de campanha
* Obter um resumo dos insights do público
* Gerar personalidades de público
* Mensagens de campanha de ideias
* Trabalhe em uma tela visual grande, usando prompts de IA para gerar texto, imagem, arquivo, gráfico e cartões insight
* Organize, revise e expanda cartões para eventualmente traduzi-los em resumos de campanha
* Colabore com vários usuários que podem adicionar ideias, deixar comentários em itens específicos da tela ou usar notas adesivas para ideias de forma livre antes que um resumo seja finalizado
* Recomendamos as seguintes práticas recomendadas ao usar o Colaborador no espaço de ideação:

  * **Seja específico**. Descrições de campanha mais ricas produzem cartões mais relevantes e com melhor base.
  * **Verifique antes de finalizar**. As respostas geradas por IA podem ser imprecisas, portanto, sempre verifique **Fontes** em um cartão e confirme em relação às fontes vinculadas antes de finalizar um registro.
  * **Misture cartões de IA com registros reais**. Arraste e solte registros reais no espaço de ideação.

## Obter acesso ao espaço de ideação

Para obter acesso ao espaço de ideação:

1. Verifique se você atende aos requisitos do produto conforme descrito na seção [Requisitos do produto](#product-requirements) deste artigo.
1. Entre em contato com seu representante de conta da Adobe para expressar interesse em participar do Closed Beta ou associar-se ao Open Beta, quando ele estiver disponível.

   Os administradores do sistema têm acesso ao espaço de ideação por padrão e não podem removê-lo quando ele se torna disponível no Open Beta. Eles podem ativá-lo para todos os outros usuários.
1. (Recomendado) Identifique a primeira campanha: uma recente para atualizar ou uma nova iniciativa para criar do zero.

Para obter mais informações sobre como usar o espaço de ideação, consulte também os seguintes artigos:

* [Acesso necessário para usar o espaço de ideação](/help/quicksilver/planning/ideation/access-needed-to-use-ideation-space.md)
* [Criar registros do Planning a partir de resumos de espaço de ideação](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md)
* [Criar resumos no espaço de ideação](/help/quicksilver/planning/ideation/create-briefs-in-ideation-space.md)

## Localize o espaço de ideação

Depois de garantir o acesso aos produtos, pacotes e sistema adequados e ao nível de acesso configurado, é possível localizar o espaço de ideação nas seguintes áreas do Workfront:

* Ao adicionar manualmente um novo registro no Workfront Planning

  ![Espaço de ideação em planejamento](assets/ideation-space-in-planning-new-record.png)
* No menu principal do Workfront, abrindo a área Espaço de ideação

  ![Área do espaço de ideação no menu principal](assets/ideation-space-area-icon-in-main-menu.png)

>[!TIP]
>
>Não é possível remover a área Espaço de ideação do menu Principal usando um modelo de layout. Para obter mais informações sobre como bloquear o acesso de um usuário ao espaço de ideação, consulte [Acesso necessário para usar o espaço de ideação](/help/quicksilver/planning/ideation/access-needed-to-use-ideation-space.md).
>

## Objetos gerados pelo espaço de ideação

Você pode usar o espaço de ideação para debater e formular ideias que poderão ser convertidas posteriormente em itens importantes para o seu fluxo de trabalho.

O espaço de ideação pega todas as suas ideias e informações de fontes internas ou externas (Web) e cria um resumo. Depois de decidir que o resumo está concluído, você pode exportá-lo para os seguintes arquivos ou objetos:

* Um dos seguintes formatos de arquivo: PDF, Word, PowerPoint, modelo do PowerPoint
* Um registro do Planning

  É possível exportar um resumo para um registro de Planejamento somente quando você acessa o espaço de Ideação do Workfront Planning ou quando você conecta anteriormente um registro de Planejamento a um resumo de Ideação.

<!--
**************** CONSIDER INCLUDING THIS INFORMATION FROM JESH BARLOW ABOUT COWORKER IN CATALYZE?? - https://adobecorpdev.slack.com/archives/C091C0Y735W/p1788917610365089?thread_ts=1788917251.550099&cid=C091C0Y735W

Catalyze Coworker needs — panel inside Catalyze, not a rail from Unified ShellWhy this matters. Catalyze is AI-first. You can't use it without a prompt, so the prompting surface can't be something you open and close from Unified Shell. Coworker's rail was built to bolt onto apps that already work fine without AI. We need the opposite.

What we need

* Coworker embedded as a panel inside Catalyze (the Photoshop/Illustrator model), always present, minimized or expanded, never fully closeable.
* Not the Unified Shell rail that slides in, pushes the app, and only opens and closes from the shell.
* Quick terminology flag, since Coworker inverts it. By "panel" we mean embedded in the app. Their team uses "panel" for the shell version, so we have to be explicit every time.


Must-haves

* Minimized and expanded prompt bar states that live inside Catalyze, not tied to the shell.
* Minimize, never close. There's no state where the prompt disappears.
* Full UI control over how the prompt behaves.
* Headless Coworker so the panel can always sit on the canvas.


Where it stands (Aug 20 Shell/Catalyze sync with Stephen Gould)

* Headless is technically possible. Coworker can be hosted in Catalyze's own front-end.
* But Horia's team has no capacity to build or own an in-app rail. Deeper embedding means Catalyze eng builds the panel and owns it going forward.
* The open question is ownership, one-time integration vs owning the panel long-term. Still unresolved, and it's the thing that decides this.


Worth noting

* Experience Workspace and Brand Visibility (AM) already run Coworker without the shell, so headless isn't net-new. Let's learn how they did it before anyone calls it infeasible.
* Next step everyone agreed on is getting clarity from Horia's team and Joshua on rail ownership.

*************************************
-->

<!--
## Additional resources

* [Adobe Workfront Campaign Planning](https://business.adobe.com/br/products/workfront/campaign-planning.html)
* [Adobe Workfront Planning documentation](/help/quicksilver/planning/planning-information.md)
* [Adobe GenStudio Overview](https://business.adobe.com/br/products/genstudio.html)
* [Adobe Customer Journey Analytics](https://business.adobe.com/br/products/adobe-analytics/customer-journey-analytics.html)

-->

<!--

Not sure if we should disclose this: 

## The problem the Ideation space solves

Before the Ideation space, campaign strategy relied on two slow, manual processes:

- **Gathering insights** — fragmented, time-consuming, and difficult when no prior audience data exists
- **Aligning stakeholders** — without a shared, data-backed "hook," executives, creatives, and channel partners often work from different assumptions, causing rework and delays

The Ideation space automates insight synthesis and generates a structured brief that gives everyone a shared starting point.
-->

<!--
## What's included, phase by phase

| Phase | Timeline | What's included |
|---|---|---|
| Closed Beta | July 2026 | Limited customers/users/campaigns; core agent skills (strategy framing, messaging ideation, audience definition, data ingestion, brief generation); CJA data integration |
| Open Beta | ~Sept 2026 (planned) | Quality/performance improvements; CJA integration refinements; Workfront Planning handoff; data visualization; Planning workspace structure ingestion; Unity/Conversational UI integration |
| General Availability | H2 2026 (planned) | Bring Your Own Data Source (BYODS); Workfront/Workfront Planning data integration; audience data integration; social data integration; workflow ingestion; strategy testing capabilities |

At GA, the Ideation space is also expected to be accessible through the GenStudio Home conversational UI, running as part of Adobe's Agent Orchestrator suite of agents.
-->