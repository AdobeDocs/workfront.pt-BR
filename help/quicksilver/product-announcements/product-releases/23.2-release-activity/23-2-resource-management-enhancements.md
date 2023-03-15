---
title: 23.2 Melhorias no gerenciamento de recursos
description: 23.2 Melhorias no gerenciamento de recursos
author: Courtney
draft: Probably
feature: Product Announcements
source-git-commit: 93071f9c9d359ff98a269b07f81ebcf251b1f23c
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# 23.2 Melhorias no gerenciamento de recursos

Esta página descreve todas as melhorias no gerenciamento de recursos realizadas com a versão 23.2 para o ambiente de visualização. Esses aprimoramentos serão disponibilizados no ambiente de Produção com a versão 23.2.

Para obter uma lista de todas as alterações disponíveis neste ponto do ciclo de versão 23.2, consulte [Visão geral da versão 23.2](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

## Introdução do campo Tempo de trabalho para calcular com precisão a capacidade do usuário

>[!NOTE]
>
>Versão de visualização: 16 de fevereiro de 2023; Versão de produção planejada: 2 de março de 2023

Para permitir que os gerentes de recursos calculem com precisão a disponibilidade de seus usuários e contabilizem o tempo que os usuários dedicam ao trabalho real relacionado ao projeto, estamos introduzindo o conceito de Tempo de Trabalho na Adobe Workfront.

Você pode definir o valor do campo Tempo de trabalho para cada usuário, ao criar ou editar seu perfil. Para obter mais informações, consulte [Editar o perfil de um usuário](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

O campo Tempo de Trabalho representa a porcentagem do tempo FTE (Equivalente de Tempo Total) que o usuário está disponível para o trabalho real, sem incluir a sobrecarga. O Tempo de Trabalho deve ser um número decimal com um valor entre 0 e 1. Por exemplo, uma disponibilidade de 20% para o trabalho real seria de 0,2.

O padrão do campo é 1, indicando que um usuário gasta o FTE inteiro no trabalho real relacionado ao projeto.

Como resultado dessa atualização, o Workfront calcula a disponibilidade do usuário usando as fórmulas abaixo, dependendo de sua seleção na área de preferências do Gerenciamento de Recursos:

* Calendário padrão:
* Capacidade do usuário = [(Horário agendado - Exceções agendadas) * FTE - Tempo desligado] * Tempo de trabalho
* Programação do usuário:
* Capacidade do Usuário = (Horas de Programação - Exceções de Programação - Tempo limite) * Tempo de Trabalho.

Para obter mais informações, consulte [Configurar [!UICONTROL Gerenciamento de recursos] preferências](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

[Ver uma demonstração em vídeo deste recurso](https://video.tv.adobe.com/v/3415608/){target=_blank}