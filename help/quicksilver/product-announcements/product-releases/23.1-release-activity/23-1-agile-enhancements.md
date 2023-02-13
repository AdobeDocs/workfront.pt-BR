---
title: 23.1 Melhorias no ágil
description: 23.1 Melhorias no ágil
author: Courtney
draft: Probably
feature: Product Announcements
exl-id: 4bd041a5-a6e3-4fe3-ae23-45980701e904
source-git-commit: f0e21f9b2846c5665474903a2910ce9f41cdf810
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 0%

---

# 23.1 Melhorias no ágil

Esta página descreve todas as melhorias do Agile feitas com a versão 23.1 para o ambiente de visualização. Esses aprimoramentos serão disponibilizados no ambiente de Produção na semana de 16 de janeiro de 2023.

Para obter uma lista de todas as alterações disponíveis com a versão 23.1, consulte [Visão geral da versão 23.1](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

## Planejamento de Scrum para Workfront Boards

Os novos recursos de planejamento do Scrum nas Adobe Workfront Boards oferecem opções flexíveis para gerenciar seus processos ágeis. Com essas ferramentas, você pode:

* Rastrear trabalhos em iterações ou impressões
* Use a velocidade para orientar os compromissos da equipe
* Rastrear o detalhamento e a taxa de conclusão

Os recursos de planejamento do Scrum serão um &quot;seguimento rápido&quot; após a versão 23.1.

## As datas de vencimento nos cartões são mapeadas para a data de conclusão planejada no objeto Workfront

>[!NOTE]
>
>Esse recurso está disponível somente por meio da aceitação antecipada de recursos para as placas Workfront.

As datas de vencimento das placas conectadas nas placas Workfront agora são mapeadas para a data de conclusão planejada no objeto Workfront associado. Se você atualizar a data de vencimento em um cartão, a data de conclusão planejada será atualizada na tarefa ou problema. Alterar a data de conclusão planejada também altera a data de vencimento no cartão. Anteriormente, a data de vencimento do cartão era uma entrada manual e não era mapeada para qualquer data em uma tarefa ou problema.

O mapeamento de data também se aplica a itens da lista de verificação conectados que são sincronizados com subtarefas.

A data de vencimento nos cartões conectados e nos cartões ad hoc agora também inclui um campo de hora.

Para obter mais informações, consulte [Usar placas conectadas em placas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

[Ver uma demonstração em vídeo deste recurso](https://video.tv.adobe.com/v/3411952/){target=_blank}

## Os itens da lista de verificação do quadro e as subtarefas do Workfront agora estão vinculados

>[!NOTE]
>
>Esse recurso está disponível somente por meio da aceitação antecipada de recursos para as placas Workfront.

Quando você adiciona um cartão conectado a um quadro para uma tarefa do Workfront, qualquer subtarefa é importada como itens de lista de verificação no cartão. Além disso, ao criar um item de lista de verificação em um cartão conectado, uma subtarefa é adicionada à tarefa do Workfront. Os itens da lista de verificação em problemas não estão conectados a nenhum objeto Workfront.

Anteriormente, os itens da lista de verificação e as subtarefas não eram vinculadas. Se quiser incluir uma subtarefa no quadro, você poderá importá-la como um cartão conectado separado ou adicionar manualmente um item de lista de verificação a um cartão.

Para obter mais informações, consulte [Usar placas conectadas em placas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) e [Gerenciar itens da lista de verificação em cartões](/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md).

[Ver uma demonstração em vídeo deste recurso](https://video.tv.adobe.com/v/3411951/){target=_blank}

## Contador de cartão em colunas de quadro

>[!NOTE]
>
>Esse recurso está disponível somente por meio da aceitação antecipada de recursos para as placas Workfront.

Uma nova configuração está disponível para ativar um contador de cartão para todas as colunas em um quadro. Se você estiver usando o limite WIP em uma coluna, um contador de cartão separado não será adicionado.

Para obter mais informações, consulte [Gerenciar colunas do quadro](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

## Pesquisar e classificar no painel de quadros

>[!NOTE]
>
>Esse recurso está disponível somente por meio da aceitação antecipada de recursos para as placas Workfront.

Agora é possível classificar o painel de quadros por nome ou data do quadro e procurar um quadro específico na lista.

Para obter mais informações, consulte [Usar o painel de quadros](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md).

## Status é exibido no cartão

>[!NOTE]
>
>Esse recurso está disponível somente por meio da aceitação antecipada de recursos para as placas Workfront.

Se um cartão em um quadro tiver um status atribuído, o status agora será exibido no cartão para que você não tenha que abrir o cartão para ver o status. Esse aprimoramento se aplica a cartões ad hoc e conectados.

Para obter mais informações, consulte [Usar placas conectadas em placas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) e [Adicionar um cartão ad hoc a um quadro](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

![status no cartão](/help/quicksilver/product-announcements/product-releases/assets/boards-connected-card-details-110922.png)

## Placas vinculáveis agora disponíveis em quadros

>[!NOTE]
>
>Esse recurso está disponível somente por meio da aceitação antecipada de recursos para as placas Workfront.

Agora você pode enviar um link para um cartão específico para outro usuário do boards. A pessoa deve ter acesso para visualizar o quadro antes de poder abrir o link.

Quando você abre um cartão em um quadro, o URL do navegador tem esta aparência:

```
https://<Workfront-URL>/boards/<board-id>/card/<card-id>. 
```

Você pode copiar o URL completo e enviá-lo para outra pessoa. Eles irão diretamente para o cartão aberto quando acessarem o link.

Anteriormente, os links estavam disponíveis para quadros, mas não para cartões específicos.

Para obter informações sobre cartões, consulte [Adicionar um cartão ad hoc a um quadro](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md) e [Usar placas conectadas em placas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Filtrar por conexão nos quadros

>[!NOTE]
>
>Esse recurso está disponível somente por meio da aceitação antecipada de recursos para as placas Workfront.

A lista de filtros em um quadro agora inclui a opção para filtrar por conexão, que mostra todos os cartões conectados para um projeto específico. Também é possível filtrar por cartões que não estão conectados.

Para obter mais informações, consulte [Filtrar e pesquisar em um quadro](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

[Ver uma demonstração em vídeo deste recurso](https://video.tv.adobe.com/v/3412381/){target=_blank}

## Arquivar cartões de um quadro de acordo com uma programação

>[!NOTE]
>
>Esse recurso está disponível somente por meio da aceitação antecipada de recursos para as placas Workfront.

Você pode configurar um quadro de forma que os cartões sejam arquivados, ou &quot;desistam&quot; do quadro, de acordo com uma programação. As opções estão disponíveis para definir cartões em uma coluna específica para arquivar em um determinado número de dias ou semanas. Por exemplo, você pode definir a falloff para que os cartões em uma coluna Complete sejam arquivados depois de ficarem na coluna por duas semanas.

Se quiser exibir os cartões novamente depois que eles saírem do quadro, você pode definir o filtro de quadro para exibir os cartões arquivados.

Para obter mais informações, consulte [Configurar fallout de cartão](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md).

[Ver uma demonstração em vídeo deste recurso](https://video.tv.adobe.com/v/3412323/){target=_blank}
