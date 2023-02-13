---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Filtrar informações no Balanceador de Carga de Trabalho
description: Para encontrar itens de trabalho com eficiência e se concentrar nos usuários ou itens que você gerencia, recomendamos que você use filtros no Balanceador de Carga de Trabalho.
author: Alina
feature: Resource Management
exl-id: f8ffb40e-4e71-45fe-bcae-801d45d75a21
source-git-commit: 10b905c8a66f2507cbfac7c15a01f38d40ab3e00
workflow-type: tm+mt
source-wordcount: '2466'
ht-degree: 0%

---

# Filtrar informações no Balanceador de Carga de Trabalho

<!--
(when they add custom fields to fitlering, add the caveat you added for the Resource Planner : only field NAMES and not LABELS are to be found in the drop-down >> ADD THIS IN THE STEP BELOW WHEN ADDING A FILTER)
-->

Como gerenciador de recursos, você pode usar o Balanceador de Carga de Trabalho para exibir e gerenciar a carga de trabalho dos usuários. Para obter informações mais gerais sobre o Balanceador de Carga de Trabalho, consulte os seguintes artigos:

* [Visão Geral do Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)
* [Navegar pelo Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>Para encontrar itens de trabalho com eficiência e se concentrar nos usuários ou itens que você gerencia, recomendamos que você use filtros no Balanceador de Carga de Trabalho. Isso permite exibir as informações corretas antes de começar a gerenciar as atribuições de seus recursos.
>
>Quando você salva e aplica um novo filtro e depois navega para fora do Balanceador de carga de trabalho, o filtro é preservado mesmo depois que você faz logoff e faz logon novamente.


Este artigo contém informações sobre filtros no Balanceador de Carga de Trabalho. Para obter informações sobre filtros no Workfront, consulte [Visão geral dos filtros no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer plano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Planejar, ao usar o Balanceador de Carga de Trabalho para uma equipe ou na área Recursos </p>
   <p>Trabalhe, ao usar o Balanceador de Carga de Trabalho de um projeto </p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nível de acesso*</td> 
   <td> <p>Visualizar ou aumentar o acesso ao seguinte:</p> 
    <ul> 
     <li> <p>Gerenciamento de recursos</p> </li> 
     <li> <p>Projetos</p> </li> 
     <li> <p>Tarefas</p> </li> 
     <li> <p>Problemas</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Filtros, exibições e agrupamentos</p> </li> 
    </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span>Editar acesso a filtros, exibições e agrupamentos ao criar ou editar filtros</span> </p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualizar permissões ou permissões mais altas para projetos, tarefas, problemas</p>
   <p>Gerenciar permissões dos filtros que deseja editar ou excluir</p>
     </p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Visão Geral dos Filtros no Balanceador de Carga de Trabalho

Considere o seguinte ao trabalhar com filtros no Balanceador de Carga de Trabalho:

* Dependendo de onde você acessa o Balanceador de Carga de Trabalho, a Workfront pode já estar filtrando as informações para você. Para obter informações sobre filtros pré-aplicados, consulte a seção [Filtros pré-aplicados no Balanceador de carga de trabalho](#pre-applied-filters-in-the-workload-balancer) neste artigo.
* Você pode criar e aplicar um filtro sem salvá-lo ou salvar um filtro para reutilização posteriormente.
* Ao aplicar um filtro sem salvá-lo, você pode reverter para as listas originais atualizando sua página.
* Você pode exibir filtros criados ou filtros que outros usuários criaram e compartilharam com você.
* Ao excluir ou editar um filtro compartilhado, ele também é excluído ou editado para todos com os quais foi compartilhado.
* Ao criar filtros no Balanceador de Carga de Trabalho em uma área, eles não ficam disponíveis em outras áreas.

   Por exemplo, os filtros criados na área Recursos não estão disponíveis no Balanceador de Carga de Trabalho de um projeto ou equipe.

   Para obter informações sobre onde localizar o Balanceador de Carga de Trabalho, consulte [Localizar o Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

* Você pode exibir apenas os itens que correspondem aos filtros selecionados, que também correspondem às datas na linha do tempo exibida na tela do Balanceador de carga de trabalho.

## Filtros pré-aplicados no Balanceador de carga de trabalho {#pre-applied-filters-in-the-workload-balancer}

O Balanceador de Carga de Trabalho exibe informações em duas áreas separadas:

* **A área de trabalho não atribuída**: itens de trabalho que ainda não foram atribuídos aos usuários.
* **Área de Trabalho Atribuída**: itens de trabalho atribuídos aos usuários.

   Para obter informações sobre o que é exibido em cada uma das áreas, consulte [Navegar pelo Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

>[!IMPORTANT]
>
>Cada área do Balanceador de Carga de Trabalho tem seu próprio conjunto de filtros que funcionam independentemente um do outro. Você deve configurar ambos os filtros para indicar quais informações deseja ver em cada área.

O Balanceador de Carga de Trabalho exibe os usuários e seus itens de trabalho.
Os itens de trabalho atribuídos aos usuários somente são exibidos quando as datas dos itens correspondem ao período exibido na tela.

Dependendo de onde você acessar o Balanceador de Carga de Trabalho, as áreas Não Atribuídas e Atribuídas já são filtradas por determinados critérios, conforme descrito na tabela a seguir:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Área do Workfront na qual você acessa o Balanceador de Carga de Trabalho</strong></td> 
   <td><b>Itens que são exibidos na área de Trabalho Não Atribuído por padrão</b> </td> 
   <td><b>Itens exibidos na área de Trabalho Atribuído por padrão</b> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">A área Recursos</td> 
   <td>Nenhum item é exibido aqui por padrão. Você deve personalizar filtros para exibir itens de trabalho nessa área.</td> 
   <td>Usuários que são membros de qualquer uma de suas equipes e seus itens de trabalho. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Uma equipe</td> 
   <td>Itens de trabalho que são atribuídos à equipe ou à equipe e uma função de trabalho. </td> 
   <td> <p>Usuários que são membros da equipe selecionada e seus itens de trabalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Um projeto</td> 
   <td> <p>Itens de trabalho não atribuídos ou itens atribuídos a equipes ou funções de trabalho no projeto selecionado são exibidos nessa área.</p> </td> 
   <td> <p>Usuários atribuídos a pelo menos um item de trabalho no projeto selecionado e seus itens de trabalho no projeto quando o filtro padrão do sistema <b>Itens de trabalho deste projeto</b> está selecionada. </p>

<p>Quando o filtro padrão do sistema <b>Itens de trabalho deste projeto</b> for desmarcada, a área de Trabalho atribuído de um projeto exibirá todos os itens de trabalho dos usuários atribuídos a pelo menos um item no projeto selecionado.  </p> Esse filtro é desmarcado por padrão.

<b>Nota</b>
<p>Você pode ativar a opção Mostrar todos os usuários no Balanceador de Carga de Trabalho de um projeto para exibir todos os usuários no sistema. Para obter mais informações, consulte <a href="../workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navegar pelo Balanceador de Carga de Trabalho</a></p>

</td> 
  </tr> 
 </tbody> 
</table>

## Criar filtros de balanceador de carga de trabalho

O processo para criar filtros para as áreas Trabalho não atribuído e Trabalho atribuído no Balanceador de Carga de Trabalho é idêntico, independentemente de onde você acessa o Balanceador de Carga de Trabalho. Para obter informações sobre como localizar o Balanceador de Carga de Trabalho, consulte [Localizar o Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

Você pode criar um filtro do zero ou editar um dos filtros predefinidos. Para obter informações sobre filtros existentes que podem ser editados, consulte o [Editar um filtro existente no Balanceador de Carga de Trabalho](#edit-an-existing-filter-in-the-workload-balancer) neste artigo.

1. Vá para o Balanceador de Carga de Trabalho.

   Para obter informações sobre como acessar o Balanceador de Carga de Trabalho, consulte [Navegar pelo Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Clique no botão **Filtro** ícone ![](assets/filter-icon.png) no canto superior direito de qualquer uma das **Trabalho Não Atribuído** ou **Trabalho Atribuído** áreas.

   A caixa do construtor de filtros é exibida à direita. O nome da área onde você cria o filtro é exibido no cabeçalho da caixa.

   ![](assets/filters-list-wb-assigned-work-with-filters-listed-nwe-350x377.png)

1. (Opcional e condicional) Se você acessar o Balanceador de Carga de Trabalho na área Recursos, o filtro Padrão predefinido talvez já tenha sido aplicado à área de Trabalho Atribuído. Você pode editar e salvar uma cópia do filtro Padrão.

   >[!TIP]
   >
   >O filtro Padrão exibe usuários que pertencem a qualquer uma das equipes e seus itens de trabalho. Você pode editar uma cópia deste filtro.

   Se você acessar o [!UICONTROL Balanceador de Carga de Trabalho] de um projeto, o &quot;[!UICONTROL Itens de trabalho deste projeto]&quot;pode já estar sendo aplicado. Isso exibe somente itens de trabalho atribuídos a usuários neste projeto. Você pode duplicar e salvar uma cópia desse filtro.

   Por padrão, a variável [!UICONTROL Balanceador de Carga de Trabalho] de um projeto exibe todos os itens de trabalho atribuídos a todos os usuários no projeto.


1. Clique em **Novo filtro.**

   ![](assets/new-filters-empty-panel-workload-balancer-350x460.png)

1. Para criar um filtro, faça o seguinte:

   1. Selecione um nome de campo no primeiro menu suspenso ou clique em **Procurar campos** para começar a digitar o nome de um campo que não é exibido por padrão.

      >[!IMPORTANT]
      >
      >Ao fazer referência a campos personalizados, você deve digitar o nome do campo e não o rótulo do campo. O rótulo do campo é exibido em um formulário personalizado anexado a um objeto. Para obter informações sobre a diferença entre o rótulo e o nome de um campo personalizado, consulte [Criar ou editar um formulário personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   1. (Condicional) Se você clicou **Procurar campos**, digite o nome de um campo no **Pesquisar** e selecione-o quando for exibido na lista.

      ![](assets/new-filters-search-for-a-field-highlighted-wb-nwe-350x386.png)

      >[!TIP]
      >
      >Você pode selecionar um campo nas seguintes seções:
      >
      >* **Seleções recentes**: os campos para os quais você filtrou recentemente.
      >* **Campos sugeridos**: os campos mais usados.



   1. Selecione um modificador no segundo menu suspenso. Para obter informações sobre modificadores de filtro Workfront, consulte [Filtros e modificadores de condição](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).
   1. Selecione ou digite um valor para o campo para o qual você está filtrando.

      >[!NOTE]
      >
      > Quando quiser exibir objetos de trabalho de um portfólio específico, você pode aplicar o seguinte filtro: &quot;O nome do Portfolio contém marketing.&quot; Isso exibe itens de trabalho que pertencem a qualquer portfólio que contenha &quot;marketing&quot; no nome.
      >
      >![](assets/portfolio-name-filter-statement-wb-350x262.png)

   1. (Opcional) Clique no botão **Excluir** ícone ![](assets/delete.png) para remover um critério de filtro.

1. (Opcional) Clique em **Adicionar filtro** para adicionar outro critério de filtro, repita as ações da etapa 4.

   <!--(NOTE: ensure this stays correct)-->

1. Clique em **Aplicar** para aplicar os resultados do filtro à área Balanceador de Carga de Trabalho selecionada sem salvá-la.

   A lista de itens de trabalho é atualizada à esquerda.

   >[!IMPORTANT]
   >
   >Os resultados são exibidos no Balanceador de Carga de Trabalho quando todas as instruções de filtro adicionadas são simultaneamente verdadeiras.

   O filtro é preservado até que você atualize a página.

   O **Aplicar** é substituído por um botão **Salvar como novo** botão.

1. Clique em **Salvar como novo** para salvar o filtro para uso futuro.

   ![](assets/new-filters-save-as-box-unassigned-area-wb-350x467.png)

   >[!TIP]
   >
   >Clicar **Cancelar** a qualquer momento, o direcionará de volta para a área de construção do filtro.

1. Selecionar **Filtro sem título** e insira o nome do novo filtro.
1. Selecione um ícone para o novo filtro na **Ícone** menu suspenso.

   ![](assets/new-filters-select-icon-expanded-drop-down-wb.png)

1. (Opcional) Adicione uma descrição para o filtro para indicar o que é exclusivo sobre ele. A descrição é exibida abaixo do nome do filtro na lista de filtros.
1. Clique em **Salvar**.

   Filtros salvos são exibidos na área Meus filtros da caixa de filtro.

   Para obter informações sobre como aplicar filtros salvos, consulte a seção [Excluir um filtro salvo no Balanceador de Carga de Trabalho](#delete-a-saved-filter-in-the-workload-balancer) neste artigo.

1. (Condicional) Passe o mouse sobre o **Ícone Filtro** ![](assets/filter-icon.png) no canto superior direito do **Trabalho Não Atribuído** ou **Trabalho Atribuído** áreas para exibir uma dica de ferramenta com o nome ou o número de filtros aplicados atualmente.

   ![](assets/filter-icon-with-number-and-tooltip-with-name-of-filter-wb-nwe-350x98.png)

## Duplicar um filtro

Você pode duplicar e editar um filtro para criar um novo.

1. Vá para o Balanceador de Carga de Trabalho.

   Para obter informações sobre como acessar o Balanceador de Carga de Trabalho, consulte [Navegar pelo Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Clique no botão **Filtro** ícone ![](assets/filter-icon.png) no canto superior direito de qualquer uma das **Trabalho Não Atribuído** ou **Trabalho Atribuído** áreas.

   A caixa do construtor de filtros é exibida à direita. O nome da área onde você cria o filtro é exibido no cabeçalho da caixa.

1. Passe o mouse sobre um filtro existente, clique no botão **Mais** menu ![](assets/more-menu.png), depois clique em **Duplicar**.

   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   > Ao editar um filtro, você pode clicar no botão **Mais** no canto inferior esquerdo da caixa Editar filtro e clique em **Duplicar**.

1. Edite as seguintes informações para o filtro duplicado:

   * Nome

      Por padrão, o novo nome do filtro é &quot;(Nome do filtro original) Copy.&quot;

   * Ícone
   * Descrição
   * Qualquer um dos campos, modificadores ou valores.

1. (Opcional) Clique em **Adicionar filtro** para adicionar mais instruções ao filtro duplicado.
1. Clique em **Salvar** para salvar o filtro duplicado no **Meus filtros** área.

   O filtro original permanece inalterado e o filtro duplicado é salvo como um novo filtro.

## Editar um filtro existente no Balanceador de Carga de Trabalho {#edit-an-existing-filter-in-the-workload-balancer}

Você pode editar um filtro salvo no Balanceador de Carga de Trabalho.

>[!TIP]
>
>Ao editar um filtro compartilhado com outras pessoas, elas também verão as alterações feitas.

1. Vá para o Balanceador de Carga de Trabalho.

   Para obter informações sobre como acessar o Balanceador de Carga de Trabalho, consulte [Navegar pelo Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Clique no botão **Ícone Filtro** ![](assets/filter-icon.png) no canto superior direito do **Não atribuído** ou **Trabalho Atribuído** áreas.\
   O construtor de filtros é exibido à direita.

1. Passe o mouse sobre o filtro que deseja editar, em seguida, clique no botão **Editar** ![](assets/wb-edit-filter-icon.png).

   ![](assets/filter-more-menu-options-wb.png)

1. Siga um destes procedimentos:

   * Modifique qualquer uma das instruções de filtro
   * Clique em **Adicionar filtro** para adicionar novas instruções de filtro
   * Clique no botão **Excluir** ícone ![](assets/delete.png) para remover instruções de filtro existentes.

1. (Opcional) Clique em **Aplicar**.

   Os resultados são atualizados no Balanceador de Carga de Trabalho à esquerda para ilustrar as alterações feitas no filtro.

1. Clique em **Salvar.**

   Os resultados são atualizados no Balanceador de Carga de Trabalho à esquerda e o filtro é atualizado com as novas informações selecionadas.

## Excluir um filtro salvo no Balanceador de Carga de Trabalho {#delete-a-saved-filter-in-the-workload-balancer}

Considere o seguinte antes de excluir um filtro:

* Não é possível recuperar filtros excluídos.
* Não é possível excluir filtros predefinidos.
* Não é possível excluir um filtro não salvo. Eles são removidos automaticamente após o logout e o logon novamente no Workfront.
* Ao excluir um filtro compartilhado, ele também é excluído para todos os usuários com os quais ele é compartilhado.
* Após excluir todos os filtros salvos, o Balanceador de carga de trabalho é exibido de acordo com os padrões originais.

>[!NOTE]
>
>Ao excluir um filtro compartilhado com outras pessoas, ele também será excluído.

1. Vá para o Balanceador de Carga de Trabalho
1. Clique no botão **Ícone Filtro** ![](assets/filter-icon.png) no canto superior direito do **Trabalho Não Atribuído** ou **Trabalho Atribuído** áreas.\
   A caixa do construtor de filtros é exibida à direita.

1. Passe o mouse sobre um filtro, em seguida, clique no botão **Mais** menu ![](assets/more-menu.png), depois clique em **Excluir**.
   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   >Ao editar um filtro, você pode clicar no botão **Mais** no canto inferior esquerdo da caixa Editar filtro e clique em **Excluir**.

1. (Opcional) Clique em **Cancelar** para evitar a exclusão e retornar à lista de filtros.
1. Clique em **Excluir** para confirmar a exclusão.

   O filtro é excluído para você e para todos os usuários com permissões nele.

## Compartilhar um filtro no Balanceador de Carga de Trabalho

Você pode compartilhar um filtro que você criou ou que foi compartilhado com você por outros usuários.

Considere o seguinte ao compartilhar filtros no Balanceador de Carga de Trabalho:

* Você pode compartilhar filtros com usuários ativos, equipes, funções e empresas, ou pode torná-los visíveis para todos na sua instância do Workfront.
* Os filtros que você compartilha na área Recursos não estão visíveis no Balanceador de Carga de Trabalho de um projeto ou equipe.
* Os filtros de Balanceador de carga de trabalho que você compartilha com outras pessoas não estão visíveis em outras áreas do Workfront.

Para compartilhar um filtro:

1. Vá para o Balanceador de Carga de Trabalho
1. Clique no botão **Ícone Filtro** ![](assets/filter-icon.png) no canto superior direito do **Trabalho Não Atribuído** ou **Trabalho Atribuído** áreas.\
   A caixa do construtor de filtros é exibida à direita.

1. Passe o mouse sobre um filtro, em seguida, clique no botão **Mais** menu ![](assets/more-menu.png), depois clique em **Compartilhar.**

   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   > Ao editar um filtro, você pode clicar no botão **Mais** no canto inferior esquerdo da caixa Editar filtro e clique em **Compartilhar**.

   A caixa Compartilhamento de filtro é exibida.

1. Ative o **Exibir todo o sistema** configuração. Isso dá a qualquer pessoa no Workfront permissão para visualizar o filtro.

   Ou

   Comece a digitar os nomes de usuários, equipes, funções, grupos ou empresas com os quais você deseja compartilhar o filtro na **Conceder acesso a** campo.

   ![](assets/new-filters-sharing-ui-wb-350x422.png)

1. (Opcional) Clique na seta apontando para a direita ao lado do nome de uma entidade para editar suas permissões para o filtro e, em seguida, habilite a opção **Exibir** ou **Gerenciar** opção.

   ![](assets/new-filters-granular-permissions-for-manage-wb-350x107.png)

1. (Opcional) Ative ou desative as permissões adicionais para uma entidade seguindo um destes procedimentos:

   1. Clique em **Exibir** e desative o **Compartilhar** opção. Está ativada por padrão.

   1. Clique em **Gerenciar** e desative qualquer uma das **Compartilhar** ou **Excluir** opção. Eles são ativados por padrão.
   >[!TIP]
   >
   >Os usuários não podem receber uma permissão maior do que o nível de acesso. Se não tiverem acesso a Editar filtros em seu nível de acesso, não poderão receber permissões para gerenciar um filtro. O Workfront desativa a opção Gerenciar para esses usuários e a opção está esmaecida.

1. Clique em **Compartilhar**. O filtro é compartilhado com as entidades especificadas.

   Os filtros compartilhados são exibidos na **Compartilhado comigo** área da caixa de filtro.

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
