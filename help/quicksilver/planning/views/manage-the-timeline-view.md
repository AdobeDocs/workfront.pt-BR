---
title: Gerenciar a exibição de linha do tempo
description: Acesse e edite registros em uma exibição de linha do tempo na página tipo de registro do Adobe Workfront Planning. Este artigo descreve como criar uma visualização de linha do tempo e editar ou excluir uma existente. Personalize a linha do tempo com filtros, agrupamentos e configurações. Use o recurso Detalhamento para exibir registros conectados.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: f348af7f-5bb9-4d88-9bcb-3bef7e8892dd
source-git-commit: 9debb7c6d9df0f9f4962f3e66f146e5f605d20f0
workflow-type: tm+mt
source-wordcount: '2638'
ht-degree: 0%

---

# Gerenciar a exibição de linha do tempo

{{planning-important-intro}}

Você pode exibir registros em uma exibição de linha do tempo, ao acessar a página tipo de registro no Adobe Workfront Planning.

Para obter informações sobre exibições de registros, consulte [Gerenciar exibições de registros](/help/quicksilver/planning/views/manage-record-views.md).

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso do Workfront Planning.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

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
   <td role="rowheader"><p>Plano de planejamento do Adobe Workfront*</p></td> 
   <td> 
<p>Qualquer </p> 
<p>Para obter mais informações sobre o que está incluído em cada plano do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma Adobe Workfront</p></td> 
   <td> 
<p>A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para acessar todos os recursos do Workfront Planning.</p> 
<p>Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada do Adobe para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td> 
   <td><p> Padrão </p>
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
   <p>Permissões de exibição para uma exibição para alterar temporariamente as configurações de exibição</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modelo de layout</p></td> 
   <td> <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclua a área Planejamento no Menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--OLD: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   Or
   <p>Current: Plan </p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> There are no access controls for Adobe Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->


## Gerenciar uma exibição de linha do tempo {#manage-a-timeline-view}

<!--insert screen shot of timeline view-->

Ao criar uma exibição de linha do tempo, todos os registros do tipo de registro selecionado são exibidos em uma linha do tempo cronológica.

Considere o seguinte:

* Você pode criar um modo de exibição de Linha do tempo somente quando tem pelo menos dois campos de data associados a um tipo de registro. Quando você tem um ou nenhum campo de data associado a um tipo de registro, a opção de exibição Linha do tempo fica esmaecida.

  Você pode selecionar entre os seguintes campos de data ao criar uma exibição de linha do tempo:

   * Registrar datas
   * Registrar campos gerados pelo sistema: Data de criação, Data da última modificação
   * Pesquisar datas de tipos de objeto ou registro conectado.
* Dependendo das datas associadas aos registros, alguns registros podem não ser exibidos na exibição de linha do tempo nos seguintes cenários:

   * Quando as datas de início e término não têm valores
   * Quando as datas de Início ou Término não têm valor
   * Quando a data inicial for posterior à data final

Para gerenciar uma exibição de linha do tempo:

1. Vá para a página do tipo de registro para a qual deseja exibir a linha do tempo.
1. Crie uma exibição de linha do tempo, conforme descrito no artigo [Gerenciar exibições de registros](/help/quicksilver/planning/views/manage-record-views.md).

   ![](assets/timeline-view-example.png)

   Os registros associados ao tipo de registro selecionado são exibidos como barras em uma linha do tempo e são classificados em ordem cronológica de sua Data inicial, por padrão.

   >[!TIP]
   >
   >    A classificação dos registros na linha do tempo não está visível na exibição Compacta.

1. (Opcional e condicional) Quando o nome do registro estiver truncado, passe o mouse sobre uma barra de registro para exibir o nome completo do registro e informações adicionais.

1. Siga um destes procedimentos para navegar pela linha do tempo:

   * Clique nos ícones esquerdo e direito ou use a rolagem horizontal para mover-se para trás e para frente na linha do tempo. Atualizar a página preserva o intervalo de tempo selecionado.
   * Clique em **Hoje** para centralizar a linha do tempo para a data de hoje.
   * Selecione uma das seguintes opções no menu suspenso de intervalo de tempo para atualizar os incrementos de tempo:

      * Ano
      * Trimestre
      * Mês
1. Clique na exibição **Alternar para Padrão** para exibir registros em linhas separadas <!--check to see if they updated the name of the setting here-->

   Ou

   Clique em **Alternar para o modo de exibição Compacto** para exibir os registros cujas datas não se cruzam na mesma linha. <!--check to see if they updated the name of the setting here-->

   Os registros são exibidos na exibição Compacta por padrão.

