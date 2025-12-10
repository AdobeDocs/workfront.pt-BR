---
title: Visão geral da hierarquia e da navegação estrutural
description: Você pode criar várias hierarquias de espaço de trabalho entre os tipos de registro em um espaço de trabalho.
hide: true
hidefromtoc: true
source-git-commit: 3d0a6932bda338af1e6b3dcba49bfc0ac486d919
workflow-type: tm+mt
source-wordcount: '746'
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

As hierarquias são conexões entre tipos de registro ou entre tipos de registro e um projeto do Workfront.

Para obter informações sobre como criar hierarquias, consulte [Criar hierarquias do espaço de trabalho](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).

Estes são os benefícios de usar hierarquias em seus espaços de trabalho:

* Organizar o trabalho de uma forma que reflita como suas equipes realmente planejam, operam e entregam.
* Para que os usuários entendam onde estão, como os tipos de registro se conectam e como a estratégia flui para a execução por meio de uma referência a um conjunto de navegações estruturais que indicam seu lugar no sistema.
* Para oferecer uma melhor navegação e criar clareza e continuidade em todos os workflows.
* Para definir fluxos que se encaixem em como sua organização funciona, oferecendo suporte à flexibilidade e consistência em todos os estágios de trabalho.

## Considerações ao trabalhar com hierarquia

* Você pode criar várias hierarquias para um espaço de trabalho.
* É possível ter até quatro tipos de registro e objeto conectados em uma hierarquia.
* Você pode conectar apenas os seguintes tipos de objetos em uma hierarquia de espaço de trabalho:
   * Tipos de registro que pertencem ao espaço de trabalho no qual você está criando as hierarquias.
   * Projetos Workfront.
* Não é possível adicionar os seguintes tipos de objeto em uma hierarquia:
   * Tipos de registro de outros espaços de trabalho, mesmo quando definidos como conectáveis ou tipos de registro globais.
   * Todos os outros objetos do Workfront.
   * AEM Assets
* As hierarquias podem incluir tipos de registro do Planning e tipos de objeto do Workfront ao mesmo tempo.

      Por exemplo, você pode ter um tipo de registro de Campanha com Táticas de Planejamento e Projetos Workfront como filhos na mesma hierarquia de espaço de trabalho.
  * Se uma conexão entre os tipos de registro selecionados já existir, o sistema reutilizará a conexão existente.
* Se não houver uma conexão, o Workfront criará uma como parte da configuração da hierarquia.
* A configuração **Criar campo correspondente no tipo de registro vinculado** deve ser ativada para o campo conectado.

  Os tipos de registro com conexões que não criam um campo correspondente em seus tipos de registro vinculados também podem fazer parte de hierarquias, mas quando você cria uma nova conexão durante a configuração da hierarquia, sempre terá que criar um campo correspondente no tipo de registro vinculado.
* A seguir estão as regras para configuração de hierarquia:
   * Um tipo de registro só pode ter um tipo de registro pai em um determinado espaço de trabalho.

     Por exemplo, um tipo de registro Tático não pode ter um tipo de registro Campanha e Meta como pai no mesmo espaço de trabalho.
   * Um tipo de registro pode ser o pai em várias hierarquias.

     Por exemplo, você pode ter três hierarquias diferentes em um espaço de trabalho e cada uma delas pode ter Campanhas como seu tipo de registro principal.
   * Um registro pode ser conectado a vários registros pai do mesmo tipo quando você conecta um a muitos ou muitos a muitos tipos de registro.
Por exemplo, a Tática A pode pertencer à Campanha X e à Campanha Y.
   * Um tipo de registro pode se conectar a vários tipos de registros secundários.

     Por exemplo, um tipo de registro de Campanha pode ser o pai de vários outros tipos de registro, como Táticas, Testes e outros tipos de registro.
   * Os tipos de registro global podem aparecer em vários espaços de trabalho dentro de várias hierarquias, após serem adicionados a esses espaços de trabalho.

     Por exemplo, se uma Campanha for um tipo de registro global e parte de uma hierarquia no Workspace 1, ela poderá ser adicionada como um tipo de registro existente ao Workspace 2 e poderá fazer parte de uma hierarquia lá. Mas ela não pode fazer parte de uma hierarquia no Workspace 2 somente quando designada como um tipo de registro global no Workspace 1, mas não adicionada ao Workspace 2.


## Considerações ao visualizar navegações estruturais

Quando você cria hierarquias entre tipos de registro, elas geram navegações estruturais para os registros que pertencem a esses tipos de registro.

Por exemplo, se você criar uma hierarquia e conectar Campanhas com Táticas, depois com Programas e, em seguida, com Projetos, ao navegar para um registro de qualquer um dos tipos conectados na hierarquia, você poderá visualizar onde o registro é colocado na hierarquia.

Considere o seguinte:

* Se um tipo de registro fizer parte de várias hierarquias, você poderá alternar entre hierarquias a partir da navegação estrutural do registro na página do registro.
* As navegações estruturais funcionam no Workfront e no Planning.

  Por exemplo, ao observar um projeto que está conectado a campanhas e táticas do Planning, e também a portfólios e programas do Workfront, é possível alternar entre os tipos de objeto do Planning e do Workfront na navegação estrutural.

  Para obter mais informações, consulte [Criar hierarquias do espaço de trabalho](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).


