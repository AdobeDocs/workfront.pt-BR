---
content-type: release-notes
title: Atividade da versão do primeiro trimestre de 2026 para o Adobe Workfront Planning
description: Esta é a atividade de lançamento do produto Adobe Workfront Planning para o primeiro trimestre de 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 7fb12a3fbdad661baf2d0ad472ce8017e178ddef
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Atividade da versão do primeiro trimestre de 2026 para o Adobe Workfront Planning

Este artigo descreve os recursos que estão sendo lançados para o Workfront Planning durante a versão do Primeiro Trimestre de 2026.

<!--keep the sentence below for all future quarterly release pages-->

Para obter uma lista de todos os recursos lançados para o Adobe Workfront Planning, consulte [atividade de versão do Adobe Workfront Planning: índice do artigo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).


<!--## New field search box in the Filters, Fields, and Row colors icons in Planning views

>[!NOTE]
>
>Preview: October 30, 2025 
>Production fast release: November 13, 2025 
>Production for everyone:  January 15, 2026 


You can now search for a specific field when building a view element in record type view. The new search boxes have been added when you build a filter, sort, grouping, or when you configure your fields or row colors. Prior to this enhancement, you could simply scroll through the list of available fields.
This improvement is available in all views.

For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md).-->


## Tipos de registro global e a capacidade de adicioná-los como tipos de registro existentes a outros espaços de trabalho

>[!NOTE]
>
>Visualização: 16 de outubro de 2025
>&#x200B;>Versão rápida de produção: 13 de novembro de 2025
>&#x200B;>Produção para todos: 15 de janeiro de 2026

Ao implementar o Workfront Planning para uma organização de várias equipes com workflows comuns, talvez seja necessário definir uma estrutura coesa e metadados para os principais tipos de registro (como Campanhas ou Materiais de entrega) que podem ser adicionados aos espaços de trabalho de cada equipe para capturar e gerenciar o trabalho.

Além disso, pode ser necessário que o trabalho de cada equipe atinja um nível central.

Nesse fluxo de trabalho, você pode garantir que as equipes capturem seu trabalho de forma consistente ao desbloquear a visibilidade entre equipes, sem a necessidade de adicionar todos na organização a cada espaço de trabalho. Você pode usar tipos de registro global para fazer isso.

Agora você pode designar um tipo de registro para ser global e usá-lo em vários espaços de trabalho. Os usuários podem usar a mesma estrutura de campo e conexões já configuradas em um espaço de trabalho central.

Para obter mais informações, consulte os seguintes artigos:

* [Visão geral do tipo de registro entre espaços de trabalho](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)

* [Configurar recursos entre espaços de trabalho do tipo de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)

* [Adicionar tipos de registro existentes de outro espaço de trabalho](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)

## Novo limite para campos de conexão para um tipo de registro

>[!NOTE]
>
>Visualização: 16 de outubro de 2025
>&#x200B;>Versão rápida de produção: 13 de novembro de 2025
>&#x200B;>Produção para todos: 15 de janeiro de 2026

Introduzimos um limite de 30 campos de conexão para cada tipo de registro.

OBSERVAÇÃO: se sua organização tiver mais de 30 campos de conexão para um tipo de registro, você poderá manter os campos adicionais que excedam o limite de 30. No entanto, não é possível adicionar mais campos de conexão aos tipos de registro que excedem o limite. O novo limite de 30 campos de conexão será aplicado a partir de agora.

Para obter mais informações, consulte [Visão geral dos Tipos de Registros Conectados](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Definir valores amigáveis para opções de campo do tipo seleção

>[!NOTE]
>
>Visualização: 16 de outubro de 2025
>&#x200B;>Versão rápida de produção: 13 de novembro de 2025
>&#x200B;>Produção para todos: 15 de janeiro de 2026

Ao adicionar opções de campo a um campo de seleção única ou múltipla, o Workfront atribuirá valores amigáveis exclusivos a cada escolha. Antes dessa melhoria, o Workfront gerou uma ID alfanumérica que era difícil de entender e usar em chamadas de API e outras integrações.

Considere o seguinte com esta melhoria:

* Os novos valores serão adicionados às novas opções de campo. As opções de campo existentes manterão as IDs alfanuméricas.

* Valores de escolha são exclusivos para um campo, mas podem ser repetidos entre campos diferentes.

* Renomear uma opção não atualiza seu valor original.

* Os valores de escolha são exibidos em minúsculas e são separados por sublinhados no caso de opções de várias palavras. Se você usar um rótulo já usado como outro nome de opção para o mesmo campo, o Workfront adicionará um número sequencial ao valor.

Para obter informações, consulte [Criar campos](/help/quicksilver/planning/fields/create-fields.md).