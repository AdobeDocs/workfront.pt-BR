---
title: Gerenciar a exibição de calendário
description: Você pode exibir registros e seus campos em uma exibição de calendário. Este artigo descreve como criar uma exibição de calendário e editar ou excluir uma existente.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: fbf902196c9f5b55ddd1e20516e4237309dff2ed
workflow-type: tm+mt
source-wordcount: '1895'
ht-degree: 4%

---

# Gerenciar a exibição de calendário

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Você pode exibir registros e seus campos em uma exibição de calendário na página de tipo de registro.

Para obter informações sobre os modos de exibição do Adobe Workfront Planning e como gerenciá-los, consulte [Gerenciar modos de exibição de registro](/help/quicksilver/planning/views/manage-record-views.md).

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

## Gerenciar uma exibição de calendário {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

Considere o seguinte:

* Você pode criar uma exibição de Calendário somente quando tem pelo menos dois campos de data associados a um tipo de registro. Quando você tem um ou nenhum campo de data associado a um tipo de registro, a opção de exibição Calendário fica esmaecida.

  Você pode selecionar entre campos de data de registro ou campos de data de pesquisa a partir de tipos de objeto ou registro conectados.
* Existem os seguintes cenários:

   * Quando as datas de Início e Término não têm valores, os registros não são exibidos no calendário
   * Quando as datas Start ou End não têm valor, o registro é exibido como um evento de um dia
   * Quando a data de início é posterior à data de término, o registro não é exibido no calendário.

Para gerenciar uma exibição de calendário:

1. Vá para a página do tipo de registro para a qual deseja exibir o calendário.
1. Crie uma exibição de calendário, conforme descrito no artigo [Gerenciar exibições de registros](/help/quicksilver/planning/views/manage-record-views.md).

   <div class="preview">

   ![Exemplo de exibição de calendário](assets/calendar-view-example.png)

   Os registros associados ao tipo de registro selecionado são exibidos como barras em um calendário. A cor das barras corresponde à cor do ícone de registro, por padrão.

   </div>

1. Siga um destes procedimentos para navegar pelo calendário:

   * Clique nos ícones esquerdo e direito no canto superior esquerdo do calendário ou use a rolagem horizontal para mover-se para trás e para frente no calendário.
   * Clique em **Hoje** no canto superior direito para centralizar o calendário na data de hoje.
   * Selecione uma das seguintes opções no menu suspenso de intervalo de tempo para atualizar os incrementos de tempo:

      * **Mês**: os registros são exibidos em um calendário mensal.

      * **Semana**: os registros são exibidos nas seguintes áreas:

         * Os registros que se estendem por vários dias são exibidos na parte superior do calendário.
         * Os registros que duram um dia ou menos são exibidos na metade inferior da exibição do calendário. Se você optou por exibir a hora das datas inicial e final, o registro será exibido no horário apropriado no dia em que ocorre.

1. <span class="preview">(Opcional) Clique no ícone **Tela cheia** ![Abrir ícone de tela cheia](assets/open-full-screen-icon.png) para abrir o modo de exibição em tela cheia, em seguida, no ícone **Sair da tela cheia** ![Sair do ícone de tela cheia](assets/exit-full-screen-icon.png) ou em Escape no teclado para sair da tela cheia.  </span>

1. <span class="preview">Para criar registros na exibição de calendário ou editar suas datas, siga um destes procedimentos:</span>

   * <span class="preview">Clique duas vezes em qualquer lugar do calendário para criar um registro. </span>

     <span class="preview">Para obter informações, consulte [Criar registros](/help/quicksilver/planning/records/create-records.md).</span>

   * <span class="preview">Clique na margem esquerda ou direita de uma barra de registros e arraste-a e solte-a em uma nova posição. O redimensionamento das barras de registros atualiza as datas de início ou término imediatamente. </span>

   * <span class="preview">Arraste e solte as barras de registro para atualizar sua posição e datas. Mover as barras dos registros atualiza as datas de início e término imediatamente.</span>

     <span class="preview">Para obter informações, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).</span>

