---
title: Visão geral da hierarquia e da navegação estrutural
description: Você pode criar várias hierarquias de espaço de trabalho entre os tipos de registro em um espaço de trabalho.
hide: true
hidefromtoc: true
source-git-commit: 1f1db1c9184a6a8a2abcd3139e4e4e61d2f08bc4
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Hierarchy and Breadcrumb Overview
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---
-->

# Visão geral da hierarquia e da navegação estrutural

Como um gerenciador de espaço de trabalho, você pode definir hierarquias flexíveis mas estruturadas entre tipos de registro e outros tipos de objeto no Adobe Workfront Planning.

Hierarquias são conexões entre tipos de registro. É possível ter até quatro tipos de registro e objeto conectados em uma hierarquia.

Para obter informações sobre como criar hierarquias, consulte [Criar hierarquias do espaço de trabalho](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).

Estes são os benefícios de usar hierarquias em seus espaços de trabalho:

* Organizar o trabalho de uma forma que reflita como suas equipes realmente planejam, operam e entregam.
* Para que os usuários entendam onde estão, como os tipos de registro se conectam e como a estratégia flui para a execução por meio de uma referência a um conjunto de navegações estruturais que indicam seu lugar no sistema.
* Para oferecer uma melhor navegação e criar clareza e continuidade em todos os workflows.
* Para definir fluxos que se encaixem em como sua organização funciona, oferecendo suporte à flexibilidade e consistência em todos os estágios de trabalho.

## Considerações ao trabalhar com hierarquia

* Como um gerenciador de espaço de trabalho, você pode criar várias hierarquias para um espaço de trabalho.
* Se uma conexão entre os tipos de registro selecionados já existir, o sistema reutilizará a conexão existente.
* Se não houver uma conexão, o Workfront criará automaticamente uma como parte da configuração da hierarquia.
* A seguir estão as regras para configuração de hierarquia:
   * Um tipo de registro só pode ter um tipo de registro pai em um determinado espaço de trabalho.

     Por exemplo, um tipo de registro Tático não pode ter um tipo de registro Campanha e Meta como pai no mesmo espaço de trabalho.
   * Um registro pode ser conectado a vários registros pai do mesmo tipo quando você conecta um a muitos ou muitos a muitos tipos de registro.
Por exemplo, a Tática A pode pertencer à Campanha X e à Campanha Y.
   * Um tipo de registro pode se conectar a vários tipos de registros secundários.

     Por exemplo, um tipo de registro de Campanha pode ser o pai de vários outros tipos de registro, como Táticas, Testes e outros tipos de registro.
   * As hierarquias podem incluir tipos de registro do Planning e tipos de objeto do Workfront.

     Por exemplo, você pode ter um tipo de registro de Campanha com Táticas de planejamento e Projetos Workfront como filhos.

     <!--asking if ONLY projects are supported here in slack; if yes, make a note to say that only Projects are supported; also add a note about AEM -->
   * Os tipos de registro global podem aparecer em vários espaços de trabalho dentro de várias hierarquias. <!--not sure if this AFTER they were added to another workspace; right now, I can see only the current workspace when building one??-->
   * Os tipos de objeto do Workfront também podem aparecer em várias hierarquias e em espaços de trabalho diferentes.
   * Os tipos de registro global não podem fazer parte de hierarquias em espaços de trabalho diferentes.

     Por exemplo, se uma Campanha for um tipo de registro global e parte de uma hierarquia no Workspace 1, ela poderá ser adicionada como um tipo de registro existente ao Workspace 2, mas não poderá fazer parte de uma hierarquia lá. <!--verifying that this is not connectable RT and it is about global ones - checking in slack-->
   * Os tipos de registro com conexões que não criam um campo correspondente em seus tipos de registro vinculados também podem fazer parte de hierarquias. Por padrão, as novas conexões criadas durante a configuração da hierarquia sempre criarão um campo correspondente nos tipos de registro vinculados.

## Considerações ao visualizar navegações estruturais

Quando você cria hierarquias entre tipos de registro, elas geram navegações estruturais para os registros que pertencem a esses tipos de registro.

Por exemplo, se você criar uma hierarquia e conectar Campanhas com Táticas com Programas e Projetos, ao navegar para um registro de qualquer um dos tipos conectados na hierarquia, poderá visualizar onde o registro é colocado na hierarquia.

Considere o seguinte:

* Se um tipo de registro fizer parte de várias hierarquias em vários espaços de trabalho, você poderá alternar entre hierarquias a partir da navegação estrutural do registro na página do registro.
* As navegações estruturais funcionam no Workfront e no Planning.

  Por exemplo, ao observar um projeto que está conectado a campanhas e táticas do Planning, e também a portfólios e programas do Workfront, é possível alternar entre as hierarquias do Planning e do Workfront na navegação estrutural.

  Para obter mais informações, consulte [Criar hierarquias do espaço de trabalho](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).


