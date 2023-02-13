---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Desativar ou reativar um grupo
description: É possível desativar um grupo que você gerencia e que não é mais usado.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 99b81090-8d09-4130-a746-44ed1d76f971
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 0%

---

# Desativar ou reativar um grupo

<!--
If Callisto adds the <b>Is active</b> checkbox to the Details page for groups you view, add that info to Manage groups/Create and manage groups/manage-a-group and to Manage groups/Create and manage groups/view-and-manage-a-groups-details
-->

É possível desativar um grupo que você gerencia e que não é mais usado.

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Workfront*</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> <p>Você deve ser um administrador de grupo do grupo ou um administrador do Workfront. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores do grupo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Se precisar descobrir qual plano ou tipo de licença você tem, entre em contato com o administrador da Workfront.

## Desativar ou reativar um grupo

>[!IMPORTANT]
>
>Ao desativar um grupo, os subgrupos abaixo também são desativados.
>
>Se precisar reativar um deles, é possível fazer isso depois de:
>
>* Remova-o do grupo pai. Para obter mais informações, consulte a seção [Remova um subgrupo de seu grupo pai e torne-o um grupo de nível superior](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) no artigo [Gerenciar um subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>
>* Mova-o para baixo de um grupo ativo. Para obter mais informações, consulte a seção [Criar, mover, exibir, editar, copiar, renomear, exportar ou excluir um subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#create) no artigo [Gerenciar um subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>


1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, selecione **Grupos**.

   Na lista que é exibida, é possível ver os grupos gerenciados, juntamente com os subgrupos que eles possuem. Os administradores do Adobe Workfront podem visualizar todos os grupos.

1. Clique no nome do grupo para abrir a página.

1. Clique no menu Mais ![](assets/more-icon.png) ao lado do nome do grupo, em seguida, clique em **Desativar** ou **Reativar**.

   >[!NOTE]
   >
   >A opção Is Ative (Reativar na Visualização) não estará disponível se o grupo for um subgrupo de um grupo desativado. Antes de poder reativá-lo, você deve removê-lo do grupo pai ou movê-lo em um grupo que esteja ativo, conforme descrito na observação Importante acima.

1. (Condicional) Se você estiver desativando o grupo, clique em **Desativar** no **Desativar grupo** que é exibida.

## Considerações para grupos inativos

Considere o seguinte sobre um grupo que você desativa ao desabilitar a opção Está ativo explicada na seção [Desativar ou reativar um grupo](#View) neste artigo.

* Desativar um grupo também desativa todos os subgrupos abaixo dele. Isso inclui subgrupos que você adiciona depois de desativá-lo.

   Para obter informações sobre a reativação de um subgrupo nessa situação, consulte [Sobre a reativação de um subgrupo abaixo de um grupo pai inativo](#about-reactivating-a-subgroup-below-an-inactive-parent-group) neste artigo.

* Quando você vai para a área Grupos em Configurar, você pode ver somente grupos ativos na lista porque Ativo é o filtro padrão ![](assets/filter-nwepng.png) para isso. Se quiser ver todos os grupos gerenciados, incluindo os inativos, use o filtro Todos . Ou use o filtro Inativo para listar apenas os inativos.

   Para obter mais informações sobre filtros em listas, consulte [Visão geral dos filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* Desativar um grupo não altera o seguinte:

   * As associações do grupo aos objetos. Os objetos associados continuam a funcionar como antes, sem alterações.

      Por exemplo, se um projeto estiver associado a um grupo que você desativar, o projeto continuará a usar as preferências e os status do grupo sem alterações.

   * Sua capacidade de criar um novo objeto, como uma aprovação, equipe ou empresa, dentro da página do grupo na configuração. Por padrão, o novo objeto é associado ao grupo inativo.
   * Sua capacidade, como administrador, de encontrar o grupo em filtros e relatórios.

      Também é possível encontrá-lo em campos do tipo group ahead, onde você pode desejar gerenciar as configurações do grupo na área Configuração. Isso inclui as áreas Preferências, Notificações de eventos e Licenças do sistema.

      Por exemplo, se você acessar Configurar > Preferência do projeto > Projetos e limpar o campo do tipo avançado acima das opções, ainda poderá encontrar um grupo inativo e configurar suas preferências de projeto.

## Sobre a reativação de um subgrupo abaixo de um grupo pai inativo {#about-reactivating-a-subgroup-below-an-inactive-parent-group}

Desativar um grupo também desativa todos os subgrupos abaixo dele. Se você precisar reativar um dos subgrupos em um grupo inativo, é possível fazer uma das duas coisas a seguir:

* Mova o subgrupo em um grupo ativo. Em seguida, ative a opção Is Ative para o grupo movido, conforme explicado na seção [Desativar ou reativar um grupo](#View) neste artigo.

   Para obter instruções sobre como mover um grupo, consulte [Mover um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

* Remova o subgrupo de seu grupo pai (o que faz do subgrupo um grupo de nível superior). Em seguida, ative a opção Is Ative para o grupo movido, conforme explicado na seção [Desativar ou reativar um grupo](#View) neste artigo.

   Para obter instruções sobre como remover um subgrupo de seu grupo pai, consulte a seção [Remova um subgrupo de seu grupo pai e torne-o um grupo de nível superior](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) no artigo [Gerenciar um subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
