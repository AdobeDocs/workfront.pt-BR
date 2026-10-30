---
content-type: release-notes
title: Atividade da versão do primeiro trimestre de 2027 para o Adobe Workfront Planning
description: Esta é a atividade de lançamento do produto Adobe Workfront Planning para o primeiro trimestre de 2027.
author: Becky
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: a29813d3-f0cc-4b60-9396-13b558370803
    internal-label: Product announcements
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 65b1e818b321dd396720fb791e49e8ae9eb7af92
workflow-type: tm+mt
source-wordcount: '1191'
ht-degree: 0%
---
# Atividade da versão do primeiro trimestre de 2027 para o Adobe Workfront Planning

Este artigo descreve os recursos que estão sendo lançados para o Workfront Planning durante a versão do Primeiro Trimestre de 2027.

Para obter uma lista de todos os recursos lançados para o Adobe Workfront Planning, consulte [atividade de versão do Adobe Workfront Planning: índice do artigo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Melhor visibilidade de descobertas de pesquisa rápida na exibição de tabela

>[!NOTE]
>
>Visualização: 29 de outubro de 2026
>Versão rápida de produção: 12 de novembro de 2026
>Produção para todos: 21 de janeiro de 2027

Quando você usa a pesquisa rápida na exibição de tabela para localizar um item, a exibição elimina todos os registros que não correspondem à pesquisa e exibe apenas os itens que correspondem.

Antes desse aprimoramento, todos os registros eram exibidos com os que correspondiam aos resultados da pesquisa destacados.

Para obter informações, consulte [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md).

<!--

## Record-level permissions - restricted access to records

PLACEHOLDER: The release note field on the Workfront task points to an anchor story that no longer exists, so there is no description yet. Add the description and help link before unhiding.

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

-->

## Permitir a conexão de registros de tipos de registros globais conectados em espaços de trabalho secundários quando a conectividade entre espaços de trabalho estiver desativada

>[!NOTE]
>
>Visualização: 29 de outubro de 2026
>Versão rápida de produção: 12 de novembro de 2026
>Produção para todos: 21 de janeiro de 2027

Quando dois tipos de registros globais conectados são adicionados a um espaço de trabalho secundário, você pode desativar a conectividade entre espaços de trabalho e ainda vincular registros localmente.

Cada tipo de registro secundário exibe somente seus próprios registros para ambos os tipos de registro e pode conectá-los uns aos outros. Os registros do espaço de trabalho global e de outros espaços de trabalho secundários não são mais exibidos.

Antes desse aprimoramento, se a conectividade entre espaços de trabalho fosse desativada para tipos de registros globais conectados, os espaços de trabalho secundários não poderiam vincular seus próprios registros uns aos outros. Se ele fosse ativado, os usuários poderiam ver e vincular registros do espaço de trabalho global e de todos os outros espaços de trabalho secundários.

Para obter mais informações, consulte [Visão geral do tipo de registro entre espaços de trabalho](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).

## Exibir a contagem total de registros nas exibições de tabela, linha do tempo e lista

>[!NOTE]
>
>Visualização: 29 de outubro de 2026
>Versão rápida de produção: 12 de novembro de 2026
>Produção para todos: 21 de janeiro de 2027

As exibições de tabela, linha do tempo e lista agora mostram o número total de registros e a contagem de atualizações automaticamente à medida que você aplica filtros, pesquisa ou altera a exibição. A contagem de registros sempre reflete os resultados completos filtrados e respeita as permissões.

A contagem de registros é exibida à esquerda da caixa de pesquisa rápida, no canto superior direito da tabela, linha do tempo ou exibição de lista.

Para obter mais informações, consulte [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md).

<!--

## Field aggregators available for groupings in the table view

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

Grouped records in the table views now show a summary row for each grouping, plus a grand total for the full table. Groupings and the grand total use the same summary functions, and nested groupings get their own summaries that include all child records. Aggregators update automatically as you filter, search, regroup, or edit records.

For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md).

## Add sections to organize Planning views

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

