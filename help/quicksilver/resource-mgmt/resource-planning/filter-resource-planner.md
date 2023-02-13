---
product-area: resource-management
navigation-topic: resource-planning
title: Filtrar informações no Planejador de Recursos
description: '"AL:*Iterar este artigo: filtragem por dados personalizados. Outras melhorias? Caracteres especiais que podem mudar - siga a história para saber quando. Originalmente veio na Beta 3 17.3.)'''
author: Alina
feature: Resource Management
exl-id: 7186cae5-1e16-421e-b26d-afb50aa7f6eb
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '2442'
ht-degree: 0%

---

# Filtrar informações no Planejador de Recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(AL:*Iterate on this article: filtering by custom data. Other enhancements? Special characters caveat might change - follow the story to know when. It originally came in Beta 3 17.3.)</p>
-->

Usando filtros, você pode modificar quais informações são exibidas no Planejador de Recursos de todas as informações armazenadas no sistema.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Pro e superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Revisar ou superior<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Visualizar ou obter mais acesso a Projetos, Usuários e Gerenciamento de Recursos </p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou superior para projetos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Visão geral dos filtros do Planejador de recursos

Para minimizar a quantidade de informações exibidas no Planejador de Recursos, o Adobe Workfront fornece um Filtro Padrão com critérios pré-configurados. Para obter informações sobre o Filtro padrão, consulte a seção [Visão Geral do Filtro Padrão no Planejador de Recursos](#overview-of-the-default-filter-in-the-resource-planner) neste artigo.

Você também pode criar filtros personalizados. Para obter informações sobre como personalizar filtros no Planejador de Recursos, consulte a seção [Criar filtros do Planejador de recursos](#create-resource-planner-filters) neste artigo.

Considere o seguinte ao usar filtros no Planejador de Recursos:

* Os filtros criados são visíveis somente para você. Você pode compartilhar filtros para disponibilizá-los a outros usuários.
* Como administrador do Workfront, você só pode ver filtros que criar ou que sejam compartilhados com você.
* Os resultados filtrados não são alterados quando você seleciona uma exibição diferente para o Planejador de Recursos.\
   Para obter mais informações sobre como alterar a exibição no Planejador de Recursos, consulte a seção de seleção &quot;Projeto/Função/exibição do usuário&quot; em [Visão geral da navegação do Planejador de recursos](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

* A aplicação de um filtro não altera os dados de alocação e disponibilidade no Planejador de Recursos para projetos, funções ou usuários. Um filtro altera apenas o número de objetos que você vê no Planejador de Recursos.
* A filtragem se aplica a todos os objetos exibidos no Planejador de Recursos ao mesmo tempo. Por exemplo, se você filtrar um usuário específico, o Planejador de Recursos exibirá apenas os seguintes resultados:

   * Projetos em que esse usuário faz parte do Pool de Recursos (para as exibições Projeto e Função) ou tem uma atribuição no projeto (para a exibição Usuário)
   * Funções associadas ao usuário nesses projetos\
      Outras funções ou usuários nos projetos aos quais o usuário está associado não são exibidos.

## Visão Geral do Filtro Padrão no Planejador de Recursos {#overview-of-the-default-filter-in-the-resource-planner}

Quando você abre o Planejador de Recursos pela primeira vez, o Workfront aplica o filtro Padrão. Você pode editar o filtro Padrão para filtrar apenas os itens que deseja exibir. Para obter informações sobre modificação de filtros, consulte a seção [Editar um filtro no Planejador de Recursos](#edit-a-filter-in-the-resource-planner) neste artigo.

Considere o seguinte ao usar o filtro Padrão:

* O Filtro padrão recupera informações apenas de projetos com o seguinte:

   * Uma Data de Conclusão Planejada que ocorre após a primeira data do mês atual
   * Uma Data Inicial Planejada que ocorre antes do último dia do quarto mês a partir da data atual
   * Um Status de Planejamento ou Atual

   >[!IMPORTANT]
   >
   >O filtro Padrão recupera informações dos projetos que ocorrem sempre dentro de quatro meses, começando pelo primeiro dia do mês atual, independentemente do período selecionado para exibição no Planejador de Recursos.

* Na Visualização de usuário, todos os usuários do sistema são exibidos, mas somente os usuários associados aos projetos filtrados mostram informações de hora.
* Você pode editar as informações no filtro Padrão sem salvar o filtro.
* Você pode duplicar e editar uma cópia do filtro Padrão, alterar os critérios desejados e salvá-lo como um novo filtro.
* Não é possível excluir ou compartilhar o filtro Padrão.

   ![RP_new_default_fitler_criteria__1_.PNG](assets/rp-new-default-fitler-criteria--1--301x547.png)

## Criar filtros do Planejador de recursos {#create-resource-planner-filters}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: **^ This section is somewhat duplicated (format more than content) from the "Filtering Utilization Information" section in "Viewing Utilization Information for Projects, Programs, and Portfolios.")</p>
-->

Criar um filtro no Planejador de Recursos é idêntico para todas as exibições.

Verifique se os pré-requisitos para visualizar as informações corretas no Planejador de Recursos estão em vigor antes de criar um filtro.\
Para obter informações sobre como atender aos pré-requisitos necessários para trabalhar com o Planejador de Recursos, consulte a seção &quot;Pré-requisitos para trabalhar no Planejador de Recursos&quot; no [Visão geral do Planejador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md) artigo 10. o

Considere o seguinte ao criar um filtro:

* Não há limite para o número de objetos que podem ser filtrados de uma vez.
* Os campos disponíveis que podem ser adicionados a uma alteração de filtro de acordo com o objeto da exibição aplicada ao Planejador de Recursos. Por exemplo, você pode filtrar os campos Problema ou Tarefa somente na Exibição do Usuário, pois esses objetos são exibidos somente na Exibição do Usuário. Se você criar um filtro para Problemas ou Tarefas na exibição Usuário e depois aplicá-lo às exibições Projeto ou Função, ele será ignorado porque os campos não existem nas exibições Projeto ou Função. Nesse caso, o filtro parece indisponível.

Para criar um filtro no Planejador de Recursos:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.

1. Clique em **Recursos**.

   O **Planejador** é exibido por padrão.

   Por padrão, na primeira vez que você acessar o Planejador de Recursos, a variável <strong>Filtro padrão</strong> é aplicada.<br>Para obter mais informações sobre o filtro Padrão, consulte o <a href="#overview-of-the-default-filter-in-the-resource-planner" class="MCXref xref">Visão Geral do Filtro Padrão no Planejador de Recursos</a> neste artigo.

1. No canto superior esquerdo do , clique no botão **Filtro** ícone .\
   ![filter_icon.png](assets/filter-icon.png)\
   Ou\
   Expanda o **Filtro** e clique em **Adicionar novo filtro**.\
   ![](assets/rp-filter-dropdown-expanded-with-default-filter-selected-350x283.png)

1. Para criar um filtro usando os critérios incorporados, especifique qualquer um dos seguintes campos:

   * **Portfolio**: Comece a digitar o nome do portfólio que contém as informações que deseja incluir no Planejador de Recursos e clique no nome quando ele aparecer na lista.\
      Repita esse processo para incluir informações de vários portfólios.

   * **Status do projeto**: Expanda o menu suspenso Status do projeto e selecione um ou vários status de projeto disponíveis na lista.
   * **Equipe**: Comece a digitar o nome de uma ou várias equipes associadas aos usuários atribuídos às tarefas nos projetos que deseja visualizar.
   * **Função da Tarefa**: Comece digitando o nome de uma ou várias funções de trabalho associadas aos usuários atribuídos às tarefas nos projetos que deseja visualizar.
   * **Pools**: Comece a digitar o nome de um ou vários Pools de Recursos associados aos projetos (para a Exibição do Projeto), aos usuários (para a Exibição do Usuário) ou associados aos projetos e aos usuários (para a Exibição da Função) que você deseja visualizar.
   * **Grupo**: Comece digitando o nome de um ou vários grupos associados aos usuários (na exibição Usuário) ou projetos (nas exibições Projeto e Função) que você deseja visualizar.

1. Clique em **Adicionar regra de filtro** e comece a digitar o nome do campo que deseja filtrar no **Digite para filtrar itens** caixa. Se o campo estiver disponível, ele será preenchido para cada objeto ao qual pode ser associado.

   >[!IMPORTANT]
   >
   >Ao fazer referência a campos personalizados, você deve digitar o nome do campo e não o rótulo do campo. O rótulo do campo é exibido em um formulário personalizado anexado a um objeto. Para obter informações sobre a diferença entre o rótulo e o nome de um campo personalizado, consulte  [Criar ou editar um formulário personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) .

1. Clique no nome do campo para adicioná-lo ao filtro quando ele aparecer na lista.\
   Para obter mais informações sobre os campos que você vê na lista, consulte [Glossário da terminologia do Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

1. (Opcional) Selecione o filtro e os modificadores de condição para o filtro. Os modificadores disponíveis são descritos em [Modificadores de filtro e condição](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   Você pode usar curingas com base em usuário ou com base em data para filtrar informações associadas ao usuário conectado.\
   Para obter informações sobre curingas compatíveis em filtros, consulte [Variáveis de filtro curinga](../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Clique em **Salvar** para salvar a regra de filtro.
1. (Opcional) Clique em **Adicionar regra de filtro** para adicionar uma nova regra para outro objeto ou campo.
1. Clique em **Aplicar** para aplicar o filtro sem salvá-lo.

   Ou

   Clique em **Salvar filtro** para salvar o filtro.\
   ![RP_Apply_or_Save_button_on_filters.png](assets/rp-apply-or-save-buttons-on-filters-320x79.png)

1. (Condicional) Depois de clicar em **Salvar**, especifique um nome para o filtro na **Nome do filtro** dentro da caixa **Salvar filtro** caixa de diálogo. Este campo é obrigatório.\
   ![RP_new_save_filter_box__with_Save_button__without_apply.png](assets/rp-new-save-filter-box--with-save-button--without-apply-350x175.png)

   >[!NOTE]
   >
   >Se o nome do filtro incluir caracteres especiais, use apenas os seguintes caracteres:
   >
   >* Vírgula
   >* Barra
   >* Hífen
   >* Sublinhado


1. Clique em **Salvar**.

   Os resultados no Planejador de Recursos agora são filtrados pelas informações incluídas nas regras de filtro.

## Aplicar um filtro existente

Quando você ou alguém com acesso ao Planejador de Recursos salva um filtro, ele fica disponível para todos que usam o Planejador de Recursos.

Para aplicar um filtro existente:

1. Vá para o Planejador de Recursos.
1. No canto superior esquerdo, expanda o **Filtro** menu suspenso.

   Você pode ver filtros que você criou ou outros criados e compartilhados com você neste menu.\
   ![RP_filter_drop_down.png](assets/rp-filter-drop-down-350x152.png)

1. Selecione um filtro no menu suspenso. Você pode ver filtros que você ou outros usuários criaram neste menu.\
   Ao selecionar um filtro, ele reduz automaticamente a quantidade de informações exibidas no Planejador de Recursos.

## Editar um filtro no Planejador de Recursos {#edit-a-filter-in-the-resource-planner}

Você pode editar um filtro no Planejador de Recursos seguindo um destes procedimentos:

* [Renomear um filtro](#rename-a-filter)
* [Editar as informações em um filtro](#edit-the-information-in-a-filter)
* [Duplicar um filtro](#duplicate-a-filter)

Ao editar um filtro, ele é atualizado para todos os usuários no sistema que têm acesso ao Planejador de Recursos.

### Renomear um filtro {#rename-a-filter}

Você pode alterar o nome de um filtro sem alterar seus critérios. Recomendamos que outros usuários do sistema saibam dessa alteração, pois os filtros ficam visíveis para outros usuários. Essa alteração afeta as listas de filtros para todos que podem ver o Planejador de Recursos.

1. Vá para o Planejador de Recursos e expanda o **Filtro** menu suspenso para selecionar um filtro salvo.
1. Expanda o **Filtro** menu suspenso. Localize o filtro que deseja renomear e passe o mouse sobre seu nome.
1. Selecione o **Renomear filtro** ícone ao lado do nome do filtro.

   ![](assets/rp-filter-options-edit-350x154.png)

1. Especifique um novo nome para o filtro no **Nome do filtro** caixa.
1. Clique em **Salvar**.\
   As informações incluídas no filtro são iguais e o nome é atualizado.

### Editar as informações em um filtro {#edit-the-information-in-a-filter}

É possível alterar as informações incluídas em um filtro sem alterar seu nome. Recomendamos que outros usuários do sistema saibam dessa alteração, pois os filtros ficam visíveis para eles. Essa alteração afeta as listas de filtros para todos que podem ver o Planejador de Recursos.

1. Vá para o Planejador de Recursos e expanda o **Filtro** menu suspenso no canto superior esquerdo.
1. Selecione um filtro existente que deseja editar.
1. Clique no botão **Filtro** ícone .\
   ![filter_icon.png](assets/filter-icon.png)

1. Adicione novos campos ao filtro.\
   Para obter informações sobre como criar filtros, consulte [Criar filtros do Planejador de recursos](#create-resource-planner-filters).

1. Passe o mouse sobre os campos existentes selecionados para o filtro, e clique no botão **Editar** ícone para selecionar outro campo, ou o **Excluir** ícone para excluir o campo.\
   ![RP_custom_filter_delete_and_edit_icons.png](assets/rp-custom-filter-delete-and-edit-icons-350x169.png)

1. (Opcional) Clique em **Adicionar regra de filtro** para adicionar novos campos ao filtro.\
   Para obter mais informações sobre como definir critérios de filtro, consulte [Criar filtros do Planejador de recursos](#create-resource-planner-filters).

1. Clique em **Aplicar** para aplicar o filtro sem salvá-lo.

   Ou

   Clique em **Salvar** para salvar o filtro.\
   O filtro é salvo com o mesmo nome, mas com novos critérios de filtragem.

### Duplicar um filtro {#duplicate-a-filter}

Você pode duplicar um filtro existente. Os critérios de filtragem originais permanecem os mesmos no filtro duplicado e você pode salvar o novo filtro com um novo nome.

1. Vá para o Planejador de Recursos e expanda o **Filtro** menu suspenso no canto superior esquerdo.
1. Passe o mouse sobre o nome de um filtro salvo que você deseja duplicar.
1. Clique no botão **Duplicar** ícone .

   ![](assets/rp-filter-options---duplicate-350x154.png)\
   A caixa Filtro duplicado é exibida.

1. No **Nome do filtro** , especifique um novo nome para o filtro duplicado.\
   O nome padrão do novo filtro é *`<Original Filter Name>`(cópia)*.

1. Clique em **Salvar**. Um novo filtro é criado com os mesmos critérios do filtro original e com um novo nome.

   >[!NOTE]
   >
   >Embora você possa ter dois filtros pelo mesmo nome e com critérios idênticos, recomendamos que salve os filtros com critérios de filtragem e nomes exclusivos no Planejador de recursos para evitar confusão.

## Excluir um filtro

Você pode excluir um filtro quando ele não é mais necessário. Não é possível excluir o filtro padrão.

Para obter informações sobre o Filtro padrão, consulte o [Visão Geral do Filtro Padrão no Planejador de Recursos](#overview-of-the-default-filter-in-the-resource-planner) neste artigo.

Ao excluir um filtro, ele é excluído para todos os usuários do Workfront que têm acesso ao Planejador de Recursos. Antes de removê-lo, verifique se o filtro que você deseja remover não é mais usado por ninguém que esteja trabalhando no Planejador de Recursos. Não é possível recuperar um filtro excluído.

Para remover um filtro:

1. Vá para o Planejador de Recursos.
1. Expanda o **Filtro** menu suspenso.
1. Localize o filtro que deseja remover e passe o mouse sobre seu nome.
1. Selecione o **Excluir filtro** ícone ao lado do nome do filtro.

   ![](assets/rp-filter-options---delete-350x154.png)

1. Clique em **Excluir** no **Excluir filtro** caixa de diálogo.

1. O filtro é excluído e removido do Planejador de Recursos.

## Compartilhar um filtro

Você pode compartilhar um filtro criado ou que tenha acesso para compartilhar com outros usuários. Não é possível compartilhar o Filtro padrão, mas você pode duplicá-lo e compartilhá-lo.

>[!NOTE]
>
>Todos os usuários, incluindo administradores do Workfront, podem acessar somente filtros que eles criaram ou que foram compartilhados com eles. Você pode compartilhar um filtro com usuários específicos para disponibilizar um filtro para todos os usuários do Resource Planner.

Para obter informações sobre o Filtro padrão, consulte o [Visão Geral do Filtro Padrão no Planejador de Recursos](#overview-of-the-default-filter-in-the-resource-planner) neste artigo.

Para obter informações sobre duplicação de filtros, consulte [Duplicar um filtro](#duplicate-a-filter) neste artigo.

1. Vá para o Planejador de Recursos.
1. Expanda o **Filtro** menu suspenso.
1. Localize o filtro que deseja compartilhar e passe o mouse sobre seu nome.
1. Selecione o **Compartilhar filtro** ícone ao lado do nome do filtro.

   ![](assets/rp-filter-options---share-350x154.png)

   A caixa de diálogo Acesso ao filtro é exibida.

1. (Opcional) Para disponibilizar o filtro para todos os usuários do Planejador de Recursos, clique no **Configurações** ícone e selecione **Tornar esse sistema visível**.

   ![](assets/make-this-visible-system-wide-350x119.png)

1. No **Conceder acesso ao filtro do planejador de recursos para:** , comece digitando os nomes de usuários, equipes, funções, grupos ou empresas com os quais deseja compartilhar o filtro.
1. Selecione entre os seguintes níveis de permissões:

   * Exibir
   * Gerenciar

      Para obter informações sobre permissões no Workfront, consulte [Visão geral do compartilhamento de permissões em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)

1. (Opcional) Clique em **Configuração avançada** s para adicionar permissões para cada nível, selecionando-as ou removendo permissões para cada nível, desmarcando-as.

   ![](assets/rp-share-filter-manage-advanced-settings-350x271.png)

1. Clique em **Salvar**.

   O filtro é compartilhado com as entidades selecionadas e aparece na variável **Compartilhado comigo** área.

   ![](assets/rp-shared-with-me-area.png)
