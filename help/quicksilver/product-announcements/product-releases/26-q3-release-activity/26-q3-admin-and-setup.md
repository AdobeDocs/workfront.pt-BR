---
title: Aprimoramentos do administrador no terceiro trimestre de 2026
description: Aprimoramentos do administrador no terceiro trimestre de 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: eb59acc816f0fd82330b60ddc9cd2f3aad851198
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 2%

---

# Aprimoramentos do administrador no terceiro trimestre de 2026

Esta página descreve as melhorias de Administrador feitas com a versão do terceiro trimestre de 2026 no ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de produção, conforme indicado.

Para obter uma lista de todas as alterações disponíveis neste momento no ciclo de lançamento do terceiro trimestre de 2026, consulte [Visão geral da versão do terceiro trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Rich Text substituindo o texto pelo tipo de campo Formatação

>[!NOTE]
>
>Visualização: 28 de maio de 2026>Versão rápida de produção: 11 de junho de 2026>Produção para todos: 16 de julho de 2026

O novo tipo de campo **Rich text** em formulários personalizados é um editor de texto robusto, com opções de formatação como sobrescrito e subscrito, cabeçalhos e tabelas, além das opções tradicionais de negrito, itálico, sublinhado, marcadores, numeração, hiperlinks e aspas duplas. O limite de caracteres permanece de 15.000.

O tipo de campo Rich text está substituindo o texto pelo tipo de campo de formatação. Você pode converter rapidamente Texto existente com campos de formatação em Rich text, clicando no botão nas opções de campo à direita. Quando você converte, os dados históricos permanecem no campo e são usados da mesma maneira nos relatórios.

>[!IMPORTANT]
>
>Integrações externas, como cenários do Workfront Fusion ou automações baseadas em API, podem fazer referência a estruturas de campo herdadas e exigir atualizações após a conversão. Você deve verificar todas as integrações antes de converter campos em Rich text.

Para obter mais informações, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Campos financeiros nativos suportados em formulários personalizados

>[!NOTE]
>
>Visualização: 28 de maio de 2026>Versão rápida de produção: 11 de junho de 2026>Produção para todos: 16 de julho de 2026

Agora é possível incluir campos financeiros nativos do Workfront em formulários personalizados. Anteriormente, os campos financeiros não eram compatíveis.

Os campos financeiros disponíveis que você pode referenciar dependem do tipo de formulário.

Para obter mais informações, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-workfront-native-fields).

## Os formulários personalizados podem ser compartilhados em todo o sistema com acesso para anexar

>[!NOTE]
>
>Visualização: 28 de maio de 2026>Versão rápida de produção: 11 de junho de 2026>Produção para todos: 16 de julho de 2026

Uma nova opção de compartilhamento, &quot;Todos no sistema podem visualizar e anexar&quot;, foi adicionada aos formulários personalizados. Ao selecionar essa opção, todos os usuários em todo o sistema podem anexar o formulário a outros objetos.

O compartilhamento em todo o sistema elimina a necessidade de compartilhar formulários manualmente e atualizar permissões entre grupos ou agências quando novos grupos são adicionados.

Para obter mais informações, consulte [Compartilhar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).

## Nova preferência do sistema para aplicar campos obrigatórios na edição de itens em massa

>[!NOTE]
>
>Visualização: 28 de maio de 2026>Versão rápida de produção: 11 de junho de 2026>Produção para todos: 16 de julho de 2026

Atualmente, ao editar objetos em massa, os campos obrigatórios só são aplicados quando um usuário modifica o campo. Se um campo não for modificado, será tratado como opcional e não validado.

Uma nova preferência do sistema agora permite aplicar campos obrigatórios na edição de itens em massa. Para não permitir que objetos editados em massa sejam salvos a menos que todos os campos obrigatórios tenham valores, selecione a opção **Sempre impor campos obrigatórios na edição em massa** na página Configuração > Sistema > Preferências.