---
title: Aprimoramentos do administrador no terceiro trimestre de 2026
description: Aprimoramentos do administrador no terceiro trimestre de 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: d83d823426b42202e83cb4db64f85d27d4dca0bb
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 8%

---

# Aprimoramentos do administrador no terceiro trimestre de 2026

Esta página descreve as melhorias de Administrador feitas com a versão do terceiro trimestre de 2026 no ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de produção, conforme indicado.

Para obter uma lista de todas as alterações disponíveis neste momento no ciclo de lançamento do terceiro trimestre de 2026, consulte [Visão geral da versão do terceiro trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Controle de alterações para revisão e aprovação unificadas

>[!NOTE]
>
>Visualização: 7 de julho de 2026Versão rápida de produção: 15 de julho de 2026Produção para todos: 16 de julho de 2026

A página Histórico de alterações no Workfront agora captura a atividade em fluxos de trabalho unificados de revisão e aprovação, fornecendo aos administradores uma trilha de governança completa para eventos de ciclo de vida de revisão e documento.

Agora, as ações de aprovação, preparo e participante são rastreadas. Essas ações podem incluir:

* Tomada de decisão de aprovação no visualizador Frame.io
* Criação ou exclusão de uma aprovação
* Atualizar um documento, como renomear, mover ou excluí-lo

Cada entrada inclui os campos rastreados padrão: data e hora, operação, nome de usuário (ou &quot;gerado pelo sistema&quot;) e nome do objeto. Os comentários do visualizador Frame.io não estão incluídos.

Essa fase do controle de alterações não inclui eventos MCP. Eles farão parte de uma versão futura.

Para obter mais informações, consulte [Exibir e gerenciar o histórico de alterações](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

<!--

## Internal lookup field replacing Typeahead field type

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

The new **Internal lookup** field type in custom forms provides dynamic filtering. It is similar to the Typeahead field type and allows users to search and select existing Workfront objects by typing part of the name. The filter on the internal lookup can reference the value in another field on the form, which is not possible with Typeaheads.

Multi-select is supported on internal lookups, and this field type also provides improved performance for large datasets. The following native Workfront objects are supported in internal lookups: Project, Company, Group, Job Role, Portfolio, Program, Team, Template, User, Task, Issue, Document, and Location.

The Internal lookup field type is replacing the Typeahead field type. You can quickly convert existing Typeahead fields to Internal lookups by clicking the button in the field options on the right. When you convert, historical data remains on the field and it is used the same way in reports.

>[!IMPORTANT]
>
>External integrations such as Workfront Fusion scenarios or API-based automations may reference legacy field structures and require updates after the conversion. You should verify any integrations before converting Typeahead fields to Internal lookup fields.

For more information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

-->

<!--

## Default value logic supported on native reference fields

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026
>
>This feature is only available for organizations on the Workflow Prime or Ultimate packages.

In custom forms, native reference fields now allow you to add default value logic.

This logic type on native reference fields is available only in the user interface and not in the Workfront API.

For information, see [Add default value logic to a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md#add-default-value-logic-to-a-custom-form) in the article [Add logic rules to custom forms and fields](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).

-->

<!--

## Updates to native field filtering in custom forms

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

System filters that exist on native fields are now applied to the fields in custom forms and are visible to administrators.

When you add a native reference field that has a system filter applied, you can apply the same filter to the field in the custom form and modify the filter if needed in the Text Mode box.

Adding your own custom filter to the field overrides the system filter for the field. If you do not enter a custom filter, the system filter is applied by default.

Also, dynamic filtering is now available on native reference fields. A dynamic filter allows you to narrow the list of items based on the value of another field.

For example, when you use `?portfolioID={portfolio}.{ID}` in a Project field filter and a Portfolio native field is on the custom form, the Project field shows only projects that are in the selected portfolio. If the Portfolio field is left blank, then all projects are available in the Project field.

For information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

-->

<!--

## Protect field names from accidental renaming

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

To protect integrations and data integrity, we've updated how field names can be edited in the field settings panel of a custom form.

Field names in the field settings panel are now read-only by default. You can still edit the field name, but renaming requires an explicit confirmation step. The field previously called **Name** has also been updated to **API Name** to better reflect its technical significance. The **Label** field remains editable.

For information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#notes-on-field-names-and-labels).

-->

## Exibir histórico de alterações para objetos do Workfront

>[!NOTE]
>
>Visualização: 11 de junho de 2026Versão rápida de produção: 11 de junho de 2026Produção para todos: 16 de julho de 2026

Para facilitar a visualização das alterações que ocorreram em uma lista central, criamos a Lista do histórico de alterações. Essa lista exibe informações como o objeto, a operação e a origem da alteração (como um usuário ou o sistema Workfront).

Anteriormente, os logs de auditoria estavam disponíveis, mas não cobriam objetos.

Para obter mais informações, consulte [Exibir e gerenciar o histórico de alterações](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

## Nova preferência do sistema para converter portfólios de armazenamento herdados em armazenamento em nuvem Adobe

>[!NOTE]
>
>Visualização: 11 de junho de 2026Produção para todos: 11 de junho de 2026

Agora, os administradores do Workfront podem converter portfólios de armazenamento herdados para o Adobe Cloud Storage diretamente das Preferências do sistema. Para converter portfólios, selecione-os no novo campo Selecionar portfólios para conversão em armazenamento corporativo e salve a página.

Quando um portfólio é convertido em armazenamento em nuvem do Adobe:

* Não é mais possível mover para esse portfólio os projetos que usam o armazenamento herdado do Workfront
* Todos os novos projetos criados nesse portfólio usam o armazenamento em nuvem da Adobe
* O Frame.io é o visualizador de documentos usando o armazenamento em nuvem do Adobe
* Os objetos secundários que usam o armazenamento Workfront herdado permanecem no armazenamento herdado

Anteriormente, adicionar um projeto de armazenamento em nuvem do Adobe a um portfólio de armazenamento herdado convertia automaticamente o portfólio em armazenamento em nuvem do Adobe.

Para obter mais informações, consulte [Configurar preferências do sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Rich Text substituindo o Texto pelo tipo de campo Formatação

>[!NOTE]
>
>Visualização: 28 de maio de 2026Versão rápida de produção: 11 de junho de 2026Produção para todos: 16 de julho de 2026

O novo tipo de campo **Rich text** em formulários personalizados é um editor de texto robusto, com opções de formatação como sobrescrito e subscrito, cabeçalhos e tabelas, além das opções tradicionais de negrito, itálico, sublinhado, marcadores, numeração, hiperlinks e aspas duplas. O limite de caracteres permanece de 15.000.

O tipo de campo Rich text está substituindo o texto pelo tipo de campo de formatação. Você pode converter rapidamente Texto existente com campos de formatação em Rich text, clicando no botão nas opções de campo à direita. Quando você converte, os dados históricos permanecem no campo e são usados da mesma maneira nos relatórios.

>[!IMPORTANT]
>
>Integrações externas, como cenários do Workfront Fusion ou automações baseadas em API, podem fazer referência a estruturas de campo herdadas e exigir atualizações após a conversão. Você deve verificar todas as integrações antes de converter campos em Rich text.

Para obter mais informações, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Campos financeiros nativos aceitos em formulários personalizados

>[!NOTE]
>
>Visualização: 28 de maio de 2026Versão rápida de produção: 11 de junho de 2026Produção para todos: 16 de julho de 2026

Agora é possível incluir campos financeiros nativos do Workfront em formulários personalizados. Anteriormente, os campos financeiros não eram compatíveis.

Os campos financeiros disponíveis que você pode referenciar dependem do tipo de formulário.

Para obter mais informações, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-workfront-native-fields).

## Os formulários personalizados podem ser compartilhados em todo o sistema com acesso para anexar

>[!NOTE]
>
>Visualização: 28 de maio de 2026Versão rápida de produção: 11 de junho de 2026Produção para todos: 16 de julho de 2026

Uma nova opção de compartilhamento, &quot;Todos no sistema podem visualizar e anexar&quot;, foi adicionada aos formulários personalizados. Ao selecionar essa opção, todos os usuários em todo o sistema podem anexar o formulário a outros objetos.

O compartilhamento em todo o sistema elimina a necessidade de compartilhar formulários manualmente e atualizar permissões entre grupos ou agências quando novos grupos são adicionados.

Para obter mais informações, consulte [Compartilhar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).

## Nova preferência do sistema para exigir campos obrigatórios na edição em massa

>[!NOTE]
>
>Visualização: 28 de maio de 2026Versão rápida de produção: 11 de junho de 2026Produção para todos: 16 de julho de 2026

Atualmente, ao editar objetos em massa, os campos obrigatórios só são aplicados quando um usuário modifica o campo. Se um campo não for modificado, será tratado como opcional e não validado.

Uma nova preferência do sistema agora permite aplicar campos obrigatórios na edição de itens em massa. Para não permitir que objetos editados em massa sejam salvos a menos que todos os campos obrigatórios tenham valores, selecione a opção **Sempre impor campos obrigatórios na edição em massa** na página Configuração > Sistema > Preferências.

Para obter mais informações, consulte [Configurar preferências do sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).
