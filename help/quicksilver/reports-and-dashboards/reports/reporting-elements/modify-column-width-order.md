---
product-area: reporting
navigation-topic: reporting-elements
title: Modificar a largura e a ordem da coluna
description: Leia este artigo para saber mais sobre as diretrizes de largura da coluna e como alterar a largura e a ordem da coluna no Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: ece3f908-a0da-45d4-9f4f-0b34c69ce8fa
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '990'
ht-degree: 0%

---

# Modificar a largura e a ordem da coluna

A seguir estão as diretrizes sobre como as larguras de coluna funcionam no Adobe Workfront:

* Por padrão, o Workfront define a largura das colunas em listas e relatórios.
* O Workfront ajusta automaticamente a largura das colunas de acordo com a `valueformat`informações em todas as listas e relatórios, salvo especificação em contrário no modo texto da coluna.

   >[!NOTE]
   >
   >O Workfront não ajusta a largura das colunas de acordo com a variável `valueformat` informações nas listas disponíveis nas áreas Configuração e Relatórios.

   A variável `valueformat` define que tipo de informação é exibida na coluna. Por exemplo, as colunas que exibem um número são mais estreitas do que as colunas que exibem o campo Descrição.

* Você pode personalizar a largura das colunas em suas listas e relatórios do Workfront para atender às suas necessidades, dependendo do tipo de informação que deseja exibir nas colunas.

   Você pode modificar a largura das colunas temporariamente, ao exibir uma lista ou relatório, ou permanentemente, ajustando a largura da coluna no construtor de exibições. Para obter informações sobre como modificar temporariamente a largura das colunas, consulte a [Considerações ao modificar temporariamente a largura e a ordem das colunas](#considerations-when-temporarily-modifying-the-width-and-order-of-columns) neste artigo.

* As colunas que aparecem nas exibições integradas têm larguras definidas anteriormente pelo Workfront e codificadas. Para modificar essas larguras, você deve atualizar manualmente a largura dessas colunas usando o modo de texto no construtor de exibições.

   Para obter informações sobre como modificar a coluna no modo de texto, consulte [Exibir: edite permanentemente a largura de uma coluna](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plano do Adobe Workfront*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença da Adobe Workfront*</strong></td> 
   <td> <p>Solicitação ou superior </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p> <p>Editar acesso a Relatórios, Painéis, Calendários para editar a visualização em um relatório</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Gerenciar permissões de um relatório para editar uma visualização em um relatório</p> <p>Gerenciar permissões em uma exibição para editá-la</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Modificar a largura e a ordem da coluna

Você pode modificar a largura e a ordem das colunas em seus relatórios das seguintes maneiras:

* [Modificar temporariamente a largura e a ordem das colunas](#modify-width-and-order-of-columns-temporarily)
* [Modificar permanentemente a largura e a ordem das colunas](#modify-width-and-order-of-columns-permanently)

### Modificar temporariamente a largura e a ordem das colunas {#modify-width-and-order-of-columns-temporarily}

Você pode arrastar bordas de colunas para redimensionar colunas e arrastar e soltar colunas para reorganizá-las temporariamente na maioria das listas no site do Workfront. Isso inclui relatórios, visualizações, relatórios nos painéis e a visualização de Gantt.

Para obter mais informações sobre listas do Workfront, consulte o artigo [Introdução a listas no Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* [Considerações ao modificar temporariamente a largura e a ordem das colunas](#considerations-when-temporarily-modifying-the-width-and-order-of-columns)
* [Redimensionar colunas temporariamente](#resize-columns-temporarily)
* [Reordenar colunas temporariamente](#reorder-columns-temporarily)

#### Considerações ao modificar temporariamente a largura e a ordem das colunas {#considerations-when-temporarily-modifying-the-width-and-order-of-columns}

É possível modificar temporariamente a largura e a ordem das colunas em uma lista sem editar sua visualização.

Considere o seguinte ao redimensionar e ordenar temporariamente as colunas:

* Ao redimensionar colunas, os novos tamanhos são armazenados no armazenamento local do navegador e salvos por padrão. Usar um navegador diferente ou limpar o cache ou procurar dados resulta na reversão dos tamanhos das colunas para o padrão. Atualizar a página mantém as alterações feitas na largura das colunas.
* Ao reordenar colunas, a ordem escolhida é mantida somente até você sair da lista ou atualizar a página do navegador. Depois de sair da lista ou atualizar a página do navegador, as colunas retornam à ordem padrão.
* Para um desempenho ideal, as colunas que você está reordenando não devem ter mais de 100 itens na lista.
* Ao redimensionar colunas, as alterações se aplicam somente à exibição usada no momento e ficam visíveis somente para você. Compartilhar uma visualização com outro usuário não compartilha os tamanhos de coluna definidos.
* Depois de redimensionar uma coluna arrastando sua borda para a direita, a largura da coluna vizinha é preservada, exceto no seguinte:

   * A área Configuração
   * A área Relatórios
   * Listas de documentos e relatórios

   >[!NOTE]
   >
   >Não é possível mover a borda esquerda de uma coluna além da borda esquerda da coluna vizinha em nenhuma lista.

* Se você exportar qualquer lista para um arquivo, a ordem temporária das colunas não será transferida para o arquivo exportado. O arquivo exportado exibe a ordem das colunas na lista original, antes que as colunas tenham sido reordenadas.

Para obter mais informações sobre como exportar dados de listas e relatórios, consulte o artigo [Exportar dados](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

#### Redimensionar colunas temporariamente {#resize-columns-temporarily}

1. Vá para a lista que deseja modificar.
1. Arraste a borda de uma coluna até que ela atinja o tamanho desejado.\
   ![](assets/column-resize-350x124.png)

#### Reordenar colunas temporariamente {#reorder-columns-temporarily}

1. Vá para a lista que deseja modificar.
1. Clique em uma coluna que você deseja mover para outro local para selecionar a coluna.
1. Arraste a coluna para o local correto.
1. Solte a coluna no local para movê-la.

   ![](assets/column-reorder-350x118.png)

>[!TIP]
>
>Isso é especialmente útil ao visualizar o Gráfico de Gantt e a exibição em lista simultaneamente. Ao exibir o Gráfico de Gantt, as colunas podem ficar ocultas. Para exibir uma coluna enquanto o Diagrama de Gantt é exibido, basta arrastar a coluna que deseja exibir para exibi-la no lado esquerdo da página.

### Modificar permanentemente a largura e a ordem das colunas {#modify-width-and-order-of-columns-permanently}

Para reordenar colunas permanentemente, consulte a seção [Criar ou personalizar um modo de exibição padrão](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-a-standard-view) no artigo [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Você pode modificar permanentemente a largura de uma coluna somente usando o modo de texto.

Para obter mais informações sobre como usar o modo de texto e modificar permanentemente a largura de uma coluna, consulte o artigo [Visão geral de usos comuns do modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
