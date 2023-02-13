---
content-type: overview
product-area: documents
navigation-topic: proofing-overview
title: Visão geral do fluxo de trabalho automatizado
description: Os fluxos de trabalho automatizados permitem criar uma série de estágios de análise sequencial ou paralela, estabelecer dependências entre esses estágios e limitar sua visibilidade a determinados usuários. Se houver estágios interdependentes em seu processo de revisão, os fluxos de trabalho automatizados moverão sua prova pelos estágios automaticamente, notificando os revisores e aprovadores relevantes ao longo do caminho. Para obter informações sobre como configurar um fluxo de trabalho automatizado, consulte Criar uma prova avançada com um fluxo de trabalho automatizado.
author: Courtney
feature: Digital Content and Documents
exl-id: d643970a-c00c-4fb4-94bc-fca4e090dcc9
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 0%

---

# Visão geral do fluxo de trabalho automatizado

Os fluxos de trabalho automatizados permitem criar uma série de estágios de análise sequencial ou paralela, estabelecer dependências entre esses estágios e limitar sua visibilidade a determinados usuários. Se houver estágios interdependentes em seu processo de revisão, os fluxos de trabalho automatizados moverão sua prova pelos estágios automaticamente, notificando os revisores e aprovadores relevantes ao longo do caminho. Para obter informações sobre como configurar um Fluxo de Trabalho Automatizado, consulte [Criar uma prova avançada com um fluxo de trabalho Automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

**Exemplos:**  Os fluxos de trabalho automatizados ajudam você a gerenciar processos de revisão de prova complexos, como

* Quando diferentes grupos ou revisores precisarem revisar o conteúdo em uma ordem específica
* Quando há dependências entre a atividade dos usuários enquanto eles revisam o conteúdo
* Quando o conteúdo é revisado regularmente pelos mesmos grupos de pessoas
* Quando você deseja controlar o período em que os revisores analisam o conteúdo
* Quando quiser manter alguma atividade de revisão privada

## Estágios

Para cada estágio do Fluxo de trabalho automatizado, você pode definir configurações, como um prazo para o palco, um bloqueio em um palco, um revisor definido como o decisor do palco e uma configuração de privacidade que permite que apenas determinadas pessoas vejam comentários do revisor no palco.

Os estágios podem ser ativados manualmente, na criação da prova, após atingir um prazo, em uma data e hora específica ou quando uma decisão é tomada no estágio principal.

Os estágios podem ser bloqueados manualmente, bem como quando o próximo estágio começa ou quando todas as decisões são tomadas no palco. Você também pode optar por nunca bloquear um palco.

Você pode nomear um decisor principal para um estágio. A decisão desta pessoa torna desnecessárias todas as outras decisões para o palco.

Da mesma forma, você pode optar por exigir apenas uma decisão para um estágio. Ao fazer isso, o processo de revisão do palco é marcado como concluído depois que qualquer um dos recipients tomar a decisão no palco.

Você pode ter todos os revisores notificados sobre o convite para revisar o conteúdo quando o processo de revisão começar, ou pode ter cada revisor notificado somente quando seu estágio for ativado.

## Estágios privados

Por padrão, os comentários deixados pelos revisores em todos os estágios ficam visíveis para todos que estão revisando o conteúdo e recebendo notificações por email e resumos de comentários sobre o processo de revisão.

Se quiser impedir que determinados grupos de revisores vejam os comentários de outros revisores, é possível criar estágios privados.

Estágios privados são visíveis apenas para revisores adicionados a esses estágios. Eles também ficam visíveis para usuários que têm direitos de edição na prova ou direitos de edição em todos os itens criados na conta do Adobe Workfront de sua organização (supervisor e superior ou usuários com perfis personalizados para os quais a edição de informações de outras pessoas está ativada).

Comentários adicionados por participantes do estágio privado não são incluídos em notificações por email e resumos de comentários de prova solicitados por qualquer pessoa que não tenha os direitos de exibi-los.

## Diagrama de fluxo de trabalho

O Diagrama de Fluxo de Trabalho é uma representação visual do processo de revisão da prova. Ele mostra a ordem dos estágios e quaisquer dependências entre os estágios à medida que você cria ou exibe os detalhes de uma prova. Qualquer estágio privado é exibido com um símbolo de chave.

![intro-to-aw-example-diagrama.png](assets/intro-to-aw-example-diagram-350x199.png)

Em provas ao vivo, as dependências de palco são exibidas com uma linha cinza tracejada para palcos inativos ou uma linha preta sólida para palcos ativos. As etapas são exibidas em verde se o processo de aprovação foi concluído dentro do prazo especificado. As etapas que se aproximam de seus prazos são exibidas em laranja e os estágios passados de seu prazo são exibidos em vermelho.

![workflow_2.png](assets/workflow-2-350x183.png)

## Templates de workflows automatizados

Se sua organização usar o mesmo processo de revisão para várias provas, o administrador do Workfront poderá criar modelos de Fluxo de trabalho automatizado para facilitar muito a criação da prova. Você pode escolher um modelo de Fluxo de trabalho automatizado enquanto configura uma prova para adicionar os estágios e revisores nesse modelo à prova. Você pode modificar o template aplicado à prova conforme necessário antes e depois de criar a prova.

O administrador do Workfront pode criar um número ilimitado de modelos de acordo com as necessidades da sua empresa.

Para saber mais sobre como criar, usar e gerenciar modelos, consulte o administrador do Workfront.
