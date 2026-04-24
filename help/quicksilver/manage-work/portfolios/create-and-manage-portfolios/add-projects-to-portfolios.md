---
product-area: portfolios;projects
navigation-topic: create-and-manage-portfolios
title: Adicionar projetos a uma Portfolio
description: Recomendamos que você adicione projetos aos portfólios ao iniciá-los. No entanto, você pode adicioná-los a um portfólio a qualquer momento durante sua vida útil.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 97f36c18-3ac8-45ac-b5bc-dfe8b1363faf
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: fee6b71eeb0ca79703a2a9e29a14040b91cb7387
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 4%

---

# Adicionar projetos a um portfólio

<!--Audited: 08/2025-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>
-->

Recomendamos que você adicione projetos aos portfólios ao iniciá-los. No entanto, você pode adicioná-los a um portfólio a qualquer momento durante sua vida útil.

Considere o seguinte ao adicionar projetos a portfólios:

* Você pode associar apenas um portfólio a um projeto.
* Um projeto permanece em um portfólio até ser removido ou associado a outro portfólio.
* Um portfólio pode conter um número ilimitado de projetos.

>[!CAUTION]
>
>   As permissões herdadas podem não ser aplicadas corretamente quando usadas em um grande número de objetos filho.
>   
>   Para ajudar a evitar problemas de permissões herdadas, recomendamos o seguinte:
>
>   * Limitar o número de objetos filho (projetos) em um único pai (portfólio ou programa). Recomendamos no máximo 10.000 projetos por portfólio ou programa.
>   * Reduza a profundidade da herança aplicando permissões em um objeto de nível inferior.
>
>     Por exemplo, aplique permissões diretamente no nível do projeto, em vez de confiar nas permissões herdadas do portfólio para o programa e, em seguida, para o projeto.
>   * Divida os programas para conter menos projetos, o que reduz a complexidade das permissões.


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] pacote</td> 
   <td> <p>Qualquer</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td><p>Padrão</p> 
   <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuração do nível de acesso</td> 
   <td> <p>Portfólios de acesso ao [!UICONTROL Editar]</p> <p>[!UICONTROL Editar] acesso a Projetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Permissões do [!UICONTROL Manager] para o portfólio</p> <p>[!UICONTROL Gerenciar] permissões para os projetos</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>New: Standard</p> 
   <p>Current: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>[!UICONTROL Edit] access Portfolios</p> <p>[!UICONTROL Edit] access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio</p> <p>[!UICONTROL Manage] permissions to the projects</p>  </td> 
  </tr> 
 </tbody> 
</table>
-->

## Adicionar um projeto a um portfólio

1. Go to a portfolio, then click **[!UICONTROL Projects]** in the left panel.

   ![Portfolio with projects](assets/qs-portfolio-with-projects-350x90.png)

1. Click **[!UICONTROL New Project]** and select a method for adding a project.

   >[!TIP]
   >
   >You cannot add a project when you view the list of projects in the [!UICONTROL Milestone] view.

   Selecione entre as seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Existing Project]</td> 
      <td> <p>Add a project that has already been created.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL New Project]</td> 
      <td> <p>Add a new project. </p> <p>For more information about creating a new project, see <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">Create a project</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Import a Project from [!DNL MS Project]] </td> 
      <td> <p>Add a project that you previously exported from [!DNL MS Project] and have saved on your computer. </p> <p>For more information about creating a new project by importing it from [!DNL Microsoft Project], see <a href="../../../manage-work/projects/create-projects/import-project-from-ms-project.md" class="MCXref xref">Import a project from [!DNL Microsoft Project]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Request Project]</td> 
      <td> <p>Request that a project is approved.</p> <p>For information about requesting projects, see <a href="../../../manage-work/projects/create-projects/request-project.md">Requesting a Project</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL New from Template]</td> 
      <td> <p>Add a new project using an existing template. </p> <p>For more information about creating a project from a template, see <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Create a project using a template</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![Lista suspensa de novos projetos](assets/new-project-dropdown-expanded-from-portfolio-nwe-350x376.png)

1. (Conditional) If you selected to add an existing project, the **Add Projects** box opens. <!--check this after UI changes-->

   ![Add existing project](assets/add-existing-projects-to-portfolios-box.png) <!--check this after UI changes-->

1. Start typing the name of a project in the **[!UICONTROL Add Projects to this Portfolio]** field, then click them when they appear in the list.  <!--check this after UI changes-->

   You can add more than one project.

1. (Optional) Click the **X** icon to the right of the project name to remove it from the list, if you decide not to add it to the portfolio.

   <!--replace last step with this, for unshim: 1. (Optional) Click the **Delete** icon ![Delete icon](assets/delete-icon.png) next to the name of a project if you decide not to add it to the portfolio.-->

1. Click **[!UICONTROL Add Projects]**. <!--check this after UI changes-->

   The project or projects you selected are now associated with the portfolio.
