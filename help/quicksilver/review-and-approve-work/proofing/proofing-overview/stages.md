---
content-type: overview
product-area: documents
navigation-topic: proofing-overview
title: Visão geral das etapas do fluxo de trabalho automatizado
description: Estágios de prova são segmentos de tempo em que usuários diferentes revisam uma prova. À medida que a prova vai de um estágio para o seguinte, o Adobe Workfront notifica os revisores para informá-los quando é hora de trabalhar nela.
author: Courtney
feature: Digital Content and Documents
exl-id: a03d2cf2-edb3-43b7-a739-32600f2ae2a0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# Visão geral das etapas do fluxo de trabalho automatizado

Estágios de prova são segmentos de tempo em que usuários diferentes revisam uma prova. À medida que a prova vai de um estágio para o seguinte, o Adobe Workfront notifica os revisores para informá-los quando é hora de trabalhar nela.

![stage_diagrama.png](assets/stages-diagram-350x63.png)

Os estágios ocorrem em duas situações diferentes:

* [Criar uma prova com um fluxo de trabalho Automatizado](#create-a-proof-with-an-automated-workflow)
* [Atribuir prazos para diferentes revisores em uma prova](#assign-deadlines-for-different-reviewers-on-a-proof)

## Criar uma prova com um fluxo de trabalho Automatizado {#create-a-proof-with-an-automated-workflow}

Ao adicionar um fluxo de trabalho automatizado a uma prova, você configura os estágios do trabalho de revisão que deseja que ocorra.

Ao configurar estágios para uma prova com um fluxo de trabalho automático:

* Você pode configurar os estágios para serem executados consecutiva ou simultaneamente.
* Você pode configurar alguns estágios para ficarem ativos somente após uma etapa anterior ser concluída.
* Você pode tornar alguns estágios privados. Isso é útil, por exemplo, para uma agência que analisa uma prova antes de ela ser compartilhada com um cliente e não deseja que os comentários resultantes sejam visíveis para o cliente.

Para obter instruções sobre como criar estágios para uma prova com um fluxo de trabalho automatizado, consulte [Criar uma prova avançada com um fluxo de trabalho Automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

>[!NOTE]
>
>Se um usuário não estiver incluído em nenhum estágio, mas tiver acesso ao documento e abrir a prova, o sistema criará um estágio chamado *Workfront*.
>
>O usuário que abriu a prova recebe a função especificada em Configurar > Revisar e aprovar > Funções para não destinatários que abrem uma prova de documento.

## Atribuir prazos para diferentes revisores em uma prova {#assign-deadlines-for-different-reviewers-on-a-proof}

Ao atribuir diferentes prazos de prova aos revisores em uma prova, o sistema cria um estágio para cada prazo e agrupa os revisores para cada prazo no estágio correspondente. 

**Exemplo:** Por exemplo, se você criar uma prova com quatro revisores:

* Para os revisores Olivia e Tony, especifique um prazo para as 14:00 daqui a alguns dias.
* Para Aaron e Amy, especifique um prazo para 17:00 dias depois.
* Você não especifica um prazo para si mesmo.

O sistema cria um palco para cada um desses três &quot;grupos&quot; de revisores:

![stage.png](assets/stages-350x239.png)

Se você compartilhar a prova com outro revisor e não especificar um prazo, o Workfront adicionará o usuário ao Estágio 3, onde não há prazo. 
