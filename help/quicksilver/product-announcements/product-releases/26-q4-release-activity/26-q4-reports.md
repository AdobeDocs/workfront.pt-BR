---
title: Melhorias na emissão de relatórios no quarto trimestre de 2026
description: Melhorias na emissão de relatórios no quarto trimestre de 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: ee1fceee828c97db535ccc03c8b428940d6f7eed
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 8%

---

# Melhorias na emissão de relatórios no quarto trimestre de 2026

Esta página descreve as melhorias de relatórios feitas com a versão do quarto trimestre de 2026 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de produção, conforme indicado.

Para obter uma lista de todas as alterações disponíveis neste momento do ciclo de lançamento do quarto trimestre de 2026, consulte [Visão geral da versão do quarto trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

<!--

## Duplicate dashboards in Canvas Dashboards

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

You can now duplicate a Canvas Dashboard using the new **Duplicate dashboard** action. This action is available to any user whose access level grants edit or create rights to Dashboards, even if they only have view access to the specific dashboard being copied. Users without edit or create rights to Dashboards do not see this action.

When you duplicate a dashboard, you can rename it, update its description and currency, and choose which widgets, dashboard filters, and dashboard prompts to carry over to the copy.

Run as user configurations on widgets are only preserved if you are the designated user or a system administrator. Sharing preferences are not copied to the new dashboard, and a confirmation message with a link to the new dashboard displays once the copy is complete.

Previously, there was no way to duplicate a dashboard; users had to rebuild dashboards from scratch to create audience-specific variations.

For more information, see 

-->

## Campo Tipo de aprovação nos Painéis de Controle da Tela

>[!NOTE]
>
>Produção para todos: 28 de agosto de 2026
>[!BADGE Fora do cronograma]{type=Neutral}

A entidade Approval agora inclui um campo **Tipo de Aprovação**, que permite que os usuários façam a distinção entre aprovações de prova, aprovações de versão de documento, aprovações de entrada e outros tipos de aprovação.

## Atualização da terminologia de aprovação nos Painéis do Canvas

>[!NOTE]
>
>Produção para todos: 28 de agosto de 2026
>[!BADGE Fora do cronograma]{type=Neutral}

Os seguintes nomes de campo usados em Painéis de tela para aprovações de documentos e trabalhos foram renomeados para maior clareza:

| Nome anterior | Novo nome |
| --- | --- |
| Aprovação de documento | Aprovação |
| Estágio de aprovação do documento | Estágio de aprovação |
| Participante do estágio de aprovação do documento | Participante do estágio de aprovação |
| Processo de aprovação | Processo de aprovação de trabalho |
| Estágio de aprovação | Estágio de aprovação de trabalho |
| Status do aprovador | Status do aprovador do trabalho |
| Aguardando Aprovação | Aguardando aprovação do trabalho |

Essa alteração não afeta a forma como os relatórios atuais funcionam.

## Relatórios de tabela dinâmica em Painéis da tela de desenho

>[!NOTE]
>
>Visualização: 27 de agosto de 2026
>Versão rápida de produção: 17 de setembro de 2026
>Produção para todos: 15 de outubro de 2026

O novo tipo de relatório de tabela dinâmica nos Painéis da tela agrega dados com roll-ups precisos e completos. Você pode criar métricas como contagens, somas e médias diretamente no painel e, em seguida, detalhar os registros subjacentes atrás de qualquer total.

Para obter mais informações, consulte [Criar um relatório de tabela dinâmica em um Painel da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-pivot-table-report.md).

## Imposição de datas de término para relatórios agendados

>[!NOTE]
>
>Visualização: 13 de agosto de 2026
>Versão rápida de produção: 17 de setembro de 2026
>Produção para todos: 15 de outubro de 2026

Os relatórios agendados agora exigem uma data de término para evitar entrega indefinida. Os cronogramas que passarem da data final serão desativados automaticamente.

As programações existentes foram atualizadas com datas de término para melhorar a confiabilidade e reduzir o uso desnecessário do sistema. A Workfront também oferece visibilidade e avisos adicionais para ajudar você a gerenciar os ciclos de vida do agendamento de relatórios à medida que se aproximam da data de término.

Para obter mais informações, consulte [Agendar uma entrega automática de relatório](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

## Campos de referência nativos estão disponíveis para listas e relatórios

>[!NOTE]
>
>Visualização: 30 de julho de 2026
>Versão rápida de produção: 13 de agosto de 2026
>Produção para todos: 15 de outubro de 2026

Agora é possível adicionar campos de referência nativos a listas e relatórios no Workfront.

Um campo de referência nativo é um campo personalizado. Quando o campo está em um formulário personalizado anexado a um objeto, o campo é preenchido a partir dos dados do objeto. Por exemplo, se o campo fizer referência ao campo Descrição e estiver em um formulário personalizado anexado a um projeto, ele extrairá a descrição do projeto. (O campo pode mostrar “N/A” se não houver dados disponíveis.)

Para obter informações sobre como criar campos de referência nativos, incluindo a lista de campos nativos com suporte, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
Para obter informações sobre como adicionar campos a relatórios, consulte [Criar um relatório personalizado](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Ordem consistente para valores de campo de seleção múltipla em listas e relatórios herdados

>[!NOTE]
>
>Visualização: 30 de julho de 2026
>Versão rápida de produção: 13 de agosto de 2026
>Produção para todos: 15 de outubro de 2026

Agora você vê as opções selecionadas para seleção múltipla de campos personalizados em uma ordem consistente e previsível em listas e relatórios herdados. A ordem dos campos é determinada pela organização dos campos no formulário personalizado.

![A ordem dos campos de formulário personalizados corresponde à ordem dos valores selecionados em uma lista ou relatório](assets/new-field-order-multi-select.png)

Anteriormente, as opções selecionadas eram exibidas na ordem em que você as escolhia ou em uma ordem inconsistente, o que tornava as linhas mais difíceis de serem digitalizadas e comparadas.

Observação: a nova classificação não se aplica se o campo estiver usando o modo de texto.
