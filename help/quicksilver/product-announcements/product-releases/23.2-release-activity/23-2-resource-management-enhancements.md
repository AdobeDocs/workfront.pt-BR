---
title: 23.2 Aprimoramentos no gerenciamento de recursos
description: 23.2 Aprimoramentos no gerenciamento de recursos
author: Courtney
draft: Probably
feature: Product Announcements
source-git-commit: 93071f9c9d359ff98a269b07f81ebcf251b1f23c
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# 23.2 Aprimoramentos no gerenciamento de recursos

Esta página descreve todas as melhorias de gerenciamento de recursos feitas com a versão 23.2 para o ambiente de Pré-visualização. Esses aprimoramentos serão disponibilizados no ambiente de produção com a versão 23.2.

Para obter uma lista de todas as alterações disponíveis neste ponto do ciclo de versão 23.2, consulte [23.2 Visão geral da versão](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

## Introdução ao campo Horário de trabalho para calcular com precisão a capacidade do usuário

>[!NOTE]
>
>Versão de pré-visualização: 16 de fevereiro de 2023; Versão de produção planejada: 2 de março de 2023

Para permitir que os gerentes de recursos calculem com precisão a disponibilidade de seus usuários e contabilizem o tempo que os usuários dedicam ao trabalho real relacionado ao projeto, estamos introduzindo o conceito de Tempo de trabalho ao Adobe Workfront.

Você pode definir o valor do campo Horário de trabalho para cada usuário ao criar ou editar seu perfil. Para obter mais informações, consulte [Editar o perfil de um usuário](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

O campo Tempo de Trabalho representa a porcentagem de tempo FTE (Equivalente a Tempo Integral) em que o usuário está disponível para o trabalho real, sem incluir as despesas indiretas. O horário de trabalho deve ser um número decimal com um valor entre 0 e 1. Por exemplo, uma disponibilidade de 20% para o trabalho real seria de 0,2.

O campo padrão é 1, indicando que um usuário gasta todo o FTE em trabalho real relacionado ao projeto.

Como resultado dessa atualização, o Workfront calcula a disponibilidade do usuário usando as fórmulas abaixo, dependendo de sua seleção na área Preferências de gerenciamento de recursos:

* Calendário padrão:
* Capacidade do usuário = [(Horas Programadas - Exceções Programadas) * FTE - Tempo livre] * Horário de trabalho
* Cronograma do usuário:
* Capacidade do Usuário = (Horas Programadas - Exceções Programadas - Folga) * Tempo de Trabalho.

Para obter mais informações, consulte [Configurar [!UICONTROL Gerenciamento de recursos] preferências](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

[Exibir uma demonstração em vídeo desse recurso](https://video.tv.adobe.com/v/3415608/){target=_blank}