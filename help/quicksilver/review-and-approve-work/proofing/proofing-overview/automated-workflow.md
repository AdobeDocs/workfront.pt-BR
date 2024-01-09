---
content-type: overview
product-area: documents
navigation-topic: proofing-overview
title: Visão geral do fluxo de trabalho automatizado
description: Os fluxos de trabalho automatizados permitem criar uma série de estágios de revisão sequenciais ou paralelos, estabelecer dependências entre esses estágios e limitar sua visibilidade a determinados usuários. Se houver estágios interdependentes no processo de revisão, os Fluxos de trabalho automatizados movem a prova pelos estágios automaticamente, notificando os revisores e aprovadores relevantes ao longo do caminho.
author: Courtney
feature: Digital Content and Documents
exl-id: d643970a-c00c-4fb4-94bc-fca4e090dcc9
source-git-commit: 1fd3b135682c096f1715e5da0455fed12e882582
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 0%

---

# Visão geral do fluxo de trabalho automatizado

<!-- Audited: 01/2024 -->

Os fluxos de trabalho automatizados permitem criar uma série de estágios de revisão sequenciais ou paralelos, estabelecer dependências entre esses estágios e limitar sua visibilidade a determinados usuários. Se houver estágios interdependentes no processo de revisão, os Fluxos de trabalho automatizados movem a prova pelos estágios automaticamente, notificando os revisores e aprovadores relevantes ao longo do caminho. Para obter informações sobre como configurar um fluxo de trabalho automatizado, consulte [Criar uma prova avançada com um fluxo de trabalho automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

**Exemplos:**  Os fluxos de trabalho automatizados ajudam você a gerenciar processos complexos de revisão de prova, como:

* Quando diferentes grupos ou revisores precisam revisar o conteúdo em uma ordem específica
* Quando há dependências entre a atividade dos usuários enquanto eles revisam o conteúdo
* Quando o conteúdo é revisado regularmente pelos mesmos grupos de pessoas
* Quando quiser controlar o período no qual os revisores visualizam o conteúdo
* Quando quiser manter algumas atividades de revisão privadas

## Estágios

Para cada estágio do Fluxo de trabalho automatizado, é possível definir configurações, como um prazo para o estágio, um bloqueio em um estágio, um revisor definido como o tomador de decisão para o estágio e uma configuração de privacidade que permite que apenas determinadas pessoas vejam os comentários do revisor no estágio.

Os estágios podem ser ativados manualmente, na criação da prova, ao atingir um prazo, em uma data e hora específicas ou quando uma decisão é tomada no estágio principal.

Os estágios podem ser bloqueados manualmente, bem como quando o próximo estágio é iniciado ou quando todas as decisões são tomadas no estágio. Você também pode optar por nunca bloquear um estágio.

Você pode indicar um tomador de decisão principal para um estágio. A decisão dessa pessoa torna todas as outras decisões do estágio desnecessárias.

Da mesma forma, é possível optar por exigir apenas uma decisão para um estágio. Ao fazer isso, o processo de revisão do estágio é marcado como concluído depois que qualquer um dos recipients toma sua decisão no estágio.

É possível notificar todos os revisores sobre o convite para revisar o conteúdo quando o processo de revisão começar, ou notificar cada revisor somente quando o estágio for ativado.

## Estágios privados

Por padrão, os comentários deixados pelos revisores em todos os estágios ficam visíveis para todos que estão revisando o conteúdo e recebendo notificações por email e resumos de comentários sobre o processo de revisão.

Se você quiser impedir que determinados grupos de revisores vejam os comentários de outros revisores, é possível criar estágios privados.

Os estágios privados só são visíveis para revisores adicionados a esses estágios. Eles também estão visíveis para usuários que têm direitos de edição na prova ou direitos de edição em todos os itens criados na conta da Adobe Workfront da sua organização (Supervisor e superior, ou usuários com perfis personalizados para os quais a edição de informações de outras pessoas está habilitada).

Comentários adicionados por participantes privados do estágio não são incluídos nas notificações por email e nos resumos de comentários de prova solicitados por qualquer pessoa que não tenha os direitos para visualizá-los.

## Diagrama de Fluxo de Trabalho

O diagrama de fluxo de trabalho é uma representação visual do processo de revisão da prova. Ela mostra a ordem dos estágios e todas as dependências entre estágios à medida que você cria ou exibe os detalhes de uma prova. Todos os estágios privados são exibidos com um símbolo de chave.

![intro-to-aw-example-chart.png](assets/intro-to-aw-example-diagram-350x199.png)

Nas provas em tempo real, as dependências de estágio são exibidas com uma linha cinza tracejada para estágios inativos ou uma linha preta sólida para estágios ativos. Os estágios são exibidos em verde se o processo de aprovação foi concluído dentro do prazo especificado. As etapas que se aproximam de seus prazos são exibidas em laranja e as etapas que ultrapassam seus prazos são exibidas em vermelho.

![workflow_2.png](assets/workflow-2-350x183.png)

## Modelos automatizados de fluxo de trabalho

Se sua organização usar o mesmo processo de revisão para várias provas, o administrador do Workfront poderá criar modelos de fluxo de trabalho automatizado para facilitar bastante a criação de provas. Você pode escolher um modelo de Fluxo de trabalho automatizado ao configurar uma prova para adicionar os estágios e revisores nesse modelo à prova. Você pode modificar o modelo aplicado à prova conforme necessário antes e depois de criar a prova.

O administrador do Workfront pode criar um número ilimitado de modelos de acordo com as necessidades da empresa.

Para saber mais sobre como criar, usar e gerenciar modelos, consulte o administrador do Workfront.
