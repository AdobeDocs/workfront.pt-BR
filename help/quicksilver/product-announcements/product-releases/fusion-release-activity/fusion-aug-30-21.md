---
title: 'Atividade de lançamento do Workfront Fusion: &nbsp;Semana de 30 de agosto de 2021'
description: 'Atividade de lançamento do Workfront Fusion: &nbsp;Semana de 30 de agosto de 2021'
author: Luke
draft: Probably
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: 988349f9-aa12-4017-9032-be4d0078959e
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# Atividade de lançamento do Workfront Fusion: semana de 30 de agosto de 2021

Esta página descreve todas as melhorias feitas no Adobe Workfront Fusion na semana de 30 de agosto de 2021.

Para obter uma lista de todas as alterações recentes, consulte [Atividade de lançamento do Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Para obter uma lista de correções de erros recentes no Workfront Fusion, consulte o [Atualizações de manutenção do Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) e verificar se há atualizações rotuladas como Atualização de manutenção do Workfront Fusion.

## Filtrar eventos que acionam o módulo Workfront > Eventos de observação

1. Configure um filtro personalizado para eventos que acionam o módulo Workfront > Eventos de observação

   Para reduzir o número de execuções de cenários desnecessários, atualizamos o módulo Workfront > Registros de observação para ativar a filtragem de eventos. Agora, você pode definir um filtro ao criar um webhook. Isso permite que o cenário seja acionado somente quando o evento atender a determinados critérios.

   Atualmente, o filtro de eventos oferece as seguintes operações:

   * Igual: acione um cenário somente quando um evento corresponder às condições do filtro. Por exemplo, você pode configurar um filtro que aciona um cenário somente se o evento ocorrer em um projeto específico.
   * Diferente: acione um cenário somente se um evento não corresponder às condições do filtro. Por exemplo, você pode criar um filtro que aciona um cenário somente se o problema em que um evento ocorre não tiver um status Fechado.

   Anteriormente, o módulo Observar registros recuperava todos os registros. Os usuários só podem filtrar configurando filtros posteriormente no cenário.

   Para aproveitar a filtragem de eventos, crie um novo webhook no módulo Observar eventos. No momento, não é possível editar webhooks existentes para incluir essa funcionalidade. É altamente recomendável criar novos webhooks usando filtros de evento para seus cenários existentes.

1. Filtrar eventos acionados pela conexão atual.

   Para facilitar a configuração dos webhooks no módulo Workfront > Eventos de observação, incluímos o filtro de eventos mais comum. Agora, o webhook tem uma opção para filtrar todas as alterações feitas pelos módulos usando a conexão especificada para o módulo Observar eventos. Em outras palavras, com esse filtro ativado, qualquer alteração feita pelo usuário do Workfront associado a essa conexão não poderá acionar o cenário.

   Anteriormente, esse filtro não estava disponível. Portanto, foi mais fácil para as alterações feitas nos módulos do Workfront acionarem cenários que contêm esses módulos, potencialmente fazendo com que os cenários se acionassem em um loop infinito.

Para obter mais informações sobre filtros de evento no módulo Workfront > Eventos de observação, consulte [Módulos do Adobe Workfront](../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