1. Atualize os seguintes elementos de exibição conforme descrito nas subseções abaixo:
   * [Filtros](#add-filters)
   * <span class="preview">[Altura da linha](#modify-row-height)</span>
   * [Configurações](#edit-the-calendar-view-settings)

   <!--* [Grouping](#add-grouping)-->
   <!--* [Sort](#add-sort) not sure if this is present in calendar views?!; also check the anchor and make sure it's correct-->

### Adicionar filtros

Você pode reduzir a quantidade de informações exibidas na tela usando filtros.

Considere o seguinte ao trabalhar com filtros na exibição de calendário:

<!-- this list is almost identical to the one for the table view - update both-->

* Os filtros criados para uma exibição de calendário funcionam independentemente dos filtros em qualquer outra exibição aplicada ao mesmo tipo de registro.

* Os filtros são exclusivos para a exibição selecionada. Duas exibições de calendário do mesmo tipo de registro podem ter filtros diferentes aplicados a elas.

* Dois usuários que visualizam o mesmo calendário veem o mesmo filtro aplicado no momento.

* Não é possível nomear os filtros criados para uma exibição de calendário.

* A remoção de filtros os remove de qualquer pessoa que acesse o mesmo tipo de registro que você e que exiba a mesma visualização que você.

* Você pode filtrar por campos de registro conectados ou campos de pesquisa.

* Você pode filtrar por campos de pesquisa que exibem vários valores.

Para adicionar um filtro a uma exibição de calendário:

1. Crie uma exibição de calendário para uma página de tipo de registro, conforme descrito no artigo [Gerenciar exibições de registro](/help/quicksilver/planning/views/manage-record-views.md).
1. Selecione um modo de exibição de calendário e clique em **Filtros** na barra de ferramentas do calendário.
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

<span class="preview">

### Modificar altura da linha

Você pode modificar a altura da linha de uma célula do calendário para aumentar ou diminuir o número de barras de registro exibidas em cada célula.

O número de registros exibidos no calendário varia dependendo de quantos campos você exibe nas barras dos registros.

>[!TIP]
>
>Esta configuração só está disponível durante a visualização mensal do calendário.


1. Crie uma exibição de calendário para uma página de tipo de registro, conforme descrito no artigo [Gerenciar exibições de registro](/help/quicksilver/planning/views/manage-record-views.md).
1. (Condicional) Exiba a exibição de calendário por mês e clique em **Altura da linha** na barra de ferramentas do calendário.
1. Escolha entre as seguintes opções:

   <table>
    <thead>
    <tr>
        <th><b>Opção Altura da linha</b></th>
        <th><b>Número máximo padrão de registros</b></th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td>Pequena</td>
        <td><p>Contém:</p>

   <ul><li>2 registros exibindo 1 campo</li>
    <li>1 registro exibindo mais de 1 campo</li></ul>
        </td>
    </tr>
    <tr><td>Standard</td>
        <td><p>Contém:</p>

   <ul><li>4 registros exibindo 1 campo</li>
    <li>2 registros exibindo mais de 1 campo</li></ul>
        </td>
    </tr>
    <tr>
        <td>Médio</td>
        <td><p>Contém:</p>

   <ul><li>8 registros exibindo 1 campo</li>
    <li>4 registros exibindo mais de 1 campo</li></ul>
        </td>
    </tr>
    <tr>
        <td>Alta</td>
        <td><p>Contém:</p>

   <ul><li>12 registros exibindo 1 campo</li>
    <li>6 registros exibindo mais de 1 campo</li></ul>
        </td>
    </tr>
    <tr>
        <td>Ajustar ao conteúdo</td>
        <td><p>Todos os registros estão visíveis, até 500 registros</p></td>
    </tr>
    </tbody>
    </table>

1. (Opcional) Clique em **mais** se houver registros que não estejam visíveis no calendário.

</span>

### Editar as configurações de exibição do calendário

Atualize as configurações de exibição do calendário para indicar quais informações e como elas são exibidas na exibição.

1. Crie uma exibição de calendário para um tipo de registro, conforme descrito no artigo [Gerenciar exibições de registro](/help/quicksilver/planning/views/manage-record-views.md).
1. Clique em **Configurações**.
1. Clique em **Data e hora** no painel esquerdo e selecione uma **Data inicial** e uma **Data final** para exibir no calendário. Você pode escolher as datas padrão de Início e Término ou escolher qualquer campo de data disponível.

   As barras que representam os registros começam na data que você indica para a Data inicial e terminam na data correspondente à Data final.

   >[!NOTE]
   >
   >* Os registros que não têm valores para as datas de Início ou Término ou que têm uma data de Início posterior à data de Término não são exibidos na exibição de calendário.
   >
   >* Se você exibir registros adicionais usando a opção Breakdown, as datas Start e End serão as do registro principal. Não é possível escolher datas de Início e Término para os registros conectados nesta área.

1. Clique em **Estilo de barra** no painel esquerdo para indicar quais informações você deseja exibir nas barras de registro.

   O campo principal (ou título) do registro, conforme definido na exibição de tabela do registro, é selecionado por padrão.
   <!--adjust this when the primary field is released??-->

1. (Opcional e condicional) Se você adicionou miniaturas a registros, selecione a opção **Miniatura** para exibir a imagem associada aos registros na barra de registros.

   >[!NOTE]
   >
   >    Você deve primeiro adicionar miniaturas na exibição de tabela antes de exibi-las na exibição de calendário. Para obter mais informações, consulte [Adicionar uma miniatura a um registro](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

1. Clique em **Adicionar campo**, clique dentro da caixa **Pesquisar campos** e clique no campo que deseja adicionar.

   >[!TIP]
   >
   >   * Você deve criar os campos antes de adicioná-los às barras de registro.
   > 
   >   * Você deve ter pelo menos um campo selecionado. O **Nome** está selecionado por padrão.
   >
   >   * Você pode adicionar até 5 campos.

   Uma visualização da aparência das barras no calendário é exibida à direita.

   ![Seção de estilo de barra nas configurações de exibição do calendário](assets/bar-style-section-in-calendar-view-settings-with-preview.png)

1. Clique em **Cor** no painel esquerdo para personalizar as cores dos registros no calendário.

   ![Painel de cores nas configurações de exibição do calendário](assets/color-panel-on-calendar-view-settings.png)

1. Na seção **Definir cor de registro como**, selecione uma das seguintes opções para definir uma cor para os registros:

   * **Tipo de registro**: a cor das barras de registro no calendário corresponde à cor do tipo de registro selecionado. Esta é a opção padrão.
   * **Valores de campo**: a cor dos registros corresponde à cor de um campo especificado.
   * **Nenhum**: os registros são exibidos em uma barra branca.

1. (Condicional) Se você selecionou **Valores de campo** para as cores do registro, selecione um campo no menu suspenso **Corresponder a cor do registro a**.

   ![Menu suspenso do seletor de campos para exibição de calendário](assets/field-selector-drop-down-menu-calendar-view.png)

   Somente campos com opções codificadas por cores são exibidos no menu suspenso.

   Por exemplo, campos de seleção múltipla ou seleção única podem ter opções codificadas por cores.

   Se você não tiver um campo com opções codificadas por cores para o tipo de registro selecionado, essa opção ficará esmaecida.


1. Clique em **Salvar**.

   Os registros são exibidos na exibição de calendário com as especificações selecionadas.