---
title: Gerenciar a exibição de calendário
description: Você pode exibir registros e seus campos em uma exibição de calendário. Este artigo descreve como criar uma exibição de calendário e editar ou excluir uma existente.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 1%

---

# Gerenciar a exibição de calendário

{{planning-important-intro}}

Você pode exibir registros e seus campos em uma exibição de calendário na página de tipo de registro.

Para obter informações sobre os modos de exibição do Adobe Workfront Planning e como gerenciá-los, consulte [Gerenciar modos de exibição de registro](/help/quicksilver/planning/views/manage-record-views.md).

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso do Workfront Planning.

Para acessar o Workfront Planning, é necessário ter o seguinte:

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

   ![](assets/calendar-view-example.png)

   Os registros associados ao tipo de registro selecionado são exibidos como barras em um calendário. A cor das barras corresponde à cor do ícone de registro.

1. Siga um destes procedimentos para navegar pelo calendário:

   * Clique nos ícones esquerdo e direito ou use a rolagem horizontal para mover-se para trás e para a frente no calendário.
   * Clique em **Hoje** para centralizar o calendário na data de hoje.
   * Selecione uma das seguintes opções no menu suspenso de intervalo de tempo para atualizar os incrementos de tempo:

      * Mês
1. Atualize os seguintes elementos de exibição conforme descrito nas subseções abaixo:
   * [Filtros](#add-filters)
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

* A adição de filtros na exibição de calendário é idêntica à adição de filtros na exibição de tabela.

  Para obter mais informações, consulte a seção &quot;Adicionar filtros&quot; no artigo [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md).

* Você pode filtrar por campos de registro conectados ou campos de pesquisa.

* Você pode filtrar por campos de pesquisa que exibem vários valores.

### Editar as configurações de exibição do calendário

A edição das configurações de exibição do calendário é idêntica à edição das configurações de uma exibição de linha do tempo.

Para obter mais informações, consulte a seção &quot;Editar as configurações de exibição da linha do tempo&quot; no artigo [Gerenciar a exibição da linha do tempo](/help/quicksilver/planning/views/manage-the-timeline-view.md).