You can now create sections in the Workfront Planning View dropdown menu to organize related views as your list grows. You can name each section when you create it, then move views from My Views and Shared with Me into your custom sections. System views stay fixed in the System section.

For information, see [Manage record views](/help/quicksilver/planning/views/manage-record-views.md).

-->

<!--

## Filters for Workfront objects connected record fields

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

You can now filter for certain Workfront object types that meet a filter criteria when you add them as a connected field in Planning.

Only those Workfront objects that meet your filtering criteria will display as options in connected fields when editing a record.

For this feature, we added a new Record filtering rules option in the New connection tab when connecting the following Workfront object types: projects, portfolios, programs, groups, companies. Prior to this enhancement, filters were available only when connecting two record types.

For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).

-->

## Limitações do número do campo de pesquisa

>[!NOTE]
>
>Visualização: 29 de outubro de 2026
>Versão rápida de produção: 12 de novembro de 2026
>Produção para todos: 21 de janeiro de 2027

Estamos introduzindo limites em quantos campos de pesquisa você pode adicionar a um tipo de registro:

* Até 40 campos de pesquisa por tipo de registro
* Até 5 campos de pesquisa de texto longo por tipo de registro. Os campos de pesquisa conectados são contados em relação ao limite de seu campo original.
* Até 50.000 caracteres no valor de uma única célula de pesquisa de texto longo. Se o conteúdo combinado dos valores de pesquisa exceder esse limite, os valores serão mostrados na ordem de conexão até que o limite seja atingido. O primeiro valor que excederia ele e todos os valores depois dele são omitidos. O campo original do objeto conectado nunca é alterado.

Você recebe um erro ao tentar criar ou editar um campo de pesquisa além dos dois primeiros limites. Os tipos de registro que já excedem esses limites não são afetados por essa alteração. Você pode editá-los, mas não pode adicionar mais campos ou valores de pesquisa até que esteja abaixo do limite.

Para obter informações, consulte [visão geral das limitações de objetos do Adobe Workfront Planning](/help/quicksilver/planning/general/limitations-overview.md).

## Agora os novos campos são exibidos somente na exibição em que você os cria

>[!NOTE]
>
>Visualização: 29 de outubro de 2026
>Versão rápida de produção: 12 de novembro de 2026
>Produção para todos: 21 de janeiro de 2027

Ao adicionar um novo campo a um tipo de registro, ele agora é mostrado somente na exibição em que você está trabalhando e oculto em todas as outras exibições existentes. Outras exibições permanecem configuradas e você pode reexibir o novo campo nelas, se necessário.

Antes desse aprimoramento, novos campos eram adicionados de forma oculta a cada visualização, às vezes causando confusão para usuários não familiarizados com os novos campos.

Para obter informações, consulte [Criar campos](/help/quicksilver/planning/fields/create-fields.md).

## Exportar detalhes do registro de qualquer modo de exibição

>[!NOTE]
>
>Visualização: 29 de outubro de 2026
>Versão rápida de produção: 12 de novembro de 2026
>Produção para todos: 21 de janeiro de 2027

Agora é possível exportar os detalhes de um registro de qualquer exibição de detalhes, sem precisar alternar para a exibição Todos os campos.

Anteriormente, a opção de exportação estava disponível somente quando a exibição Todos os campos era selecionada.

Para obter informações, consulte [Exportar os detalhes de um registro](/help/quicksilver/planning/records/export-the-record-page.md).

<!--

## Cancel and revert changes when editing records when business rules are violated

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

To ensure data integrity, when a business rule is violated while you edit a record, the change is blocked, the value reverts, and a toast notification explains why the edit is not allowed. The warning is visible in all areas where you are editing records, including the table view or details page.

If multiple rules are violated, each violation issues its own toast notification.

For more information, see [Configure business rules](/help/quicksilver/planning/architecture/configure-business-rules.md).

-->

## Desempenho aprimorado com carregamento de dados incremental nas visualizações de tabela e linha do tempo

