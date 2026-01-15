---
navigation-topic: get-started-with-workfront
title: Usar listas aprimoradas
description: As listas aprimoradas usam um formato de tabela para exibir os itens de lista e têm uma aparência diferente das listas padrão
author: Lisa
feature: Get Started with Workfront
exl-id: 4c25ed54-b147-4fd3-8d00-6f1ba61bbd38
source-git-commit: b935f3013c1be670dea834c041e02165f0e7047c
workflow-type: tm+mt
source-wordcount: '1620'
ht-degree: 2%

---

# Usar listas aprimoradas

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
   <p>Colaborador ou superior</p>
   <p>Solicitação ou superior</p></td>
  </tr>
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Objetos que usam listas aprimoradas

Abaixo estão alguns tipos de listas de objetos do Workfront que usam o formato de lista aprimorado e algumas das áreas em que eles são exibidos por padrão quando você tem direitos para visualizar o objeto.

>[!NOTE]
>
>Esta lista não é abrangente. Cada uma dessas listas de objetos também pode aparecer em um relatório ou painel. Por exemplo, um relatório de Projeto ou um painel que contém um relatório de Projeto também exibe uma lista de projetos.

| lista do Workfront | Local da lista de objetos |
|--- |--- |
| Prioridades | <ul><li>Início > selecione o ícone Prioridades no menu esquerdo</li><li>Menu principal > Prioridades</li></ul> |
| Lista de solicitações | <ul><li>Solicitações (somente nova experiência)</li><li>Widget Minhas solicitações na página inicial</li></ul> |
| Listas de status, prioridades, severidades e taxas de câmbio em Configuração | <ul><li>Configuração > Preferências do Projeto > Status</li><li>Configuração > Preferências do Projeto > Prioridades</li><li>Configuração > Preferências do Projeto > Severidades</li><li>Configuração > Preferências do Projeto > Taxas de Câmbio</li></ul> |

## Adicionar e editar itens em uma lista aprimorada

Dependendo da configuração da lista aprimorada, pode haver duas maneiras de adicionar um item à lista:

* Clique em um botão acima da lista. Essa opção abre uma caixa de diálogo onde você insere informações e as salva.
* Clique em **Nova linha** na parte inferior da lista. Essa opção adiciona uma nova linha à tabela e você insere informações em cada célula.

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

  Ao editar uma célula, cada tipo de campo tem suas próprias opções de edição.

Para editar um item na lista, clique duas vezes na célula que deseja editar e digite as informações. Algumas células podem ser somente leitura.

![Exemplo de lista aprimorada](assets/glist-exchange-rates.png)

## Usar a barra de ações e o menu Mais em uma lista aprimorada

A barra de ações mostra ações que você pode realizar em um item da lista. Algumas ações podem ser específicas dessa lista e não aparecem em nenhuma outra lista.

1. Marque a caixa de seleção ao lado de um item na lista aprimorada.

   A barra de ação aparece na parte inferior da tela.

   >[!NOTE]
   >
   >Listas aprimoradas diferentes podem permitir a seleção de um único item, a edição em massa (seleção de mais de um item) ou nenhuma seleção de item.

1. Clique em um botão na barra de ações para realizar essa ação, como visualizar o item da lista, excluir o item ou editar o item.

   Se nenhuma ação estiver disponível para o item selecionado, a barra de ação indicará &quot;Nenhuma ação disponível&quot;.

   ![Exemplo da barra de ações](assets/glist-action-bar-statuses.png)

1. Passe o mouse sobre um campo principal de um item de lista para ver o menu **Mais**. (O campo principal é a coluna mais à esquerda da tabela.)

1. Clique no menu para ver as ações adicionais do item. Algumas ações podem ser específicas dessa lista e não aparecem em nenhuma outra lista.

   ![Mais exemplo de menu](assets/glist-more-menu-priorities.png)

## Personalizar colunas em uma lista aprimorada

Algumas listas aprimoradas permitem ocultar e exibir colunas e reordenar as colunas.

1. Clique em **Colunas** acima da lista.

   ![Exibir exemplo de colunas](assets/glist-display-move-columns.png)

1. Use os botões para exibir ou ocultar colunas na lista.
1. Para reordenar as colunas, clique no ícone **Arrastar** e mova uma coluna para o local desejado. Mover colunas altera a lista automaticamente.

   >[!NOTE]
   >
   >O campo principal é a coluna mais à esquerda da tabela. Ela é fixada na primeira posição e não é possível alterar sua coluna. Se o número de colunas for grande, o campo principal é congelado à esquerda e, ao rolar a tela horizontalmente, você sempre o verá.
   >
   >O ícone ao lado de um nome de campo mostra o tipo de campo, como texto ou campo de data.

   Um indicador é exibido no botão **Colunas** quando as colunas estão ocultas. O indicador não aparece ao reordenar as colunas.

   ![Indicador para colunas ocultas](assets/glist-columns-hidden-indicator.png)

## Adicionar e remover colunas em uma lista com o Gerenciador de colunas

Algumas listas aprimoradas oferecem o **Gerenciador de colunas**, que permite adicionar colunas facilmente à lista e remover colunas. Campos nativos e personalizados estão disponíveis para seleção como colunas. Campos personalizados devem existir no sistema antes que você possa adicioná-los como colunas de lista.

Para adicionar e remover colunas:

