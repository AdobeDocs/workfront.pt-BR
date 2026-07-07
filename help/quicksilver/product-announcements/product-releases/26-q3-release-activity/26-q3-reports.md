---
title: Melhorias na emissão de relatórios no terceiro trimestre de 2026
description: Melhorias na emissão de relatórios no terceiro trimestre de 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 0c7265c477030137d14e95f42eaf67580589d70b
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 1%

---

# Melhorias na emissão de relatórios no terceiro trimestre de 2026

Esta página descreve as melhorias de relatórios feitas com a versão do terceiro trimestre de 2026 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de produção, conforme indicado.

Para obter uma lista de todas as alterações disponíveis neste momento no ciclo de lançamento do terceiro trimestre de 2026, consulte [Visão geral da versão do terceiro trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Controle de acesso automatizado para o Workfront Planning no Snowflake

>[!NOTE]
>
>Pré-visualização e produção para todos os clientes: 16 de julho de 2026Fora do cronograma]{type=Neutral}

Esta versão apresenta o gerenciamento de acesso automatizado e orientado por direitos para dados do Workfront Planning no Snowflake como parte da Workfront Data Connect.
Ele começa estendendo a geração de exibição segura para tabelas do Planning, estabelecendo a base necessária para o controle de acesso downstream e possibilitando concessões baseadas em direitos.Com base nisso, o provisionamento da conta de leitor agora verifica os direitos do TMS no momento da criação e aplica ou retém automaticamente concessões ao banco de dados do Planning, garantindo a correção.
Antes desse aprimoramento, ele estava disponível somente para o Workfront.
A atualização inclui os seguintes recursos: 

* Um trabalho diário automatizado detecta alterações de direito para clientes existentes
* A nova tarefa concede, revoga ou preserva o acesso com base em qualificações
* Cobertura de ciclo de vida completo em todas as alterações de provisionamento, criação de conta e direitos contínuos.

O artigo [Dicionário de dados da Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/data-dictionary.md) será atualizado após a data de lançamento.

## Adicionar suporte a dados personalizados para novos objetos

>[!NOTE]
>
>Pré-visualização e produção para todos os clientes: 7 de julho de 2026Fora do cronograma]{type=Neutral}

Durante o Segundo trimestre de 2026, adicionamos novos objetos para oferecer suporte aos aprimoramentos nas operações empresariais do Workfront.Com a versão atual, também adicionamos suporte a dados personalizados para vários objetos novos no Painel de controle da tela.

Para obter informações, consulte [Visão Geral do Painel da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/canvas-dashboards-overview.md).

## Padrões do prompt do Painel de controle do Canvas e persistência de preferências do usuário

>[!NOTE]
>
>Visualização: 25 de junho de 2026Versão rápida de produção: 15 de julho de 2026Produção para todos: 16 de julho de 2026

Para melhorar a eficiência dos usuários que se movem entre painéis e registros, preservando o estado do filtro de trabalho, os gerentes de painel agora podem definir valores de prompt padrão para painéis do Canvas. Esses padrões são aplicados automaticamente para todos os visualizadores de painel.

Quando um usuário atualiza prompts, suas seleções são salvas e restauradas na atualização, reabertura ou após navegar até um registro e retornar.

Os gerentes podem redefinir o estado padrão do painel a qualquer momento. Os usuários também podem reverter rapidamente para os padrões por meio do menu de três pontos.

Antes dessa melhoria, os prompts do painel não tinham um padrão configurável ou uma preferência de usuário salva para o status do prompt.

Para obter informações, consulte [Filtrar um Painel da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/filter-canvas-dashboard.md).

## Adicionar vários intervalos de endereço IP do Power BI ao incluo na lista de permissões de conexão de dados de uma só vez

>[!NOTE]
>
>Visualização: N/DVersão rápida de produção: 11 de junho de 2026Produção para todos: 16 de julho de 2026

Os administradores do Workfront que conectam o Microsoft Power BI ao Workfront Data Connect agora podem adicionar um conjunto inteiro de intervalos de endereço IP do Azure de uma região ao incluo na lista de permissões em uma única etapa. Na guia **Incluo na lista de permissões IP** em **Data Connect**, o botão **Novo endereço IP** agora inclui uma opção **Adicionar blocos de endereço IP do Power BI** que abre uma caixa de diálogo na qual você pode colar entradas de etiqueta de serviço do Power BI a partir do arquivo JSON de Intervalos IP e Tags de Serviço do Azure publicado pela Microsoft.

