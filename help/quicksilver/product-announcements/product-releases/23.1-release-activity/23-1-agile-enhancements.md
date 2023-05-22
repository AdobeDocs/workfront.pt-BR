---
title: 23.1 Melhorias na agilidade
description: 23.1 Melhorias na agilidade
author: Courtney
draft: Probably
feature: Product Announcements
exl-id: 4bd041a5-a6e3-4fe3-ae23-45980701e904
source-git-commit: f0e21f9b2846c5665474903a2910ce9f41cdf810
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 0%

---

# 23.1 Melhorias na agilidade

Esta página descreve todas as melhorias de Agile feitas com a versão 23.1 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de Produção na semana de 16 de janeiro de 2023.

Para obter uma lista de todas as alterações disponíveis com a versão 23.1, consulte [Visão geral da versão 23.1](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

## Planejamento de Scrum para painéis do Workfront

Os novos recursos de planejamento de Scrum nas placas Adobe Workfront oferecem opções flexíveis para gerenciar seus processos ágeis. Com essas ferramentas, você pode:

* Rastrear trabalhos em iterações ou sprints
* Usar a velocidade para orientar os compromissos da equipe
* Rastrear burndown e taxa de conclusão

Os recursos de planejamento do Scrum serão um &quot;acompanhamento rápido&quot; após a versão 23.1.

## As datas de vencimento nos cartões são mapeadas para a data de conclusão planejada no objeto do Workfront

>[!NOTE]
>
>Esse recurso está disponível apenas por meio da aceitação antecipada de recursos para placas Workfront.

As datas de vencimento dos cartões conectados nas placas Workfront agora mapeiam para a data de conclusão planejada no objeto Workfront associado. Se você atualizar a data de vencimento em um cartão, a data de conclusão planejada será atualizada na tarefa ou problema. Alterar a data de conclusão planejada também altera a data de vencimento no cartão. Anteriormente, a data de vencimento do cartão era uma entrada manual e não era mapeada para nenhuma data em uma tarefa ou problema.

O mapeamento de datas também se aplica a itens de lista de verificação conectados que são sincronizados com subtarefas.

A data de vencimento em cartões conectados e cartões ad hoc agora também inclui um campo de tempo.

Para obter mais informações, consulte [Usar placas conectadas em placas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

[Exibir uma demonstração em vídeo desse recurso](https://video.tv.adobe.com/v/3411952/){target=_blank}

## Os itens da lista de verificação do painel e as subtarefas do Workfront agora estão vinculados

>[!NOTE]
>
>Esse recurso está disponível apenas por meio da aceitação antecipada de recursos para placas Workfront.

Quando você adiciona um cartão conectado a um quadro para uma tarefa do Workfront, todas as subtarefas são importadas como itens da lista de verificação no cartão. Além disso, ao criar um item de lista de verificação em um cartão conectado, uma subtarefa é adicionada à tarefa do Workfront. Os itens da lista de verificação em problemas não estão conectados a objetos do Workfront.

Anteriormente, os itens da lista de verificação e as subtarefas não eram vinculados. Se quiser incluir uma subtarefa no quadro, você pode importá-la como um cartão conectado separado ou adicionar manualmente um item de lista de verificação a um cartão.

Para obter mais informações, consulte [Usar placas conectadas em placas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) e [Gerenciar itens da lista de verificação em cartões](/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md).

[Exibir uma demonstração em vídeo desse recurso](https://video.tv.adobe.com/v/3411951/){target=_blank}

## Contador de cartões em colunas a bordo

>[!NOTE]
>
>Esse recurso está disponível apenas por meio da aceitação antecipada de recursos para placas Workfront.

Uma nova definição de configuração está disponível para ativar um contador de cartão para todas as colunas em uma placa. Se você estiver usando o limite de WIP em uma coluna, não será adicionado um contador de placa separado.

Para obter mais informações, consulte [Gerenciar colunas do quadro](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

## Pesquisar e classificar no painel de painéis

>[!NOTE]
>
>Esse recurso está disponível apenas por meio da aceitação antecipada de recursos para placas Workfront.

Agora é possível classificar o painel de painéis de discussão por nome ou data do painel de discussão e pesquisar por um painel de discussão específico na lista.

Para obter mais informações, consulte [Usar o painel de painéis](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md).

## Status exibido no cartão

>[!NOTE]
>
>Esse recurso está disponível apenas por meio da aceitação antecipada de recursos para placas Workfront.

Se um cartão em um quadro receber um status, o status agora é exibido no cartão para que você não precise abrir o cartão para ver o status. Esse aprimoramento se aplica a placas ad hoc e conectadas.

Para obter mais informações, consulte [Usar placas conectadas em placas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) e [Adicionar um cartão ad hoc a um quadro](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

![status no cartão](/help/quicksilver/product-announcements/product-releases/assets/boards-connected-card-details-110922.png)

## Cartões vinculáveis agora disponíveis em quadros

>[!NOTE]
>
>Esse recurso está disponível apenas por meio da aceitação antecipada de recursos para placas Workfront.

Agora é possível enviar um link para um cartão específico para outro usuário do boards. A pessoa deve ter acesso para visualizar o quadro antes de abrir o link.

Ao abrir um cartão em um quadro, o URL do navegador é semelhante a:

```
https://<Workfront-URL>/boards/<board-id>/card/<card-id>. 
```

Você pode copiar o URL completo e enviá-lo para outra pessoa. Eles irão diretamente para o cartão aberto quando acessarem o link.

Anteriormente, os links estavam disponíveis para placas, mas não para placas específicas.

Para obter informações sobre cartões, consulte [Adicionar um cartão ad hoc a um quadro](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md) e [Usar placas conectadas em placas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Filtrar por conexão em quadros

>[!NOTE]
>
>Esse recurso está disponível apenas por meio da aceitação antecipada de recursos para placas Workfront.

A lista de filtros em um quadro agora inclui a opção de filtrar por conexão, que mostra todos os cartões conectados de um projeto específico. Também é possível filtrar por cartões que não estejam conectados.

Para obter mais informações, consulte [Filtrar e pesquisar em um quadro](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

[Exibir uma demonstração em vídeo desse recurso](https://video.tv.adobe.com/v/3412381/){target=_blank}

## Arquivar cartões de um quadro em uma programação

>[!NOTE]
>
>Esse recurso está disponível apenas por meio da aceitação antecipada de recursos para placas Workfront.

Você pode configurar uma placa para que as placas sejam arquivadas, ou &quot;cair&quot; da placa, de acordo com uma programação. As opções estão disponíveis para definir cartões em uma coluna específica para arquivar em um determinado número de dias ou semanas. Por exemplo, você pode definir a queda para que os cartões em uma coluna Concluído sejam arquivados depois de estarem na coluna por duas semanas.

Se quiser exibir os cartões novamente depois que eles caírem do quadro, você pode definir o filtro de quadro para exibir cartões arquivados.

Para obter mais informações, consulte [Configurar queda de cartão](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md).

[Exibir uma demonstração em vídeo desse recurso](https://video.tv.adobe.com/v/3412323/){target=_blank}
