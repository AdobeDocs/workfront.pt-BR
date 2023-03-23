---
product-area: resource-management
navigation-topic: resource-pools
title: Associar pools de recursos a projetos e modelos
description: Os pools de recursos são coleções de usuários que ajudam a gerenciar recursos no Adobe Workfront.
author: Alina
feature: Resource Management
exl-id: bbfe8257-ff02-4f06-9763-3f2ae4871c9d
source-git-commit: addcff71ff067be22e9ee80f997af545293fa5db
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 0%

---

# Associar pools de recursos a projetos e modelos


<!-- drafted for bulk editing projects: keep this in yellow till this releases to ALL customers - May 1, 2023

Also - take out all the references to Preview and Prod at prod final
-->

<span class="preview">As informações destacadas nesta página se referem à funcionalidade ainda não disponível no geral. Ele está disponível para todos os clientes no ambiente de Visualização e para um grupo selecionado de clientes no ambiente de Produção.</span>


<!--
<p>The sections about how to add resource pools to templates, projects are duplicated from the articles listed in those sections (Editing Projects, Creating a Template, etc).</p>
<p>***I decided to keep these steps here, though, because it's hard to parse through those much lunger articles for just updating this one field.)</p>
-->

Os pools de recursos são coleções de usuários que ajudam a gerenciar recursos no Adobe Workfront.

Depois de criar pools de recursos, você pode associá-los a projetos ou modelos para poder orçar seus recursos posteriormente nos projetos.

Recomendamos que você crie seus pools de recursos antecipadamente, associe-os a projetos e faça o orçamento de seus recursos antes que o projeto inicie.

Para obter informações sobre pools de recursos, consulte [Visão geral dos pools de recursos](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

Para obter informações sobre a criação de pools de recursos, consulte [Criar pools de recursos](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

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
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso ao Gerenciamento de recursos que inclui acesso a Gerenciar conjuntos de recursos</p> <p>Editar acesso a Projetos, Modelos e Usuários</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerencie permissões para projetos, modelos e usuários aos quais você associou os pools de recursos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Associar pools de recursos a um projeto ou modelo

Você pode associar pools de recursos a um modelo da mesma maneira que associa pools de recursos a um projeto. Este artigo descreve como você pode associar pools de recursos a projetos.

1. Vá para um projeto e clique no botão **Mais** ícone ![](assets/more-icon.png)ao lado do nome do projeto, em seguida, clique em **Editar**.

1. Clique em **Configurações do projeto**.

1. Comece a digitar o nome de um pool de recursos no **Pools de Recursos** e, em seguida, selecione-o na lista quando aparecer.\
   Você pode associar vários pools de recursos a um projeto ou modelo.

   ![](assets/nwe-project-settings-in-edit-project-box-350x380.png)

1. Clique em **Salvar**.

Para obter mais informações sobre como editar um projeto e associá-lo a pools de recursos, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

Para obter mais informações sobre como editar um modelo e associá-lo a pools de recursos, consulte [Editar modelos de projeto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Associar pools de recursos a vários projetos ou modelos em massa

É possível editar vários projetos ou modelos em massa e associar os mesmos pools de recursos a todos ao mesmo tempo.

Você pode associar pools de recursos a modelos da mesma maneira que associa pools de recursos a projetos.

Para associar pools de recursos a vários projetos em massa:

1. Acesse uma lista de projetos.
1. Selecione vários projetos e clique no botão **Editar** ícone ![](assets/edit-icon.png) na parte superior da lista.

1. Clique em **Configurações**.
1. Comece a digitar o nome de um pool de recursos no **Pools de Recursos** e, em seguida, selecione-o na lista quando aparecer.\
   Você pode associar vários pools de recursos aos projetos ou modelos.

   >[!NOTE]
   >
   >* No ambiente Produção, ao editar projetos ou modelos em massa, somente os pools de recursos comuns a todos os projetos ou modelos selecionados aparecem nesse campo. Se os projetos selecionados não tiverem pools de recursos compartilhados, esse campo estará vazio. Os pools de recursos especificados aqui substituirão os pools de recursos individuais dos projetos ou modelos.
   >
   >* <span class="preview">No ambiente de Visualização, ao editar projetos em massa, há um indicador &quot;Vários valores&quot; se os projetos selecionados tiverem pools de recursos diferentes. Se você adicionar pools de recursos em massa, todos os pools serão adicionados ao projeto selecionado, substituindo os pools de recursos originais.</span>


   <span class="preview">![add_resource_pools_to_multiple_projects.png](assets/add-resource-pools-to-multiple-projects-350x358.png)</span>

1. Clique em **Salvar alterações**.\
   Quando os pools de recursos estão associados a seus projetos ou modelos, você pode orçar alocações de usuários para seus projetos dentro do Planejador de Recursos.\
   Para obter mais informações sobre o Planejador de Recursos, consulte [Visão geral do Planejador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Para obter mais informações sobre como editar projetos em massa, consulte a seção &quot;Editar projetos em massa&quot; em [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

Para obter mais informações sobre como editar modelos em massa, consulte a seção &quot;Editar modelos em massa&quot; em [Editar modelos de projeto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
