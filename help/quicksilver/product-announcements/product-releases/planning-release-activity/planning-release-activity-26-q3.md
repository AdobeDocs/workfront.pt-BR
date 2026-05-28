---
content-type: release-notes
title: Atividade da versão do terceiro trimestre de 2026 para o Adobe Workfront Planning
description: Esta é a atividade de lançamento do produto Adobe Workfront Planning para o terceiro trimestre de 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: ab1ac1363d6531352e905536218618196651c3b9
workflow-type: tm+mt
source-wordcount: '1448'
ht-degree: 1%

---

# Atividade da versão do terceiro trimestre de 2026 para o Adobe Workfront Planning

<!--
take the next sentence out when we start listing features
-->

<!--
There are no features released during the Third Quarter Release for 2026. When features are released for this quarter, we will document them in this article. 
-->

<!--keep the sentence below for all future quarterly release pages-->

Este artigo descreve os recursos que estão sendo lançados para o Workfront Planning durante a versão do terceiro trimestre de 2026.

Para obter uma lista de todos os recursos lançados para o Adobe Workfront Planning, consulte [atividade de versão do Adobe Workfront Planning: índice do artigo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).



<!--

## Planning Designer now available in Beta for all Workfront Planning customers

>[!NOTE]
>
>Preview: May 28, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 
>[!BADGE In Beta]{type=Neutral}

You can now use the Adobe Planning Designer powered by AI to configure your workspaces and data structures with ease. The Planning Designer supports everything from creating and configuring workspaces to defining fields and formulas, managing records, reviewing change history and building custom views.  

Whether used directly or through the AI Assistant, the Planning Designer provides a flexible, powerful environment for building and maintaining structured, connected information. 

A Workfront administrator can manage the availability of the Planning Designer from the System Preferences area in Setup.   

For information, see [Get started with the Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md).

## New Sample workspaces tab added to the Planning landing page

>[!NOTE]
>
>Preview: May 28, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 

We have added the Sample workspaces tab in the Planning landing area where you can view example of best-practice workspaces. The workspaces are not editable and we recommend that you use them as examples to create your own.  

We also recommend that you use the multi-workspace template to create, and edit and share workspaces that result as a use of that template.  The template contains the same workspaces as the Sample workspaces tab.   

Workspace managers can modify views in sample workspaces.     

For information, see Workspaces overview (/help/quicksilver/planning/architecture/workspaces-overview.md). 

-->

## API do Workfront Planning versão 2

>[!NOTE]
>
>Disponível para todos os clientes: 28 de maio de 2026>[!BADGE Fora do cronograma]{type=Neutral}

A versão 2 da API do Workfront Planning agora está disponível e expande significativamente os recursos da Versão 1.

Os seguintes aprimoramentos estão incluídos na versão 2:

* Crie, atualize e exclua espaços de trabalho, tipos de registro e campos de forma programática.

* Gerenciar totalmente os registros.
* Melhorias na estrutura do URL, tratamento de erros, paginação, filtragem e permissões.
* Inclui atualizações parciais via PATCH
* Inclui operações de registro em massa.

A versão 1 permanece disponível, embora recomendemos que você alterne para a versão 2.

>[!NOTE]
>
>O conector do Workfront Planning para Fusion não foi atualizado para a API Versão 2 e continuará a usar a Versão 1 até aviso em contrário.

Para obter informações, consulte [noções básicas sobre API do Adobe Workfront Planning](/help/quicksilver/planning/general/planning-api-basics.md).

