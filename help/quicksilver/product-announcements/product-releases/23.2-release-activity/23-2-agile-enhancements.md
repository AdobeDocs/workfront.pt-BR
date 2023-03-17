---
title: 23.2 Melhorias no ágil
description: 23.2 Melhorias no ágil
author: Courtney
draft: Probably
feature: Product Announcements
source-git-commit: 938bccf3b3eedf010b7d1db451c365f6097dc64d
workflow-type: tm+mt
source-wordcount: '1032'
ht-degree: 0%

---

# 23.2 Melhorias no ágil

Esta página descreve todas as melhorias ágeis feitas com a versão 23.2 para o ambiente de visualização. Esses aprimoramentos serão disponibilizados no ambiente de Produção com a versão 23.2.

Para obter uma lista de todas as alterações disponíveis neste ponto do ciclo de versão 23.2, consulte [Visão geral da versão 23.2](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

## Funcionalidade de iteração disponível nas Adobe Workfront Boards

Vários novos recursos disponíveis nas Workfront Boards possibilitam o uso da funcionalidade de Scrum ágil. Esses recursos incluem:

* Fluxos de trabalho para agrupar quadros relacionados à mesma equipe e colaborar no trabalho
* Uma lista de cartões ou o backlog do trabalho, com a opção de usar fontes para conectar cartões a tarefas e problemas do Workfront
* Placas de processo de iteração e planejamento de iteração

Observe que as coleções foram renomeadas para fluxos de trabalho. Fluxos de trabalho ajudam você a visualizar dados de diferentes maneiras. Você pode exibir itens em cartões em uma lista, em um quadro ou em uma iteração. Os cartões em uma sequência de trabalho também podem ser compartilhados entre vários quadros. Você pode facilitar facilmente os fluxos de trabalho usando cartões e quadros em uma sequência de trabalho.

Para obter mais informações, consulte [Gerenciar fluxos de trabalho](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md), [Criar uma iteração](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration.md)e [Usar a lista de cartões](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md). Os dois segundos artigos não estarão disponíveis em Principal até que eu publique minha ramificação.

## Adicionar tarefas e problemas aos fluxos de trabalho do Placas a partir de listas e relatórios

Agora é possível adicionar tarefas ou problemas existentes a um fluxo de trabalho nos Workfront Boards diretamente de uma lista ou exibição de relatório. Todos os itens adicionados ao fluxo de trabalho são adicionados à lista de cartões como cartões não planejados.

Para obter mais informações, consulte [Adicionar tarefas ou problemas existentes a um quadro](/help/quicksilver/agile/get-started-with-boards/add-card-from-list-to-board.md).


## Registrar horas em placas conectadas em um quadro

>[!NOTE]
>
>Esse recurso está disponível somente por meio da aceitação antecipada de recursos para as placas Workfront.

Agora você pode registrar horas em cartões conectados, da mesma forma que faria em uma tarefa ou problema. Você deve ter as permissões corretas para a tarefa ou problema para registrar o tempo.

Os campos de registro de tempo não são exibidos nos cartões conectados por padrão. Você deve ativar **Horas** na área Configurar , em Cartões.

Para obter mais informações, consulte [Usar placas conectadas em placas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Adicionar tarefas e problemas aos Workfront Boards a partir de listas e relatórios

Agora é possível adicionar tarefas ou problemas existentes a um quadro do Workfront diretamente de uma lista ou exibição de relatório. Qualquer item adicionado ao quadro se tornará placas conectadas.

Além disso, o campo Quadros agora está disponível para adicionar a listas e relatórios para tarefas ou problemas. Este campo exibe todos os quadros aos quais uma tarefa ou problema foi adicionado.

Para obter mais informações, consulte [Adicionar tarefas ou problemas existentes a um quadro](/help/quicksilver/agile/get-started-with-boards/add-card-from-list-to-board.md).

## Personalizar exibição de campos em um cartão

>[!NOTE]
>
>Esse recurso está disponível somente por meio da aceitação antecipada de recursos para as placas Workfront.


A personalização agora está disponível para configurar quais campos são exibidos em um cartão, tanto na visualização completa quando o cartão está aberto, quanto na visualização condensada do cartão no quadro. Quando você desativa, um campo não é exibido em nenhuma das exibições. Você também pode ativar um campo na visualização completa e ocultá-lo da visualização condensada.

Para obter mais informações, consulte [Personalizar quais campos são exibidos em um cartão](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

[Ver uma demonstração em vídeo deste recurso](https://video.tv.adobe.com/v/3415710/){target=_blank}

## Definir um status padrão para os cartões movidos para uma coluna do quadro

>[!NOTE]
>
>Esse recurso está disponível somente por meio da aceitação antecipada de recursos para as placas Workfront.

Agora é possível definir um status padrão para aplicar aos cartões movidos para uma coluna específica, selecionando um status personalizado e um status do sistema nas políticas de coluna. Quando você move um cartão para a coluna, o Workfront tenta primeiro aplicar o status personalizado (por exemplo, Aguardando feedback). Se o status personalizado não estiver disponível para esse cartão, a Workfront aplicará o status do sistema (por exemplo, Em espera). Além disso, se o status na tarefa ou problema conectado for alterado para o status personalizado ou do sistema definido na política de coluna, o cartão será movido automaticamente para a coluna .

Anteriormente, você era solicitado a selecionar um status para cada cartão movido para a coluna, se vários status estivessem disponíveis.

Para obter mais informações, consulte [Gerenciar colunas](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

[Ver uma demonstração em vídeo deste recurso](https://video.tv.adobe.com/v/3415711/){target=_blank}

## Coleções agora disponíveis nos Adobe Workfront Boards

>[!NOTE]
>
>Esse recurso está disponível somente por meio da aceitação antecipada de recursos para as placas Workfront.

Agora você pode criar coleções no painel de quadros. Uma coleção é um grupo de quadros para colaborar no trabalho. Depois de nomear a coleção, você pode adicionar quadros à coleção usando um conjunto de modelos que oferecem configurações predefinidas, como nomes de colunas. Você também pode mover quadros independentes para uma coleção. Quando um quadro estiver em uma coleção, ele poderá ser movido para outra coleção, mas não poderá se tornar um quadro independente.

Adicionar membros a uma coleção funciona da mesma maneira que adicionar membros a um quadro. Uma pessoa ou equipe deve ser membro da coleção antes de ser adicionada como membros em um quadro da coleção.

Para obter mais informações, consulte [Gerenciar coleções](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

[Ver uma demonstração em vídeo deste recurso](https://video.tv.adobe.com/v/3415609/){target=_blank}

## O campo Estimativa em cartões conectados mapeia para o campo Pontos de história em objetos Workfront

>[!NOTE]
>
>Esse recurso está disponível somente por meio da aceitação antecipada de recursos para as placas Workfront.

O campo Estimation em cartões conectados nos Workfront Boards agora mapeia para o campo Story Points do objeto Workfront associado.

O novo campo Pontos de história é um campo de formulário gratuito editável que pode ser adicionado a uma exibição em uma lista ou relatório para tarefas ou problemas. Não está vinculado a horas planejadas ou atribuições de equipe.

Anteriormente, a estimativa do cartão era uma entrada manual e não era mapeada para nenhum campo em uma tarefa ou problema.

Além disso, o campo Estimation em cartões ad hoc e conectados não tem mais um limite de caracteres. Anteriormente, o número máximo de caracteres era de 99.

Para obter mais informações, consulte [Usar placas conectadas em placas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Visualizar cartão na coluna de entrada

>[!NOTE]
>
>Esse recurso está disponível somente por meio da aceitação antecipada de recursos para as placas Workfront.

Agora você pode clicar em um cartão conectado na coluna de entrada para ver uma versão somente exibição de seu conteúdo. Não é possível editar o conteúdo do cartão até que ele seja movido da coluna de entrada para outra coluna no quadro.
