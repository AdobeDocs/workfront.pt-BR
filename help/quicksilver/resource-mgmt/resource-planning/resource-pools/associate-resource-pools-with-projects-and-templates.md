---
product-area: resource-management
navigation-topic: resource-pools
title: Associar Conjuntos de Recursos a Projetos e Modelos
description: Conjuntos de recursos são coleções de usuários que ajudam você a gerenciar recursos no Adobe Workfront.
author: Lisa
feature: Resource Management
exl-id: bbfe8257-ff02-4f06-9763-3f2ae4871c9d
source-git-commit: a3b2ac192e1f37e0c3d16d059ed96e8d5cadf8be
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 1%

---

# Associar conjuntos de recursos a projetos e modelos


<!-- drafted for bulk editing projects: keep this in yellow till this releases to ALL customers - May 1, 2023

Also - take out all the references to Preview and Prod at prod final
-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->


<!--
<p>The sections about how to add resource pools to templates, projects are duplicated from the articles listed in those sections (Editing Projects, Creating a Template, etc).</p>
<p>***I decided to keep these steps here, though, because it's hard to parse through those much lunger articles for just updating this one field.)</p>
-->

Conjuntos de recursos são coleções de usuários que ajudam você a gerenciar recursos no Adobe Workfront.

Depois de criar conjuntos de recursos, você pode associá-los a projetos ou modelos para que possa estimar seus recursos nos projetos posteriormente.

Recomendamos que você crie seus conjuntos de recursos antecipadamente, associe-os a projetos e faça um orçamento de recursos antes do início do projeto.

Para obter informações sobre pools de recursos, consulte [Visão geral sobre pools de recursos](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

Para obter informações sobre como criar pools de recursos, consulte [Criar pools de recursos](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td><p>Novo: Qualquer um</p>
       <p>ou</p>
       <p>Atual: Pro ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Novo: Padrão</p>
       <p>ou</p>
       <p>Atual: Plano</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso ao Gerenciamento de recursos que inclui acesso a Gerenciar conjuntos de recursos</p> <p>Editar acesso a projetos, modelos e usuários</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permissões de objeto</td> 
   <td>Gerenciar permissões para projetos, modelos e usuários aos quais você deseja associar os Conjuntos de recursos</td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Associar conjuntos de recursos a um projeto ou modelo

É possível associar conjuntos de recursos a um modelo da mesma maneira que você associa conjuntos de recursos a um projeto. Este artigo descreve como associar conjuntos de recursos a projetos.

1. Vá para um projeto e clique no ícone **Mais** ícone ![Mais](assets/more-icon.png)ao lado do nome do projeto e clique em **Editar**.

1. Clique em **Configurações do projeto**.

1. Comece digitando o nome de um pool de recursos no campo **Pools de Recursos** e selecione-o na lista quando ele for exibido.\
   É possível associar vários conjuntos de recursos a um projeto ou modelo.

   ![Configurações do projeto](assets/nwe-project-settings-in-edit-project-box-350x380.png)

1. Clique em **Salvar**.

Para obter mais informações sobre como editar um projeto e associá-lo a conjuntos de recursos, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

Para obter mais informações sobre como editar um modelo e associá-lo a conjuntos de recursos, consulte [Editar modelos de projeto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Associar conjuntos de recursos a vários projetos ou modelos em massa

É possível editar vários projetos ou modelos em massa e associar os mesmos conjuntos de recursos a todos eles ao mesmo tempo.

É possível associar conjuntos de recursos a modelos da mesma maneira que você associa conjuntos de recursos a projetos.

Para associar conjuntos de recursos a vários projetos em massa:

1. Ir para uma lista de projetos.
1. Selecione vários projetos e clique no **ícone Editar** ![ícone Editar](assets/edit-icon.png) na parte superior da lista.

1. Clique em **Configurações**.
1. Comece digitando o nome de um pool de recursos no campo **Pools de Recursos** e selecione-o na lista quando ele for exibido.\
   É possível associar vários conjuntos de recursos aos projetos ou modelos.

   >[!NOTE]
   >
   >* Ao editar modelos em massa, somente os conjuntos de recursos comuns a todos os modelos selecionados aparecem nesse campo. Se os modelos selecionados não tiverem conjuntos de recursos compartilhados, esse campo estará vazio. Os conjuntos de recursos especificados aqui substituem os conjuntos de recursos individuais dos projetos ou modelos.
   >
   >* Quando você edita projetos em massa, há um indicador &quot;Vários valores&quot; se os projetos selecionados tiverem conjuntos de recursos diferentes. Se você adicionar conjuntos de recursos em massa para projetos, todos os conjuntos serão adicionados ao projeto selecionado, substituindo os conjuntos de recursos originais.

   ![add_resource_pools_to_multiple_projects.png](assets/add-resource-pools-to-multiple-projects-350x358.png)

1. Clique em **Salvar alterações**.\
   Quando o conjunto de recursos estiver associado aos projetos ou modelos, você poderá estimar as alocações de usuário para os projetos dentro do Planejador de recursos.\
   Para obter mais informações sobre o Planejador de recursos, consulte [Visão geral do Planejador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Para obter mais informações sobre como editar projetos em massa, consulte a seção &quot;Editar projetos em massa&quot; em [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

Para obter mais informações sobre como editar modelos em massa, consulte a seção &quot;Editar modelos em massa&quot; em [Editar modelos de projeto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
