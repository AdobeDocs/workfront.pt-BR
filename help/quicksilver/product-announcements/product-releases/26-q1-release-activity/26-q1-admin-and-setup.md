---
title: Aprimoramentos de administrador no primeiro trimestre de 2026
description: Aprimoramentos de administrador no primeiro trimestre de 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a74d036b-e4fa-49e0-bb10-4baf379e1b1c
TQID: https://experienceleague.adobe.com/IYlqpTdS-pJNpBaCeYywassuOaTQdaSZlctxd1J0NPA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 669
ht-degree: 96%

---

# Aprimoramentos de administrador no primeiro trimestre de 2026

Esta página descreve as melhorias de Administrador feitas com a versão do primeiro trimestre de 2026 no ambiente de pré-visualização. Essas melhorias serão disponibilizadas no ambiente de produção, conforme indicado.

Para obter uma lista de todas as alterações disponíveis neste momento no ciclo de lançamento do primeiro trimestre de 2026, consulte [Visão geral de lançamentos do primeiro trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Gerenciar prioridades no modelo de layout

>[!NOTE]
>
>Este recurso está temporariamente indisponível no ambiente de Visualização>Visualização: 2 de dezembro de 2025>Versão rápida de produção: 14 de janeiro de 2026>Produção para todos: 15 de janeiro de 2026


Agora você pode habilitar ou desabilitar prioridades para usuários específicos no modelo de layout. Se você já tinha as prioridades desabilitadas para sua organização, elas permanecerão desabilitadas no modelo de layout com essa alteração.

As prioridades serão automaticamente incluídas para os tipos de licença que têm acesso padrão às solicitações. Por exemplo, uma licença de colaborador verá Solicitações, Quadros e Prioridades por padrão no menu principal, enquanto uma licença externa verá apenas Documentos e Quadros, pois não tem acesso para visualizar ou enviar solicitações.


Para obter mais informações, consulte [Personalizar o menu principal usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

## Verifique se há conflitos entre vários formulários para campos personalizados calculados

>[!NOTE]
>
>Visualização: 18 de dezembro de 2025>Versão rápida de produção: 14 de janeiro de 2026>Produção para todos: 15 de janeiro de 2026

O mesmo campo calculado pode ter fórmulas diferentes quando anexado a formulários personalizados diferentes. Se dois ou mais formulários contendo o mesmo campo calculado estiverem anexados a um objeto, as fórmulas devem ser idênticas em todos os formulários. Não é permitido editar a fórmula se a alteração puder causar um conflito.

Para fornecer visibilidade sobre quais objetos podem ser afetados ao editar uma expressão em campos personalizados, adicionamos uma opção para verificar se há conflitos. Esta caixa de diálogo mostra todos os objetos que podem ser afetados pela alteração da fórmula, agrupados por tipo de objeto. Você pode navegar até os detalhes de cada objeto e revisar os campos para decidir se o campo deve ser removido de algum dos formulários ou se a expressão deve permanecer inalterada.

Para obter mais informações, consulte [Adicionar campos calculados a um formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).


## Data de entrada e ID de quem realizou a entrada armazenados em objetos personalizados

>[!NOTE]
>
>Visualização: 13 de novembro de 2025>Versão rápida de produção: 13 de novembro de 2025>Produção para todos: 13 de novembro de 2025

A data de entrada e a ID de quem realizou a entrada agora são armazenados em formulários personalizados, campos e seções. Você pode usar essas opções de dados em relatórios como filtros, exibições ou agrupamentos. Para exibi-los na lista de formulários personalizados, campos ou seções em Configuração, adicione “Data de entrada” e “Inserido por: nome” como colunas em uma exibição nova ou já existente.

>[!NOTE]
>
>A data de entrada e a ID de quem realizou a entrada estão disponíveis apenas em formulários personalizados, campos e seções criados em 13 de novembro de 2025 ou após essa data.

## Atualizações dos nomes dos botões ao editar um modelo de layout

>[!NOTE]
>
>Visualização: 30 de outubro de 2025>Versão rápida de produção: 13 de novembro de 2025>Produção para todos: 15 de janeiro de 2026

Para proporcionar mais consistência com outras áreas da configuração, como o designer de formulários personalizados, os botões exibidos ao editar um modelo de layout foram alterados para **Aplicar**, **Salvar e Fechar** e **Cancelar**. A nova opção, **Aplicar**, permite salvar as alterações no modelo de layout e continuar editando. Anteriormente, as opções disponíveis eram **Salvar** e **Cancelar**.

Para obter mais informações, consulte [Criar e gerenciar modelos de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

## Gerenciamento de campos aprimorado com o sinalizador Ativo em campos personalizados

>[!NOTE]
>
>Visualização: 30 de outubro de 2025>Versão rápida de produção: 13 de novembro de 2025>Produção para todos: 15 de janeiro de 2026

Quando há um grande número de campos personalizados no sistema, o gerenciamento desses campos em formulários e relatórios personalizados pode ser difícil. Agora você pode marcar campos personalizados como inativos com o novo sinalizador **Ativo**. Este sinalizador está disponível ao trabalhar com um campo em um formulário personalizado ou ao adicionar ou editar um campo da lista Campos.

Se você marcar um campo como inativo:

* Ele é excluído de relatórios, filtros, exibições ou outros locais no Workfront onde você pode adicionar um campo personalizado
* Não fica disponível na biblioteca de campos para ser adicionado a outros formulários personalizados

>[!NOTE]
>
>Marcar um campo existente como inativo torna-o indisponível para uso em elementos de relatórios e formulários personalizados a partir desse momento. Se o campo inativo estiver sendo usado atualmente em um relatório ou formulário, o campo e seus dados históricos permanecerão no lugar.

Para obter mais informações, consulte [Adicionar ou editar um campo personalizado, quebra de seção ou widget](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/edit-a-custom-field.md).
