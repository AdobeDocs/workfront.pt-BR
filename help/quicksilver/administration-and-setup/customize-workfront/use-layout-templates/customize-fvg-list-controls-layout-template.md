---
title: Personalizar filtros, visualizações e agrupamentos usando um modelo de layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Como administrador do Workfront, você pode usar um modelo de layout para especificar quais controles de lista aparecem nos menus suspensos Filtro, Exibir e Agrupamento. Esses menus são exibidos acima em listas em todo o Workfront, como a lista de tarefas de um projeto.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: e9b61da8-2eca-4d88-969b-ae337e402540
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 0%

---

# Personalizar filtros, visualizações e agrupamentos usando um modelo de layout

Como administrador do Adobe Workfront, você pode usar um modelo de layout para especificar quais controles de lista aparecem nos menus suspensos Filtro, Exibir e Agrupamento. Esses menus são exibidos acima em listas em todo o Workfront, como a lista de tarefas de um projeto:

![](assets/filter-view-grouping-layout-templates.png)

Para obter mais informações sobre modelos de layout, consulte [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Para obter informações sobre modelos de layout para grupos, consulte [Criar e modificar os modelos de layout de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Após configurar um modelo de layout, você deve atribuí-lo aos usuários para que as alterações feitas fiquem visíveis para outros usuários. Para obter informações sobre como atribuir um modelo de layout aos usuários, consulte [Atribuir usuários a um modelo de layout](../use-layout-templates/assign-users-to-layout-template.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Para executar essas etapas no nível do sistema, você precisa do nível de acesso Administrador do sistema.
Para executá-las para um grupo, você deve ser um gerente desse grupo.</p> <p><b>NOTA</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalizar controles de Filtro, Exibição e Lista de Agrupamento:

1. Comece a trabalhar em um modelo de layout, conforme descrito em [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Clique na seta para baixo ![](assets/down-arrow-blue.png) em **Personalize o que os usuários veem** e, em seguida, clique em **Listas** no menu suspenso que é exibido.

   ![](assets/customize-what-users-see-dropdown-on-pg-adobe-branding.png)

1. Clique na seta para baixo ![](assets/down-arrow-blue.png) em **Selecione uma lista para personalizar**, em seguida, selecione o tipo de objeto do Workfront para o qual deseja personalizar os controles Filtro, Exibição e Lista de agrupamento.

   ![](assets/select-a-list-to-customize-menu-on-pg-adobe-branding.png)

   >[!NOTE]
   >
   >Se você selecionar Projetos como a lista a ser personalizada e desativar Projetos aos quais pertenço ou Projetos que possuo na seção Filtro, os usuários não verão mais esse filtro ou não poderão mais usá-lo:
   >
   >* Na lista de filtros exibida ao clicar no ícone de filtro ![](assets/filter-nwepng.png) acima de uma lista:
   >   
   >  ![](assets/disable-filters-projects-im-on-or-own.png)
   >   
   >* No cabeçalho do cabeçalho da área Projetos:
   >   
   >  ![](assets/disable-filter-pills.png)

1. (Opcional) Se desejar alterar o filtro, a exibição ou o agrupamento padrão do modelo de layout, passe o mouse sobre o filtro, a exibição ou o agrupamento e clique em **Definir como padrão**.

   Os padrões escolhidos determinam qual Filtro, Exibição e Agrupamento os usuários verão nas listas em todo o Workfront quando o modelo de layout for atribuído a eles. Se você não alterar esses padrões, os usuários verão todas as listas da seguinte maneira:

   * **Filtros**: Todos
   * **Exibir**: Padrão (quando aplicável; algumas listas não têm essa visualização)
   * **Agrupamento**: Nada

   Você pode ocultar as opções Tudo, Padrão e Nada após selecionar padrões diferentes (consulte a Etapa 5), mas eles não podem ser excluídos.

   É possível excluir qualquer outra opção que esteja sendo usada como padrão, mas primeiro é necessário selecionar um padrão diferente.

   Para obter informações sobre a exclusão de filtros, visualizações e agrupamentos, consulte [Criar, editar e compartilhar filtros, visualizações e agrupamentos padrão](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md).

1. Ocultar e adicionar controles de lista da seguinte maneira:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ocultar um controle de lista</td> 
      <td> <p>Desmarque ou marque a caixa ao lado do controle de lista que deseja ocultar ou mostrar.</p> <p>Se uma caixa de seleção estiver esmaecida, você não poderá ocultar esse controle de lista. O padrão <img src="assets/default-pill.png"> a configuração de cada controle de lista está esmaecida porque não é possível ocultar a configuração que está definida como padrão no momento.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Adicionar um controle de lista personalizado</td> 
      <td> <p> 
        <ol> 
         <li value="1"> Clique em <strong>Adicionar filtro</strong>, <strong>Adicionar visualização</strong>ou <strong>Adicionar Agrupamento</strong> na parte inferior da lista Filtro, Exibição ou Agrupamento. Na caixa exibida, comece digitando o nome de um controle de lista personalizado existente criado anteriormente para sua organização e, em seguida, clique no nome quando ele for exibido.</li> 
         <li value="2"> Se desejar que o novo controle de lista personalizado seja definido como filtro, exibição ou agrupamento padrão para o modelo de layout, clique em <strong>Definir como padrão</strong>. </li> 
         <li value="3"> <p>Clique em <strong>Adicionar</strong> quando terminar.</p> <p><b>NOTA</b>: <p>Os usuários podem adicionar controles de lista personalizados a suas próprias listas. Se você adicionar controles de lista personalizados em um modelo de layout, os controles de lista serão adicionados e os deles serão movidos para a parte inferior do painel; os seus não substituirão os deles.</p> <p>Isso também será verdadeiro se você atribuir o usuário a um novo modelo de layout que tenha controles de lista personalizados. </p> <p>Para obter informações sobre como personalizar controles de lista, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Visão geral dos filtros</a>, <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Visão geral das exibições no Adobe Workfront</a>, e <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Visão geral de agrupamentos no Adobe Workfront</a>.</p> </p> </li> 
        </ol> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Continue personalizando o modelo de layout.

   Ou

   Se tiver terminado de personalizar, clique em **Salvar**.

   >[!TIP]
   >
   >Você pode clicar em Salvar a qualquer momento para salvar seu progresso e, em seguida, continuar modificando o modelo posteriormente.
