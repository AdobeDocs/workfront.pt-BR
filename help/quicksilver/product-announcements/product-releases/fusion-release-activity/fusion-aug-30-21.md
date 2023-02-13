---
title: 'Atividade de lançamento do Workfront Fusion: &nbsp;Semana de 30 de agosto de 2021'
description: 'Atividade de lançamento do Workfront Fusion: &nbsp;Semana de 30 de agosto de 2021'
author: Luke
draft: Probably
feature: Product Announcements, Workfront Fusion
exl-id: 988349f9-aa12-4017-9032-be4d0078959e
hidefromtoc: true
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# Atividade de lançamento do Workfront Fusion: semana de 30 de agosto de 2021

Esta página descreve todas as melhorias feitas no Adobe Workfront Fusion na semana de 30 de agosto de 2021.

Para obter uma lista de todas as alterações recentes, consulte [Atividade de versão do Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Para obter uma lista de correções de erros recentes no Workfront Fusion, consulte o [Atualizações de manutenção do Workfront](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350) e verifique se há atualizações rotuladas como Atualização de manutenção do Workfront Fusion.

## Filtrar eventos que acionam o módulo Workfront > Eventos de observação

1. Configurar um filtro personalizado para eventos que acionam o módulo Workfront > Eventos de observação

   Para reduzir o número de execuções desnecessárias de cenário, atualizamos o módulo de registros Workfront > Watch para ativar a filtragem de eventos. Agora, você pode definir um filtro ao criar um webhook. Isso permite que o cenário seja acionado somente quando o evento atender a determinados critérios.

   No momento, o filtro de eventos oferece as seguintes operações:

   * Igual: Acione um cenário somente quando um evento corresponder às condições do filtro. Por exemplo, você pode configurar um filtro que acione um cenário somente se o evento ocorrer em um projeto específico.
   * Diferente de: Acione um cenário somente se um evento não corresponder às condições do filtro. Por exemplo, você pode criar um filtro que acione um cenário somente se o problema em que um evento ocorre não tiver um status de Fechado.

   Anteriormente, o módulo de registros Watch recuperava todos os registros. Os usuários podem filtrar somente ao configurar filtros posteriormente no cenário.

   Para aproveitar ao máximo a filtragem de eventos, crie um novo webhook no módulo de eventos Watch. No momento, não é possível editar webhooks existentes para incluir essa funcionalidade. Recomendamos que você crie novos webhooks usando filtros de evento para seus cenários existentes.

1. Filtre os eventos acionados pela conexão atual.

   Para facilitar a configuração dos seus webhooks no módulo Workfront > Watch events , incluímos o filtro de eventos mais comum. Agora, o webhook tem uma opção para filtrar todas as alterações feitas pelos módulos usando a conexão especificada para o módulo de eventos Watch. Em outras palavras, com esse filtro ativado, qualquer alteração feita pelo usuário do Workfront associado a essa conexão não pode acionar o cenário.

   Anteriormente, esse filtro não estava disponível. Portanto, era mais fácil que as alterações feitas nos módulos Workfront acionassem cenários contendo esses módulos, possivelmente fazendo com que cenários se acionassem em um loop infinito.

Para obter mais informações sobre filtros de evento no módulo Workfront > Eventos de monitoramento , consulte [Módulos Adobe Workfront](../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