Para obter as especificações da API do Workfront Planning, consulte a documentação do desenvolvedor da [API do Workfront Planning](https://developer.adobe.com/wf-planning/).

## Conceder permissões a registros

>[!NOTE]
>
>Visualização: 28 de maio de 2026>Versão rápida de produção: 11 de junho de 2026>Produção para todos: 16 de julho de 2026

Agora você pode ajustar permissões de registro individuais para controlar quem pode gerenciá-las em um tipo de registro.

Por padrão, os usuários herdam permissões de registro do espaço de trabalho e do tipo de registro. Para conceder somente a usuários selecionados com permissões de tipo de registro Gerenciar permissões para apenas determinados registros, você pode desativar permissões herdadas em registros selecionados e conceder somente a esses usuários Gerenciar acesso a esses registros. É possível ajustar permissões para um registro ou para vários registros ao mesmo tempo, em massa.

Você pode conceder aos usuários os seguintes níveis de permissão:

* Exibir
* Gerenciar

>[!NOTE]
>
>* As permissões de nível de registro de um usuário não podem exceder suas permissões de tipo de registro. Por exemplo, um usuário com acesso de Visualização a um tipo de registro não pode receber acesso de Gerenciamento a registros individuais desse tipo.
>* No momento, não é possível remover as permissões de um usuário de um registro. Qualquer usuário com pelo menos acesso de Visualização ao tipo de registro pode visualizar todos os registros desse tipo.

Para obter informações, consulte [Compartilhar registros](/help/quicksilver/planning/access/share-records.md).

## Adição simplificada de tipo de registro global

>[!NOTE]
>
>Visualização: 28 de maio de 2026>Versão rápida de produção: 11 de junho de 2026>Produção para todos: 16 de julho de 2026

Para reduzir cliques e ajudar você a encontrar rapidamente os tipos de registro necessários, aprimoramos a experiência de adição de registros para torná-la mais rápida e intuitiva ao adicionar tipos de registro globais a outro espaço de trabalho.

Ao optar por adicionar um registro a partir de tipos existentes, você verá imediatamente uma lista de todos os Tipos de Registro Global disponíveis.

É possível selecionar e adicionar um ou vários tipos de registro global ao mesmo tempo diretamente nessa tela.

Para obter informações, consulte [Adicionar tipos de registro existentes de outro espaço de trabalho](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).


## Sincronizar metadados do Planning para o AEM Assets

>[!NOTE]
>
>Visualização: 28 de maio de 2026>Versão rápida de produção: 28 de maio de 2026>Produção para todos: 28 de maio de 2026>[!BADGE Fora do cronograma]{type=Neutral}

Para melhorar a integridade dos dados, lançamos a sincronização perfeita de metadados entre os tipos de registro do GenStudio for Performance Marketing e do AEM Assets quando o AEM Assets é vinculado aos tipos de registro do GenStudio no Workfront Planning.

Os seguintes tipos de registros do GenStudio for Performance Marketing podem ser conectados ao AEM Assets: Campanha, Produto, Pessoa, Região e Canal.

As informações adicionadas a um tipo de registro do GenStudio no Workfront Planning são exibidas em uma guia Campanha separada de um AEM Asset no AEM. As informações sobre Produto, Pessoa, Região e Canal para essa campanha também são exibidas nessa guia, no modo somente leitura.

Com esta versão, os metadados principais são consistentes em ambas as plataformas e refletem atualizações em tempo quase real, reduzindo a reconciliação manual.

Para obter informações, consulte [Gerenciar o espaço de trabalho do GenStudio no Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md).

## Sincronizar metadados dos fragmentos de conteúdo do Planning para o AEM

>[!NOTE]
>
>Visualização: 28 de maio de 2026>Versão rápida de produção: 28 de maio de 2026>Produção para todos: 28 de maio de 2026>[!BADGE Fora do cronograma]{type=Neutral}

Para melhorar a integridade dos dados, lançamos a sincronização perfeita de metadados entre os tipos de registro do Planning no espaço de trabalho do GenStudio e os Fragmentos de conteúdo do AEM quando os Fragmentos de conteúdo são vinculados às campanhas do GenStudio for Performance Marketing.

As informações de campanha do GenStudio agora são exibidas na guia Metadados de um Fragmento de conteúdo no AEM.  As informações sobre Produto, Pessoa, Região e Canal para essa campanha também são exibidas nessa guia, no modo somente leitura.

Com esta versão, os metadados principais são consistentes em ambas as plataformas e refletem atualizações em tempo quase real, reduzindo a reconciliação manual.

Para obter informações, consulte [Gerenciar o espaço de trabalho do GenStudio no Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md).


## Atualizações da exibição de lista

>[!NOTE]
>
>Visualização: 27 de maio de 2026>Versão rápida de produção: 11 de junho de 2026>Produção para todos: 16 de julho de 2026

Vários tipos de campo na exibição de lista foram atualizados para incluir navegação pelo teclado e outras melhorias.

Os campos Múltiplo, Seleção única e Destinatário agora oferecem navegação pelo teclado na exibição de lista:

* Use as setas para cima e para baixo do teclado para percorrer a lista de pessoas.

* Pressione a barra de espaços para selecionar uma pessoa ou para remover uma pessoa selecionada.

Em campos de seleção única e múltipla na exibição de lista:

* Você pode adicionar novas opções diretamente do editor quando nenhum resultado for encontrado. Observe que esse recurso pode não estar disponível em todas as listas.

* A interação de campo agora pode ser acessada pelo teclado. Isso inclui a navegação entre as tags, as opções de pesquisa e a lista usando as setas para cima e para baixo. Pressione a barra de espaço para selecionar um item ou remover um item selecionado.

Campos de referência, como campos de digitação antecipada e pesquisa externa, receberam algumas melhorias na interface.

Além disso, quando disponível, a experiência de arrastar e soltar colunas foi aprimorada visualmente.

Para obter mais informações, consulte [Gerenciar a exibição de lista no Adobe Workfront Planning](/help/quicksilver/planning/views/manage-the-list-view.md).

## Os campos de referência do Workfront são ativados como campos de pesquisa para conexões do Planning

>[!NOTE]
>
>Visualização: 27 de maio de 2026>Versão rápida de produção: 11 de junho de 2026\
>Produção para todos: 16 de julho de 2026

Agora é possível adicionar campos de referência do Workfront como campos de pesquisa ao conectar um tipo de registro do Planning a um tipo de objeto do Workfront.

Por exemplo, você pode adicionar as informações de Portfolio, Programa, Grupo ou Empresa do objeto Projeto a um campo de conexão do projeto de uma campanha no Planning.

Para obter informações, consulte [Tipos de registro de conexão](/help/quicksilver/planning/architecture/connect-record-types.md).

## Novos filtros para o recurso de detalhamento de exibição de linha do tempo

>[!NOTE]
>
>Visualização: 27 de maio de 2026>Versão rápida de produção: 11 de junho de 2026>Produção para todos: 16 de julho de 2026

Agora é possível filtrar informações na exibição de linha do tempo com base nos critérios que correspondem aos objetos incluídos no detalhamento dos registros.

Antes desse aprimoramento, você só podia aplicar filtros para os registros principais na exibição de linha do tempo.

Para obter informações, consulte [Gerenciar a exibição da linha do tempo](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Nova indicação de que campos editados e excluídos afetam formulários de solicitação

>[!NOTE]
>
>Visualização: 27 de maio de 2026>Versão rápida de produção: 11 de junho de 2026>Produção para todos: 16 de julho de 2026

Adicionamos um lembrete de que os campos de registro editados ou excluídos podem afetar os formulários de solicitação que contêm esses campos. Agora, você terá a chance de revisar os formulários afetados e garantir que as alterações que deseja fazer nos campos não afetarão as informações existentes.

Para obter informações, consulte [Editar configurações de campo](/help/quicksilver/planning/fields/edit-fields.md).

## Editar solicitações de Planejamento enviadas

>[!NOTE]
>
>Visualização: 27 de maio de 2026>Versão rápida de produção: 11 de junho de 2026>Produção para todos: 16 de julho de 2026

Agora é possível editar as solicitações do Planning depois de enviá-las, antes que um registro seja criado a partir da solicitação.

Os seguintes usuários podem editar uma solicitação enviada:

* O criador da solicitação
* Gerenciadores do Workspace para o espaço de trabalho onde a solicitação foi enviada
* Administradores do sistema

Antes dessa melhoria, não era possível editar solicitações enviadas.

Para obter mais informações, consulte [Enviar solicitações do Adobe Workfront Planning para criar registros](/help/quicksilver/planning/requests/submit-requests.md).

## Nova janela de visualização para fragmentos de conteúdo do AEM

>[!NOTE]
>
>Visualização: 14 de maio de 2026>Versão rápida de produção: 14 de maio de 2026>Produção para todos: 14 de maio de 2026>[!BADGE Fora do cronograma]{type=Neutral}

Para melhor visibilidade ao trabalhar com fragmentos de conteúdo do AEM conectados a registros do Workfront Planning, adicionamos uma janela de visualização que exibe informações sobre os fragmentos no Workfront Planning.

Essa funcionalidade estava disponível anteriormente para ativos do AEM e agora a adicionamos aos fragmentos de conteúdo.

Para obter informações, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

## Campos de pesquisa agora disponíveis para fragmentos de conteúdo do AEM no Workfront Planning

>[!NOTE]
>
>Visualização: 14 de maio de 2026>Versão rápida de produção: 14 de maio de 2026>Produção para todos: 14 de maio de 2026>[!BADGE Fora do cronograma]{type=Neutral}

Agora é possível adicionar os seguintes campos de pesquisa ao conectar um tipo de registro do Planning a um Fragmento de conteúdo do AEM:

* Criado por
* Criação em
* Modificado por
* Modificado em

Antes desse aprimoramento, os campos de pesquisa só estavam disponíveis para ativos e pastas da AEM.

Para obter informações, consulte [Tipos de registro de conexão](/help/quicksilver/planning/architecture/connect-record-types.md).



## Exibições personalizadas da página Detalhes de um registro

>[!NOTE]
>
>Visualização: 14 de maio de 2026>Versão rápida de produção: 11 de junho de 2026>Produção para todos: 16 de julho de 2026

Para permitir maior flexibilidade na visualização de suas informações na página de detalhes de um registro, introduzimos a capacidade de criar exibições personalizadas para esta página.

Além de adicionar duas exibições de página de detalhes já criadas que contêm todos os campos de registros ou apenas os campos visíveis na exibição de tabela, agora é possível criar exibições personalizadas para as páginas de detalhes de um registro. As exibições criadas estão visíveis para todos que podem acessar o registro.

Esta atualização remove a configuração **Mostrar todos os campos** e a substitui por exibições de detalhes personalizadas.

Para obter informações, consulte [Gerenciar a página de registro](/help/quicksilver/planning/records/manage-the-record-page.md).

## Adicionar agrupamentos a uma página de registro conectada de Projetos

>[!NOTE]
>
>Visualização: 14 de maio de 2026\
>Produção rápida: 11 de junho de 2026>Produção para todos: 16 de julho de 2026

Agora é possível agrupar suas informações na página de registros conectados de projetos de um registro no Workfront Planning. Esse recurso não existia nessa área antes desse aprimoramento.

Para obter informações, consulte [Gerenciar a exibição de lista](/help/quicksilver/planning/views/manage-the-list-view.md).
