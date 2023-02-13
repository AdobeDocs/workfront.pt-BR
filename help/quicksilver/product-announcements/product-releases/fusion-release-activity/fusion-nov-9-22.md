---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: '"Atividade da versão do Workfront Fusion: Semana de 7 de novembro de 2022'''
description: Esta página descreve todas as melhorias feitas no Adobe Workfront Fusion na semana de 7 de novembro de 2022.
author: Luke
feature: Product Announcements, Workfront Fusion
hidefromtoc: true
exl-id: 802db851-39bb-4f40-8a66-ecb8c8b3ced6
source-git-commit: 9aaba3062bc5d1166c37821a6a3216f7f1d965b1
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# Atividade de versão do Workfront Fusion: Semana de 7 de novembro de 2022

**Otimização da fila do Webhook**

A fila do webhook Fusion foi otimizada com esta versão. O serviço que aceita webhooks agora é separado da fila e de outros processos. Essa alteração possibilita que o Fusion processe filas de webhook a uma taxa mais rápida e consistente.

Durante a implementação dessa alteração, pudemos entender melhor o tempo esperado de processamento de log para eventos de webhook na fila. Espera-se que a página do visualizador do webhook Fusion não tenha mais de 1 minuto.

Para ver eventos do webhook na fila, navegue até Webhooks, na navegação à esquerda. Ícones de caminhão com um número no numerador indicam eventos de fila para esse webhook. Clique no ícone do caminhão para ver os eventos na fila.

![](assets/fusion-webhook-queue-1866x567.png)


**Os webhooks não usados agora serão desativados ou excluídos**

Fizemos algumas alterações no modo como o Workfront Fusion lida com os webhooks não utilizados. Agora, os Webhooks são desativados automaticamente se uma das seguintes opções se aplicar:

* O webhook não está conectado a nenhum cenário há mais de 5 dias.
* O webhook é usado apenas em cenários inativos, que ficaram inativos por mais de 30 dias.

Os webhooks desativados são excluídos e não são registrados automaticamente se não estiverem conectados a nenhum cenário e estiverem com o status desativado por mais de 30 dias.