1. Clique no ícone + na parte superior direita da tabela para abrir a caixa **Gerenciador de colunas**.
1. Procure um campo de objeto existente na coluna **Disponível** e clique em + à direita do nome do campo para adicioná-lo à coluna **Selecionado**.
1. Clique em - à direita de um campo na coluna **Selecionado** para removê-lo da lista.

   >[!NOTE]
   >
   >Alguns campos podem ser corrigidos e não podem ser removidos.

1. Clique em **Salvar**.

   ![Gerenciador de colunas](assets/glist-column-manager.png)

<!-- Add info about Properties and KPIs when something gets released with those options -->

## Exibir dados com exibições em uma lista aprimorada

Uma exibição é um conjunto personalizado de arranjos e filtros de coluna que você pode aplicar a uma lista. Você pode criar novas visualizações e editar visualizações existentes.

### Aplicar e criar visualizações

Para aplicar uma exibição, clique na lista suspensa **Exibições** e selecione a exibição que deseja aplicar à lista.

Para criar uma nova view:

1. Clique na lista suspensa **Exibições** e selecione **Nova exibição**.
1. Insira um nome para o modo de exibição e clique em **Criar**.
1. (Opcional) Oculte, exiba ou reorganize as colunas. Para obter mais informações, consulte [Personalizar colunas em uma lista aprimorada](#customize-columns-in-an-enhanced-list).
1. (Opcional) Filtre e agrupe os itens da lista. Para obter mais informações, consulte [Filtrar e agrupar itens em uma lista aprimorada](#filter-and-group-items-in-an-enhanced-list).

   As alterações nas exibições são salvas automaticamente e ficam visíveis para qualquer pessoa que use a exibição.

   Na próxima vez que você aplicar essa visualização, as configurações de coluna e filtro permanecerão da maneira definida.

### Compartilhar uma exibição

Na lista suspensa **Exibições**, você pode ver três categorias de exibições:

* **Exibições do Sistema**: exibições que o administrador do sistema atribuiu a você.
* **Exibições compartilhadas**: exibições que foram compartilhadas com você por outros usuários.
* **Minhas Exibições**: Exibições que você criou e pode compartilhar com outras pessoas. Você pode compartilhar visualizações com outros usuários, equipes ou grupos.

Para compartilhar uma exibição:

1. Na lista suspensa **Exibições**, passe o mouse sobre a exibição em **Minhas Exibições** que você deseja compartilhar, depois clique no menu de três pontos quando ele aparecer.
1. Selecione **Compartilhar**.
1. Na caixa de diálogo Compartilhar, digite os nomes dos usuários, equipes ou grupos com os quais deseja compartilhar a exibição e selecione-os na lista quando eles forem exibidos.

   Você pode conceder as seguintes permissões aos recipients:

   * **Modo de exibição**: os usuários podem aplicar o modo de exibição à lista, mas não podem compartilhá-lo.
   * **Gerenciar**: os usuários podem renomear o modo de exibição, compartilhá-lo com outras pessoas e excluí-lo.

1. Clique em **Salvar**.

## Filtrar e agrupar itens em uma lista aprimorada

Os filtros ajudam a reduzir a quantidade de informações exibidas na lista. Agrupamentos separam os objetos na lista em áreas com base em critérios específicos.

### Usar filtros

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

1. Clique em **Adicionar condição** para adicionar outra condição ao filtro como uma instrução OR.
1. Quando o filtro for aplicado, você poderá abrir as opções **Filtro** novamente para alterar as opções de filtro ou limpar todos os filtros.

   Um indicador é exibido no botão **Filtro** quando um filtro é aplicado à lista.

   ![Indicador aplicado de filtro](assets/glist-filter-applied-indicator.png)

### Usar agrupamentos

1. Clique em **Grupo** acima da lista.
1. Selecione um agrupamento para organizar sua lista.

   ![Selecionar um agrupamento](assets/glist-grouping-choose-a-group-by.png)

1. Quando o agrupamento é aplicado, você pode abrir as opções de Grupo novamente para recolher ou expandir todos os agrupamentos de uma vez, alterar o agrupamento para agrupar por um campo diferente ou limpar todos os agrupamentos.

   ![Agrupamento em listas aprimoradas](assets/glist-group-by-due-date-priorities.png)

   Um indicador é exibido no botão **Grupo** quando um agrupamento é aplicado à lista.

   ![Indicador de agrupamento aplicado](assets/glist-grouping-applied-indicator.png)

## Classificar e pesquisar em uma lista aprimorada

Para classificar colunas individuais:

1. Vá para a coluna e clique na seta para baixo.

   Um ícone ao lado de um nome de coluna indica que a lista é classificada pelos valores dessa coluna e a direção da classificação.

   >[!NOTE]
   >
   >Algumas colunas podem não ser classificáveis, dependendo da lista.

   ![Classificar por uma coluna](assets/glist-sort-by-column.png)

Para classificar seu trabalho em um agrupamento:

1. Clique em **Grupo** e selecione se deseja classificar em ordem crescente ou decrescente.

   ![Classificar em um agrupamento](assets/sort-in-groups.png)

Para pesquisar:

1. Digite o termo de pesquisa no campo de pesquisa acima da lista. Os resultados são destacados na lista à medida que você digita.

   ![Termo de pesquisa destacado](assets/glist-search-highlighted.png)
