---
product-area: projects;templates
navigation-topic: plan-a-project
title: Designar gerentes de recursos para um projeto ou modelo
description: Você pode designar Gerentes de recursos para um projeto para indicar quem é responsável pelo gerenciamento de recursos no projeto.
author: Alina
feature: Work Management
exl-id: ae2a89e7-8049-4ee6-9b28-ce247d3f2a6f
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 3%

---

# Designar gerentes de recursos para um projeto ou modelo

<!--
<p This article might have to be deleted when the Resource Manager field/ requirement will be forever removed from the system; right now it's still a requirement for Scheduler - January 2023/p>
-->

<!-- remove Prod and Prev references with Prod release - Jan 2023-->

Você pode designar Gerentes de recursos para um projeto para indicar quem é responsável pelo gerenciamento de recursos no projeto. Este é um campo informativo e não está conectado a nenhuma ferramenta de gerenciamento de recursos.

<!-- drafted for res scheduling deprecation blurb for preview release
Designating Resource Managers for a project is a prerequisite for using the Scheduling tools in Adobe Workfront, in the Production environment.
  
>[!CAUTION]  
>  
>  
> <span class="preview">Some of the information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span>  
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span>  
>  
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../../resource-mgmt/workload-balancer/workload-balancer.md).</span>  
>  
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Padrão</p> 
   <p>Plano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a projetos e modelos</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões no projeto ou modelo</p>

</td> 
  </tr> 
 </tbody> 
</table>

Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Templates</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project or template</p> 
   
   <p><b>NOTE</b>
   
   Users who are added as Resource Managers to a project or a template immediately gain Manage permissions on the project or the template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Considerações sobre gerentes de recursos

>[!NOTE]
>
>O Gerenciador de Recursos não é uma função de trabalho; é um campo disponível em um projeto ou modelo que você pode atualizar manualmente.

* Você pode designar até 30 usuários como Gerentes de recursos para um projeto ou modelo individual.

<!--
* In the Production environment,designating Resource Managers on projects is a prerequisite to allowing users to schedule resources for work on the project when using the Scheduling tools.

  For information about resource scheduling, see [Resource Scheduling](../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md). 

  <span class="preview">Scheduling tools have been removed from the Preview environment.</span>

* Designating Resource Managers on projects is not a prerequisite to allowing users to schedule resources for work using the Workload Balancer.

  For information about the Workload Balancer, see [Workload Balancer overview](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md). 

 -->

* Não é possível designar equipes ou grupos como gerentes de recursos. Você só pode designar usuários como gerentes de recursos.

* Os usuários designados como Gerentes de recursos em um projeto ou modelo não se tornam automaticamente parte da Equipe do projeto.

  Para obter informações sobre equipes de projeto, consulte [Gerenciar a Equipe do Projeto](../../../manage-work/projects/planning-a-project/manage-project-team.md).

* Você pode designar Gerentes de recursos para projetos ou modelos de projeto. Quando você designa Gerentes de recursos em um modelo de projeto, os usuários designados como Gerentes de recursos no modelo tornam-se automaticamente Gerentes de recursos em qualquer projeto criado usando esse modelo.
* Você pode exibir o campo Gerenciador de Recursos nas seguintes áreas:

   * Ao editar um projeto, conforme descrito neste artigo.
   * Ao editar um modelo, conforme descrito neste artigo.
   * Ao criar relatórios de projeto ou modelo. Para obter informações sobre como criar relatórios, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
   * Ao criar ou personalizar uma visualização de projeto ou modelo para uma lista. Para obter mais informações, consulte [Visão geral na Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

* Você pode adicionar ou remover Gerentes de recursos rapidamente em vários projetos ou modelos, adicionando o campo Gerenciador de recursos a uma exibição de uma lista ou um projeto e editando esse campo usando a edição em linha.

## Designar gerentes de recursos para um projeto

1. Siga um destes procedimentos:

   * Para adicionar Gerentes de Recursos a um único projeto, vá para o projeto em que deseja designar um ou mais gerentes de recursos e clique no menu **Mais** ao lado do nome do projeto e em **Editar.**

   * Para adicionar Gerenciadores de recursos a vários projetos simultaneamente, navegue até uma lista de projetos, selecione os projetos para os quais deseja designar um ou mais gerenciadores de recursos e clique em **Editar**.

     Os gerentes de recursos existentes não são removidos dos projetos que você está editando; todos os usuários adicionados dessa forma são adicionados como gerentes de recursos no projeto, além de qualquer gerente de recursos existente.

   * Para adicionar Gerentes de recursos a um novo projeto, comece a criar um novo projeto.

     Para obter informações sobre como criar um projeto, consulte [Criar um projeto](../../../manage-work/projects/create-projects/create-project.md).

1. Na seção **Visão geral** da caixa de diálogo Editar projeto, clique no campo **Gerenciador de Recursos**.
1. Comece digitando o nome do usuário que deseja adicionar como gerenciador de recursos para o projeto e clique no nome quando ele aparecer na lista.

   Repita esta etapa para adicionar vários gerenciadores de recursos ao projeto.

1. Clique em **Salvar alterações**.

## Designar Gerentes de Recursos para um modelo

{{step1-to-templates}}

1. Siga um destes procedimentos:

   * Para adicionar Gerentes de Recursos a um único modelo, vá para o modelo em que deseja designar um ou mais gerentes de recursos, em seguida, clique no menu **Mais** ao lado do nome do modelo e **Editar.**

   * Para adicionar Gerenciadores de Recursos a vários modelos simultaneamente, vá para uma lista de modelos e selecione os modelos para os quais deseja designar um ou mais Gerenciadores de Recursos e clique em **Editar**.

     Os gerentes de recursos existentes não são removidos dos modelos que você está editando; todos os usuários adicionados dessa forma são adicionados como gerentes de recursos no modelo além de quaisquer gerentes de recursos existentes.

   * Para adicionar Gerentes de Recursos a um novo modelo, clique em **Novo Modelo**, depois no menu **Mais** ao lado do nome do modelo e, em seguida, em **Editar.**

1. Na seção **Visão geral**, clique no campo **Gerenciador de Recursos**.
1. Comece digitando o nome do usuário que deseja adicionar como gerenciador de recursos para o modelo e clique no nome quando ele aparecer na lista.

   Repita esta etapa para adicionar vários gerenciadores de recursos ao modelo.

1. Clique em **Salvar alterações**.
