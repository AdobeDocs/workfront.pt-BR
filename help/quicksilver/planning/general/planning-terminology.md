---
title: Visão Geral da Terminologia do Workfront Planning
description: Embora o Adobe Workfront Planning seja um produto Workfront, ele vem com conceitos e terminologia proprietários. Não se esqueça de se familiarizar com esses conceitos antes de iniciar a configuração do Workfront Planning para sua organização.
author: Alina
feature: Workfront Planning
role: User, Admin
source-git-commit: f8dfa5a4aec4541d885bcc45933488cd1fdefac4
workflow-type: tm+mt
source-wordcount: '1555'
ht-degree: 59%

---

# Visão geral da terminologia do Workfront Planning


<!--do not use the snippet for IMPORTANT as it links to this article-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

>[!IMPORTANT]
>
>As informações neste artigo se referem ao Adobe Workfront Planning. O Workfront Planning é um produto independente ou um recurso adquirido adicionalmente do Adobe Workfront.
>
>
>Este artigo contém informações gerais sobre o Workfront Planning quando os clientes também compram um pacote do Workfront ou Workflow.
>
>Para obter a lista completa de artigos que contêm a documentação do Workfront Planning, consulte [Informações gerais e índice do artigo do Adobe Workfront Planning](/help/quicksilver/planning/planning-information.md).
>
>Para obter informações sobre o Workfront Planning como um produto independente, consulte [Introdução ao Adobe Workfront Planning como um produto independente](/help/quicksilver/planning/planning-sta/planning-sta-overview.md).

Embora o Workfront Planning faça parte do Workfront, ele vem com conceitos e terminologia próprios. Não se esqueça de se familiarizar com esses conceitos antes de iniciar a configuração do Workfront Planning para sua organização.

A estrutura do Workfront Planning é totalmente personalizável. Você pode criar todos os tipos de registros, seus atributos e quaisquer campos associados a eles para atender às necessidades específicas da sua organização.

Existem limitações quanto ao número de objetos do Workfront Planning que você pode criar. Para obter mais informações, consulte [Visão geral das limitações de objetos Adobe Workfront Planning](/help/quicksilver/planning/general/limitations-overview.md).

A seguir estão os principais objetos e conceitos do Workfront Planning:

