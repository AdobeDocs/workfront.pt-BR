---
title: Gerenciar a exibição de tabela
description: Você pode exibir registros e seus campos em uma exibição de tabela, ao acessar a página tipo de registro no Adobe Workfront Planning. Este artigo descreve como criar ou editar uma edição de exibição de tabela e como ativar indicadores de presença em tempo real para a exibição.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 0dd723b5-d674-4626-8fc2-7da41f3b7f35
source-git-commit: 10fec10e1bb885ac20e1ef9526cfa8a59086d874
workflow-type: tm+mt
source-wordcount: '3494'
ht-degree: 2%

---

# Gerenciar a exibição de tabela

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Você pode exibir registros e seus campos em uma exibição de tabela, ao acessar a página tipo de registro no Adobe Workfront Planning.

Para obter informações sobre exibições de registros e como gerenciá-las, consulte [Gerenciar exibições de registros](/help/quicksilver/planning/views/manage-record-views.md).

Este artigo descreve as seguintes informações:

* [Criar ou editar colunas e linhas em uma exibição de tabela](#manage-a-table-view)
* [Habilitar indicadores de presença em tempo real para a exibição de tabela](#enable-the-real-time-presence-indicator)

Para obter informações sobre como exportar a exibição de tabela para um arquivo do Excel ou CSV, consulte [Exportar registros da exibição de tabela](/help/quicksilver/planning/records/export-records-from-the-table-view.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produtos</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planejamento do Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>plano do Adobe Workfront*</p></td> 
   <td> 
<p>Qualquer um dos seguintes planos da Workfront:</p> 
<ul><li>Selecionar</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>O Workfront Planning não está disponível para planos herdados do Workfront</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Pacote de planejamento do Adobe Workfront*</p></td> 
   <td> 
<p>Qualquer </p> 
<p>Para obter mais informações sobre o que está incluído em cada plano do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma Adobe Workfront</p></td> 
   <td> 
<p>A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para acessar o Workfront Planning.</p> 
<p>Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada da Adobe para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
    <td role="rowheader"><p>Licença da Adobe Workfront*</p></td> 
   <td><p> Padrão para criar e excluir visualizações</p>
   <p>Colaborador ou superior para atualizar elementos de visualização</p>
   <p>O Workfront Planning não está disponível para licenças herdadas do Workfront</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões para uma exibição</p>  
   <p>Exibir permissões de um modo de exibição para alterar temporariamente as configurações de modo de exibição ou duplicá-lo</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> Os usuários com uma licença Light ou Contributor devem receber um modelo de layout que inclua o Planning.
   <p>Usuários padrão e Administradores do sistema têm as áreas do Planning habilitadas por padrão.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Editar registros usando a exibição de tabela

É possível editar informações de registro somente na exibição de tabela.

Para obter mais informações sobre como editar registros na exibição de tabela, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

## Gerenciar uma exibição de tabela {#manage-a-table-view}

Ao criar uma exibição de tabela, todos os registros do tipo selecionado são exibidos em uma tabela. Cada linha é um registro exclusivo e cada coluna é um campo de registro. Todos os campos e registros são exibidos por padrão.

Para gerenciar uma exibição de tabela:

1. Crie uma exibição de tabela, conforme descrito no artigo [Gerenciar exibições de registros](/help/quicksilver/planning/views/manage-record-views.md).

   ![Exemplo de exibição de tabela](assets/table-view-example.png)

1. (Opcional) Clique em **Altura da linha** e selecione uma das seguintes opções para modificar a altura das linhas da tabela:
   * Pequena
   * Média
   * Alta

1. <span class="preview">(Opcional) Clique no ícone **Tela cheia** ![Abrir ícone de tela cheia](assets/open-full-screen-icon.png) para abrir o modo de exibição em tela cheia, em seguida, no ícone **Sair da tela cheia** ![Sair do ícone de tela cheia](assets/exit-full-screen-icon.png) ou em Escape no teclado para sair da tela cheia.  </span>

1. Atualize os seguintes elementos de exibição conforme descrito nas subseções abaixo:
   * [Colunas (ou campos)](#add-columns-or-fields)
   * [Linhas (ou registros)](#add-rows-or-records)
   * [Filtros](#add-filters)
   * [Classificar](#add-a-sort)
   * [Agrupamento](#add-groupings)
   * [Cores da linha](#add-row-colors)
   * [Indicador de presença em tempo real](#enable-the-real-time-presence-indicator)


### Adicionar colunas (ou campos) {#add-columns}

Os cabeçalhos de coluna de uma exibição de tabela exibem campos associados aos registros na exibição. Os campos exibidos na visualização de tabela também são exibidos na seção Detalhes de um registro.

Para obter mais informações, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

<!--this is not available yet:You can display record fields (or columns) in both a table and a timeline view. However, the number of columns displayed in the table of the timeline view is limited and you cannot add columns in addition to those selected by default.-->

Adicionar colunas a uma exibição é idêntico a adicionar campos a um tipo de registro.

É possível adicionar até 500 campos (ou colunas) em uma exibição de tabela.

1. Vá para uma página de tipo de registro e clique em uma guia de exibição de tabela ou clique em **+ Exibição** para adicionar um novo modo de exibição e, em seguida, escolha **Tabela**.

1. Comece a adicionar campos (ou colunas), conforme descrito no artigo [Criar campos](/help/quicksilver/planning/fields/create-fields.md).

   As colunas adicionadas ficam visíveis para todos os usuários que acessam o tipo de registro e são adicionadas como novos campos na página do registro.

1. Siga um destes procedimentos para reordenar colunas na tabela:

   * Segure o cabeçalho da coluna e arraste e solte-o na posição desejada. A coluna movida brevemente será exibida com um plano de fundo azul até que você faça outros ajustes na tabela.

   * Clique em **Campos** na barra de ferramentas da tabela, arraste e solte os campos na ordem desejada e clique fora da caixa **Visibilidade e ordem dos campos** para fechá-la.

     ![Barra de ferramentas de exibição de tabela de configuração de campos expandida](assets/fields-setting-table-view-toolbar-expanded.png)


     >[!TIP]
     >
     >* Por padrão, o campo Nome é sempre o primeiro campo na exibição de tabela. Este é considerado um campo primário.
     >
     >* Não é possível mover o campo Nome para outra posição, a menos que você designe outro campo como o principal. Para obter mais informações, continue com a Etapa 4. <!--accurate?-->
     >
     >

   * Substitua o campo na primeira coluna por outro campo alterando o campo primário. Para obter mais informações, continue para a etapa 4. <!--accurate?-->

1. (Opcional) Passe o mouse sobre um nome de campo no cabeçalho da coluna de qualquer campo que não seja exibido na primeira coluna da tabela, clique na seta para baixo à direita do nome do campo e clique em **Definir como campo principal**.

   ![Definir como opção de campo primário na exibição de tabela](assets/set-as-primary-field-option-table-view.png)

1. Clique em **Definir campo** para confirmar.

   O campo se torna um campo primário, o que significa que ele é exibido como a primeira coluna da exibição de tabela. O campo principal anterior é movido para a segunda coluna.

   Os campos primários se tornam o título e a exibição do registro na área de cabeçalho da página do registro e em todos os locais onde os registros são exibidos. Por exemplo, o título do registro é exibido em campos conectados e em todas as exibições. Para obter mais informações sobre campos primários, consulte [Visão geral do campo primário](/help/quicksilver/planning/fields/primary-field-overview.md).

1. Clique e arraste as linhas de separação da coluna e solte-as no ponto desejado para aumentar a largura das colunas.

   >[!TIP]
   >
   >As alterações feitas na largura e na ordem da coluna são permanentes e visíveis a todos os usuários que acessam o tipo de registro.

1. Passe o mouse sobre o cabeçalho da coluna, clique na seta para baixo e clique em **Ocultar campo**

   Ou

   Clique em **Campos** na barra de ferramentas da tabela e desabilite a alternância associada aos campos (ou colunas) que você deseja ocultar. A caixa **Visibilidade e ordem dos campos** é exibida.

   >[!TIP]
   >
   >O número de campos ocultos é exibido à esquerda do ícone Campos na barra de ferramentas.


1. Clique no ícone **Campos** e habilite a alternância associada aos campos que deseja exibir nas colunas da tabela. Todos os campos são exibidos por padrão.

1. Faça o seguinte para localizar rapidamente registros que correspondam a uma palavra-chave:

   1. Clique no ícone **Pesquisar** ![Ícone Pesquisar](assets/search-icon.png) e comece a digitar uma palavra-chave associada a qualquer campo de um registro exibido na tela. O número de correspondências corretas é exibido ao lado do item de pesquisa e o campo com a correspondência correta é realçado.

      ![Caixa de pesquisa com estrutura azul de resultados na exibição de tabela](assets/search-box-with-results-blue-outline-table-view.png)

      Você pode usar qualquer palavra ou caractere especial visível na tela.

      Não é possível usar palavras-chave associadas a campos ocultos na exibição de tabela.

   1. Pressione **Enter** no teclado para ir para o próximo campo encontrado.

   1. (Opcional) Se houver mais de uma correspondência, clique nas setas para cima e para baixo à direita da palavra-chave de pesquisa para localizar todas as correspondências na tabela.

   1. Clique no ícone **x** na caixa de pesquisa para limpar a palavra-chave de pesquisa.


### Adicionar linhas (ou registros) {#add-rows}

As linhas de uma exibição de tabela exibem registros individuais do tipo de registro selecionado.

É possível ter até 50.000 registros (ou linhas) para um tipo de registro S.

1. Vá para uma página de tipo de registro e clique em uma guia de exibição de tabela ou clique em **+ Exibição** para adicionar um novo modo de exibição e, em seguida, escolha **Tabela**.

1. Comece a adicionar registros (ou linhas), conforme descrito no artigo [Criar registros](/help/quicksilver/planning/records/create-records.md).

   Os registros adicionados na exibição de tabela são salvos imediatamente e ficam visíveis para todos os usuários que têm permissões de Exibição ou superiores para o espaço de trabalho.

1. (Opcional) Adicione uma miniatura a cada registro e clique em **Campos** no canto superior direito da tabela e selecione o alternador do campo **Miniatura** para exibi-lo à esquerda do campo principal. Ela é desmarcada por padrão.

   Para obter informações, consulte [Adicionar uma miniatura a um registro](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

1. (Opcional) Selecione um ou vários registros em uma linha, em seguida, arraste e solte o ícone **alça** ![alça de ícone](assets/handle-icon.png) à esquerda do registro para reordenar as linhas.

   >[!NOTE]
   >
   >Não é possível reordenar linhas se você aplicar pelo menos uma classificação à exibição de tabela.
   >
   >As alterações feitas na ordem das linhas ficam visíveis para todos os usuários que acessam o tipo de registro

<!-- this section below links from the timeline view; consider splitting them if they become different-->

### Adicionar filtros {#add-filters}

Os filtros ajudam a reduzir a quantidade de informações exibidas na tela.

Considere o seguinte ao trabalhar com filtros na exibição de tabela:

<!-- this list is almost identical to the one for the table view - update both-->

* Os filtros criados para a exibição de tabela funcionam independentemente dos filtros na exibição de linha do tempo quando aplicados ao mesmo tipo de registro.

* Os filtros são exclusivos para a exibição selecionada. Duas exibições de tabela do mesmo tipo de registro podem ter filtros diferentes aplicados a elas. Dois usuários que visualizam a mesma visualização de tabela veem o mesmo filtro aplicado no momento.

* Não é possível nomear os filtros criados e aplicar a uma exibição de tabela.

* A remoção de filtros os remove de qualquer pessoa que acesse o mesmo tipo de registro que você e use a mesma visualização que você usa.

* Você pode filtrar por campos de registro conectados ou campos de pesquisa.

* Você pode filtrar por campos de pesquisa que exibem vários valores.

* Você pode fazer referência a um campo que esteja a até 4 níveis de distância do tipo de registro atual. Por exemplo, se você estiver criando um filtro para um tipo de registro de Atividade e a Atividade estiver conectada ao tipo de registro de Produto que está conectado ao tipo de registro de Campanha que está conectado a um Projeto do Workfront, será possível fazer referência ao Orçamento do projeto no filtro que está sendo criado para o tipo de registro de Atividade.

Para adicionar um filtro a uma exibição de tabela:

1. Crie uma exibição de tabela para uma página de tipo de registro, conforme descrito no artigo [Gerenciar exibições de registro](/help/quicksilver/planning/views/manage-record-views.md).
1. Selecione uma exibição de tabela e clique em **Filtros** no canto superior direito da tabela.
1. Clique em **Adicionar condição** e adicione as seguintes informações:

   * **Selecione um campo** que você deseja filtrar por <!-- the tip below might change-->

   * **Selecione uma opção** (ou um modificador de filtro) para definir que tipo de condição o campo deve atender

     A tabela abaixo exibe os modificadores disponíveis para cada tipo de campo.

     <table>
        <thead>
        <tr>
            <th><b>Tipo de campo</b></th>
            <th><b>Modificadores</b></th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>Linha única, Parágrafo, Fórmula </td>
            <td><p>Contém</p>
            <p>Não contém</p>
            <p>É</p>
            <p>Não é</p>
            <p>Está vazio</p>
            <p>Não está vazio</p></td>
        </tr>
        <tr><td>Seleção única</td>
            <td><p>É</p>
            <p>Não é</p>
            <p>É algum dos</p>
            <p>Não é nenhum dos</p>
            <p>Está vazio</p>
            <p>Não está vazio</p></td>
        </tr>
        <tr>
            <td>Multisseleção, Pessoas</td>
            <td><p>Tem qualquer um dos</p>
            <p>Possui todos os</p>
            <p>É exatamente</p>
            <p>Não tem nenhum dos</p>
            <p>Está vazio</p>
            <p>Não está vazio</p></td>
        </tr>
        <tr>
            <td>Número, Porcentagem, Moeda</td>
            <td><p>=</p>
            <p>≠</p>
            <p> &lt; </p>
            <p>&gt;</p>
            <p>≤</p>
            <p>≥</p>
            <p>Está vazio</p>
            <p>Não está vazio</p></td>
        </tr>
        <tr>
            <td>Data</td>
            <td><p>É</p>
            <p>Não é</p>
            <p>Está depois</p>
            <p>Está antes</p>
            <p>Está entre</p><p>Não está entre</p>
            <p>Está vazio</p><p>Não está vazio</p></td>
        </tr>

     <tr>
            <td>Caixa de seleção</td>
            <td><p>É</p>
        </tr>
        </tbody>
        </table>

   * Selecione um valor para o campo selecionado.

   ![Exibição da tabela da interface do usuário do filtro](assets/filter-ui-table-view.png)

   Não há limite para quantas condições de filtragem você pode adicionar.

1. (Opcional) Clique em **Adicionar condição** para adicionar outra opção de filtragem e repita as etapas acima. O número de filtros aplicados é exibido à esquerda do ícone Filtros.
1. Clique nos seguintes operadores para indicar como as condições de filtro são unidas e devem ser aplicadas:

   * **AND**: todas as condições especificadas devem ser atendidas.
   * **OU**: qualquer uma das condições especificadas deve ser atendida. Esta é a opção padrão.

   1. (Opcional) Adicione operadores **AND** ou **OR** adicionais entre vários agrupamentos de condição.

      ![Filtros de várias camadas em exibições](assets/multi-tiered-filters-in-views.png)

   A lista de registros é filtrada automaticamente.  <!--at this time, you can't name and save the filter - but will this change?!-->
   <!-- asked on the task for the simple filters whether there is a limitation for how many statements a filter can have?!-->

1. (Opcional) Clique no ícone **x** para remover uma condição de filtro.
1. (Opcional) Clique em **Filtros** para fechar a caixa de filtros. <!--right now you cannot "clear all" for filters, but this might come later-->

### Adicionar uma classificação {#sort-information}

Ao aplicar uma classificação, você pode organizar as informações em uma determinada ordem.

Você pode classificar as seguintes informações:

* Todos os registros em uma exibição de tabela. <!--or timeline view. ***********verify this is the case for the timeline view*********************-->
  <!--* All groupings. - this is not available yet-->

Considere o seguinte ao classificar registros na exibição de tabela:

<!-- if this is available for the timeline view, update both when you update one-->

* A classificação é exclusiva da exibição selecionada. Duas exibições de tabela do mesmo tipo de registro podem ter critérios de classificação diferentes aplicados a elas. Dois usuários que observam a mesma exibição de tabela veem a mesma classificação aplicada atualmente.

* Não é possível nomear as classificações criadas e aplicar a uma exibição de tabela.

* A classificação criada é preservada ao sair.

* É possível classificar por quantos campos forem exibidos na exibição de tabela de um tipo de registro.

* Não é possível classificar por campos de registro conectados, mas você pode classificar por campos de pesquisa a partir de tipos de registro conectados.

* Quando você classifica por campos de pesquisa com vários valores (que não foram resumidos por um agregador), o primeiro valor é usado para classificação.

* A remoção dos critérios de classificação os remove de qualquer pessoa que acesse o mesmo tipo de registro que você e use a mesma exibição usada.

* Você pode fazer referência a um campo que esteja a até 4 níveis de distância do tipo de registro atual. Por exemplo, se você estiver criando uma classificação para um tipo de registro de Atividade e a Atividade estiver conectada ao tipo de registro de Produto que está conectado ao tipo de registro de Campanha que está conectado a um Projeto do Workfront, será possível fazer referência ao Status do projeto na classificação que você está criando para o tipo de registro de Atividade.

Para classificar <!--ungrouped (add this when sorting for groupings will be available--> registros, faça o seguinte:

1. Crie uma exibição de tabela, conforme descrito no artigo [Gerenciar exibições de registros](/help/quicksilver/planning/views/manage-record-views.md).
1. Clique no ícone **Classificar** ![Ícone Classificar](assets/sort-icon.png) no canto superior direito da tabela

   Ou

   Passe o mouse sobre o nome de uma coluna na exibição de tabela, clique na seta para baixo à direita do nome do cabeçalho da coluna e clique em **Classificar por este campo**. O campo é adicionado como uma seleção de classificação no ícone Classificar no canto superior direito da exibição de tabela.

1. (Condicional) Na caixa **Classificar registros por**, clique em um dos campos sugeridos ou clique em **Escolher um campo diferente** e procure um campo diferente. Em seguida, clique nele quando ele for exibido na lista.

   A classificação é aplicada automaticamente à exibição de tabela e os registros são classificados pelos critérios selecionados.

   <!-- add a step that you can rearrange the sorting fields here, when this will be possible-->

1. (Opcional) Clique em **Adicionar condição** e repita as etapas acima para classificar por campos adicionais.

   O número de campos que você está classificando é exibido à esquerda do ícone Classificar no canto superior direito da barra de ferramentas. Você pode escolher somente campos que sejam exibidos nas colunas da exibição de tabela.

1. (Opcional) Na caixa **Classificar registros por**, clique no ícone **x** à direita de um campo de classificação para remover a classificação

   Ou

   Clique em **Limpar tudo** para remover todos os campos da classificação.

1. Clique fora da caixa **Classificar registros por** para fechá-la.

   ![Classificando na exibição de tabela](assets/sorting-in-table-view.png)

   As informações exibidas na tabela são classificadas de acordo com os critérios selecionados.

   Os campos selecionados para a classificação exibem um ícone de classificação seguido de um número que indica a ordem em que a classificação é aplicada.

### Adicionar agrupamentos {#add-groupings}

<!--this section exists in the timeline view too, but the display is slightly different, so I kept both steps; consider updating both sections if any updates to groupings are introduced-->

Você pode agrupar registros por informações semelhantes ao aplicar um agrupamento a uma exibição.

Considere o seguinte:

* Você pode aplicar agrupamentos nas visualizações de tabela e linha do tempo. Os agrupamentos da exibição de tabela são independentes daqueles na exibição de linha do tempo do mesmo tipo de registro.
* Você pode aplicar três níveis de agrupamento em uma visualização. Os registros são agrupados na ordem de agrupamentos selecionada.
&lt;!—* É possível aplicar até 4 níveis de agrupamento ao usar a API. —verificando este por enquanto—>
* Os agrupamentos são exclusivos para a exibição selecionada. Duas exibições de tabela do mesmo tipo de registro podem ter agrupamentos diferentes aplicados a elas. Dois usuários observando a mesma visualização de tabela veem o mesmo agrupamento aplicado no momento.
* Não é possível nomear os agrupamentos criados para uma exibição de tabela.
* A remoção de agrupamentos os remove de qualquer pessoa que acesse o mesmo tipo de registro que você e que exiba a mesma visualização que você.
* É possível editar registros listados em um agrupamento.
* Você pode agrupar por campos de registro conectados ou campos de pesquisa.
* Quando você agrupa por campos de pesquisa com vários valores (que não foram resumidos por um agregador), os registros são agrupados por cada combinação exclusiva de valores de campo.
* Você pode fazer referência a um campo que esteja a até 4 níveis de distância do tipo de registro atual. Por exemplo, se você estiver criando um agrupamento para um tipo de registro de Atividade e a Atividade estiver conectada ao tipo de registro de Produto que está conectado ao tipo de registro de Campanha que está conectado a um Projeto do Workfront, você poderá fazer referência ao Status do projeto no agrupamento que está criando para o tipo de registro de Atividade.
* Os agrupamentos são listados na ordem alfabética de seus valores.
<!--checking into this: * You can apply up to 4 levels of grouping when using the API. -->
<!-- checking also into this: * You cannot group by a Paragraph-type field.-->

Para adicionar um agrupamento:

1. Crie uma exibição de linha do tempo para um tipo de registro, conforme descrito no artigo [Gerenciar exibições de registros](/help/quicksilver/planning/views/manage-record-views.md).
1. Clique em **Agrupamento** no canto superior direito da exibição de tabela.

   ![Exibição de tabela de interface de agrupamento com campos vinculados](assets/grouping-ui-table-view-with-linked-fields.png)

1. Clique em um dos campos sugeridos ou clique em **Escolher um campo diferente**, procure um campo diferente e clique nele quando ele for exibido na lista.

   O agrupamento é aplicado automaticamente à tabela e os registros são exibidos na linha de separação de agrupamento.

1. (Opcional) Clique em **Adicionar condição** e repita as etapas acima para adicionar até três agrupamentos.

   O número de campos selecionados para o agrupamento é exibido ao lado do ícone Grouping.

   ![Agrupamento aplicado na exibição de tabela](assets/grouping-applied-in-table-view.png)

1. (Opcional) Dentro da caixa **Agrupar registros por**, clique no ícone **x** à direita de um campo selecionado para o agrupamento para remover o agrupamento

   Ou

   Clique em **Limpar tudo** para remover todos os campos.

1. Clique fora da caixa **Agrupar registros por** para fechá-la.
1. (Opcional) Clique em **+ Novo registro** no final de qualquer agrupamento para adicionar novos registros e, em seguida, atualize a página para adicionar o novo registro ao agrupamento apropriado. <!--this might need to be changed when they add the Refresh button on the toolbar of the table view-->

1. Para expandir ou recolher agrupamentos, siga um destes procedimentos:

   1. Clique no ícone **Agrupamento** e depois em **Expandir tudo** ou **Recolher tudo**. Isso expande todos os agrupamentos e subagrupamentos na visualização de tabela.

      ![Expandir e recolher todos os botões na exibição de tabela de caixa de agrupamento](assets/expand-collapse-all-buttons-on-grouping-box-table-view.png)

   1. Clique com o botão direito do mouse em qualquer um dos cabeçalhos de agrupamento na exibição de tabela e clique em uma das seguintes opções:
      * **Expandir grupo**
      * **Recolher grupo**
      * **Expandir tudo**
      * **Recolher tudo**
      * **Expandir subgrupos**
      * **Recolher subgrupos**

      Dependendo do número de agrupamentos aplicados à exibição, algumas opções podem não estar disponíveis.

<!-- this is not available yet: 

To sort grouped records: 

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. ************************* add steps here for sorting grouped records****************

-->

### Adicionar cores da linha

1. (Opcional) Clique em **Cores da linha** para definir condições e escolher a configuração de cores diferentes para linhas da tabela.

1. Clique em **Adicionar cor** e **Selecione um campo** cujo valor você deseja determinar a cor de uma linha.

   Por exemplo, para exibir campanhas com um status de Ativo em verde, selecione **Status** e escolha um modificador e um valor para o campo.

   ![Caixa de cores de linha com status Ativo selecionado e opção de cor padrão](assets/row-colors-box-with-active-status-selected-default-color-choice.png)

1. Clique no menu suspenso do seletor de cores no canto superior esquerdo da condição selecionada para escolher a cor da condição e clique fora da caixa do seletor de cores para fechá-lo.

   ![Menu suspenso de seletor de cores na caixa Cores da linha realçado](assets/drop-down-color-picker-menu-in-row-colors-box-highlighted.png)

1. (Opcional) Clique em **Adicionar condição** para adicionar mais campos e valores ao primeiro conjunto de condições

   Ou

   Clique em **Adicionar cor** para adicionar um novo conjunto de condições e identificar uma nova cor.

   Por exemplo, você pode exibir campanhas em um status Planning em amarelo definindo um novo conjunto de condições.

   ![Caixa de cores de linha com cores personalizadas de status Ativo e do Planning](assets/row-colors-box-with-active-and-planning-status-custom-colors.png)

1. (Opcional) Ative a configuração **Aplicar a toda a linha** no canto superior direito da caixa Cores da linha. A linha inteira em que a condição é atendida é exibida automaticamente na cor selecionada.

   >[!NOTE]
   >
   >* Se a configuração Aplicar a toda a linha estiver desativada, somente o lado esquerdo do campo Primário exibirá um indicador de cor estreito com a cor selecionada. A configuração é desativada por padrão.
   >
   >* Não é possível aplicar cores de linha a uma linha inteira quando há pelo menos um agrupamento selecionado na exibição de tabela.

1. Clique fora da caixa **Cores da linha** para fechá-la. As cores são aplicadas automaticamente.

### Ativar o indicador de presença em tempo real

Os avatares de outros usuários que estão editando informações de registro ao mesmo tempo que você exibe no canto superior direito de todas as visualizações de registro, por padrão.

Ao exibir a visualização de tabela, você também pode visualizar qual campo outro usuário está editando no momento em que você está visualizando o registro.

1. Ir para uma página de tipo de registro e abrir qualquer exibição.
1. (Condicional) Se houver outros usuários editando os registros do tipo selecionado ao mesmo tempo, seus avatares serão exibidos no canto superior direito da exibição.
1. Clique no menu suspenso ao lado dos avatares e selecione a opção **Mostrar colaboradores**. O botão de alternância é selecionado por padrão.

   ![Exibir alternância de colaboradores selecionada](assets/show-collaborators-toggle-selected.png)

1. (Condicional) Abra uma exibição de tabela e o campo que outra pessoa está editando ativamente será destacado na cor correspondente ao contorno do avatar na exibição de tabela.

   Se a cor de destaque do avatar for cinza, o usuário parou de editar ativamente o registro há mais de 30 segundos.

   ![Conexão de avatar e campo da tabela de indicadores em tempo real](assets/real-time-indicator-table-field-and-avatar-connection.png)

   >[!TIP]
   >
   >Você pode selecionar a opção **Mostrar colaboradores** de qualquer modo de exibição. O campo atualmente editado por outros é descrito somente na exibição de tabela.





