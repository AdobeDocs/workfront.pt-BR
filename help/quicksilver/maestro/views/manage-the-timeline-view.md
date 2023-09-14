---
title: Gerenciar a exibição de linha do tempo
description: Você pode exibir registros em uma visualização de linha do tempo, ao acessar a página de tipo de registro no Adobe Maestro.
hidefromtoc: true
hide: true
source-git-commit: bac066b90c7fd69ffd423988c4cf736c16807f2b
workflow-type: tm+mt
source-wordcount: '1078'
ht-degree: 1%

---


# Gerenciar a exibição de linha do tempo

<!--
title: Manage the timeline view in Adobe Maestro
description: You can display records in a timeline view, when accessing the record type page in Adobe Maestro. 
hidefromtoc: yes
hide: yes
author: Alina
feature: Work Management
role: User
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>Atualmente, o Adobe Maestro faz parte de um programa beta fechado que está aberto a um número limitado de clientes.
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro-overview.md).

Você pode exibir registros em uma visualização de linha do tempo, ao acessar a página de tipo de registro no Adobe Maestro.

Para obter informações sobre visualizações do Maestro, consulte [Gerenciar visualizações de registro no Adobe Maestro](../views/manage-record-views.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> produto Adobe</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>contrato do Adobe Workfront</p></td>
   <td>
<p>Sua organização deve estar inscrita no programa beta fechado do Adobe Maestro. Entre em contato com seu representante de conta para obter mais informações sobre esta nova oferta. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plano do Adobe Workfront</p></td>
   <td>
<p>Qualquer Um</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td>
   <td>
   <p>Qualquer Um</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Nível de acesso</td>
   <td> <p>Qualquer Um</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Modelo de layout</td>
   <td> <p>O administrador do sistema deve adicionar a área Maestro no modelo de layout. Para obter informações, consulte <a href="../access/grant-access.md">Conceder acesso ao Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Gerenciar uma exibição de linha do tempo {#manage-a-timeline-view}

<!--insert screen shot of timeline view-->

Ao criar uma exibição de linha do tempo, todos os registros do tipo de registro selecionado são exibidos em uma linha do tempo cronológica.

Considere o seguinte:

* Você pode criar um modo de exibição de Linha do tempo somente quando tem pelo menos dois campos de data associados a um tipo de registro. Quando você tem um ou nenhum campo de data associado a um tipo de registro, a opção de exibição Linha do tempo fica esmaecida.
* Dependendo das datas associadas aos registros, alguns registros podem não ser exibidos na exibição de linha do tempo nos seguintes cenários:

   * Quando as datas de início e término não têm valores
   * Quando as datas de Início ou Término não têm valor
   * Quando a data inicial for posterior à data final

<!--these are NOT available now because there won't be a table for the timeline view for the near future, per Andy: 
* The records displayed in the timeline view also display in a view-only table to the left of the timeline. 
* Each row in the table and each bar on the timeline represent the same record. 
* Each column in the table is a record field. The columns of this table are preconfigured and cannot be customized. 
* Only a limited number of fields (or columns) display in the timeline view table. 
* You cannot do the following in a timeline view:
     * Add rows or records
     * Add columns or fields
     * Edit record information
-->

Ao criar uma exibição de linha do tempo, todos os registros do tipo de registro selecionado são exibidos em uma linha do tempo como barras, por padrão.

Para gerenciar uma exibição de linha do tempo:

1. Vá para a página do tipo de registro para a qual deseja exibir a linha do tempo.
1. Crie uma exibição de linha do tempo, conforme descrito no artigo [Gerenciar exibições de registro](../views/manage-record-views.md).

   ![](assets/timeline-view-example.png)

   Os registros associados ao tipo de registro selecionado são exibidos em uma linha do tempo cronológica, como barras.

1. Siga um destes procedimentos para navegar pela linha do tempo:

   * Clique nos ícones esquerdo e direito ou use a rolagem horizontal para mover-se para trás e para frente na linha do tempo.
   * Clique em **Hoje** para centralizar a linha do tempo na data de hoje.
   * Selecione uma das seguintes opções no menu suspenso de intervalo de tempo para atualizar os incrementos de tempo:

      * Ano
      * Trimestre
      * Mês
1. Clique em **Mudar para o padrão** exibir para exibir registros em linhas separadas <!--check to see if they updated the name of the setting here-->

   Ou

   Clique em **Alternar para exibição compacta** para exibir os registros cujas datas não se cruzam na mesma linha. <!--check to see if they updated the name of the setting here-->

   Os registros são exibidos na exibição Compacta por padrão.

1. Atualize os seguintes elementos de exibição conforme descrito nas subseções abaixo:
   * [Filtros](#add-filters)
   * [Agrupamento](#add-grouping)
     <!--* [Sort](#add-sort) not sure if this is present in timeline views?!; also check the anchor and make sure it's correct-->
   * [Configurações](#edit-the-timeline-view-settings)

### Adicionar filtros

Os filtros ajudam a reduzir a quantidade de informações exibidas na tela.

Considere o seguinte ao trabalhar com filtros na exibição de linha do tempo:

<!-- this list is almost identical to the one for the table view - update both-->

* Os filtros criados para a exibição da linha do tempo funcionam independentemente dos filtros na exibição de tabela quando aplicados ao mesmo tipo de registro.

* Os filtros são exclusivos para a exibição selecionada. Duas exibições de linha do tempo do mesmo tipo de registro podem ter filtros diferentes aplicados a elas. Dois usuários que visualizam a mesma linha do tempo veem o mesmo filtro aplicado no momento.

* Não é possível nomear os filtros criados e aplicar a uma exibição de linha do tempo.

* A remoção de filtros os remove de qualquer pessoa que acesse o mesmo tipo de registro que você e use a mesma visualização que você usa.

A adição de filtros na exibição de linha do tempo é idêntica à adição de filtros na exibição de tabela.

Para obter mais informações, consulte a seção &quot;Adicionar filtros&quot; no artigo [Gerenciar a exibição de tabela](../views/manage-the-table-view.md).

### Adicionar agrupamento

<!-- if groupings are identical between the table and the timeline, consider replacing this section with this: 

Adding groupings in the timeline view is identical to adding filters in the table view. 

For more information, see the "Add filters" section in the article [Manage the table view](../views/manage-the-table-view.md). -->


Você pode agrupar registros por informações semelhantes ao aplicar um agrupamento a uma exibição.

Considere o seguinte ao trabalhar com agrupamentos na exibição de linha do tempo:

* Você pode aplicar agrupamentos nas visualizações de tabela e linha do tempo. Os agrupamentos da exibição de tabela são independentes daqueles na exibição de linha do tempo do mesmo tipo de registro.
* Você pode aplicar três níveis de agrupamento em uma visualização Maestri. Os registros são agrupados na ordem de agrupamentos selecionada.
* É possível aplicar até 4 níveis de agrupamento ao usar a API.

Para adicionar um agrupamento:

1. Crie uma exibição de linha do tempo, conforme descrito no artigo [Gerenciar exibições de registro](../views/manage-record-views.md).
1. Clique em **Agrupamento**.

   ![](assets/grouping-ui-timeline-view.png)

1. Clique em um dos campos sugeridos ou clique em **Escolha um campo diferente** e procure um campo diferente, em seguida, clique nele quando ele for exibido na lista.

   >[!TIP]
   >
   >Não é possível selecionar campos vinculados.

   O agrupamento é aplicado automaticamente à linha do tempo e os registros são exibidos dentro da caixa de agrupamento. O número de itens em um agrupamento é exibido na linha de agrupamento.

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. (Opcional) Repita as etapas acima para adicionar até três agrupamentos.

   O número de agrupamentos aplicados é exibido à esquerda do ícone Grouping no canto superior direito da barra de ferramentas.

   ![](assets/grouping-applied-in-timeline-view.png)

1. (Opcional) Clique no link **x** ícone à direita de um agrupamento para remover o agrupamento

   Ou

   Clique em **Limpar tudo** para remover todos os agrupamentos.

1. Clique fora da **Agrupar registros por** para fechá-la.

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### Editar as configurações de exibição da linha do tempo {#edit-the-timeline-view-settings}

Atualize as configurações de exibição da linha do tempo para indicar quais informações são exibidas na seção de linha do tempo da exibição.

1. Crie uma exibição de linha do tempo, conforme descrito no artigo [Gerenciar exibições de registro](../views/manage-record-views.md).
1. Clique em **Configurações**.
1. Clique em **Data e hora** no painel esquerdo, selecione uma **Data inicial** e uma **Data final** para exibir na linha do tempo. Você pode escolher as datas padrão de Início e Término ou escolher qualquer campo de data disponível. As barras que representam os registros começam na data que você indica para a Data inicial e terminam na data correspondente à Data final.

   >[!NOTE]
   >
   >    Os registros que não têm valores para as datas de Início ou Término ou que têm uma data de Início posterior à data de Término não são exibidos na exibição de linha do tempo.


1. Clique em **Detalhes do registro** para indicar quais campos você deseja exibir nos cartões de registro.

   O campo Nome é selecionado por padrão.

1. Clique em **Adicionar campo** para adicionar até 4 campos às barras de registro.
1. Clique dentro do **Pesquisar campos** e clique no campo que deseja adicionar.

   >[!TIP]
   >
   >   * Você deve criar os campos antes de adicioná-los às barras de registro.
   > 
   >   * Você deve ter pelo menos um campo selecionado. **Nome** é selecionada por padrão.

   Uma visualização da aparência das barras na linha do tempo é exibida à direita.

   ![](assets/record-details-panel-timeline-settings-with-preview.png)

1. Clique em **Salvar**.

   Os registros são exibidos na exibição de linha do tempo com as especificações selecionadas.