* [Espaços de trabalho](#workspaces)
* [Tipos de registro](#record-types)
* [Registros](#records)
* [Modelos de espaço de trabalho](#workspace-templates)
* [Campos](#fields)
* [Tipos de registro, registros e campos conectados](#connected-record-types-records-and-fields)
* [Campos de pesquisa](#lookup-fields)
* [Hierarquias](#hierarchies)
* [Exibições](#views)
* [Automações](#automations)
* [Formulários de solicitação](#request-forms)

## Espaços de trabalho

Os espaços de trabalho representam a estrutura de uma unidade organizacional. São coleções de tipos de registro que definem o ciclo de vida operacional de uma determinada organização.

![Espaço de trabalho de marketing com taxonomias de tipos de registros na página inicial](assets/marketing-workspace-with-record-type-taxonomies-opening-page.png)

Para obter mais informações, consulte [Criar áreas de trabalho](/help/quicksilver/planning/architecture/create-workspaces.md).

## Tipos de registro

Os tipos de registro são os tipos de objeto no Workfront Planning.

Os tipos de registro preenchem as áreas de trabalho.

Ao contrário do Workfront, onde os tipos de objeto são predefinidos, no Workfront Planning você pode criar seus próprios tipos de objeto.

Por exemplo, no Workfront, os tipos de objeto Programa, Portfólio, Projeto, Tarefa ou Problema já estão criados.

No Workfront Planning, você pode criar qualquer tipo de registro que atenda aos fluxos de trabalho da sua organização. Posteriormente, você poderá definir como os tipos de registros se relacionam entre si ou formam dependências.

Para obter mais informações, consulte [Visão geral dos tipos de registros](/help/quicksilver/planning/architecture/overview-of-record-types.md).

## Registros

Um registro é uma instância de um tipo de registro.

![Registros destacados na lista de tipos de registros da campanha](assets/records-highlighted-in-campaign-record-type-list.png)

Depois de adicionar um tipo de registro a um espaço de trabalho, você pode começar a adicionar registros desse tipo na página do tipo de registro.

Por exemplo, “Campanha” pode ser um tipo de registro e “Campanha de verão para EMEA” é um registro do tipo de registro Campanha.

Para obter mais informações, consulte [Criar registros](/help/quicksilver/planning/records/create-records.md).

## Modelos de espaço de trabalho

Você pode criar um espaço de trabalho usando modelos predefinidos. Você pode usar os tipos de registros e campos predefinidos que vêm em um modelo ou pode adicionar os seus próprios.

![Página de espaços de trabalho com miniaturas de modelos](assets/workspaces-page-with-templates-thumbnails.png)

O Adobe Workfront Planning contém os seguintes modelos:

* Operações do Initiative Studio
* Communications Planning Studio
* Básico: Gestão de Marketing
* Avançado: Gestão de Marketing
* Corporativo: Gestão de Marketing
* Gestão de vendas
* Gerenciamento de produtos

Os administradores do sistema também podem instalar seis espaços de trabalho ao usarem o modelo multiespaço de prática recomendada. O template de vários espaços contém os seguintes templates que geram 6 espaços de trabalho separados, mas conectados ao mesmo tempo:

* 1.Classificações e taxonomias globais
* 2.Fréscopa Marketing Global
* 3.Fréscopa Marketing Social
* 4.Fréscopa Mídia e RP
* 5.Eventos globais da Fréscopa
* 6.Fréscopa Liderança da Empresa Executiva

Para obter mais informações, consulte os seguintes artigos:

* [Lista de modelos de espaço de trabalho](/help/quicksilver/planning/architecture/workspace-templates.md).
* [Criar espaços de trabalho](/help/quicksilver/planning/architecture/create-workspaces.md).

## Campos

Os campos são atributos que podem ser adicionados aos tipos de registro. Os campos contêm informações sobre o tipo de registro.

![Lista suspensa de campos de registro](assets/drop-down-list-of-record-fields.png)

Considerações sobre campos de registro:

* Os campos que você adiciona para um tipo de registro são automaticamente associados a todos os registros desse tipo e podem ser usados para capturar dados sobre esses registros.

* Os campos são exibidos como colunas na visualização Tabela aplicada a uma página do tipo registro. Eles também são exibidos na página do registro.

* Os campos são exclusivos de um tipo de registro e não são transferidos de um para outro.

* Os campos são totalmente personalizáveis e podem ser acessados somente no Workfront Planning. Não é possível acessar os campos do Workfront Planning no Workfront.

Para obter mais informações, consulte [Criar campos](/help/quicksilver/planning/fields/create-fields.md).

Um novo tipo de registro está associado aos seguintes campos predefinidos, por padrão:

* Nome
* Descrição
* Data de início
* Data final
* Status

Você pode criar campos personalizados dos seguintes tipos:

* Texto de linha única
* Parágrafo
* Seleção múltipla
* Seleção única
* Data
* Número
* Porcentagem
* Moeda
* Caixa de seleção
* Fórmula
* Pessoas
* Criado por
* Data de criação
* Última modificação por
* Data da última modificação
* Aprovada por
* Data de aprovação
* ID do registro

<!--update the screen shot above-->

## Tipos de registro, registros e campos conectados

Você pode criar uma conexão entre as seguintes entidades no Workfront Planning:

* Dois tipos de registro do Workfront Planning.
* Um tipo de registro e um tipo de objeto de projeto, programa, portfólio, empresa ou grupo do Workfront.
* Um tipo de registro e um ativo ou pasta do Adobe Experience Manager.

  Você deve ter uma licença do Adobe Experience Manager para conectar tipos de registro com objetos do Experience Manager.

  ![Nova guia de conexão com opções do Workfront AEM](assets/new-connection-tab-with-workfront-aem-options.png)

* Um tipo de registro e uma marca do Adobe GenStudio for Performance Marketing.

  Você deve ter uma licença do Adobe GenStudio for Performance Marketing para conectar tipos de registros às Marcas GenStudio.

  ![Guia Nova conexão com a opção Marca do Adobe GenStudio](assets/new-connection-tab-with-genstudio-option.png)

Depois de estabelecer uma conexão entre os tipos de registro ou os tipos de registro e objeto, você pode conectar registros ou objetos individuais desses tipos uns aos outros. A conexão entre os registros é exibida como um campo de registro conectado, ou uma conexão.

Conectar tipos de registro é útil quando você tem vários tipos de objetos de trabalho que afetam uns aos outros. Por exemplo, você pode trabalhar com campanhas, e cada campanha pode atender a várias marcas. Para indicar essa relação, você pode conectar campanhas a marcas. Além disso, o trabalho de cada campanha pode ser planejado em vários projetos no Workfront. Para indicar isso, você pode conectar as campanhas aos projetos relevantes. Conectar tipos de registro e, em seguida, conectar registros individuais estabelece essa relação no Workfront Planning.

## Campos de pesquisa

Depois de estabelecer a conexão entre dois tipos de registro e conectar registros individuais, é possível fazer referência aos campos a partir dos registros conectados do registro a partir do qual você está se conectando.

Por exemplo, se você conectar um tipo de registro Campanha a um tipo de objeto Projeto do Workfront, é possível exibir o campo Orçamento dos projetos conectados nos registros da campanha.

![Adicionar caixa de campos de pesquisa](assets/add-lookup-fields-modal.png)

>[!TIP]
>
>* Você não pode adicionar os seguintes tipos de campo como campos de pesquisa a partir dos tipos de registro ou objeto conectados:
>
>   * Criado por
>   * Última modificação por
>   * Campos de preenchimento automático do Workfront (incluindo campos como Proprietário do projeto ou Patrocinador do projeto)
>

Para obter informações sobre como conectar tipos de registros, registros e criar campos vinculados, consulte os seguintes artigos:

* [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md)
* [Conectar registros](/help/quicksilver/planning/records/connect-records.md)

<!--
not yet:* Fields are reusable across Record Types.
-->

## Hierarquias

Depois que os tipos de registro forem conectados em um espaço de trabalho, você poderá criar hierarquias que organizam essas conexões. As hierarquias organizam tipos de registro e objeto em relacionamentos pai-filho e podem conter até quatro tipos de objeto.

![Hierarquias na área Configurações do espaço de trabalho](assets/hierarchies-in-workspace-settings-area.png)

Se uma conexão entre dois tipos de registro ainda não existir, ela poderá ser criada conforme você configura a hierarquia. Uma vez definida, a hierarquia estabelece um caminho estruturado entre tipos de registro relacionados no espaço de trabalho.

As hierarquias geram navegações estruturais para seus respectivos registros que são exibidos em seus cabeçalhos. Dessa forma, os usuários sabem onde estão na hierarquia em qualquer estágio do fluxo de trabalho.

Para obter informações gerais sobre hierarquias e navegações estruturais, consulte [Visão geral sobre hierarquia e navegação estrutural](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

## Exibições

Os registros são exibidos em sua respectiva página de tipo de registro em diferentes tipos de exibições.

![Menu suspenso de tipos de visualização da lista de tipos de registros](assets/view-types-drop-down-from-record-type-list.png)

As exibições contêm configurações personalizadas de um tipo específico de visualização, como a lista de campos (colunas), uma lista de registros (linhas), sua ordem (classificação), um filtro aplicado ou aplicável e um agrupamento.

A seguir estão os tipos de exibição que você pode aplicar à página do tipo de registro:

* **Exibição em tabela**: exibe registros e seus campos, incluindo campos conectados e de pesquisa, em formato de tabela. As linhas da tabela são os registros individuais e as colunas são os campos dos registros. A exibição em tabela é a exibição padrão.

  ![Exemplo de exibição em tabela](assets/table-view-example.png)

* **Exibição da linha do tempo**: exibe registros que possuem pelo menos dois campos do tipo Data em uma linha do tempo cronológica. Você pode exibir até 5 tipos de registros conectados e seus registros na visualização da linha do tempo.

  ![Agrupamento aplicado na exibição da linha do tempo](assets/grouping-applied-in-timeline-view.png)

* **Exibição de calendário**: exibe registros que possuem pelo menos dois campos do tipo Data em formato de calendário.
  ![Exemplo de exibição do calendário](assets/calendar-view-example.png)

<!--
add List view here when it's possible to display Planning RTs in it??
-->

Exibição adicional:

* **Exibição de lista**: você pode exibir objetos em uma exibição de lista nas seguintes áreas do Workfront Planning:

  * Páginas conectadas de projetos.
  * Lista de formulários de solicitação

  ![Projetos conectaram página em uma exibição de lista](assets/list-view-projects-connected-page.png)

Para obter mais informações, consulte [Gerenciar exibições de registros](/help/quicksilver/planning/views/manage-record-views.md).

## Automações

Você pode configurar automações no Adobe Workfront Planning que, quando ativadas, criam registros no Workfront Planning quando acionadas a partir de um registro do Planning. Os registros criados são conectados automaticamente aos registros dos quais você está acionando a automação.

Você pode configurar e ativar a automação na página do tipo de registro no Workfront Planning.

Por exemplo, você pode criar uma automação que use uma campanha do Workfront Planning e crie uma Marca para associar à campanha.

Para obter informações sobre como criar objetos usando uma automação existente, consulte [Criar objetos usando as automações de registro do Adobe Workfront Planning](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).

## Formulários de solicitação

Você pode criar um formulário de solicitação e associá-lo a um tipo de registro no Adobe Workfront Planning. Em seguida, você pode compartilhar o formulário com outras pessoas, que podem enviar solicitações para criar registros desse tipo.

Para obter mais informações, consulte [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).