>[!NOTE]
>
>Visualização: 29 de outubro de 2026
>Versão rápida de produção: 12 de novembro de 2026
>Produção para todos: 21 de janeiro de 2027

Para melhorar o desempenho em um grande número de registros, fizemos as seguintes melhorias nas exibições de tabela e linha do tempo:

* A exibição em tabela agora carrega os primeiros 500 registros inicialmente, com registros adicionais carregados automaticamente à medida que você rolar a tela em lotes de 500.
* A exibição de linha do tempo tem um comportamento semelhante, mas carrega 1000 registros de uma vez com os próximos 1000 carregados à medida que você rolar a tela.
* A pesquisa rápida se aplica a todos os registros, não apenas àqueles exibidos na exibição atual. Mais registros são carregados à medida que você rolar a tela na linha do tempo e na exibição de tabela.
* Ao aplicar uma pesquisa rápida na exibição de linha do tempo e houver mais de 1000 itens encontrados, você poderá clicar em Carregar mais na parte inferior da linha do tempo para exibir mais registros que correspondam à pesquisa.

Para obter informações, consulte [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md) e [Gerenciar a exibição de linha do tempo](/help/quicksilver/planning/views/manage-the-timeline-view.md).

<!--

## Additional permissions for users other than requestors to submitted requests

>[!NOTE]
>
>Preview: October 28, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

Workspace managers can now define what access to submitted requests users other than requestors have.

By editing the Permissions area of a request form, you can define additional access for other users to requests submitted using the form.

You can grant permissions to workspace users or any other users, groups, teams, job roles or companies in the system. Once defined in the request queue, the permissions are granted automatically when the request is submitted, and any permission changes apply only to new requests.

Prior to this enhancement, you could only grant permissions to requestors.

For information, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

-->

## Reorganização de agrupamento manual na exibição de linha do tempo

>[!NOTE]
>
>Visualização: 29 de outubro de 2026
>Versão rápida de produção: 12 de novembro de 2026
>Produção para todos: 21 de janeiro de 2027

Agora é possível arrastar e soltar agrupamentos, subagrupamentos e registros para criar uma ordem personalizada na exibição de linha do tempo. Sua organização manual é preservada entre as sessões e você pode alternar facilmente entre a ordenação manual e a classificação baseada em campo, conforme as necessidades de planejamento mudam.

A funcionalidade arrastar e soltar está disponível para raias e versões empilhadas da exibição de linha do tempo.

Para obter informações, consulte [Gerenciar a exibição da linha do tempo](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Regras de negócio para tipos de registro global

>[!NOTE]
>
>Visualização: 28 de outubro de 2026
>Versão rápida de produção: 12 de novembro de 2026
>Produção para todos: 21 de janeiro de 2027

Agora, os gerentes do Workspace podem configurar regras de negócios em tipos de registros globais nos espaços de trabalho principal e secundário. As regras se aplicam a todos os registros do mesmo tipo em todos os espaços de trabalho aos quais são adicionadas.

Regras de negócios adicionadas em espaços de trabalho globais são exibidas como somente leitura em espaços de trabalho secundários nos quais os tipos de registro foram importados. As regras de negócios adicionadas aos espaços de trabalho secundários são exibidas como somente leitura nos espaços de trabalho principais onde os tipos de registro foram originalmente criados. As regras podem ser editadas somente nos espaços de trabalho em que são criadas.

Para obter informações, consulte [Configurar regras de negócios do tipo registro](/help/quicksilver/planning/architecture/configure-business-rules.md).

## Definir configurações padrão de prompt para a funcionalidade Preencher formulário em solicitações do Planning

>[!NOTE]
>
>Visualização: 21 de outubro de 2026
>Versão rápida de produção: 12 de novembro de 2026
>Produção para todos: 21 de janeiro de 2027

Agora é possível personalizar o prompt que os usuários veem ao usar o recurso de formulário de Preenchimento ativado por IA ao enviar uma solicitação do Planning.

Você pode criar um prompt padrão ao criar um formulário de solicitação para solicitações do Planning.

Para obter informações, consulte [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
