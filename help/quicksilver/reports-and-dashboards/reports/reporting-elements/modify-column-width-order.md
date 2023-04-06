---
product-area: reporting
navigation-topic: reporting-elements
title: Modificar a largura e a ordem da coluna
description: Leia este artigo para saber mais sobre as diretrizes de largura da coluna e como alterar a largura e a ordem da coluna no Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: ece3f908-a0da-45d4-9f4f-0b34c69ce8fa
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '988'
ht-degree: 0%

---

# Modificar a largura e a ordem da coluna

Veja a seguir as diretrizes sobre como as larguras de coluna funcionam no Adobe Workfront:

* O Workfront define a largura das colunas em listas e relatórios, por padrão.
* O Workfront ajusta automaticamente a largura das colunas de acordo com a variável `valueformat`informações em todas as listas e relatórios, a menos que especificado de outra forma no modo de texto da coluna.

   >[!NOTE]
   >
   >O Workfront não ajusta a largura das colunas de acordo com a variável `valueformat` nas listas disponíveis nas áreas Configuração e Relatórios .

   O `valueformat` define que tipo de informação é exibido na coluna . Por exemplo, as colunas que exibem um número são mais estreitas que as colunas que exibem o campo Descrição .

* É possível personalizar a largura das colunas nas listas e relatórios do Workfront para atender às suas necessidades, dependendo do tipo de informações que deseja exibir nas colunas.

   Você pode modificar a largura das colunas temporariamente, enquanto visualiza uma lista ou relatório, ou permanentemente, ajustando a largura da coluna no construtor de visualizações. Para obter informações sobre como modificar a largura das colunas temporariamente, consulte o [Considerações ao modificar temporariamente a largura e a ordem das colunas](#considerations-when-temporarily-modifying-the-width-and-order-of-columns) neste artigo.

* As colunas que aparecem em exibições integradas têm larguras definidas anteriormente pelo Workfront, que são codificadas. Para modificar essas larguras, você deve atualizar manualmente a largura dessas colunas usando o modo de texto no construtor de visualizações.

   Para obter informações sobre como modificar a coluna no modo de texto, consulte [Exibir: editar permanentemente a largura de uma coluna](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Plano Adobe Workfront*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença da Adobe Workfront*</strong></td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Editar o acesso a Relatórios, Painéis, Calendários para editar a exibição em um relatório</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Gerenciar permissões de um relatório para editar uma visualização em um relatório</p> <p>Gerenciar permissões em uma exibição para editá-la</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Modificar a largura e a ordem da coluna

Você pode modificar a largura e a ordem das colunas em seus relatórios das seguintes maneiras:

* [Modificar a largura e a ordem das colunas temporariamente](#modify-width-and-order-of-columns-temporarily)
* [Modificar a largura e a ordem das colunas permanentemente](#modify-width-and-order-of-columns-permanently)

### Modificar a largura e a ordem das colunas temporariamente {#modify-width-and-order-of-columns-temporarily}

Você pode arrastar as bordas da coluna para redimensionar as colunas e arrastar e soltar colunas para reorganizá-las temporariamente na maioria das listas no site do Workfront. Isso inclui relatórios, visualizações, relatórios sobre painéis e a visualização de Gantt.

Para obter mais informações sobre listas do Workfront, consulte o artigo [Introdução a listas no Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* [Considerações ao modificar temporariamente a largura e a ordem das colunas](#considerations-when-temporarily-modifying-the-width-and-order-of-columns)
* [Redimensionar colunas temporariamente](#resize-columns-temporarily)
* [Reordenar colunas temporariamente](#reorder-columns-temporarily)

#### Considerações ao modificar temporariamente a largura e a ordem das colunas {#considerations-when-temporarily-modifying-the-width-and-order-of-columns}

Você pode modificar temporariamente a largura e a ordem das colunas em uma lista sem editar sua visualização.

Considere o seguinte ao redimensionar e ordenar temporariamente as colunas:

* Ao redimensionar colunas, os novos tamanhos de coluna são armazenados no armazenamento local do navegador e são salvos por padrão. Usar um navegador diferente ou limpar o cache ou procurar dados resulta em tamanhos de coluna sendo revertidos para o padrão. Atualizar sua página mantém as alterações feitas na largura das colunas.
* Ao reorganizar colunas, a ordem escolhida é mantida somente até que você saia da lista ou atualize a página do navegador. Depois de sair da lista ou atualizar a página do navegador, as colunas retornam à ordem padrão.
* Para um desempenho ideal, as colunas que você está reorganizando não devem ter mais de 100 itens na lista.
* Ao redimensionar colunas, suas alterações se aplicam somente à exibição usada atualmente e são visíveis somente para você. O compartilhamento de uma exibição com outro usuário não compartilha os tamanhos de coluna definidos.
* Depois de redimensionar uma coluna arrastando sua borda para a direita, a largura da coluna vizinha é preservada, exceto no seguinte:

   * A área Configuração
   * A área Relatórios
   * Listas e relatórios de documentos

   >[!NOTE]
   >
   >Não é possível mover a borda esquerda de uma coluna para além da borda esquerda da coluna vizinha em qualquer lista.

* Se você exportar qualquer lista para um arquivo, a ordem temporária das colunas não será transferida para o arquivo exportado. O arquivo exportado exibe a ordem das colunas na lista original, antes que as colunas tenham sido reordenadas.

Para obter mais informações sobre exportação de dados de listas e relatórios, consulte o artigo [Exportar dados](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

#### Redimensionar colunas temporariamente {#resize-columns-temporarily}

1. Vá para a lista que deseja modificar.
1. Arraste a borda de uma coluna até que ela atinja o tamanho desejado.\
   ![](assets/column-resize-350x124.png)

#### Reordenar colunas temporariamente {#reorder-columns-temporarily}

1. Vá para a lista que deseja modificar.
1. Clique em uma coluna que deseja mover para outro local para escolher a coluna.
1. Arraste a coluna para o local correto.
1. Solte a coluna no local, para movê-la.

   ![](assets/column-reorder-350x118.png)

>[!TIP]
>
>Isso é especialmente útil ao visualizar o gráfico de Gantt e a exibição de lista simultaneamente. Ao visualizar o gráfico de Gantt, as colunas podem se tornar ocultas. Para exibir uma coluna enquanto o gráfico de Gantt é exibido, basta arrastar a coluna que deseja visualizar para que seja exibida no lado esquerdo da página.

### Modificar a largura e a ordem das colunas permanentemente {#modify-width-and-order-of-columns-permanently}

Para reorganizar colunas permanentemente, consulte a seção [Criar ou personalizar uma exibição padrão](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-a-standard-view) no artigo [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Você pode modificar permanentemente a largura de uma coluna somente usando o modo de texto.

Para obter mais informações sobre como usar o modo de texto e modificar permanentemente a largura de uma coluna, consulte o artigo [Visão geral dos usos comuns do modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