Isso substitui o fluxo de trabalho anterior de adicionar cada bloco CIDR do Power BI, um de cada vez, o que era demorado para regiões que publicam dezenas de prefixos de endereço.

Para obter mais informações, consulte [Estabelecer uma conexão com o Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md).


## Classificar a lista Painéis de Controle da Tela de Pintura

>[!NOTE]
>
>Visualização: 11 de junho de 2026Versão rápida de produção: 15 de julho de 2026Produção para todos: 16 de julho de 2026
>
>Painéis do Canvas atualmente está na versão beta.

Agora você pode classificar a lista de Painéis da Tela por qualquer uma das seguintes colunas: **Nome**, **Descrição**, **Criado por** ou **Data de criação**. Clique em um cabeçalho de coluna para classificar a lista por essa coluna e, em seguida, clique no mesmo cabeçalho novamente para inverter a direção da classificação. Por padrão, a lista é classificada por **Nome** de A a Z. A ordem de classificação é preservada ao alternar entre guias na lista Painéis da tela de desenho.

Para obter mais informações, consulte [Usar Painéis da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md).

## Alterações nas Horas Efetivas em fórmulas personalizadas

>[!NOTE]
>
>Visualização: 1 de junho de 2026Versão rápida de produção: 1 de junho de 2026Produção para todos: 1 de junho de 2026

Em 2025, um novo campo Horas efetivas foi adicionado ao banco de dados do Workfront como `actualWorkRequiredDouble`, e o campo Horas efetivas existente (`actualWorkRequired` no banco de dados) foi renomeado para Horas efetivas herdadas. Consulte a [nota de versão](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-project-enhancements.md) para obter mais informações.

Em junho de 2026, fórmulas personalizadas existentes usando `actualWorkRequired` (Horas efetivas herdadas) foram migradas para usar `actualWorkRequiredDouble` (Horas efetivas) em seu lugar. `actualWorkRequired` não pode mais ser usado em cálculos e fórmulas.

Além disso, é altamente recomendável usar `actualWorkRequiredDouble` em todos os relatórios.

Ao substituir o campo, observe que `actualWorkRequired` armazena valores em minutos, enquanto `actualWorkRequiredDouble` armazena valores em horas com precisão decimal.

Para obter mais informações sobre Horas Reais, consulte [Exibir Horas Reais](/help/quicksilver/manage-work/tasks/task-information/actual-hours.md).

## Campos de dados de moeda personalizados em relatórios do Painel de controle da tela

>[!NOTE]
>
>Visualização: 28 de maio de 2026Versão rápida de produção: 11 de junho de 2026Produção para todos: 16 de julho de 2026

Os relatórios do Painel do Canvas agora oferecem suporte a campos de dados de moeda personalizados como colunas, filtros, agrupamentos e agregações, inclusive quando várias taxas de câmbio são configuradas na Configuração do sistema. Quando um campo de dados de moeda personalizado é exibido como uma coluna ou agregação, os valores são convertidos na moeda selecionada na opção de taxa de câmbio do painel, a menos que o campo esteja bloqueado no nível do relatório.

Os relatórios que anteriormente falhavam com uma mensagem &quot;campo restrito&quot; após uma segunda moeda de taxa de câmbio foram adicionados agora são renderizados. Os campos de moeda de planejamento permanecem restritos quando várias taxas de câmbio são definidas.

Para obter mais informações, consulte [Usar campos de moeda em Painéis da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/switch-currencies.md).

## Melhoria na precisão dos dados nos relatórios do painel do Canvas

>[!NOTE]
>
>Visualização: 14 de maio de 2026Versão rápida de produção: 11 de junho de 2026Produção para todos: 16 de julho de 2026
>
>Painéis do Canvas atualmente está na versão beta.

Os painéis da tela agora estruturam consultas de relatório para evitar linhas duplicadas quando filtros ou campos cruzam registros relacionados, de modo que contagens, somas e outras agregações retornem valores precisos.

Anteriormente, um join entre registros relacionados poderia repetir registros pai uma vez para cada registro relacionado. Por exemplo, em um relatório de projeto filtrado para tarefas atribuídas a um usuário específico, cada projeto era repetido uma vez para cada tarefa correspondente. Um KPI que somasse o orçamento do projeto poderia mostrar US$ 6.000 em vez dos US$ 1.250 corretos.

Não há alterações na interface do painel da Tela de Pintura. Os relatórios existentes retornam automaticamente dados precisos após esta versão.

