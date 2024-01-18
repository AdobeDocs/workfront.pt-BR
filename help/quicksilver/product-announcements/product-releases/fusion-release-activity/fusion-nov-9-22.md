---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: "Atividade de lançamento do Workfront Fusion: semana de 7 de novembro de 2022"
description: Esta página descreve todas as melhorias feitas no Adobe Workfront Fusion na semana de 7 de novembro de 2022.
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
hidefromtoc: true
exl-id: 802db851-39bb-4f40-8a66-ecb8c8b3ced6
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# Atividade de lançamento do Workfront Fusion: semana de 7 de novembro de 2022

**Otimização da fila do Webhook**

A fila de webhook do Fusion foi otimizada com esta versão. O serviço que aceita webhooks agora está separado do enfileiramento e de outros processos. Essa alteração permite que o Fusion processe filas de webhook a uma taxa mais rápida e consistente.

Durante a implementação dessa alteração, foi possível entender melhor o tempo de processamento de log esperado para eventos de webhook na fila. Espera-se que a página do visualizador de webhook do Fusion não tenha mais de 1 minuto.

Para ver os eventos de webhook atualmente na fila, navegue até Webhooks, na navegação à esquerda. Os ícones de caminhão com um número no numerador indicam eventos de fila para esse webhook. Clique no ícone de caminhão para ver os eventos em fila.

![](assets/fusion-webhook-queue-1866x567.png)


**Os webhooks não utilizados agora serão desativados ou excluídos**

Fizemos algumas alterações no modo como o Workfront Fusion lida com webhooks não utilizados. Agora, os Webhooks são desativados automaticamente se qualquer uma das opções a seguir se aplicar:

* O webhook não foi conectado a nenhum cenário por mais de 5 dias.
* O webhook é usado somente em cenários inativos, que ficaram inativos por mais de 30 dias.

Os webhooks desativados são excluídos e não registrados automaticamente se não estiverem conectados a nenhum cenário e estiverem com o status desativado por mais de 30 dias.
