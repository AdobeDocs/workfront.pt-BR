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
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 0%

---

# Personalizar filtros, visualizações e agrupamentos usando um modelo de layout

Como administrador do Adobe Workfront, você pode usar um modelo de layout para especificar quais controles de lista aparecem nos menus suspensos Filtro, Exibir e Agrupamento. Esses menus são exibidos acima em listas em todo o Workfront, como a lista de tarefas de um projeto:

![Modelos de layout de agrupamento de modo de exibição de filtro](assets/filter-view-grouping-layout-templates.png)

Para obter mais informações sobre modelos de layout, consulte [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Para obter informações sobre modelos de layout para grupos, consulte [Criar e modificar modelos de layout de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Após configurar um modelo de layout, você deve atribuí-lo aos usuários para que as alterações feitas fiquem visíveis para outros usuários. Para obter informações sobre como atribuir um modelo de layout aos usuários, consulte [Atribuir usuários a um modelo de layout](../use-layout-templates/assign-users-to-layout-template.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td><p>Novo: Padrão</p>
  <p> Atual: Plano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Para executar essas etapas no nível do sistema, você precisa do nível de acesso Administrador do sistema.
Para executá-las para um grupo, você deve ser um gerente desse grupo.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizar controles de Filtro, Exibição e Lista de Agrupamento:

1. Comece a trabalhar em um modelo de layout, conforme descrito em [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Clique na seta para baixo ![Seta para baixo](assets/down-arrow-blue.png) em **Personalize o que os usuários veem** e clique em **Listas** no menu suspenso exibido.

   ![Personalize o que os usuários veem](assets/customize-what-users-see-dropdown-on-pg-adobe-branding.png)

1. Clique na seta para baixo ![Seta para baixo](assets/down-arrow-blue.png) em **Selecione uma lista para personalizar** e selecione o tipo de objeto do Workfront para o qual deseja personalizar os controles de Filtro, Exibição e Lista de Agrupamento.

   ![Selecione uma lista para personalizar](assets/select-a-list-to-customize-menu-on-pg-adobe-branding.png)

   >[!NOTE]
   >
   >Se você selecionar Projetos como a lista a ser personalizada e desativar Projetos aos quais pertenço ou Projetos que possuo na seção Filtro, os usuários não verão mais esse filtro ou não poderão mais usá-lo:
   >
   >* Na lista de filtros exibida ao clicar no ícone de filtro ![Ícone de filtro](assets/filter-nwepng.png) acima de uma lista:
   >   
   >  ![Desabilitar filtros](assets/disable-filters-projects-im-on-or-own.png)
   >   
   >* No cabeçalho do cabeçalho da área Projetos:
   >   
   >  ![Botão Desabilitar filtros](assets/disable-filter-pills.png)

1. (Opcional) Se quiser alterar o filtro, o modo de exibição ou o agrupamento padrão do modelo de layout, passe o mouse sobre o filtro, o modo de exibição ou o agrupamento e clique em **Definir como padrão**.

   Os padrões escolhidos determinam qual Filtro, Exibição e Agrupamento os usuários verão nas listas em todo o Workfront quando o modelo de layout for atribuído a eles. Se você não alterar esses padrões, os usuários verão todas as listas da seguinte maneira:

   * **Filtros**: Todos
   * **Exibição**: Padrão (onde aplicável; algumas listas não têm essa exibição)
   * **Agrupamento**: nada

   Você pode ocultar as opções Tudo, Padrão e Nada após selecionar padrões diferentes (consulte a Etapa 5), mas eles não podem ser excluídos.

   É possível excluir qualquer outra opção que esteja sendo usada como padrão, mas primeiro é necessário selecionar um padrão diferente.

   Para obter informações sobre como excluir filtros, modos de exibição e agrupamentos, consulte [Criar, editar e compartilhar filtros, modos de exibição e agrupamentos padrão](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md).

1. Ocultar e adicionar controles de lista da seguinte maneira:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ocultar um controle de lista</td> 
      <td> <p>Desmarque ou marque a caixa ao lado do controle de lista que deseja ocultar ou mostrar.</p> <p>Se uma caixa de seleção estiver esmaecida, você não poderá ocultar esse controle de lista. A configuração Padrão <img src="assets/default-pill.png"> para cada controle de lista está esmaecida porque você não pode ocultar a configuração que está definida como padrão no momento.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Adicionar um controle de lista personalizado</td> 
      <td> <p> 
        <ol> 
         <li value="1"> Clique em <strong>Adicionar filtro</strong>, <strong>Adicionar exibição</strong> ou <strong>Adicionar agrupamento</strong> na parte inferior da lista Filtro, Exibição ou Agrupamento. Na caixa exibida, comece digitando o nome de um controle de lista personalizado existente criado anteriormente para sua organização e, em seguida, clique no nome quando ele for exibido.</li> 
         <li value="2"> Se desejar que o novo controle de lista personalizado seja definido como filtro, exibição ou agrupamento padrão para o modelo de layout, clique em <strong>Definir como Padrão</strong>. </li> 
         <li value="3"> <p>Clique em <strong>Adicionar</strong> quando terminar.</p> <p><b>NOTA</b>: <p>Os usuários podem adicionar controles de lista personalizados a suas próprias listas. Se você adicionar controles de lista personalizados em um modelo de layout, os controles de lista serão adicionados e os deles serão movidos para a parte inferior do painel; os seus não substituirão os deles.</p> <p>Isso também será verdadeiro se você atribuir o usuário a um novo modelo de layout que tenha controles de lista personalizados. </p> <p>Para obter informações sobre como personalizar controles de lista, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Visão geral dos Filtros</a>, <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Visão geral das Exibições no Adobe Workfront</a> e <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Visão geral dos Agrupamentos no Adobe Workfront</a>.</p> </p> </li> 
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
