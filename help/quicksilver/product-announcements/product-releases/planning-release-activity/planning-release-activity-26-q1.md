---
content-type: release-notes
title: Atividade da versão do primeiro trimestre de 2026 para o Adobe Workfront Planning
description: Esta é a atividade de lançamento do produto Adobe Workfront Planning para o primeiro trimestre de 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 34e6f4386c768b94c3835d4a4d7e7deadc3fecda
workflow-type: tm+mt
source-wordcount: '724'
ht-degree: 0%

---

# Atividade da versão do primeiro trimestre de 2026 para o Adobe Workfront Planning

Este artigo descreve os recursos que estão sendo lançados para o Workfront Planning durante a versão do Primeiro Trimestre de 2026.

<!--keep the sentence below for all future quarterly release pages-->

Para obter uma lista de todos os recursos lançados para o Adobe Workfront Planning, consulte [atividade de versão do Adobe Workfront Planning: índice do artigo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Remoção do compartilhamento público de exibições em um tipo de registro global em um espaço de trabalho secundário


>[!NOTE]
>
>Visualização: 3 de dezembro de 2025
>Versão rápida de produção: 4 de dezembro de 2025
>Produção para todos: 15 de janeiro de 2026


Removemos a guia Compartilhamento público ao compartilhar uma exibição para um registro global em um espaço de trabalho secundário. Não é possível compartilhar uma exibição publicamente de um tipo de registro global adicionado a outro espaço de trabalho de um tipo de registro global existente. Você pode compartilhar uma visualização de tipo de registro global publicamente de seu espaço de trabalho original.

Para obter informações, consulte [Compartilhar modos de exibição](/help/quicksilver/planning/access/share-views.md).


## Conexão das Marcas GenStudio for Performance Marketing com os tipos de registro do Workfront Planning

>[!NOTE]
>
>Visualização: 13 de novembro de 2025
>Versão rápida de produção: 13 de novembro de 2025
>Produção para todos: 13 de novembro de 2025

Agora é possível conectar tipos de registro do Workfront Planning com Marcas da Adobe GenStudio for Performance Marketing. Sua organização deve ter o Workfront Planning e o Adobe GenStudio for Performance Marketing.

Para obter mais informações, consulte [Tipos de registro de conexão](/help/quicksilver/planning/architecture/connect-record-types.md).


## Nova caixa de pesquisa de campo nos ícones de cores Filtros, Campos e Linha nas exibições do Planning

>[!NOTE]
>
>Visualização: 6 de novembro de 2025
>Versão rápida de produção: 11 de dezembro de 2025
>Produção para todos: 15 de janeiro de 2026

Agora é possível pesquisar por um campo específico ao criar um elemento de exibição em uma exibição do tipo de registro. Adicionamos caixas de pesquisa ao criar um filtro, classificar, agrupar ou ao configurar as cores dos campos ou linhas. Antes dessa melhoria, você pode simplesmente rolar pela lista de campos disponíveis.

Essa melhoria está disponível em todas as exibições de tipo de registro.

Para obter informações, consulte [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md).


## Tipos de registro global e a capacidade de adicioná-los como tipos de registro existentes a outros espaços de trabalho

>[!NOTE]
>
>Visualização: 16 de outubro de 2025
>Versão rápida de produção: 13 de novembro de 2025
>Produção para todos: 15 de janeiro de 2026

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
>Versão rápida de produção: 13 de novembro de 2025
>Produção para todos: 15 de janeiro de 2026

Introduzimos um limite de 30 campos de conexão para cada tipo de registro.

OBSERVAÇÃO: se sua organização tiver mais de 30 campos de conexão para um tipo de registro, você poderá manter os campos adicionais que excedam o limite de 30. No entanto, não é possível adicionar mais campos de conexão aos tipos de registro que excedem o limite. O novo limite de 30 campos de conexão será aplicado a partir de agora.

Para obter mais informações, consulte [Visão geral dos Tipos de Registros Conectados](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Definir valores amigáveis para opções de campo do tipo seleção

>[!NOTE]
>
>Visualização: 16 de outubro de 2025
>Versão rápida de produção: 13 de novembro de 2025
>Produção para todos: 15 de janeiro de 2026

Ao adicionar opções de campo a um campo de seleção única ou múltipla, o Workfront atribuirá valores amigáveis exclusivos a cada escolha. Antes dessa melhoria, o Workfront gerou uma ID alfanumérica que era difícil de entender e usar em chamadas de API e outras integrações.

Considere o seguinte com esta melhoria:

* Os novos valores serão adicionados às novas opções de campo. As opções de campo existentes manterão as IDs alfanuméricas.

* Valores de escolha são exclusivos para um campo, mas podem ser repetidos entre campos diferentes.

* Renomear uma opção não atualiza seu valor original.

* Os valores de escolha são exibidos em minúsculas e são separados por sublinhados no caso de opções de várias palavras. Se você usar um rótulo já usado como outro nome de opção para o mesmo campo, o Workfront adicionará um número sequencial ao valor.

Para obter informações, consulte [Criar campos](/help/quicksilver/planning/fields/create-fields.md).