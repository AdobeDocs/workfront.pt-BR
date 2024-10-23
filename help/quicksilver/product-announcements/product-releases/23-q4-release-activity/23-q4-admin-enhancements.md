---
title: Aprimoramentos do administrador do quarto trimestre de 2023
description: Aprimoramentos do administrador do quarto trimestre de 2023
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7ed37978-b821-488e-9ca1-b81825255be3
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 0%

---

# Aprimoramentos do administrador do quarto trimestre de 2023

Esta página descreve todas as melhorias de administrador feitas com a versão do Quarto trimestre de 2023 para o ambiente de Pré-visualização. Essas melhorias foram disponibilizadas no ambiente de Produção com a versão 23.10.

Para obter uma lista de todas as alterações disponíveis neste momento do ciclo de lançamento do quarto trimestre de 2023, consulte [Visão geral da versão do quarto trimestre de 2023](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md).

## Decisões de prova e documento disponíveis para clientes do modelo de licença herdado

Os clientes herdados que ainda não migraram para o novo modelo de licença da Adobe Workfront agora podem ver dados com o número de decisões de prova/documento por usuário por mês, em um único relatório. Esses dados estão disponíveis quando você executa um relatório de Decisões do usuário.

Para obter mais informações, consulte [Entender objetos no Adobe Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) e [Exibir o número de decisões de prova e documento para todos os usuários](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/view-number-of-decisions-for-users.md).

## Campos calculados em formulários personalizados agora podem usar o curinga $$USER

O curinga `$$USER` agora está disponível em campos personalizados calculados e campos de pesquisa externos no novo designer de formulário. Fazer referência a `$$USER` em um cálculo adiciona a ID do usuário atual. Também é possível usar o curinga com outro campo. Por exemplo, `$$USER.{name}` adicionaria o nome do usuário atual.

Para obter mais informações sobre campos calculados, consulte [Adicionar campos calculados com o designer de formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

## Adicionar opções de valor de uma API externa a um formulário personalizado

Um novo tipo de campo, **Pesquisa externa**, agora está disponível no designer de formulário personalizado. Quando os dados são armazenados em um sistema externo, esse tipo de campo permite carregar opções de uma API externa e filtrar com base em outros valores de campo no formulário personalizado.

Quando o formulário é adicionado a um objeto, os valores retornados da API são exibidos em um campo suspenso e o usuário pode selecionar um.

>[!NOTE]
>
>O novo tipo de campo **Pesquisa externa** não está disponível no construtor de formulários herdados.

Para obter mais informações, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
