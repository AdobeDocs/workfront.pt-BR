---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Filtrar informações no Balanceador de carga de trabalho
description: Para encontrar itens de trabalho com eficiência e se concentrar nos usuários ou itens que você gerencia, recomendamos que você use filtros no Balanceador de carga de trabalho.
author: Lisa
feature: Resource Management
exl-id: f8ffb40e-4e71-45fe-bcae-801d45d75a21
source-git-commit: c3cb97a36c29b90bbc9d8438d8811cc23266d894
workflow-type: tm+mt
source-wordcount: '2496'
ht-degree: 0%

---

# Filtrar informações no Balanceador de carga de trabalho

<!--
(when they add custom fields to fitlering, add the caveat you added for the Resource Planner : only field NAMES and not LABELS are to be found in the drop-down >> ADD THIS IN THE STEP BELOW WHEN ADDING A FILTER)
-->

Como gerenciador de recursos, você pode usar o Balanceador de carga de trabalho para exibir e gerenciar a carga de trabalho dos usuários. Para obter informações mais gerais sobre o Balanceador de carga de trabalho, consulte os seguintes artigos:

* [Visão geral do Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)
* [Navegar pelo Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>Para encontrar itens de trabalho com eficiência e se concentrar nos usuários ou itens que você gerencia, recomendamos que você use filtros no Balanceador de carga de trabalho. Isso permite exibir as informações corretas antes de começar a gerenciar as atribuições dos recursos.
>
>Quando você salva e aplica um novo filtro e, em seguida, navega para fora do Balanceador de carga de trabalho, o filtro é preservado mesmo depois de fazer logoff e logon novamente.

Este artigo contém informações sobre filtros no Balanceador de carga de trabalho. Para obter informações sobre filtros no Workfront, consulte [Visão geral dos filtros](../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer plano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Planejar, ao usar o Balanceador de carga de trabalho na área Recursos</p>
   <p>Trabalhar, ao usar o Balanceador de carga de trabalho de uma equipe ou projeto</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nível de acesso*</td> 
   <td> <p>Visualize ou tenha acesso superior ao seguinte:</p> 
    <ul> 
     <li> <p>Gerenciamento de recursos</p> </li> 
     <li> <p>Projetos</p> </li> 
     <li> <p>Tarefas</p> </li> 
     <li> <p>Problemas</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Filtros, visualizações e agrupamentos</p> </li> 
    </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span>Editar acesso a Filtros, Visualizações e Agrupamentos ao criar ou editar filtros</span> </p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualize ou aumente as permissões para projetos, tarefas, problemas</p>
   <p>Gerencie permissões para os filtros que deseja editar ou excluir</p>
     </p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront.

## Visão geral dos filtros no Balanceador de carga de trabalho

Considere o seguinte ao trabalhar com filtros no Balanceador de carga de trabalho:

* Dependendo de onde você acessa o Balanceador de carga de trabalho, o Workfront já pode estar filtrando as informações para você. Para obter informações sobre filtros pré-aplicados, consulte a seção [Filtros pré-aplicados no Balanceador de carga de trabalho](#pre-applied-filters-in-the-workload-balancer) neste artigo.
* É possível criar e aplicar um filtro sem salvá-lo ou salvar um filtro para reutilização posterior.
* Ao aplicar um filtro sem salvá-lo, é possível reverter para as listas originais atualizando a página.
* É possível exibir os filtros criados ou os filtros que outros usuários criaram e compartilharam com você.
* Ao excluir ou editar um filtro compartilhado, ele também é excluído ou editado para todos com quem é compartilhado.
* Ao criar filtros no Balanceador de carga de trabalho em uma área, eles não estão disponíveis em outras áreas.

  Por exemplo, os filtros criados na área Recursos não estão disponíveis no Balanceador de carga de trabalho de um projeto ou de uma equipe.

  Para obter informações sobre onde localizar o Balanceador de carga de trabalho, consulte [Localize o Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

* Você pode visualizar somente os itens que correspondem aos filtros selecionados que também correspondem às datas na linha do tempo exibida na tela do Balanceador de carga de trabalho.

## Filtros pré-aplicados no Balanceador de carga de trabalho {#pre-applied-filters-in-the-workload-balancer}

O Balanceador de carga de trabalho exibe informações em duas áreas separadas:

* **A área Trabalho não atribuído**: itens de trabalho que ainda não foram atribuídos aos usuários.
* **A área Trabalho atribuído**: itens de trabalho atribuídos aos usuários.

  Para obter informações sobre o que é exibido em cada uma das áreas, consulte [Navegar pelo Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

>[!IMPORTANT]
>
>Cada área do Balanceador de carga de trabalho tem seu próprio conjunto de filtros que funcionam independentemente uns dos outros. Você deve configurar ambos os filtros para indicar quais informações deseja ver em cada área.

O Balanceador de carga de trabalho exibe usuários e seus itens de trabalho.
Os itens de trabalho atribuídos aos usuários são exibidos somente quando as datas dos itens correspondem ao período exibido na tela.

Dependendo de onde você acessar o Balanceador de carga de trabalho a partir de, as áreas Não atribuídas e Atribuídas já serão filtradas por determinados critérios, conforme descrito na tabela a seguir:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Área do Workfront onde você acessa o Balanceador de carga de trabalho</strong></td> 
   <td><b>Itens exibidos na área Trabalho não atribuído por padrão</b> </td> 
   <td><b>Itens exibidos na área Trabalho atribuído por padrão</b> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">A área Recursos</td> 
   <td>Nenhum item é exibido aqui por padrão. Você deve personalizar filtros para visualizar itens de trabalho nesta área.</td> 
   <td>Usuários que são membros de qualquer uma de suas equipes e seus itens de trabalho. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Uma equipe</td> 
   <td>Itens de trabalho atribuídos à equipe ou à equipe e uma função de trabalho. </td> 
   <td> <p>Usuários que são membros da equipe selecionada e seus itens de trabalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Um projeto</td> 
   <td> <p>Itens de trabalho não atribuídos ou itens atribuídos a equipes ou funções de trabalho no projeto selecionado são exibidos nesta área.</p> </td> 
   <td> <p>Usuários atribuídos a pelo menos um item de trabalho no projeto selecionado e seus itens de trabalho no projeto quando o filtro padrão do sistema <b>Os itens de trabalho deste projeto</b> está selecionada. </p>

<p>Quando o filtro padrão do sistema <b>Os itens de trabalho deste projeto</b> for desmarcada, a área Trabalho atribuído de um projeto exibirá todos os itens de trabalho dos usuários atribuídos a pelo menos um item no projeto selecionado.  </p> Esse filtro é desmarcado por padrão.

<b>NOTA</b>
<p>Você pode ativar a opção Mostrar todos os usuários no Balanceador de carga de trabalho de um projeto para exibir todos os usuários no sistema. Para obter mais informações, consulte <a href="../workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navegar pelo Balanceador de carga de trabalho</a></p>

</td> 
  </tr> 
 </tbody> 
</table>

## Criar filtros do Balanceador de carga de trabalho

O processo de criação de filtros para as áreas Trabalho não atribuído e Trabalho atribuído no Balanceador de carga de trabalho é idêntico, independentemente de onde você acessa o Balanceador de carga de trabalho. Para obter informações sobre como localizar o Balanceador de carga de trabalho, consulte [Localize o Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

É possível criar um filtro do zero ou editar um dos filtros predefinidos. Para obter informações sobre filtros existentes que podem ser editados, consulte [Editar um filtro existente no Balanceador de carga de trabalho](#edit-an-existing-filter-in-the-workload-balancer) neste artigo.

1. Vá para o Balanceador de carga de trabalho.

   Para obter informações sobre como acessar o Balanceador de carga de trabalho, consulte [Navegar pelo Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Clique em **Filtro** ícone ![](assets/filter-icon.png) no canto superior direito de uma das **Trabalho não atribuído** ou o **Trabalho atribuído** domínios.

   A caixa do construtor de filtros é exibida à direita. O nome da área para a qual você cria o filtro é exibido no cabeçalho da caixa.

   ![](assets/filters-list-wb-assigned-work-with-filters-listed-nwe-350x377.png)

1. (Opcional e condicional) Se você acessar o Balanceador de carga de trabalho na área Recursos, o filtro Padrão predefinido pode já ter sido aplicado à área Trabalho atribuído. É possível editar e salvar uma cópia do filtro Padrão.

   >[!TIP]
   >
   >O filtro Padrão exibe os usuários que pertencem a qualquer uma das equipes e seus itens de trabalho. É possível editar uma cópia desse filtro.

   Se você acessar a variável [!UICONTROL Balanceador de carga de trabalho] de um projeto, o &quot;[!UICONTROL Os itens de trabalho deste projeto]O filtro &quot; pode já ter sido aplicado. Exibe somente os itens de trabalho atribuídos aos usuários neste projeto. Você pode duplicar e salvar uma cópia desse filtro.

   Por padrão, a variável [!UICONTROL Balanceador de carga de trabalho] de um projeto exibe todos os itens de trabalho atribuídos a todos os usuários no projeto.


1. Clique em **Novo filtro.**

   ![](assets/new-filters-empty-panel-workload-balancer-350x460.png)

1. Para criar um filtro, faça o seguinte:

   1. Selecione um nome de campo no primeiro menu suspenso ou clique em **Procurar campos** para começar a digitar o nome de um campo que não é exibido por padrão.

      >[!IMPORTANT]
      >
      >Ao fazer referência a campos personalizados, você deve digitar o nome do campo, não o rótulo do campo. O rótulo do campo é exibido em um formulário personalizado anexado a um objeto. Para obter informações sobre a diferença entre o rótulo e o nome de um campo personalizado, consulte [Criar ou editar um formulário personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   1. (Condicional) Se você clicou em **Procurar campos**, digite o nome de um campo no campo **Pesquisar** e selecione-o quando ele for exibido na lista.

      ![](assets/new-filters-search-for-a-field-highlighted-wb-nwe-350x386.png)

      >[!TIP]
      >
      >Você pode selecionar um campo nas seguintes seções:
      >
      >* **Seleções recentes**: os campos que você filtrou recentemente.
      >* **Campos sugeridos**: os campos usados com mais frequência.


   1. Selecione um modificador no segundo menu suspenso. Para obter informações sobre modificadores de filtro do Workfront, consulte [Filtros e modificadores de condição](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).
   1. Selecione ou digite um valor para o campo que você está filtrando.

      >[!NOTE]
      >
      > Quando quiser exibir objetos de trabalho de um portfólio específico, você pode aplicar o seguinte filtro: &quot;Portfolio name contains marketing&quot; (O nome da contém marketing). Isso exibe itens de trabalho que pertencem a qualquer portfólio que contenha &quot;marketing&quot; no nome.
      >
      >![](assets/portfolio-name-filter-statement-wb-350x262.png)

      >[!NOTE]
      >
      >Para excluir projetos com status Em espera, você deve aplicar o seguinte filtro: &quot;Projeto: o status não é igual a Em espera&quot;. Isso impede que itens de trabalho de projetos Em espera sejam exibidos no Balanceador de carga de trabalho.

   1. (Opcional) Clique no link **Excluir** ícone ![](assets/delete.png) para remover um critério de filtro.

1. (Opcional) Clique em **Adicionar filtro** para adicionar outro critério de filtro, repita as ações da etapa 4.

   <!--(NOTE: ensure this stays correct)-->

1. Clique em **Aplicar** para aplicar os resultados do filtro à área do Balanceador de carga de trabalho selecionada sem salvá-lo.

   A lista de itens de trabalho é atualizada à esquerda.

   >[!IMPORTANT]
   >
   >Os resultados são exibidos no Balanceador de carga de trabalho quando todas as instruções de filtro adicionadas são verdadeiras simultaneamente.

   O filtro é preservado até você atualizar a página.

   A variável **Aplicar** é substituído por um botão **Salvar como novo** botão.

1. Clique em **Salvar como novo** para salvar o filtro para uso futuro.

   ![](assets/new-filters-save-as-box-unassigned-area-wb-350x467.png)

   >[!TIP]
   >
   >Clicando **Cancelar** a qualquer momento, o leva de volta à área de construção do filtro.

1. Selecionar **Filtro sem título** e insira o nome do novo filtro.
1. Selecione um ícone para o novo filtro na **Ícone** menu suspenso.

   ![](assets/new-filters-select-icon-expanded-drop-down-wb.png)

1. (Opcional) Adicione uma descrição para o filtro para indicar o que é exclusivo sobre ele. A descrição é exibida sob o nome do filtro na lista de filtros.
1. Clique em **Salvar**.

   Os filtros salvos são exibidos na área Meus filtros da caixa de filtro.

   Para obter informações sobre como aplicar filtros salvos, consulte a seção [Excluir um filtro salvo no Balanceador de carga de trabalho](#delete-a-saved-filter-in-the-workload-balancer) neste artigo.

1. (Condicional) Passe o mouse sobre o **Ícone Filtrar** ![](assets/filter-icon.png) no canto superior direito da **Trabalho não atribuído** ou o **Trabalho atribuído** áreas para exibir uma dica de ferramenta com o nome ou o número de filtros aplicados atualmente.

   ![](assets/filter-icon-with-number-and-tooltip-with-name-of-filter-wb-nwe-350x98.png)

## Duplicação de um filtro

É possível duplicar e editar um filtro para criar um novo.

1. Vá para o Balanceador de carga de trabalho.

   Para obter informações sobre como acessar o Balanceador de carga de trabalho, consulte [Navegar pelo Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Clique em **Filtro** ícone ![](assets/filter-icon.png) no canto superior direito de uma das **Trabalho não atribuído** ou o **Trabalho atribuído** domínios.

   A caixa do construtor de filtros é exibida à direita. O nome da área para a qual você cria o filtro é exibido no cabeçalho da caixa.

1. Passe o mouse sobre um filtro existente, clique no **Mais** menu ![](assets/more-menu.png)e, em seguida, clique em **Duplicar**.

   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   > Ao editar um filtro, você pode clicar no link **Mais** no canto inferior esquerdo da caixa Editar filtro e clique em **Duplicar**.

1. Edite as seguintes informações para o filtro duplicado:

   * Nome

     Por padrão, o novo nome do filtro é &quot;(Nome do filtro original) Copiar&quot;.

   * Ícone
   * Descrição
   * Qualquer campo, modificador ou valor.

1. (Opcional) Clique em **Adicionar filtro** para adicionar mais instruções ao filtro duplicado.
1. Clique em **Salvar** para salvar o filtro duplicado no **Meus filtros** área.

   O filtro original permanece inalterado e o filtro duplicado é salvo como um novo filtro.

## Editar um filtro existente no Balanceador de carga de trabalho {#edit-an-existing-filter-in-the-workload-balancer}

Você pode editar um filtro salvo no Balanceador de carga de trabalho.

>[!TIP]
>
>Ao editar um filtro compartilhado com outras pessoas, elas também verão as alterações feitas.

1. Vá para o Balanceador de carga de trabalho.

   Para obter informações sobre como acessar o Balanceador de carga de trabalho, consulte [Navegar pelo Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Clique em **Ícone Filtrar** ![](assets/filter-icon.png) no canto superior direito da **Não atribuído** ou **Trabalho atribuído** domínios.\
   O construtor de filtros é exibido à direita.

1. Passe o mouse sobre o filtro que deseja editar, em seguida, clique no **Editar** ![](assets/wb-edit-filter-icon.png).

   ![](assets/filter-more-menu-options-wb.png)

1. Siga um destes procedimentos:

   * Modifique qualquer uma das instruções de filtro
   * Clique em **Adicionar filtro** para adicionar novas instruções de filtro
   * Clique em **Excluir** ícone ![](assets/delete.png) para remover instruções de filtro existentes.

1. (Opcional) Clique em **Aplicar**.

   Os resultados são atualizados no Balanceador de carga de trabalho à esquerda para ilustrar as alterações feitas no filtro.

1. Clique em **Salve.**

   Os resultados são atualizados no Balanceador de carga de trabalho à esquerda, e o filtro é atualizado com as novas informações selecionadas.

## Excluir um filtro salvo no Balanceador de carga de trabalho {#delete-a-saved-filter-in-the-workload-balancer}

Considere o seguinte antes de excluir um filtro:

* Não é possível recuperar filtros excluídos.
* Não é possível excluir filtros predefinidos.
* Não é possível excluir um filtro não salvo. Eles são removidos automaticamente depois de fazer logout e logon novamente no Workfront.
* Ao excluir um filtro compartilhado, ele também é excluído para todos os usuários com os quais é compartilhado.
* Depois de excluir todos os filtros salvos, o Balanceador de carga de trabalho é exibido de acordo com os padrões originais.

>[!NOTE]
>
>Quando você exclui um filtro compartilhado com outras pessoas, ele também é excluído para elas.

1. Ir para o Balanceador de carga de trabalho
1. Clique em **Ícone Filtrar** ![](assets/filter-icon.png) no canto superior direito da **Trabalho não atribuído** ou **Trabalho atribuído** domínios.\
   A caixa do construtor de filtros é exibida à direita.

1. Passe o mouse sobre um filtro, em seguida clique no **Mais** menu ![](assets/more-menu.png)e, em seguida, clique em **Excluir**.
   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   >Ao editar um filtro, você pode clicar no link **Mais** no canto inferior esquerdo da caixa Editar filtro e clique em **Excluir**.

1. (Opcional) Clique em **Cancelar** para evitar a exclusão e retornar à lista de filtros.
1. Clique em **Excluir** para confirmar a exclusão.

   O filtro é excluído para você e todos os usuários que têm permissões para ele.

## Compartilhar um filtro no Balanceador de carga de trabalho

Você pode compartilhar um filtro que criou ou que foi compartilhado com você por outros usuários.

Considere o seguinte ao compartilhar filtros no Balanceador de carga de trabalho:

* É possível compartilhar filtros com usuários, equipes, funções e empresas ativos ou torná-los visíveis para todos em sua instância do Workfront.
* Os filtros compartilhados na área Recursos não estão visíveis no Balanceador de carga de trabalho de um projeto ou de uma equipe.
* Os filtros do Balanceador de carga de trabalho compartilhados com outras pessoas não estão visíveis em outras áreas do Workfront.

Para compartilhar um filtro:

1. Ir para o Balanceador de carga de trabalho
1. Clique em **Ícone Filtrar** ![](assets/filter-icon.png) no canto superior direito da **Trabalho não atribuído** ou **Trabalho atribuído** domínios.\
   A caixa do construtor de filtros é exibida à direita.

1. Passe o mouse sobre um filtro, em seguida clique no **Mais** menu ![](assets/more-menu.png)e, em seguida, clique em **Compartilhar.**

   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   > Ao editar um filtro, você pode clicar no link **Mais** no canto inferior esquerdo da caixa Editar filtro e clique em **Compartilhar**.

   A caixa Filter sharing (Compartilhamento de filtro) é exibida.

1. Ativar o **Exibir em todo o sistema** configuração. Dessa forma, qualquer pessoa no Workfront tem permissão para exibir o filtro.

   Ou

   Comece a digitar os nomes de usuários, equipes, funções, grupos ou empresas com os quais você deseja compartilhar o filtro na **Conceder acesso a** campo.

   ![](assets/new-filters-sharing-ui-wb-350x422.png)

1. (Opcional) Clique na seta ao lado do nome de uma entidade para editar suas permissões para o filtro e, em seguida, habilite a opção **Exibir** ou **Gerenciar** opção.

   ![](assets/new-filters-granular-permissions-for-manage-wb-350x107.png)

1. (Opcional) Ative ou desative as permissões adicionais de uma entidade seguindo um destes procedimentos:

   1. Clique em **Exibir** e desative a variável **Compartilhar** opção. Ela é ativada por padrão.

   1. Clique em **Gerenciar** e desative as opções **Compartilhar** ou o **Excluir** opção. Elas são ativadas por padrão.

   >[!TIP]
   >
   >Os usuários não podem receber uma permissão maior do que seu nível de acesso. Se não tiverem acesso a Editar filtros em seus níveis de acesso, eles não poderão receber permissões para gerenciar um filtro. O Workfront desativa a opção Gerenciar para esses usuários e a opção fica esmaecida.

1. Clique em **Compartilhar**. O filtro é compartilhado com as entidades especificadas.

   Os filtros que você compartilhou são exibidos no **Compartilhado comigo** área da caixa de filtro.

   ![](assets/new-filters-shared-with-me-area-wb-350x236.png)

<!--   

## Add a filter to your favorites list

You can mark a filter as a favorite for quicker access to it. 

The filters that you mark as a favorite do not count towards your system Favorites list. There is no limit for how many filters you can favorite. 

1. Go to the Workload Balancer
1. Click the **Filter** icon ![](assets/filter-icon.png) in the upper-right corner of the **Unassigned Work** or **Assigned Work** areas. The filter builder box displays on the right. 
1. Mouse over a filter, then click the **Favorite** ![](assets/favorites-icon-small.png). 
(NOTE: insert screen shot here with Favorite as part of this menu - same as above ones but with Favorite)
1. The filter is listed in the **Favorited** section inside the filter panel. 
1. (Optional) Click the **Favorite** icon again to remove the filter from the list of favorite filters
(I logged bugs for "Favorited" and "Unfavorite" wordings - make sure these have not updated)
-->
