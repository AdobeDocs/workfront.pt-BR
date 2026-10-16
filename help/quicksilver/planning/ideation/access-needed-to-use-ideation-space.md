---
title: Acesso necessário para usar o espaço de ideação
description: O Adobe Workfront Planning agora oferece um recurso adicional para identificar antes de você iniciar suas campanhas. Aproveite o potencial da IA para transformar dados e direcionar entradas em planos tangíveis e fornecer às equipes um ponto de partida informado, em vez de uma página em branco com espaço Adobe Ideation.
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
source-git-commit: e209f8e5ada29b1c488fcfe42c13c6c9523a26bd
workflow-type: tm+mt
source-wordcount: '826'
ht-degree: 0%
---

# Acesso necessário para usar o espaço de ideação

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ele está disponível somente como parte do programa **Espaço de ideação Beta**. </span>

<span class="preview">Para obter mais informações, consulte [Introdução ao Espaço de ideação do Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).</span>


{{planning-important-intro}}

O Adobe Workfront Planning agora oferece um recurso adicional para identificar antes de você iniciar suas campanhas.

Ao usar o Espaço de ideação, você pode aproveitar os recursos de conversação do Adobe Enterprise CX Coworker para transformar dados e direcionar entradas em planos tangíveis e fornecer às equipes um ponto de partida informado, em vez de uma página em branco.

Este artigo descreve o acesso e as permissões que você deve ter para acessar o espaço de ideação no Workfront Planning.

Para obter informações gerais sobre o Espaço de ideação, consulte [Introdução ao Espaço de ideação para planejamento do Adobe Workfront](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).

## Requisitos do produto

O espaço de ideação não é um produto independente, mas um recurso adicional do Adobe Workfront Planning.

É possível acessar o espaço de ideação se sua organização e você tiverem acesso aos seguintes produtos:

* Adobe Workfront com o Workfront Planning
* Enterprise CX Coworker

Dependendo do acesso ao espaço de ideação, é necessário ter acesso aos seguintes pacotes:

* Durante a versão do Open Beta, você deve ter o seguinte:

  * Um pacote de fluxo de trabalho do Adobe Workfront com um pacote do Workfront Planning

* Após a versão de Disponibilidade Geral, você poderá ter uma das seguintes opções:

  * Um pacote de fluxo de trabalho do Adobe Workfront com um pacote do Workfront Planning
  * Um produto Adobe Workfront Planning como independente

>[!NOTE]
>
>O espaço de ideação só pode ser acessado no Menu principal do Workfront ou no Workfront Planning. Não é necessário um logon separado para acessar o espaço de ideação. Ela estará disponível imediatamente se você puder fazer logon no Workfront.

Para obter informações sobre os estágios de lançamento do espaço de ideação, consulte [Introdução ao espaço de ideação do Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).


<!--
No longer the case: 

Your organization must purchase a package for the following products to access the Ideation space: 

* An Adobe Workfront Workflow package in addition to a Planning package

    Or
    
    An Adobe Workfront Planning purchased as a standalone product. 
* An Adobe GenStudio for Performance Marketing license

    >[!TIP]
    >
    >GenStudio for Performance Marketing is needed to have access to the correct font entitlements. 

-->

<!--only required for closed beta:* An Adobe Customer Journey Analytics license that includes campaign tracking-->

## Requisitos do sistema e do nível de acesso

O acesso ao espaço de ideação é configurado no Workfront ativando uma combinação de configurações de nível de sistema e nível de acesso.

As seguintes configurações são necessárias para acessar o Espaço de ideação no Workfront:

