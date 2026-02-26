---
navigation-topic: get-started-with-workfront
title: Usar listas aprimoradas
description: As listas aprimoradas usam um formato de tabela para exibir os itens de lista e têm uma aparência diferente das listas padrão
author: Lisa
feature: Get Started with Workfront
exl-id: 4c25ed54-b147-4fd3-8d00-6f1ba61bbd38
source-git-commit: 8e2f41f18b57aca77fd6af905ff8e04486879e39
workflow-type: tm+mt
source-wordcount: '2315'
ht-degree: 2%

---

# Usar listas aprimoradas

{{preview-fast-release-general}}

As listas aprimoradas estão disponíveis em algumas áreas do Adobe Workfront. Essas listas usam um formato de tabela para exibir os itens de lista e têm uma aparência diferente das listas padrão. O gerenciamento de visualizações também é aprimorado, incluindo filtragem, agrupamento, gerenciamento de colunas e pesquisa.

Para obter informações sobre as listas padrão, consulte [Introdução a listas no Adobe Workfront](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

>[!NOTE]
>
>Cada lista aprimorada pode ser configurada de forma diferente para ajudar a exibir os dados necessários. Todas as listas não usarão todos os recursos descritos neste artigo e algumas listas podem ter recursos especializados que se aplicam somente a essa lista.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td>
   <p>Colaborador ou posterior</p>
   <p>Solicitação ou posterior</p></td>
  </tr>
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Objetos que usam listas aprimoradas

Abaixo estão alguns tipos de listas de objetos do Workfront que usam o formato de lista aprimorado e algumas das áreas em que eles são exibidos por padrão quando você tem direitos para visualizar o objeto.

>[!NOTE]
>
>Esta lista não é abrangente. Cada uma dessas listas de objetos também pode aparecer em um relatório ou painel. Por exemplo, um relatório de Solicitação ou um painel que contém um relatório de Solicitação também exibe uma lista de solicitações.

| lista do Workfront | Local da lista de objetos |
| --- | --- |
| Prioridades | <ul><li>Início > selecione o ícone Prioridades no menu esquerdo</li><li>Menu principal > Prioridades</li></ul> |
| Lista de solicitações | <ul><li>Solicitações (somente nova experiência)</li><li>Widget Minhas solicitações na página inicial</li></ul> |
| Listas de status, prioridades, severidades e taxas de câmbio em Configuração | <ul><li>Configuração > Preferências do Projeto > Status</li><li>Configuração > Preferências do Projeto > Prioridades</li><li>Configuração > Preferências do Projeto > Severidades</li><li>Configuração > Preferências do Projeto > Taxas de Câmbio</li></ul> |

<!--|<span class="preview">List of reports</span> | <span class="preview">Main Menu &gt; Reports</span> <p><span class="preview">The enhanced list format is only applied when **Use shareable folders** is turned on. For information, see [Use shareable report folders](/help/quicksilver/reports-and-dashboards/reports/report-usage/use-sharable-report-folders.md).</span> |-->

## Adicionar itens a uma lista aprimorada

Dependendo da lista aprimorada que você estiver visualizando, execute um dos procedimentos a seguir:

1. Clique no botão azul no canto superior direito da lista. Essa opção abre uma caixa de diálogo onde você pode inserir informações. Os dados são salvos como uma nova linha na tabela.

   OR

1. Clique em **Nova linha** na parte inferior da lista. Essa opção adiciona uma nova linha à tabela. Clique duas vezes em uma célula para inserir informações nela. Cada célula representa um campo para o item de lista. Os campos devem existir antes de você vê-los na lista.

   As listas aprimoradas são compatíveis com estes tipos de campo:

   * Texto
   * Número
   * Moeda
   * Data
   * Data e hora
   * Menus suspensos de seleção única/múltipla
   * Typeahead
   * Parágrafo
   * Destinatário (um ou vários)
   * Seletor de cores

   >[!NOTE]
   >
   >Cada tipo de campo tem suas próprias opções de edição. Alguns campos podem ser somente leitura.

![Exemplo de lista aprimorada](assets/glist-exchange-rates.png)

## Editar itens usando a barra de ação

Você pode usar a barra de ações em uma lista aprimorada para editar itens na lista. Nem todas as barras de ação incluem as mesmas opções. Além disso, algumas listas podem não permitir a seleção de itens e a barra de ação não está disponível.

1. Marque a caixa de seleção ao lado de um item em uma lista aprimorada.

   A barra de ação aparece na parte inferior da tela.

   >[!NOTE]
   >
   >Dependendo da lista editada, é possível selecionar um ou vários itens para usar a barra de ação.

1. Clique em uma ação na barra para editar itens. Exemplos de ações que você pode escolher são:

   * Exibir
   * Editar
   * Excluir

   Se nenhuma ação estiver disponível para o item selecionado, a barra de ação exibirá &quot;Nenhuma ação disponível&quot;.

   ![Exemplo da barra de ações](assets/glist-action-bar-statuses.png)

1. Passe o mouse sobre o campo principal de um item de lista, em seguida, clique no ícone de menu **Mais** ![Mais](assets/more-icon.png) para ver ações adicionais. Algumas ações podem ser específicas dessa lista.

   >[!TIP]
   >
   >O campo principal é exibido na primeira coluna da lista.

   ![Mais exemplo de menu](assets/glist-more-menu-priorities.png)

## Personalizar colunas

Dependendo dos objetos que você está visualizando em uma lista aprimorada, é possível ocultar, mostrar ou reordenar colunas na lista.

1. Clique em **Colunas** acima da lista.

   ![Exibir exemplo de colunas](assets/glist-display-move-columns.png)

1. Use os botões para exibir ou ocultar colunas na lista.
1. Para reordenar as colunas, clique no ícone **Arrastar** ![Ícone Arrastar](assets/drag-icon.png) e mova uma coluna para o local desejado. Mover colunas altera a lista automaticamente.

   >[!NOTE]
   >
   >O campo principal é a primeira coluna na lista. Ela é fixada na primeira posição e não é possível alterar sua coluna. Se o número de colunas for grande, o campo principal é congelado à esquerda e, ao rolar a tela horizontalmente, você sempre o verá.
   >
   >O ícone ao lado de um nome de campo mostra o tipo de campo, como texto ou campo de data.

   Um indicador é exibido no botão **Colunas** quando as colunas estão ocultas. O indicador não aparece ao reordenar as colunas.

   ![Indicador para colunas ocultas](assets/glist-columns-hidden-indicator.png)

### Renomear colunas

Algumas colunas permitem salvar um nome personalizado para o título da coluna.

1. Passe o mouse sobre a coluna, clique na seta para baixo e selecione **Renomear**.

   ![Selecionar Renomear na coluna](assets/glist-rename-or-sort-column.png)

1. Na caixa de diálogo **Renomear**, digite o nome da coluna no campo **Rótulo personalizado** e clique em **Salvar**.

   O novo nome da coluna aparece na lista.

## Adicionar e remover colunas com o Gerenciador de colunas

Você pode usar o **Gerenciador de colunas** em algumas listas aprimoradas para adicionar e remover facilmente colunas na lista. Você pode adicionar ou remover campos personalizados e do sistema que já existem no Workfront como colunas para uma lista aprimorada.

Para adicionar e remover colunas:

1. Clique no ícone + no canto superior direito da tabela para abrir a caixa **Gerenciador de colunas**.
1. Procure um campo de objeto existente na coluna **Disponível** e clique em + à direita do nome do campo para adicioná-lo à coluna **Selecionado**.
1. Clique em - à direita de um campo na coluna **Selecionado** para removê-lo da lista.

   >[!NOTE]
   >
   >Alguns campos podem ser corrigidos e não podem ser removidos.

   <!-- Add info about Properties and KPIs when something gets released with those options -->

1. Clique em **Salvar**.

   ![Gerenciador de colunas](assets/glist-column-manager.png)

   A lista atualiza as colunas de acordo com as escolhas feitas.

## Atualizar elementos de lista aprimorados

Os seguintes elementos são componentes de uma lista aprimorada:

* Exibir: define as colunas, os filtros e os agrupamentos na lista com configurações predefinidas
* Filtros: limita a quantidade de informações exibidas na lista
* Agrupamentos: organize os itens da lista de acordo com campos comuns
* Classificar: organiza os itens em uma lista de acordo com a ordem identificada para um determinado campo
* Pesquisa: localiza rapidamente um item usando uma palavra-chave de pesquisa

### Aplicar e criar visualizações

>[!NOTE]
>
>Nem todas as listas aprimoradas têm todos os elementos descritos nesta seção.

Para aplicar ou criar uma view:

1. Clique na lista suspensa **Exibições** e selecione uma exibição existente para aplicá-la à lista

   OR

   Clique em **Novo modo de exibição** para criar um.

1. (Condicional) Para adicionar um novo modo de exibição, insira um nome para o modo de exibição e clique em **Criar**.
1. (Opcional) Oculte, exiba ou reorganize as colunas. Para obter mais informações, consulte [Personalizar colunas em uma lista aprimorada](#customize-columns-in-an-enhanced-list).
1. (Opcional) Filtre a lista. Para obter mais informações, consulte [Filtrar itens em uma lista aprimorada](#filter-items-in-an-enhanced-list).
1. (Opcional) Agrupe os itens na lista. Para obter mais informações, consulte [Agrupar itens em uma lista aprimorada](#group-items-in-an-enhanced-list).

   As alterações nas exibições são salvas automaticamente. Na próxima vez que você aplicar essa visualização, as configurações de coluna e filtro permanecerão da maneira definida.

### Filtrar itens em uma lista aprimorada

>[!NOTE]
>
>Nem todas as listas aprimoradas têm todos os elementos descritos nesta seção.

Os filtros ajudam a reduzir a quantidade de informações exibidas na lista.

1. Clique em **Filtro** acima da lista.
1. Na caixa Filtro, clique em **Adicionar condição**.
1. Selecione um campo para filtrar.
1. Selecione um modificador de filtro, como &quot;Tem qualquer um de&quot;, &quot;Não tem nenhum de&quot;, &quot;É antes&quot; ou &quot;É depois de&quot;. As opções do modificador são diferentes dependendo do tipo de campo pelo qual você está filtrando.
1. Selecione o valor ou os valores do campo. Dependendo do tipo de campo pelo qual você está filtrando, talvez seja solicitado que você selecione o item em uma lista, pesquise por ele ou use um calendário para selecionar um intervalo de datas.

   ![Filtrar em listas aprimoradas](assets/glist-filter-with-options.png)

   O filtro é aplicado automaticamente à lista.

   >[!TIP]
   >
   >Para aplicar um curinga de usuário atual, selecione **Eu (usuário conectado)** como o valor do campo. O filtro será aplicado ao usuário que está visualizando a lista. Esse curinga está disponível em campos nos quais o valor é um usuário.

1. Clique em **Adicionar condição** para adicionar outra condição ao filtro.

   É possível unir vários filtros por um conector AND ou OR.

1. Quando o filtro for aplicado, você poderá abrir as opções **Filtro** novamente para alterar as opções de filtro ou limpar todos os filtros.

   Um indicador é exibido no botão **Filtro** quando um filtro é aplicado à lista.

   ![Indicador aplicado de filtro](assets/glist-filter-applied-indicator.png)

### Agrupar itens em uma lista aprimorada

>[!NOTE]
>
>Nem todas as listas aprimoradas têm todos os elementos descritos nesta seção.

Agrupamentos separam os objetos na lista em áreas com base em critérios específicos.

O Workfront fornece um número limitado de agrupamentos predefinidos e você não pode modificá-los.

1. Clique em **Grupo** acima da lista.
1. Selecione um agrupamento para organizar sua lista.

   ![Selecionar um agrupamento](assets/glist-grouping-choose-a-group-by.png)

1. Clique em **Recolher tudo** para exibir a lista com todos os agrupamentos recolhidos. A opção padrão é exibir a lista com todos os agrupamentos expandidos.
1. Quando o agrupamento é aplicado, você pode abrir as opções de Grupo novamente para recolher ou expandir todos os agrupamentos de uma vez, alterar o agrupamento para agrupar por um campo diferente ou limpar todos os agrupamentos.

   ![Agrupamento em listas aprimoradas](assets/glist-group-by-due-date-priorities.png)

   Um indicador é exibido no botão **Grupo** quando um agrupamento é aplicado à lista.

   ![Indicador de agrupamento aplicado](assets/glist-grouping-applied-indicator.png)

### Classificar em uma lista aprimorada

>[!NOTE]
>
>Nem todas as listas aprimoradas têm todos os elementos descritos nesta seção.

Para classificar colunas individuais:

1. Passe o mouse sobre a coluna, clique na seta para baixo e selecione **Classificar**.

   Um ícone ao lado de um nome de coluna indica que a lista é classificada pelos valores dessa coluna e a direção da classificação.

   >[!NOTE]
   >
   >Algumas colunas podem não ser classificáveis, dependendo da lista.

   ![Classificar por uma coluna](assets/glist-sort-by-column.png)

Para classificar seu trabalho em um agrupamento:

1. Clique em **Grupo**, vá para a linha do agrupamento aplicado, clique na lista suspensa classificador e selecione uma ordem crescente ou decrescente.

   ![Classificar em um agrupamento](assets/sort-in-groups.png)

### Pesquisar em uma lista aprimorada

>[!NOTE]
>
>Nem todas as listas aprimoradas têm todos os elementos descritos nesta seção.

1. digite a palavra-chave pela qual deseja pesquisar na caixa Pesquisar no canto superior direito da lista. Os resultados são destacados na lista à medida que você digita.

   ![Termo de pesquisa destacado](assets/glist-search-highlighted.png)

   >[!NOTE]
   >
   >A pesquisa procura em todas as colunas em todos os itens da lista. Se a lista for longa, a pesquisa incluirá itens que talvez você precise rolar para ver. Quando a lista é filtrada, a pesquisa só verifica o que está sendo exibido no momento.

### Compartilhar uma exibição

>[!NOTE]
>
>Nem todas as listas aprimoradas têm todos os elementos descritos nesta seção.

Na lista suspensa **Exibições**, você pode ver três categorias de exibições:

* **Exibições do Sistema**: exibições que o administrador do sistema atribuiu a você. Não é possível compartilhar visualizações do sistema.
* **Exibições compartilhadas**: exibições que foram compartilhadas com você por outros usuários.
* **Minhas Exibições**: Exibições que você criou e pode compartilhar com outras pessoas. Você pode compartilhar visualizações com outros usuários, equipes ou grupos.

Quando você compartilha uma exibição, todos os elementos de exibição (colunas, filtros e agrupamentos) são incluídos.

Para compartilhar uma exibição:

1. Na lista suspensa **Exibições**, passe o mouse sobre a exibição em **Minhas Exibições** que você deseja compartilhar, clique no menu **Mais** ![Mais menu](assets/more-icon.png) e clique em **Compartilhar**.
1. Na caixa de diálogo Compartilhar, digite os nomes dos usuários, equipes, grupos, empresas ou funções de trabalho com os quais deseja compartilhar a exibição e selecione-os na lista quando eles forem exibidos.

   Você pode conceder as seguintes permissões aos recipients:

   * **Modo de exibição**: os usuários podem aplicar o modo de exibição à lista, mas não podem compartilhá-lo.

     <span class="preview">Quando os usuários do acesso de Visualização atualizam a visualização, essas alterações são salvas nas preferências pessoais do usuário. Um ponto azul no nome da exibição (nas **Exibições Compartilhadas** do usuário) mostra que atualizações pessoais são aplicadas à exibição.</span>

   * **Gerenciar**: os usuários podem renomear, compartilhar ou excluir o modo de exibição e editar os seus elementos.

     <span class="preview">Quando a opção Gerenciar acesso fizer alterações na exibição, todos os usuários que tiverem a exibição compartilhada com eles verão essas atualizações quando a exibição for aplicada à lista.</span>

1. Clique em **Salvar**.

   <span class="preview">Se você compartilhar um modo de exibição com um usuário e depois remover esse acesso, o modo de exibição será removido das **Exibições Compartilhadas** do usuário. Se o usuário tiver a exibição compartilhada aplicada à lista quando seu acesso for removido, a exibição padrão do sistema será aplicada.</span>

<div class="preview">

### Copiar uma exibição

>[!NOTE]
>
>Nem todas as listas aprimoradas têm todos os elementos descritos nesta seção.

Quando uma exibição é compartilhada com você e você não tem permissão para editar, é possível copiar a exibição e salvá-la com um novo nome. Você deve primeiro fazer alterações na exibição antes de copiá-la.

1. Na lista suspensa Exibições, passe o mouse sobre a exibição em **Exibições Compartilhadas** que você deseja copiar, clique no menu **Mais** ![Mais menu](assets/more-icon.png) e clique em **Copiar com preferências**.

   Uma nova visualização é criada automaticamente. Ele usa o nome de exibição original com (cópia) no final e aparece na seção de exibições **Minhas Exibições**.

   Você é o proprietário desta exibição e pode renomeá-la, editá-la, compartilhá-la ou excluí-la. Se o proprietário da visualização original remover o acesso compartilhado a ela, você ainda terá acesso a esta visualização criada.

   >[!NOTE]
   >
   >A opção **Copiar com Preferências** só estará disponível depois que você fizer alterações em uma exibição que foi compartilhada com você.

</div>

<div class="preview">

### Redefinir uma visualização

>[!NOTE]
>
>Nem todas as listas aprimoradas têm todos os elementos descritos nesta seção.

Quando uma exibição é compartilhada com você e você não tem permissão para editar e atualiza essa exibição, é possível redefini-la para a exibição original.

1. Na lista suspensa **Exibições**, passe o mouse sobre a exibição em **Exibições Compartilhadas** que você deseja redefinir, clique no menu **Mais** ![Mais menu](assets/more-icon.png) e clique em **Redefinir para o padrão**.

   Os elementos de exibição (colunas, filtros e agrupamentos) são redefinidos para as configurações originais que foram compartilhadas com você.

   >[!NOTE]
   >
   >A opção **Redefinir para o padrão** só estará disponível depois que você fizer alterações em uma exibição compartilhada com você.

   ![Copiar e redefinir opções de exibição](assets/glist-copy-view-shared-with-you.png)

</div>
