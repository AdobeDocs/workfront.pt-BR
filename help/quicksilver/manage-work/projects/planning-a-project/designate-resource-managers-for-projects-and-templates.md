---
product-area: projects;templates
navigation-topic: plan-a-project
title: Designar Gerentes de Recursos para um projeto ou modelo
description: Você pode designar Gerentes de Recursos para um projeto para indicar quem é responsável pelo gerenciamento de recursos no projeto.
author: Alina
feature: Work Management
exl-id: ae2a89e7-8049-4ee6-9b28-ce247d3f2a6f
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 0%

---

# Designar Gerentes de Recursos para um projeto ou modelo

<!--
<p This article might have to be deleted when the Resource Manager field/ requirement will be forever removed from the system; right now it's still a requirement for Scheduler - January 2023/p>
-->

<!-- remove Prod and Prev references with Prod release - Jan 2023-->

Você pode designar Gerentes de Recursos para um projeto para indicar quem é responsável pelo gerenciamento de recursos no projeto. Este é um campo informativo e não está conectado a nenhuma ferramenta de gerenciamento de recursos.

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

<!--drafted for P&P:

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
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
</table>
-->

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos e Modelos</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões no projeto ou modelo</p>

<p><b>Nota</b>

Os usuários adicionados como Gerentes de recursos a um projeto ou modelo recebem permissões de Gerenciamento imediatamente no projeto ou no modelo</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td>
</tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Considerações sobre Gerentes de Recursos

>[!NOTE]
>
>O Gerenciador de Recursos não é uma função de trabalho; é um campo disponível em um projeto ou modelo que pode ser atualizado manualmente.

* Você pode designar até 30 usuários como Gerentes de recursos para um projeto ou modelo individual.

<!--
* In the Production environment,designating Resource Managers on projects is a prerequisite to allowing users to schedule resources for work on the project when using the Scheduling tools.

  For information about resource scheduling, see [Resource Scheduling](../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md). 

  <span class="preview">Scheduling tools have been removed from the Preview environment.</span>

* Designating Resource Managers on projects is not a prerequisite to allowing users to schedule resources for work using the Workload Balancer.

  For information about the Workload Balancer, see [Overview of the Workload Balancer](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md). 

 -->

* Não é possível designar equipes ou grupos como gerentes de recursos. Você só pode designar usuários como gerentes de recursos.

* Os usuários designados como Gestores de Recursos em um projeto ou modelo não se tornam automaticamente parte da Equipe do Projeto.

   Para obter informações sobre equipes de projeto, consulte [Gerenciar a equipe do projeto](../../../manage-work/projects/planning-a-project/manage-project-team.md).

* Você pode designar Gerentes de recursos para projetos ou modelos de projeto. Ao designar Gerentes de Recursos em um modelo de projeto, qualquer usuário designado como Gerentes de Recursos no modelo se torna automaticamente Gerentes de Recursos em qualquer projeto criado usando esse modelo.
* Você pode exibir o campo Gerenciador de Recursos nas seguintes áreas:

   * Ao editar um projeto, conforme descrito neste artigo.
   * Ao editar um modelo, conforme descrito neste artigo.
   * Ao criar relatórios de projeto ou de modelo. Para obter informações sobre como criar relatórios, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
   * Ao criar ou personalizar um projeto ou uma visualização de modelo para uma lista. Para obter mais informações, consulte [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

* Você pode adicionar ou remover rapidamente Gerentes de Recursos em vários projetos ou modelos, adicionando o campo Gerenciador de Recursos a uma exibição de uma lista ou de um projeto e editando esse campo usando a edição em linha.

## Designar Gerentes de Recursos para um projeto

1. Siga um destes procedimentos:

   * Para adicionar Gerentes de recursos a um único projeto, vá para o projeto onde deseja designar um ou mais gerentes de recursos, em seguida, clique no **Menu Mais** ao lado do nome do projeto, em seguida **Editar .**

   * Para adicionar Gerentes de recursos a vários projetos simultaneamente, navegue até uma lista de projetos, selecione os projetos nos quais deseja designar um ou mais gerentes de recursos e clique em **Editar**.

      Os Gerentes de Recursos Existentes não são removidos dos projetos que você está editando; quaisquer usuários adicionados dessa forma são adicionados como Gerentes de Recursos no projeto, além de quaisquer Gerentes de Recursos existentes.

   * Para adicionar Gerentes de recursos a um novo projeto, comece a criar um novo projeto.

      Para obter informações sobre como criar um projeto, consulte [Criar um projeto](../../../manage-work/projects/create-projects/create-project.md).

1. No **Visão geral** na caixa de diálogo Editar projeto , clique em **Gerenciador de recursos** campo.
1. Comece digitando o nome do usuário que deseja adicionar como um gerenciador de recursos do projeto, em seguida, clique no nome quando ele aparecer na lista.

   Repita essa etapa para adicionar vários gerentes de recursos ao projeto.

1. Clique em **Salvar alterações**.

## Designar Gerentes de Recursos para um modelo

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.

1. Clique em **Modelos**.

1. Siga um destes procedimentos:

   * Para adicionar Gerentes de recursos a um único modelo, vá para o modelo onde deseja designar um ou mais gerentes de recursos, em seguida, clique no **Menu Mais** ao lado do nome do modelo, em seguida **Editar .**

   * Para adicionar Gerentes de Recursos a vários modelos simultaneamente, vá para uma lista de modelos e selecione os modelos nos quais deseja designar um ou mais Gerentes de Recursos, em seguida, clique em **Editar**.

      Os Gerentes de Recursos Existentes não são removidos dos modelos que você está editando; quaisquer usuários adicionados dessa forma são adicionados como Gerentes de recursos no modelo, além de quaisquer Gerentes de recursos existentes.

   * Para adicionar Gerentes de Recursos a um novo modelo, clique em **Novo modelo** e clique no botão **Menu Mais** ao lado do nome do modelo, em seguida **Editar .**

1. No **Visão geral** clique em na seção **Gerenciador de recursos** campo.
1. Comece digitando o nome do usuário que deseja adicionar como um gerenciador de recursos para o modelo e clique no nome quando ele aparecer na lista.

   Repita essa etapa para adicionar vários gerentes de recurso ao modelo.

1. Clique em **Salvar alterações**.
