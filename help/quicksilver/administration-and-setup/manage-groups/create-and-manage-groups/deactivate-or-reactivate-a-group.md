---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Desativar ou reativar um grupo
description: É possível desativar um grupo gerenciado que você não usa mais.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 99b81090-8d09-4130-a746-44ed1d76f971
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '766'
ht-degree: 0%

---

# Desativar ou reativar um grupo

<!--
If Callisto adds the <b>Is active</b> checkbox to the Details page for groups you view, add that info to Manage groups/Create and manage groups/manage-a-group and to Manage groups/Create and manage groups/view-and-manage-a-groups-details
-->

É possível desativar um grupo gerenciado que você não usa mais.

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
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Novo: Padrão</p>
       <p>Ou</p>
       <p>Atual: Plano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>Você deve ser um administrador de grupo do grupo ou um administrador do sistema.</td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Desativar ou reativar um grupo

>[!IMPORTANT]
>
>Quando você desativa um grupo, todos os subgrupos abaixo dele também são desativados.
>
>Se você precisar reativar um deles, poderá fazê-lo depois de seguir um destes procedimentos:
>
>* Remova-o do grupo pai. Para obter mais informações, consulte a seção [Remover um subgrupo de seu grupo pai e torná-lo um grupo de nível superior](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) no artigo [Gerenciar um subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>
>* Movê-lo para um grupo ativo. Para obter mais informações, consulte a seção [Criar, mover, exibir, editar, copiar, renomear, exportar ou excluir um subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#create) no artigo [Gerenciar um subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).

{{step-1-to-setup}}

1. No painel esquerdo, selecione **Grupos**.

   Na lista exibida, você pode ver os grupos que gerencia, juntamente com quaisquer subgrupos que eles tenham. Os administradores do Adobe Workfront podem visualizar todos os grupos.

1. Clique no nome do grupo para abrir sua página.

1. Clique no menu Mais ![](assets/more-icon.png) ao lado do nome do grupo e em **Desativar** ou **Reativar**.

   >[!NOTE]
   >
   >A opção Está ativo (opção Reativar na visualização) não estará disponível se o grupo for um subgrupo de um grupo desativado. Antes de reativá-la, você deve removê-la do grupo pai ou movê-la para um grupo que esteja ativo, conforme descrito na observação Importante acima.

1. (Condicional) Se você estiver desativando o grupo, clique em **Desativar** na caixa **Desativar grupo** que será exibida.

## Considerações para grupos inativos

Considere o seguinte sobre um grupo que você desativa ao desabilitar a opção Está Ativo explicada na seção [Desativar ou reativar um grupo](#View) neste artigo.

* A desativação de um grupo também desativa todos os subgrupos abaixo dele. Isso inclui subgrupos que você adiciona depois de desativá-lo.

  Para obter informações sobre como reativar um subgrupo nessa situação, consulte [Sobre a reativação de um subgrupo abaixo de um grupo pai inativo](#about-reactivating-a-subgroup-below-an-inactive-parent-group) neste artigo.

* Ao ir para a área Grupos na Configuração, você pode ver apenas os grupos ativos na lista, pois Ativo é o filtro padrão ![](assets/filter-nwepng.png) para ele. Se quiser ver todos os grupos gerenciados, incluindo os inativos, use o filtro Todos. Ou use o filtro Inativo para listar apenas os inativos.

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

* Mova o subgrupo para um grupo ativo. Em seguida, habilite a opção Está Ativo para o grupo movido, conforme explicado na seção [Desativar ou reativar um grupo](#View) deste artigo.

  Para obter instruções sobre como mover um grupo, consulte [Mover um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

* Remova o subgrupo do grupo pai (o que torna o subgrupo um grupo de nível superior). Em seguida, habilite a opção Está Ativo para o grupo movido, conforme explicado na seção [Desativar ou reativar um grupo](#View) deste artigo.

  Para obter instruções sobre como remover um subgrupo do grupo pai, consulte a seção [Remover um subgrupo do grupo pai e torná-lo um grupo de nível superior](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) no artigo [Gerenciar um subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
