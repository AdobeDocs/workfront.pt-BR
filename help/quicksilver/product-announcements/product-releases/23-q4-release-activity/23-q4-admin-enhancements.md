---
title: Aprimoramentos do administrador do quarto trimestre de 2023
description: Aprimoramentos do administrador do quarto trimestre de 2023
author: Lisa
feature: Product Announcements
source-git-commit: 8488cb46b3dd9b377c59121597db5b6fe784fdab
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 0%

---

# Aprimoramentos do administrador do quarto trimestre de 2023

Esta página descreve todas as melhorias de administrador feitas com a versão do Quarto trimestre de 2023 para o ambiente de Pré-visualização. Esses aprimoramentos serão disponibilizados no ambiente de produção com a versão 23.10.

Para obter uma lista de todas as alterações disponíveis neste momento do ciclo de lançamento do quarto trimestre de 2023, consulte [Visão geral da versão do quarto trimestre de 2023](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md).

## Campos calculados em formulários personalizados agora podem usar o curinga $$USER

A variável `$$USER` o curinga agora está disponível em campos personalizados calculados e campos de pesquisa externos no novo designer de formulário. Referenciando `$$USER` em um cálculo adiciona a ID do usuário atual. Também é possível usar o curinga com outro campo. Por exemplo, `$$USER.{name}` adicionaria o nome do usuário atual.

Para obter mais informações sobre campos calculados, consulte [Adicionar campos calculados com o designer de formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

## Adicionar opções de valor de uma API externa a um formulário personalizado

Um novo tipo de campo, **Pesquisa externa**, agora está disponível no designer de formulário personalizado. Quando os dados são armazenados em um sistema externo, esse tipo de campo permite carregar opções de uma API externa e filtrar com base em outros valores de campo no formulário personalizado.

Quando o formulário é adicionado a um objeto, os valores retornados da API são exibidos em um campo suspenso e o usuário pode selecionar um.

>[!NOTE]
>
>O novo **Pesquisa externa** o tipo de campo não está disponível no construtor de formulários herdados.

Para obter mais informações, consulte [Criar um formulário com o designer de formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
