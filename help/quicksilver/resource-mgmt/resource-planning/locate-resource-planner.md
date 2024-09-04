---
product-area: resource-management
navigation-topic: resource-planning
title: Localizar o Planejador de recursos
description: Você pode usar o Planejador de recursos para gerenciar a alocação de seus recursos para projetos. Você pode acessar o Planejador de recursos para vários projetos ao mesmo tempo ou para um projeto, a partir da área Business Case do projeto.
author: Lisa
feature: Resource Management
exl-id: 0de749df-5af9-4124-8539-06b82dca2ec4
source-git-commit: a5317e3126939d4c648977635af2dbc6add02780
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# Localizar o Planejador de recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This came off this article: draft that content in the article when this comes live: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)</p>
-->

Você pode usar o Planejador de recursos para gerenciar a alocação de seus recursos para projetos. Você pode acessar o Planejador de recursos para vários projetos ao mesmo tempo ou para um projeto, a partir da área Business Case do projeto.

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
   <td><p>Novo: Claro ou superior;</br>
          Padrão para localizar o Planejador de recursos no menu principal</p>
       <p>ou</p>
       <p>Atual: revisão ou superior;</br>
       Planejar a localização do Planejador de recursos no menu principal</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Exibir acesso ou superior ao Gerenciamento de recursos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões para projetos e usuários </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Certifique-se de que todos os pré-requisitos para acessar e trabalhar com o Planejador de recursos sejam atendidos antes de começar a usá-lo. Dessa forma, você garante que o Planejador de recursos exiba as informações corretas antes de começar a fazer o orçamento de seus recursos.

Para obter informações sobre os pré-requisitos do Planejador de Recursos, consulte [Introdução ao Planejamento de Recursos](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## Localizar o Planejador de recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this was moved from the get-started-resource-planner article)</p>
-->

Você pode localizar o Planejador de recursos em duas áreas do Workfront, dependendo se deseja fazer o orçamento de seus recursos para vários projetos ou para apenas um projeto.

* [Usar o Planejador de recursos para vários projetos](#use-the-resource-planner-for-multiple-projects)
* [Usar o Planejador de recursos para um projeto](#use-the-resource-planner-for-one-project)

### Usar o Planejador de recursos para vários projetos {#use-the-resource-planner-for-multiple-projects}

Ao usar o Planejador de recursos para vários projetos, os números de alocação dos seus recursos representam números entre vários projetos.

Para acessar a seção Planejador na área Recursos:

{{step1-to-resourcing}}

O Planejador é exibido por padrão.  Para obter informações sobre recursos de orçamento no Planejador de recursos, consulte o artigo [Recursos de orçamento no Planejador de recursos usando as exibições de Projeto e Função](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

![](assets/qs-resource-management-area-with-planner-as-default-350x152.png)

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

   ![](assets/resource-budgeting-area-on-project-350x70.png)

   Para obter informações sobre recursos de orçamento para um projeto, consulte o artigo [Recursos de orçamento no Business Case](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).