1. Faça o seguinte para localizar rapidamente registros que correspondam a uma palavra-chave:

   1. Clique no ícone ![](assets/search-icon.png) da **Pesquisa** e comece a digitar uma palavra-chave associada a qualquer campo de um registro exibido na tela. O número de correspondências corretas é exibido ao lado do item de pesquisa e o registro com a correspondência correta é realçado.

      ![](assets/search-box-and-results-timeline-view.png)

      Você pode usar qualquer palavra ou caractere especial visível na tela.

      Não é possível usar palavras-chave associadas a campos que não são exibidos na exibição de linha do tempo.

   1. Pressione Enter no teclado para ir para o próximo campo encontrado.
   1. (Opcional) Se houver mais de uma correspondência, clique nas setas para cima e para baixo à direita da palavra-chave de pesquisa para localizar todas as correspondências na tabela.
   1. Clique no ícone **x** na caixa de pesquisa para limpar a palavra-chave de pesquisa.

1. Atualize os seguintes elementos de exibição conforme descrito nas subseções abaixo:
   * [Filtros](#add-filters)
   * [Agrupamento](#add-grouping)
   * [Configurações](#edit-the-timeline-view-settings)
     <!--* [Sort](#add-sort) not yet in timeline; also check the anchor and make sure it's correct-->

1. (Opcional) Clique em **Detalhamento** para exibir os registros conectados na linha do tempo.

   Para obter informações, consulte a seção [Usar o recurso de Detalhamento para exibir registros conectados na exibição de linha do tempo](#break-down-connected-records-in-the-timeline-view)

### Adicionar filtros

Você pode reduzir a quantidade de informações exibidas na tela usando filtros.

Considere o seguinte ao trabalhar com filtros na exibição de linha do tempo:

<!-- this list is almost identical to the one for the table view - update both-->

* Os filtros criados para uma exibição de linha do tempo funcionam independentemente dos filtros em qualquer outra exibição aplicada ao mesmo tipo de registro.

* Os filtros são exclusivos para a exibição selecionada. Duas exibições de linha do tempo do mesmo tipo de registro podem ter filtros diferentes aplicados a elas.

* Dois usuários que visualizam a mesma linha do tempo veem o mesmo filtro aplicado no momento.

* Não é possível nomear os filtros criados para uma exibição de linha do tempo.

* A remoção de filtros os remove de qualquer pessoa que acesse o mesmo tipo de registro que você e que exiba a mesma visualização que você.

* A adição de filtros na exibição de linha do tempo é idêntica à adição de filtros na exibição de tabela.

  Para obter mais informações, consulte a seção &quot;Adicionar filtros&quot; no artigo [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md).

* Você pode filtrar por campos de registro conectados ou campos de pesquisa.
* Você pode filtrar por campos de pesquisa que exibem vários valores.


### Adicionar agrupamento

<!-- groupings are almost identical between this view and table  but they display a little differently, so I kept the steps for both; update in both places if they make changes to groupings-->

Você pode agrupar registros por informações semelhantes ao aplicar um agrupamento a uma exibição.

Adicionar agrupamentos na exibição de linha do tempo é semelhante a adicionar agrupamentos à exibição de tabela.

Considere o seguinte ao trabalhar com agrupamentos na exibição de linha do tempo:

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
<!--checking into this: * You can apply up to 4 levels of grouping when using the API. -->
<!-- checking also into this: * You cannot group by a Paragraph-type field.-->

Para adicionar um agrupamento na exibição de linha do tempo:

1. Crie uma exibição de linha do tempo para um tipo de registro, conforme descrito no artigo [Gerenciar exibições de registros](/help/quicksilver/planning/views/manage-record-views.md).
1. Clique em **Agrupamento** no canto superior direito do modo de exibição de linha do tempo.

   ![](assets/grouping-ui-timeline-view-with-linked-fields.png)

1. Clique em um dos campos sugeridos ou clique em **Escolher um campo diferente**, procure um campo diferente e clique nele quando ele for exibido na lista.

   O agrupamento é aplicado automaticamente à linha do tempo e os registros são exibidos dentro da caixa de agrupamento.

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. (Opcional) Repita as etapas acima para adicionar até três agrupamentos.

   O número de campos selecionados para o agrupamento é exibido ao lado do ícone Grouping.

   <!-- update screen shot with view redesign-->

   ![](assets/grouping-applied-in-timeline-view.png)

1. (Opcional) Dentro da caixa **Agrupar registros por**, clique no ícone **x** à direita de um campo selecionado para o agrupamento para remover o agrupamento

   Ou

   Clique em **Limpar tudo** para remover todos os campos.

1. Clique fora da caixa **Agrupar registros por** para fechá-la.
1. (Opcional) Clique em **Configurações** e depois em **Cor** para agrupar o código de cores. Para obter mais informações, consulte a seção [Editar as configurações de exibição da linha do tempo](#edit-the-timeline-view-settings) neste artigo.

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### Editar as configurações de exibição da linha do tempo {#edit-the-timeline-view-settings}

Atualize as configurações de exibição da linha do tempo para indicar quais informações e como elas são exibidas na seção de linha do tempo da exibição.

1. Crie uma exibição de linha do tempo para um tipo de registro, conforme descrito no artigo [Gerenciar exibições de registros](/help/quicksilver/planning/views/manage-record-views.md).
1. Clique em **Configurações**.
1. Clique em **Data e hora** no painel esquerdo e selecione uma **Data de início** e uma **Data de término** para exibir na linha do tempo. Você pode escolher as datas padrão de Início e Término ou escolher qualquer campo de data disponível. As barras que representam os registros começam na data que você indica para a Data inicial e terminam na data correspondente à Data final.

   >[!NOTE]
   >
   >Os registros que não têm valores para as datas de Início ou Término ou que têm uma data de Início posterior à data de Término não são exibidos na exibição de linha do tempo.

1. Clique em **Estilo de barra** no painel esquerdo para indicar quais campos você deseja exibir nas barras de registro.

   O campo principal (ou título) do registro, conforme definido na exibição de tabela do registro, é selecionado por padrão. <!--adjust this when the primary field is released??-->

1. (Opcional e condicional) Se você adicionou miniaturas a registros, selecione a opção Miniatura para exibir a imagem associada aos registros na barra de registro.

   >[!NOTE]
   >
   >    Você deve primeiro adicionar miniaturas na exibição de tabela antes de exibi-las na exibição de linha do tempo. Para obter mais informações, consulte [Adicionar uma miniatura a um registro](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

1. Clique em **Adicionar campo** para adicionar até 4 campos às barras de registro.
1. Clique dentro da caixa **Pesquisar campos** e clique no campo que deseja adicionar.

   >[!TIP]
   >
   >   * Você deve criar os campos antes de adicioná-los às barras de registro.
   > 
   >   * Você deve ter pelo menos um campo selecionado. O **Nome** está selecionado por padrão.

   Uma visualização da aparência das barras na linha do tempo é exibida à direita.

   ![](assets/record-details-panel-timeline-settings-with-preview.png)

1. Clique em **Cor** no painel esquerdo para personalizar as cores dos registros e agrupamentos na linha do tempo.

   ![](assets/color-tab-timeline-view.png)

1. (Condicional e opcional) Se você adicionou um agrupamento à exibição de linha do tempo, selecione uma das seguintes opções para definir uma cor para o agrupamento na seção **Definir cor de agrupamento**:

   * **Padrão (cinza)**: a cor dos agrupamentos está definida como cinza. Este é o padrão.
   * **Valores do campo**: a cor dos agrupamentos corresponde à cor do campo pelo qual você faz o agrupamento.

     >[!NOTE]
     >
     >    * É possível corresponder a cor somente a campos com opções codificadas por cores. Por exemplo, é possível corresponder a cor aos campos Status ou aos campos com opções associadas a cores.
     >    
     >    * Não é possível corresponder a cor a campos de pesquisa de tipos de objeto ou registro vinculado.


   Por exemplo, campos de seleção múltipla ou seleção única podem ter opções codificadas por cores.

   Se você agrupar por campos sem opções codificadas por cores, a cor de agrupamento permanecerá cinza.

   >[!TIP]
   >
   >Se você não tiver adicionado agrupamentos à exibição de linha do tempo, esta seção não será exibida.

1. Na seção **Definir cor do registro**, selecione uma das seguintes opções para definir uma cor para os registros:

   * **Tipo de registro**: a cor dos registros corresponde à cor do tipo de registro selecionado. Esta é a opção padrão.
   * **Valores de campo**: a cor dos registros corresponde à cor de um campo especificado. Continue na etapa 10. <!--ensure this stays accurate-->
   * **Agrupamento**: a cor dos registros corresponde à cor indicada para os agrupamentos. Essa opção fica esmaecida quando não há agrupamentos aplicados à exibição de linha do tempo.
   * **Nenhum**: os registros são exibidos em uma barra branca.

1. (Condicional) Se você selecionou **Valores de campo** para as cores do registro, selecione um campo no menu suspenso **Corresponder a cor do registro a**.

   ![](assets/field-selector-drop-down-menu-timeline-view.png)

   Somente campos com opções codificadas por cores são exibidos no menu suspenso.

   Por exemplo, campos de seleção múltipla ou seleção única podem ter opções codificadas por cores.

   Se você não tiver um campo com opções codificadas por cores para o tipo de registro selecionado, essa opção ficará esmaecida.

1. Clique em **Salvar**.

   Os registros são exibidos na exibição de linha do tempo com as especificações selecionadas.

### Use o recurso Detalhamento para exibir registros conectados na exibição de linha do tempo

Você pode exibir registros conectados na visualização da linha do tempo de um registro usando o recurso Detalhamento. Detalhar os registros por suas conexões permite visualizar as linhas do tempo de outros registros conectados e entender como elas podem afetar o desempenho e os prazos de conclusão de seus registros.

#### Considerações ao usar o recurso Detalhamento

* Você pode exibir registros ou objetos conectados nos registros do tipo de registro selecionado na exibição de linha do tempo.
* Você pode exibir o seguinte na exibição de linha do tempo, usando o recurso Detalhamento:
   * Registros do Workfront Planning conectados ao tipo de registro selecionado.
   * Tipos de objetos do Workfront ou ativos de Experience Manager conectados ao tipo de registro selecionado.
   * Registros ou objetos do Workfront Planning de outro aplicativo que estão conectados a registros conectados ao tipo de registro selecionado.

     Por exemplo, você pode conectar campanhas a portfólios. Além disso, você pode conectar outro tipo de registro, produtos, a projetos, e a campanhas. Ao criar a visualização da linha do tempo da campanha, você pode detalhar as campanhas por portfólios, produtos e projetos.

* Não é possível exibir tipos de objetos que estão conectados somente a objetos do Workfront no Workfront, mas que não estão conectados a um tipo de registro do Workfront Planning. Você só pode exibir tipos de objeto ou de registro que estejam conectados no Workfront Planning.

  Por exemplo, tarefas, estão conectadas a projetos no Workfront. Usando o recurso Detalhamento, você pode exibir projetos que estão conectados a campanhas no Planning, mas não tarefas conectadas a projetos no Workfront.

  Se você quiser exibir portfólios e projetos na exibição de linha do tempo de um tipo de registro do Workfront Planning, os portfólios e os projetos deverão estar conectados ao registro do Planning ou a um registro conectado ao registro do Planning cuja exibição de linha do tempo você está gerenciando.
* Você só pode exibir tipos de registro associados a pelo menos dois campos de data.
* Os campos de data para os tipos de registro que você deseja exibir na exibição de linha do tempo devem estar visíveis na exibição de tabela do tipo de registro selecionado, como campos de pesquisa.
* As datas de Início e Término dos tipos de registro que você deseja exibir na exibição de linha do tempo devem estar em ordem cronológica. Por exemplo, se um registro tiver uma data de início de 31 de janeiro e uma data de término de 1º de janeiro, ele não será exibido na exibição de linha do tempo. Para obter mais informações, consulte a seção [Gerenciar uma exibição de linha do tempo](#manage-a-timeline-view) neste artigo.
* Há um limite de 5 tipos de registro que você pode incluir no detalhamento de um registro.

#### Analisar registros conectados na exibição de linha do tempo

1. Crie uma exibição de linha do tempo para um tipo de registro, conforme descrito no artigo [Gerenciar exibições de registros](/help/quicksilver/planning/views/manage-record-views.md).
1. (Condicional) Se você estiver vendo a exibição da linha do tempo no modo Padrão, clique em **Detalhamento**.
1. Expanda a caixa **Selecionar um tipo de registro vinculado** e selecione um tipo de registro conectado. <!--add a new screen shot - submitted a bug to remove the "the"-->

   ![](assets/breakdown-picker-and-button-on-timeline.png)

   >[!TIP]
   >
   >    Se você não tiver registros conectados ou se os registros conectados não tiverem pelo menos dois campos de data, a caixa **Selecionar um tipo de registro vinculado** não estará disponível.

1. Escolha uma **Data de início** e um **Campo de data de término**.

   >[!TIP]
   >
   >    As datas de início e término devem ser sequenciais. Se a Data final for anterior à Data inicial, nenhum registro será exibido na linha do tempo.

   Uma seta apontando para a direita é exibida na barra do registro selecionado na linha do tempo, caso eles estejam conectados a outros registros.
1. Clique na seta à direita para expandir um tipo de registro e exibir suas conexões.

   ![](assets/campaigns-broken-down-by-programs-in-timeline-highlighted.png)

1. (Opcional) Repita as etapas acima para adicionar mais registros conectados.



