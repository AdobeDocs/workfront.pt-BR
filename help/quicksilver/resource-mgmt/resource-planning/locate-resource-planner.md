---
product-area: resource-management
navigation-topic: resource-planning
title: Localizar o Planejador de Recursos
description: '"(Este artigo saiu deste: rascunhe o conteúdo do artigo quando ele for exibido: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)'''
author: Alina
feature: Resource Management
exl-id: 0de749df-5af9-4124-8539-06b82dca2ec4
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# Localizar o Planejador de Recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This came off this article: draft that content in the article when this comes live: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)</p>
-->

Você pode usar o Planejador de Recursos para gerenciar a alocação de seus recursos para projetos. Você pode acessar o Planejador de Recursos para vários projetos ao mesmo tempo ou para um projeto, na área Caso de Negócios do projeto.

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
   <td> <p>Revisar ou superior<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> <p>Planejar ou superior para localizar o Planejador de Recursos na área global</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Exibir acesso ou superior ao Gerenciamento de recursos</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões para projetos e usuários </p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Verifique se todos os pré-requisitos para acessar e trabalhar com o Planejador de Recursos foram atendidos antes de começar a usá-lo. Dessa forma, você garante que o Planejador de Recursos exiba as informações corretas antes que você comece a orçar seus recursos.

Para obter informações sobre os pré-requisitos do Resource Planner, consulte [Introdução ao planejamento de recursos](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## Localizar o Planejador de Recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this was moved from the get-started-resource-planner article)</p>
-->

Você pode localizar o Planejador de Recursos em duas áreas do Workfront, dependendo se deseja orçar seus recursos para vários projetos ou para apenas um projeto.

* [Usar o Planejador de Recursos para vários projetos](#use-the-resource-planner-for-multiple-projects)
* [Usar o Planejador de Recursos para um projeto](#use-the-resource-planner-for-one-project)

### Usar o Planejador de Recursos para vários projetos {#use-the-resource-planner-for-multiple-projects}

Ao usar o Planejador de recursos para vários projetos, os números de alocação de seus recursos representam números em vários projetos.

Para acessar a seção Planejador na área Recursos:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.

1. Clique em **Recursos**. O Planejador é exibido por padrão.  Para obter informações sobre recursos de orçamento no Planejador de Recursos, consulte o artigo [Recursos de orçamento no Planejador de Recursos usando as exibições Projeto e Função](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   ![](assets/qs-resource-management-area-with-planner-as-default-350x152.png)

1. Passe o mouse sobre o painel esquerdo e clique em **Pools de Recursos**.\
   Para obter informações sobre a criação de pools de recursos, consulte [Criar pools de recursos](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

### Usar o Planejador de Recursos para um projeto {#use-the-resource-planner-for-one-project}

Ao usar o Planejador de Recursos para um projeto, os números de alocação de seus recursos representam números para o projeto selecionado.

1. Vá para um projeto para o qual deseja orçar recursos.
1. Clique em **Caso de negócios** no painel esquerdo.
1. Role para **Orçamentação de Recursos** seção do Caso de negócios.
1. Clique em **Editar Orçamento de Recurso** para adicionar pools de recursos ao seu projeto e começar a orçar seus recursos.

   >[!TIP]
   >
   >Você só pode adicionar um pool de recursos na área Orçamento de Recursos do Caso de Negócios quando o projeto não tiver pools de recursos associados a ele. Quando o projeto já tem um Pool de Recursos, os usuários no pool e suas funções de job são exibidos na área de Orçamento de Recursos por padrão.

   ![](assets/resource-budgeting-area-on-project-350x70.png)

   Para obter informações sobre como orçar recursos de um projeto, consulte o artigo [Recursos orçamentários no Caso de Negócios](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).