* Ative as configurações de Preferências de Colaborador e MCP na área Preferências do Sistema da Instalação <!--check the UI because Becky was going to change it-->

  Para obter mais informações, consulte [Configurar preferências do sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

  >[!IMPORTANT]
  >
  >No momento, o CX Enterprise Coworker não está disponível para organizações nos setores de assistência médica, financeiro ou de alguns outros setores com dados confidenciais. O Assistente de IA está disponível para essas organizações. No entanto, o espaço de ideação não está disponível para clientes do Workfront que não têm o CX Coworker.

* Desmarque a configuração Desativar espaço de ideação na seção Definir restrição adicional do seu nível de acesso.

  >[!TIP]
  >
  >Como administrador do Workfront, você pode limitar o acesso ao espaço de ideação a determinados usuários, desmarcando a configuração Desativar espaço de ideação no nível de acesso.

  Para obter informações, consulte [Criar e modificar níveis de acesso personalizados](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Requisitos de licença

Seu nível de acesso Workfront deve incluir os seguintes tipos de licença para acessar o espaço de ideação:

* Uma licença de Fluxo de Trabalho Padrão, quando sua empresa comprou um pacote de Fluxo de Trabalho além de um pacote do Planning.
* Uma licença do Standard Planning, quando sua empresa comprou uma das seguintes opções:

  * Um Fluxo de trabalho e um pacote de planejamento, durante o Open beta
  * Um Workflow e um pacote do Planning ou um Workfront Planning como um produto independente, após a disponibilidade geral.

## Requisitos de permissões do Workfront

Quando você usa o espaço Ideação do Workfront Planning, cada registro do Planning é conectado a um resumo no espaço Ideação.

As permissões de resumo do espaço de ideação são herdadas das permissões de registro do Workfront Planning. <!--not sure if this is right, because now you can share the ideation with others??-->

Você deve ter permissões do Contribute ou superiores para um tipo de registro no Planning para criar registros a fim de criar ou editar um registro no espaço de ideação.

Os usuários do Planning com permissões de Exibição em registros podem exibir o espaço de ideação de um registro.

A tabela a seguir mostra a conexão entre as permissões de registro do Workfront Planning e as permissões de resumo do espaço de ideação:

| Permissão de nível de registro do Planning | Permissões de nível de resumo do espaço de ideação |
|---|---|
| Contribuir com permissões ou mais altas para um registro | Pode criar um resumo no espaço de ideação do registro |
| Exibir permissões para um registro | Pode ler o resumo desse registro no espaço de ideação, mas não pode modificá-lo |

## Permissões de espaço de ideação

<!--this is also duplicated in the intro of the Share an ideation space article-->

As permissões de planejamento são transferidas para o espaço de ideação de um registro.

Além disso, você pode conceder permissões a outros usuários para usar o espaço de ideação e adicionar ideias a ele.

Considere o seguinte:

* Os criadores de ideações sempre têm permissões de Editor em suas próprias ideações.

* Você deve ter permissões de Editor em um espaço de ideação para criar resumos e exportá-los para outros aplicativos.

A seguir estão as permissões de espaço de ideação e os recursos que elas oferecem:

| Permissão de espaço de ideação | Recursos |
|---|---|
| Editor | Pode editar, baixar e compartilhar o espaço de ideação |
| Comentarista | Pode exibir e comentar no espaço de ideação |
| Visualizador | Pode visualizar o espaço de ideação |

Para obter mais informações sobre como compartilhar um espaço de ideação, consulte [Compartilhar um espaço de ideação](/help/quicksilver/planning/ideation/share-the-ideation-space.md).

<!--
there is no additional setup for Workfront layout template assignment because Contributors an below cannot access Ideation space; only Standard users
-->


<!-- 
Not sure if this is needed. Maybe all orgs have IMS for all Adobe?? - asking Becky: 

## Org/IMS-level entitlements

Beyond Planning access itself, a customer's IMS Org needs specific entitlements for the full Ideation space experience to work:

| Requirement | Type | Why it matters |
|---|---|---|
| IMS Org with Workfront Planning | Org requirement | Baseline product access |
| IMS Org with GenStudio PEM | Org requirement | Provides the font entitlements and storage needed to use the Ideation space |
| Fonts entitlement | Entitlement | Missing entitlement can block the full Ideation space experience |
| Adobe Cloud Platform / document storage entitlement | Entitlement | Existing documentation indicates users may be able to reach ideation entry points but fail during actual usage if storage-related entitlements are missing |

Historically, some customer teams relied on GenStudio (GenS) provisioning without realizing they could use the Ideation space directly — provisioning conversations should confirm both Planning and GenStudio PEM entitlements are explicitly set up for the Ideation space, not just assumed via GenS.
-->



<!--
From Claude: Internal information, not customer-facing: 

The permissions and entitlement model below reflects what was documented and confirmed as of the Closed Beta (through Aug 2026). Internal teams were still finalizing a formal access-model document and access-level definitions at this time, so treat this as the current best understanding rather than a final spec — confirm against the latest internal documentation before publishing externally.

## Practical checklist for provisioning a customer

1. Confirm the customer has Workfront Planning (via Workflow+Planning or Planning standalone).
2. Confirm the customer's IMS Org has GenStudio PEM entitlements provisioned (not just assumed).
3. Confirm font and document-storage entitlements are active — test actual usage, not just entry-point visibility.
4. Confirm the "strategic ideation" product is enabled at the org level.
5. During Closed Beta, confirm the user-level feature flag is set for named ideation users.
6. Confirm the target users have **create** (not just view) access to the records they need to ideate on.
7. If the Coworker integration inside the Ideation space is in scope, verify its availability separately.

## Packaging

| Detail | Description |
|---|---|
| Included with Workfront Planning | Yes |
| Standalone option | Can also be launched as its own surface |
| Agent platform | Runs within the Adobe Agent Orchestrator |
| Billing | Monetized through Adobe's AI-credits framework |
-->

<!--

Original Claude write-up, in addition to the info above:

## Baseline product requirement

The Ideation space isn't a standalone purchase — you need **Workfront Planning** to access it, through either:

- Adobe Workfront Workflow with a Workfront Planning package, or
- Adobe Workfront Planning as a standalone product

If your org has Workfront Planning, it has the Ideation space too. The Ideation space can't exist without Planning.

For the Closed Beta and Open Beta, the Ideation space is available only to Planning and GenStudio (GenS) customers.

## Customer-level entry requirements (Closed Beta)

To participate in the Closed Beta, customers needed to meet these criteria:

- An active Adobe Customer Journey Analytics (CJA) deployment with campaign tracking in place
- Multi-channel campaigns with a repeatable planning process
- Active use of Workfront Planning for marketing operations
- At least one identified strategist or ideation user who will be the primary Ideation space user

## Org- and user-level enablement

- Workfront surfaces the Ideation space integration to users only after a Workfront administrator enables the **strategic ideation** product at the org level.
- During the Closed Beta, a user-level feature flag also controls access, so org-level enablement alone isn't enough.
- For Open Beta, access is expected to move to an opt-in model, where customers actively configure themselves in, rather than opt-out.

## Record-level permissions

Your Ideation space permissions come from your Workfront Planning record permissions — there's no separate permission system layered on top:

- If you can create a record in Planning, you can also create a canvas in the Ideation space. Any Planning license is sufficient for this.
- If you have read-only access to a record, you have read-only access to the canvas connected to that record.
- If you only have view access to an existing record, you can't open the Ideation space from it. Workfront shows an "Insufficient permissions" message instead.
- Each canvas is related to exactly one record.

>[!NOTE]
>As of August 2026, the team was still defining discrete access levels for the Ideation space. These are expected to include, at minimum, Can read, Can view, and Can create.

## Org and IMS-level entitlements

Beyond Planning access, your organization's IMS Org needs specific entitlements for the Ideation space to work fully.

| Requirement | Type | Why it matters |
|---|---|---|
| IMS Org with Workfront Planning | Org requirement | Baseline product access |
| IMS Org with GenStudio PEM | Org requirement | Provides the font entitlements and storage needed to use the Ideation space |
| Fonts entitlement | Entitlement | A missing entitlement can block the full Ideation space experience |
| Adobe Cloud Platform or document storage entitlement | Entitlement | Users may be able to reach Ideation space entry points but fail during actual use if storage-related entitlements are missing |

>[!IMPORTANT]
>When you provision a customer, confirm that both the Planning and GenStudio PEM entitlements are set up specifically for the Ideation space. Don't assume that GenStudio (GenS) provisioning alone includes Ideation space access.

## Content-sharing and abuse controls

Because the Ideation space lets you create content and share it with other users through Adobe systems, a **Report Abuse** capability is planned as a requirement before General Availability (GA). Workfront needs this roughly one month ahead of GA to support Adobe's platform license agreement process. This capability may reuse the existing Report Abuse functionality from Adobe Horizon rather than being built from scratch.

## Coworker (conversational AI) access

Access to the **Coworker** integration inside the Ideation space, the conversational right-rail assistant, is being rolled out separately from core Ideation space and Planning access:

- As of mid-August 2026, Coworker access wasn't yet generally available for customer testing.
- By August 17, 2026, Coworker was available inside the Ideation space for internal use, but still being refined.
- If you're documenting or testing the Coworker integration inside the Ideation space specifically, verify current availability separately. Don't assume it's included automatically with standard Planning or Ideation space provisioning.

For more information, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

-->
