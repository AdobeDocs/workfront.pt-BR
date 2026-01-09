---
title: Aprimoramentos do administrador no primeiro trimestre de 2026
description: Aprimoramentos do administrador no primeiro trimestre de 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: a524dd5519f450543e486d83bff6134a15f548d7
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 0%

---

# Aprimoramentos do administrador no primeiro trimestre de 2026

Esta página descreve as melhorias de Administrador feitas com a versão do Primeiro trimestre de 2026 no ambiente de Pré-visualização. Esses aprimoramentos serão disponibilizados no ambiente de Produção, conforme observado.

Para obter uma lista de todas as alterações disponíveis neste momento no ciclo de lançamento do Primeiro trimestre de 2026, consulte [Visão geral da versão do Primeiro trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Gerenciar prioridades no modelo de layout

>[!NOTE]
>
>Este recurso está temporariamente indisponível no ambiente de Visualização
>Visualização: 2 de dezembro de 2025
>Lançamento rápido de produção: 14 de janeiro de 2026
>Produção para todos: 15 de janeiro de 2026


Agora você pode ativar ou desativar as Prioridades de usuários específicos no Modelo de Layout. Se as prioridades da sua organização já estavam desativadas, elas permanecerão desativadas no modelo de layout com essa alteração.

As prioridades serão incluídas automaticamente para os tipos de licença que têm acesso padrão a Solicitações. Por exemplo, uma licença de Colaborador verá Solicitações, Quadros e Prioridades por padrão no Menu Principal, enquanto uma licença Externa só verá Documentos e Quadros porque não tem acesso para exibir ou enviar solicitações.


Para obter mais informações, consulte [Personalizar o Menu Principal usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

## Verifique se há conflitos de vários formulários para campos personalizados calculados

>[!NOTE]
>
>Visualização: 18 de dezembro de 2025
>Lançamento rápido de produção: 14 de janeiro de 2026
>Produção para todos: 15 de janeiro de 2026

O mesmo campo calculado pode ter diferentes fórmulas quando anexado a diferentes formulários personalizados. Se dois ou mais formulários contendo o mesmo campo calculado forem anexados a um objeto, as fórmulas deverão ser idênticas em todos os formulários. A edição da fórmula não é permitida se a alteração puder causar um conflito.

Para fornecer visibilidade sobre quais objetos podem ser afetados ao editar uma expressão em campos personalizados, adicionamos uma opção para verificar se há conflitos. Esta caixa de diálogo mostra todos os objetos que podem ser afetados pela alteração da fórmula, agrupados por tipo de objeto. É possível navegar até os detalhes de cada objeto e revisar os campos para decidir se o campo deve ser removido de qualquer um dos formulários ou se a expressão deve permanecer inalterada.

Para obter mais informações, consulte [Adicionar campos calculados a um formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).


## Data de entrada e ID inserido por armazenado em objetos personalizados

>[!NOTE]
>
>Visualização: 13 de novembro de 2025
>Versão rápida de produção: 13 de novembro de 2025
>Produção para todos: 13 de novembro de 2025

A data de entrada e inserida pela ID agora são armazenadas em formulários, campos e seções personalizados. É possível usar essas opções de dados em relatórios como filtros, visualizações ou agrupamentos. Para exibi-los na lista de formulários personalizados, campos ou seções em Configurar, adicione Data de Entrada e Inserido por: Nome como colunas em uma exibição nova ou existente.

>[!NOTE]
>
>A data de entrada e a ID inserida estão disponíveis somente em formulários, campos e seções personalizados criados em ou após 13 de novembro de 2025.

## Atualizações a nomes de botão ao editar um modelo de layout

>[!NOTE]
>
>Visualização: 30 de outubro de 2025
>Versão rápida de produção: 13 de novembro de 2025
>Produção para todos: 15 de janeiro de 2026

Para oferecer mais consistência com outras áreas de Configuração, como o designer de formulário personalizado, os botões exibidos ao editar um modelo de layout foram alterados para **Aplicar**, **Salvar e Fechar** e **Cancelar**. A nova opção, **Aplicar**, permite salvar as alterações no modelo de layout e continuar a edição. Anteriormente, as opções disponíveis eram **Salvar** e **Cancelar**.

Para obter mais informações, consulte [Criar e gerenciar modelos de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

## Gerenciamento de campo aprimorado com sinalizador Ativo em campos personalizados

>[!NOTE]
>
>Visualização: 30 de outubro de 2025
>Versão rápida de produção: 13 de novembro de 2025
>Produção para todos: 15 de janeiro de 2026

Quando você tem um grande número de campos personalizados no sistema, pode ser difícil gerenciar esses campos em formulários e relatórios personalizados. Agora você pode marcar campos personalizados como inativos com o novo sinalizador **Ativo**. Esse sinalizador está disponível ao trabalhar com um campo em um formulário personalizado ou ao adicionar ou editar um campo da lista Campos.

Se você marcar um campo como inativo:

* Ele é excluído de relatórios, filtros, exibições ou outros locais no Workfront onde você pode adicionar um campo personalizado
* Não está disponível na biblioteca de campos para adicionar a outros formulários personalizados

>[!NOTE]
>
>Marcar um campo existente como inativo o torna indisponível para uso em elementos de relatórios e formulários personalizados a partir desse ponto. Se o campo inativo for usado atualmente em um relatório ou formulário, o campo e seus dados históricos permanecerão no lugar.

Para obter mais informações, consulte [Adicionar ou editar um campo personalizado, quebra de seção ou widget](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/edit-a-custom-field.md).




