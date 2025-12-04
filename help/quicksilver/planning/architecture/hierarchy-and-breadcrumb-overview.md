---
title: Visão geral da hierarquia e da navegação estrutural
description: Você pode criar várias hierarquias de espaço de trabalho entre os tipos de registro em um espaço de trabalho.
hide: true
hidefromtoc: true
source-git-commit: f345cc0d41dc1bd62e7361fa0755cb7ba72465a0
workflow-type: tm+mt
source-wordcount: '405'
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

Estes são os benefícios de usar hierarquias em seus espaços de trabalho:

* Organizar o trabalho de uma forma que reflita como suas equipes realmente planejam, operam e entregam.
* Os usuários entendem onde estão, como os tipos de registro se conectam e como a estratégia flui para a execução ao se referir a um conjunto de navegações estruturais que indicam seu lugar no sistema.
* Ofereça uma navegação melhor e crie clareza e continuidade em todos os workflows.
* As hierarquias não impõem uma estrutura rígida definida pelo sistema e, em vez disso, permitem definir fluxos que se ajustem ao funcionamento da organização, oferecendo suporte à flexibilidade e consistência em todos os estágios de trabalho.

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
   * Os tipos de registro global podem aparecer em vários espaços de trabalho dentro de várias hierarquias.
   * Os tipos de objeto do Workfront também podem aparecer em várias hierarquias e em espaços de trabalho diferentes.
     <!--Not sure what this means: * Shared record can't be part of hierarchies.-->
   * Os tipos de registro com conexões que não criam um campo correspondente em seus tipos de registro vinculados também podem fazer parte de hierarquias. Por padrão, as novas conexões criadas durante a configuração da hierarquia sempre criarão um campo correspondente nos tipos de registro vinculados.

## Considerações ao visualizar navegações estruturais


