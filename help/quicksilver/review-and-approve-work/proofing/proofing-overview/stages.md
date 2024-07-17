---
content-type: overview
product-area: documents
navigation-topic: proofing-overview
title: Visão geral dos estágios de fluxo de trabalho automatizado
description: Estágios de prova são segmentos de tempo nos quais diferentes usuários analisam uma prova. À medida que a prova avança de um estágio para o próximo, o Adobe Workfront notifica os revisores para avisá-los quando chegar a hora de trabalhar nele.
author: Courtney
feature: Digital Content and Documents
exl-id: a03d2cf2-edb3-43b7-a739-32600f2ae2a0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

# Visão geral dos estágios de fluxo de trabalho automatizado

Estágios de prova são segmentos de tempo nos quais diferentes usuários analisam uma prova. À medida que a prova avança de um estágio para o próximo, o Adobe Workfront notifica os revisores para avisá-los quando chegar a hora de trabalhar nele.

![diagrama_de_estágios.png](assets/stages-diagram-350x63.png)

Os estágios ocorrem em duas situações diferentes:

* [Criar uma prova com um fluxo de trabalho automatizado](#create-a-proof-with-an-automated-workflow)
* [Atribuir prazos para diferentes revisores em uma prova](#assign-deadlines-for-different-reviewers-on-a-proof)

## Criar uma prova com um fluxo de trabalho automatizado {#create-a-proof-with-an-automated-workflow}

Ao adicionar um fluxo de trabalho automatizado a uma prova, você configura os estágios do trabalho de revisão que deseja ocorrer.

Ao configurar estágios para uma prova com um fluxo de trabalho automático:

* Você pode configurar os estágios para serem executados consecutiva ou simultaneamente.
* Você pode configurar alguns estágios para se tornarem ativos somente depois que um estágio anterior for concluído.
* Você pode tornar algumas etapas privadas. Isso é útil, por exemplo, para uma agência que revisa uma prova antes de ela ser compartilhada com um cliente e não deseja que os comentários resultantes fiquem visíveis para o cliente.

Para obter instruções sobre como criar estágios para uma prova com um fluxo de trabalho automatizado, consulte [Criar uma prova avançada com um fluxo de trabalho automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

>[!NOTE]
>
>Se um usuário não estiver incluído em nenhum estágio, mas tiver acesso ao documento e abrir a prova, o sistema criará um estágio chamado *Workfront*.
>
>Ao usuário que abriu a prova é atribuída a função especificada em Configuração > Revisar e aprovar > Funções para usuários que não são destinatários e que abrem uma prova de documento.

## Atribuir prazos para diferentes revisores em uma prova {#assign-deadlines-for-different-reviewers-on-a-proof}

Quando você atribui diferentes prazos de prova aos revisores em uma prova, o sistema cria um estágio para cada prazo e agrupa os revisores para cada prazo no estágio correspondente. 

**Exemplo:** Por exemplo, se você criar uma prova com quatro revisores:

* Para os revisores Olivia e Tony, você especifica um prazo para as 14:00 alguns dias a partir de agora.
* Para Aaron e Amy, você especifica um prazo para 17:00 alguns dias depois.
* Você não especifica um prazo final para si mesmo.

O sistema cria um estágio para cada um desses três &quot;grupos&quot; de revisores:

![estágios.png](assets/stages-350x239.png)

Se você compartilhar a prova com outro revisor e não especificar um prazo, a Workfront adicionará o usuário ao Estágio 3, onde não há prazo. 
