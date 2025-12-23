---
title: Visão geral da hierarquia e da navegação estrutural
description: Você pode criar várias hierarquias de espaço de trabalho entre os tipos de registro em um espaço de trabalho depois de conectar os tipos de registro.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 98ef4a4f0a30dc90956132cb715393a29170d715
workflow-type: tm+mt
source-wordcount: '1042'
ht-degree: 0%

---



# Visão geral da hierarquia e da navegação estrutural

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Como um gerenciador de espaço de trabalho, você pode definir hierarquias flexíveis mas estruturadas entre tipos de registro conectados e outros tipos de objeto no Adobe Workfront Planning.

As hierarquias são conexões entre tipos de registro ou entre tipos de registro e um projeto do Workfront.

Para obter informações sobre como criar hierarquias, consulte [Criar hierarquias do espaço de trabalho](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).

Estes são os benefícios de usar hierarquias em seus espaços de trabalho:

* Organizar o trabalho de uma forma que reflita como suas equipes realmente planejam, operam e entregam.
* Para que os usuários entendam onde estão, como os tipos de registro se conectam e como a estratégia flui para a execução por meio de uma referência a um conjunto de navegações estruturais que indicam seu lugar no sistema.
* Para oferecer uma melhor navegação e criar clareza e continuidade em todos os workflows.
* Para definir fluxos que se encaixem em como sua organização funciona, oferecendo suporte à flexibilidade e consistência em todos os estágios de trabalho.

## Considerações ao trabalhar com hierarquia

* Você pode criar até 5 hierarquias para um espaço de trabalho.
* É possível ter até quatro tipos de registro e objeto conectados em uma hierarquia.
* Você pode conectar apenas os seguintes tipos de objetos em uma hierarquia de espaço de trabalho:
   * Tipos de registro que pertencem ao espaço de trabalho no qual você está criando as hierarquias.
   * Projetos Workfront. Projetos Workfront não podem ser adicionados como pais de outros tipos de registro. Eles são sempre o último tipo de objeto em uma hierarquia.
* Não é possível adicionar os seguintes tipos de objeto em uma hierarquia:
   * Tipos de registro de outros espaços de trabalho, mesmo quando definidos como conectáveis ou tipos de registro globais. Você pode adicionar tipos de registros globais a hierarquias somente quando eles tiverem sido adicionados ao espaço de trabalho a partir do qual você está construindo a hierarquia.
   * Todos os outros objetos do Workfront.
   * AEM Assets.
* As hierarquias podem incluir tipos de registro do Planning e projetos do Workfront ao mesmo tempo.

  Por exemplo, você pode ter um tipo de registro de Campanha com Táticas de Planejamento e Projetos Workfront como filhos na mesma hierarquia de espaço de trabalho.

* Se uma conexão entre os tipos de registro selecionados já existir, o sistema reutilizará a conexão existente.
* Se não houver uma conexão, o Workfront criará uma como parte da configuração da hierarquia.
* A configuração **Criar campo correspondente no tipo de registro vinculado** deve ser ativada para o campo conectado de registros e tipos de objeto que você deseja incluir em uma hierarquia.
* Não é possível deletar um tipo de registro se ele fizer parte de uma hierarquia.
* Não é possível excluir um campo de conexão se o tipo de registro referenciado no campo fizer parte de uma hierarquia. Você deve primeiro remover o tipo de registro da hierarquia ou excluir a hierarquia antes de poder excluir o tipo de registro.
* Você pode excluir um campo de pesquisa de um tipo de registro conectado. As informações no campo não podem ser recuperadas.
* A seguir estão as regras para configuração de hierarquia:
   * Um tipo de registro só pode ter um tipo de registro pai em um determinado espaço de trabalho.

     Por exemplo, um tipo de registro Tático não pode ter um tipo de registro Campanha e Meta como pai no mesmo espaço de trabalho.
   * Um tipo de registro pode ser o pai em várias hierarquias.

     Por exemplo, você pode ter três hierarquias diferentes em um espaço de trabalho e cada uma delas pode ter Campanhas como seu tipo de registro principal.
   * Um registro pode ser conectado a vários registros pai do mesmo tipo quando você conecta um a muitos ou muitos a muitos tipos de registro.

     Por exemplo, a Tática A pode pertencer à Campanha X e à Campanha Y.
   * Um tipo de registro pode se conectar somente a um tipo de registro filho por vez. Um tipo de registro filho também pode ser pai de outro tipo de registro.

     Por exemplo, um tipo de registro de Campanha pode ser o pai de apenas um outro tipo de registro na mesma hierarquia (Tático), e Tático pode, por sua vez, ser o pai de Programas, que pode ser um pai de Projetos.
   * Um tipo de registro não pode ser pai em uma hierarquia e filho em outra hierarquia no mesmo espaço de trabalho.
   * Os tipos de registro global podem aparecer em vários espaços de trabalho dentro de várias hierarquias, após serem adicionados a esses espaços de trabalho.

     Por exemplo, se uma Campanha for um tipo de registro global e parte de uma hierarquia no Workspace 1, ela poderá ser adicionada como um tipo de registro existente ao Workspace 2 e poderá fazer parte de uma hierarquia lá. Mas ela não pode fazer parte de uma hierarquia no Workspace 2 somente quando designada como um tipo de registro global no Workspace 1, mas não adicionada ao Workspace 2.
   * Quando os tipos de registro conectados fazem parte de hierarquias, você pode conectar um registro de um tipo de registro-filho a até 10 registros de um tipo de registro-pai.

     Por exemplo, se você criar uma hierarquia entre Campanhas como principal e Persona como registro secundário, poderá conectar a mesma persona a até 10 campanhas.

## Considerações ao visualizar navegações estruturais

Quando você cria hierarquias entre tipos de registro, elas geram navegações estruturais para os registros que pertencem a esses tipos de registro.

Por exemplo, se você criar uma hierarquia e conectar Campanhas com Táticas, depois com Atividades e, em seguida, com Projetos, ao navegar para um registro de qualquer um dos tipos conectados na hierarquia, você poderá visualizar onde o registro é colocado na hierarquia.

![Navegação estrutural](assets/breadcrumbs-on-project.png)

Considere o seguinte:

* Se um tipo de registro fizer parte de várias hierarquias, você poderá alternar entre hierarquias a partir da navegação estrutural do registro na página do registro.
* Se o tipo de registro em uma hierarquia tiver vários registros, você poderá selecionar registros na navegação estrutural.
* As navegações estruturais funcionam no Workfront e no Planning.

  Por exemplo, ao observar um projeto que está conectado a campanhas e táticas do Planning, e também a portfólios e programas do Workfront, é possível alternar entre os tipos de objeto do Planning e do Workfront na navegação estrutural.

  Para obter mais informações, consulte [Criar hierarquias do espaço de trabalho](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).
* Ao editar um registro, as alterações ficam visíveis em todos os espaços de trabalho e todas as hierarquias das quais o registro faz parte.


