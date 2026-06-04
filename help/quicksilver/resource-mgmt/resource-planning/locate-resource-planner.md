---
product-area: resource-management
navigation-topic: resource-planning
title: Localizar o planejador de recursos
description: Você pode usar o Planejador de recursos para gerenciar a alocação de seus recursos para projetos. Você pode acessar o Planejador de recursos para vários projetos ao mesmo tempo ou para um projeto, a partir da área Business Case do projeto.
author: Lisa
feature: Resource Management
exl-id: 0de749df-5af9-4124-8539-06b82dca2ec4
TQID: https://experienceleague.adobe.com/-p17GWsoDlmbZtZW3T47YGxOmgSOsMddnFfFXpW36C4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: d1573eb8-a2e8-4a06-9526-9c3410bf4914
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 461
ht-degree: 9%

---

# Localizar o planejador de recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This came off this article: draft that content in the article when this comes live: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)</p>
-->

Você pode usar o Planejador de recursos para gerenciar a alocação de seus recursos para projetos. Você pode acessar o Planejador de recursos para vários projetos ao mesmo tempo ou para um projeto, a partir da área Business Case do projeto.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td>
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Leve ou superior para um projeto; Padrão para vários projetos</p>
       <p>Revisão ou superior para um projeto; planejamento para vários projetos</p></td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Exibir acesso ou superior ao Gerenciamento de recursos</p> </td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td> <p>Exibir permissões para projetos e usuários </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Certifique-se de que todos os pré-requisitos para acessar e trabalhar com o Planejador de recursos sejam atendidos antes de começar a usá-lo. Dessa forma, você garante que o Planejador de recursos exiba as informações corretas antes de começar a fazer o orçamento de seus recursos.

Para obter informações sobre os pré-requisitos do Planejador de Recursos, consulte [Introdução ao Planejamento de Recursos](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## Localizar o planejador de recursos

Você pode localizar o Planejador de recursos em duas áreas do Workfront, dependendo se deseja fazer o orçamento de seus recursos para vários projetos ou para apenas um projeto.

* [Usar o Planejador de recursos para vários projetos](#use-the-resource-planner-for-multiple-projects)
* [Usar o Planejador de recursos para um projeto](#use-the-resource-planner-for-one-project)

### Usar o Planejador de recursos para vários projetos {#use-the-resource-planner-for-multiple-projects}

Ao usar o Planejador de recursos para vários projetos, os números de alocação dos seus recursos representam números entre vários projetos.

Para acessar a seção Planejador na área Recursos:

{{step1-to-resourcing}}

O Planejador é exibido por padrão.  Para obter informações sobre recursos de orçamento no Planejador de recursos, consulte o artigo [Recursos de orçamento no Planejador de recursos usando as exibições de Projeto e Função](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

![Planejador de recursos como padrão](assets/qs-resource-management-area-with-planner-as-default-350x152.png)

1. Clique em **Conjuntos de Recursos** no painel esquerdo.
Para obter informações sobre como criar pools de recursos, consulte [Criar pools de recursos](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

### Usar o Planejador de recursos para um projeto {#use-the-resource-planner-for-one-project}

Ao usar o Planejador de recursos para um projeto, os números de alocação dos recursos representam números para o projeto selecionado.

1. Vá para um projeto para o qual você deseja estimar recursos.
1. Clique em **Business Case** no painel esquerdo.
1. Role até a seção **Estimativa de recursos** do Business Case.
1. Clique em **Editar orçamento de recursos** para adicionar conjuntos de recursos ao seu projeto e começar a fazer o orçamento dos seus recursos.

   >[!TIP]
   >
   >Você só poderá adicionar um conjunto de recursos na área Orçamento de Recursos do Business Case quando o projeto não tiver nenhum conjunto de recursos associado a ele. Quando o projeto já tiver um Conjunto de Recursos, os usuários no conjunto e suas funções de trabalho serão exibidos na área Orçamento de Recursos por padrão.

   ![Estimativa de recursos](assets/resource-budgeting-area-on-project-350x70.png)

   Para obter informações sobre recursos de orçamento para um projeto, consulte o artigo [Recursos de orçamento no Business Case](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).
