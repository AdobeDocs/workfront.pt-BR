---
title: Personalizar filtros, exibições e agrupamentos usando um modelo de layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Como administrador do Workfront, você pode usar um modelo de layout para especificar quais controles de lista aparecem nos menus suspensos Filtro, Exibição e Agrupamento . Esses menus são exibidos acima de listas em todo o Workfront, como a lista de tarefas para um projeto.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e9b61da8-2eca-4d88-969b-ae337e402540
source-git-commit: f3785c66b979cc95bf1d2d2ccacbdeefe0ef0967
workflow-type: tm+mt
source-wordcount: '741'
ht-degree: 0%

---

# Personalizar filtros, exibições e agrupamentos usando um modelo de layout

Como administrador do Adobe Workfront, você pode usar um modelo de layout para especificar quais controles de lista aparecem nos menus suspensos Filtro, Exibição e Agrupamento . Esses menus são exibidos acima de listas em todo o Workfront, como a lista de tarefas de um projeto:

![](assets/filter-view-grouping-layout-templates.png)

Para obter mais informações sobre modelos de layout, consulte [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Para obter informações sobre modelos de layout para grupos, consulte [Criar e modificar modelos de layout de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Para executar essas etapas no nível do sistema, é necessário o nível de acesso Administrador do sistema.
Para executá-los para um grupo, você deve ser um gerente desse grupo.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalizar controles de Filtro, Exibição e Lista de agrupamento:

1. Comece a trabalhar em um modelo de layout, conforme descrito em [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Clique na seta para baixo ![](assets/down-arrow-blue.png) under **Personalize o que os usuários veem**, depois clique em **Listas** no menu suspenso que é exibido.

   ![](assets/customize-what-users-see-dropdown-on-pg-adobe-branding.png)

1. Clique na seta para baixo ![](assets/down-arrow-blue.png) under **Selecione uma lista para personalizar**, selecione o tipo de objeto do Workfront para o qual deseja personalizar os controles da lista Filtro, Exibição e Agrupamento.

   ![](assets/select-a-list-to-customize-menu-on-pg-adobe-branding.png)

   >[!NOTE]
   >
   >Se você selecionar Projetos como a lista a ser personalizada e, em seguida, desativar Projetos que eu sou ou Projetos que sou proprietário na seção Filtro, os usuários não verão mais ou poderão usar esse filtro:
   >
   >* Na lista de filtros que é exibida ao clicar no ícone de filtro ![](assets/filter-nwepng.png) acima de uma lista:
   >   
   >  ![](assets/disable-filters-projects-im-on-or-own.png)
   >   
   >* No cabeçalho do cabeçalho da área Projetos :
   >   
   >  ![](assets/disable-filter-pills.png)

1. (Opcional) Se desejar alterar o filtro padrão, a visualização ou o agrupamento do modelo de layout, passe o mouse sobre o filtro, a visualização ou o agrupamento e clique em **Definir como padrão**.

   Os padrões escolhidos determinam quais Filtro, Visualização e Agrupamento os usuários verão em listas em todo o Workfront quando o modelo de layout for atribuído a eles. Se você não alterar esses padrões, os usuários verão todas as listas da seguinte maneira:

   * **Filtros**: Todos
   * **Exibir**: Padrão (se aplicável; algumas listas não têm essa exibição)
   * **Agrupamento**: Nada

   É possível ocultar as opções Todos, Padrão e Nada após selecionar padrões diferentes (consulte a Etapa 5), mas eles não podem ser excluídos.

   É possível excluir qualquer outra opção que esteja sendo usada como padrão, mas é necessário selecionar primeiro um padrão diferente.

   Para obter informações sobre exclusão de filtros, exibições e agrupamentos, consulte [Criar, editar e compartilhar filtros, exibições e agrupamentos padrão](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md).

1. Ocultar e adicionar controles de lista da seguinte maneira:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ocultar um controle de lista</td> 
      <td> <p>Desmarque ou desmarque a caixa ao lado do controle da lista que deseja ocultar ou mostrar.</p> <p>Se uma caixa de seleção estiver esmaecida, você não poderá ocultar esse controle de lista. O padrão <img src="assets/default-pill.png"> para cada controle de lista está esmaecido porque você não pode ocultar a configuração que está configurada no momento como padrão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Adicionar um controle de lista personalizada</td> 
      <td> <p> 
        <ol> 
         <li value="1"> Clique em <strong>Adicionar filtro</strong>, <strong>Adicionar Exibição</strong>ou <strong>Adicionar agrupamento</strong> na parte inferior da lista Filtro, Exibição ou Agrupamento. Na caixa exibida, comece a digitar o nome de um controle de lista personalizada existente criado anteriormente para sua organização e, em seguida, clique no nome quando ele for exibido.</li> 
         <li value="2"> Se desejar que o novo controle de lista personalizada seja definido como filtro padrão, visualização ou agrupamento para o modelo de layout, clique em <strong>Definir como padrão</strong>. </li> 
         <li value="3"> <p>Clique em <strong>Adicionar</strong> quando você terminar.</p> <p><b>Nota</b>: <p>Os usuários podem adicionar controles de lista personalizados a suas próprias listas. Se você adicionar controles de lista personalizados em um modelo de layout, os controles de lista serão adicionados e os deles serão movidos para a parte inferior do painel; o seu não substitui o deles.</p> <p>Isso também é verdade se você atribuir o usuário a um novo modelo de layout que tenha controles de lista personalizados. </p> <p>Para obter informações sobre como personalizar controles de lista, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Visão geral dos filtros no Adobe Workfront</a>, <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Visão geral das exibições no Adobe Workfront</a>e <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Visão geral dos agrupamentos no Adobe Workfront</a>.</p> </p> </li> 
        </ol> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Continue personalizando o modelo de layout.

   Ou

   Se tiver terminado de personalizar, clique em **Salvar**.

   >[!TIP]
   >
   >Você pode clicar em Salvar a qualquer momento para salvar seu progresso e continuar modificando o modelo posteriormente.
