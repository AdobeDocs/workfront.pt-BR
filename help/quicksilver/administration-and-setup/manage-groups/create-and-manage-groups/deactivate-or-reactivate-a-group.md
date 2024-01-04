---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Desativar ou reativar um grupo
description: É possível desativar um grupo gerenciado que você não usa mais.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 99b81090-8d09-4130-a746-44ed1d76f971
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# Desativar ou reativar um grupo

<!--
If Callisto adds the <b>Is active</b> checkbox to the Details page for groups you view, add that info to Manage groups/Create and manage groups/manage-a-group and to Manage groups/Create and manage groups/view-and-manage-a-groups-details
-->

É possível desativar um grupo gerenciado que você não usa mais.

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Workfront*</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> <p>Você deve ser um administrador de grupo do grupo ou um administrador do Workfront. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acesso administrativo total a um usuário</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Se precisar descobrir o tipo de plano ou licença que possui, entre em contato com o administrador do Workfront.

## Desativar ou reativar um grupo

>[!IMPORTANT]
>
>Quando você desativa um grupo, todos os subgrupos abaixo dele também são desativados.
>
>Se você precisar reativar um deles, poderá fazê-lo depois de seguir um destes procedimentos:
>
>* Remova-o do grupo pai. Para obter mais informações, consulte a seção [Remover um subgrupo do grupo pai e torná-lo um grupo de nível superior](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) no artigo [Gerenciar um subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>
>* Movê-lo para um grupo ativo. Para obter mais informações, consulte a seção [Criar, mover, exibir, editar, copiar, renomear, exportar ou excluir um subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#create) no artigo [Gerenciar um subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, selecione **Grupos**.

   Na lista exibida, você pode ver os grupos que gerencia, juntamente com quaisquer subgrupos que eles tenham. Os administradores do Adobe Workfront podem visualizar todos os grupos.

1. Clique no nome do grupo para abrir sua página.

1. Clique no menu Mais ![](assets/more-icon.png) ao lado do nome do grupo, clique em **Desativar** ou **Reativar**.

   >[!NOTE]
   >
   >A opção Está ativo (opção Reativar na visualização) não estará disponível se o grupo for um subgrupo de um grupo desativado. Antes de reativá-la, você deve removê-la do grupo pai ou movê-la para um grupo que esteja ativo, conforme descrito na observação Importante acima.

1. (Condicional) Se você estiver desativando o grupo, clique em **Desativar** no **Desativar grupo** que é exibida.

## Considerações para grupos inativos

Considere o seguinte sobre um grupo que você desativa ao desativar a opção Está ativo explicada na seção [Desativar ou reativar um grupo](#View) neste artigo.

* A desativação de um grupo também desativa todos os subgrupos abaixo dele. Isso inclui subgrupos que você adiciona depois de desativá-lo.

  Para obter informações sobre como reativar um subgrupo nessa situação, consulte [Sobre a reativação de um subgrupo abaixo de um grupo pai inativo](#about-reactivating-a-subgroup-below-an-inactive-parent-group) neste artigo.

* Ao ir para a área Grupos em Configuração, você pode ver somente os grupos ativos na lista, pois Ativo é o filtro padrão ![](assets/filter-nwepng.png) para ele. Se quiser ver todos os grupos gerenciados, incluindo os inativos, use o filtro Todos. Ou use o filtro Inativo para listar apenas os inativos.

  Para obter mais informações sobre filtros em listas, consulte [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* A desativação de um grupo não altera o seguinte:

   * As associações do grupo com os objetos. Os objetos associados continuam a funcionar como antes, sem alterações.

     Por exemplo, se um projeto estiver associado a um grupo que você desativa, o projeto continuará a usar as preferências e os status do grupo sem alterações.

   * Sua capacidade de criar um novo objeto, como uma aprovação, equipe ou empresa, de dentro da página do grupo na configuração. Por padrão, o novo objeto é associado ao grupo inativo.
   * Sua capacidade de, como administrador, encontrar o grupo em filtros e relatórios.

     Você também pode encontrá-los em campos de digitação antecipada de grupo, nos quais talvez você queira gerenciar as configurações do grupo na área Configuração. Isso inclui as áreas Preferências, Notificações de eventos e Licenças do sistema.

     Por exemplo, se você for até Configurar > Preferência de projeto > Projetos e limpar o campo digitação antecipada acima das opções lá, ainda será possível encontrar um grupo inativo e configurar suas preferências de projeto.

## Sobre a reativação de um subgrupo abaixo de um grupo pai inativo {#about-reactivating-a-subgroup-below-an-inactive-parent-group}

A desativação de um grupo também desativa todos os subgrupos abaixo dele. Se precisar reativar um dos subgrupos em um grupo inativo, você pode executar uma das seguintes ações:

* Mova o subgrupo para um grupo ativo. Em seguida, ative a opção Está ativo para o grupo movido, conforme explicado na seção [Desativar ou reativar um grupo](#View) neste artigo.

  Para obter instruções sobre como mover um grupo, consulte [Mover um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

* Remova o subgrupo do grupo pai (o que torna o subgrupo um grupo de nível superior). Em seguida, ative a opção Está ativo para o grupo movido, conforme explicado na seção [Desativar ou reativar um grupo](#View) neste artigo.

  Para obter instruções sobre como remover um subgrupo de seu grupo pai, consulte a seção [Remover um subgrupo do grupo pai e torná-lo um grupo de nível superior](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) no artigo [Gerenciar um subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
