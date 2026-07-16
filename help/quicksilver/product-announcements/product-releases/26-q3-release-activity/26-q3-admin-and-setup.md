---
title: Aprimoramentos do administrador no terceiro trimestre de 2026
description: Aprimoramentos do administrador no terceiro trimestre de 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 46db578d2412d622818a599cfb27ec4ae73a5298
workflow-type: tm+mt
source-wordcount: '1553'
ht-degree: 5%

---

# Aprimoramentos do administrador no terceiro trimestre de 2026

Esta página descreve as melhorias de Administrador feitas com a versão do terceiro trimestre de 2026 no ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de produção, conforme indicado.

Para obter uma lista de todas as alterações disponíveis neste momento no ciclo de lançamento do terceiro trimestre de 2026, consulte [Visão geral da versão do terceiro trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

<!--

## Change tracking for unified review and approval

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

The Change History page in Workfront now captures activity across unified review and approval workflows, giving administrators a complete governance trail for review and document lifecycle events.

Approval, stage, and participant actions are now tracked. These actions may include:

* Making an approval decision in the Frame.io viewer
* Creating or deleting an approval
* Updating a document such as renaming, moving, or deleting it

Each entry includes the standard tracked fields: date and time, operation, user name (or "system generated"), and object name. Frame.io viewer comments are not included.

This phase of change tracking does not include MCP events. Those will be part of a future release.

For more information, see [View and manage change history](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

-->

## Campos do novo tipo de licença para Níveis de Acesso

>[!NOTE]
>
>Pré-visualização e produção para todos os clientes: 16 de julho de 2026
>
>[!BADGE Fora do cronograma]{type=Neutral}

Fizemos as seguintes alterações de campo na caixa Nível de acesso:

* Renomeamos o campo Tipo de licença na caixa Nível de acesso para Tipo de licença de fluxo de trabalho. Não há alterações de funcionalidade com esta renomeação.\
  Para obter informações,[consulte Criar e modificar níveis de acesso personalizados](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Para clientes que também compraram um pacote do Workfront Planning, adicionamos um novo campo Tipo de Licença do Planning para ilustrar a licença de um usuário no Workfront Planning.
Os clientes que compraram um número igual de licenças do Workflow e do Planning têm os seguintes tipos de licença disponíveis:

   * Planejamento padrão
   * Colaborador de planejamento
   * Nenhum

  >[!NOTE]
  >
  >Você pode atribuir aos usuários uma combinação mista de licenças entre o Workflow e o Planning, mas o tipo de licença do Planning não pode ser superior ao tipo de licença do Workflow.
  >
  >Por exemplo, uma licença do Planning Standard não pode ser atribuída a um usuário do Colaborador do Fluxo de Trabalho. Um usuário com uma licença do Workflow Light agora pode receber uma licença Standard para o Planning e, portanto, gerenciar espaços de trabalho e seu conteúdo. Anteriormente, só era possível ter acesso somente para visualização aos dados do Planning.
  >
  >Os novos clientes podem adquirir licenças de Planejamento e Fluxo de Trabalho em quantidades diferentes e usá-las com qualquer combinação. Nesse cenário, o tipo de licença Colaborador do Planning não está disponível.
  >
  >Para obter informações, consulte [Visão geral sobre acesso ao Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).

## Campo de pesquisa interna que substitui o tipo de campo Digitação antecipada

>[!NOTE]
>
>Visualização: 7 de julho de 2026
>Versão rápida de produção: 15 de julho de 2026
>Produção para todos: 16 de julho de 2026

O novo tipo de campo **Pesquisa interna** em formulários personalizados fornece filtragem dinâmica. É semelhante ao tipo de campo Digitação antecipada e permite que os usuários pesquisem e selecionem objetos existentes do Workfront digitando parte do nome. O filtro na pesquisa interna pode fazer referência ao valor em outro campo do formulário, o que não é possível com Typeaheads.

A seleção múltipla é compatível com pesquisas internas, e esse tipo de campo também fornece desempenho aprimorado para conjuntos de dados grandes. Os seguintes objetos nativos do Workfront são suportados em pesquisas internas: Projeto, Empresa, Grupo, Função de trabalho, Portfolio, Programa, Equipe, Modelo, Usuário, Tarefa, Problema, Documento e Local.

O tipo de campo de pesquisa interna está substituindo o tipo de campo Digitação antecipada. Você pode converter rapidamente campos Typeahead existentes em pesquisas internas clicando no botão nas opções de campo à direita. Quando você converte, os dados históricos permanecem no campo e são usados da mesma maneira nos relatórios.

>[!IMPORTANT]
>
>Integrações externas, como cenários do Workfront Fusion ou automações baseadas em API, podem fazer referência a estruturas de campo herdadas e exigir atualizações após a conversão. Você deve verificar todas as integrações antes de converter campos de Digitação antecipada em campos de pesquisa interna.

Para obter mais informações, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Lógica de valor padrão compatível com campos de referência nativos

>[!NOTE]
>
>Visualização: 7 de julho de 2026
>Versão rápida de produção: 15 de julho de 2026
>Produção para todos: 16 de julho de 2026
>
>Esse recurso só está disponível para organizações nos pacotes Prime ou Ultimate do fluxo de trabalho.

Em formulários personalizados, os campos de referência nativos agora permitem adicionar a lógica de valor padrão.

Esse tipo lógico em campos de referência nativos está disponível somente na interface do usuário e não na API do Workfront.

Para obter informações, consulte [Adicionar lógica de valor padrão a um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md#add-default-value-logic-to-a-custom-form) no artigo [Adicionar regras de lógica a formulários e campos personalizados](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).

## Atualizações na filtragem de campo nativo em formulários personalizados

>[!NOTE]
>
>Visualização: 7 de julho de 2026
>Versão rápida de produção: 15 de julho de 2026
>Produção para todos: 16 de julho de 2026

Os filtros de sistema que existem em campos nativos agora são aplicados aos campos em formulários personalizados e estão visíveis para administradores.

Ao adicionar um campo de referência nativo que tenha um filtro de sistema aplicado, você pode aplicar o mesmo filtro ao campo no formulário personalizado e modificar o filtro, se necessário, na caixa Modo de texto.

Adicionar seu próprio filtro personalizado ao campo substitui o filtro do sistema para o campo. Se você não inserir um filtro personalizado, o filtro do sistema será aplicado por padrão.

Além disso, a filtragem dinâmica agora está disponível em campos de referência nativos. Um filtro dinâmico permite restringir a lista de itens com base no valor de outro campo.

Por exemplo, quando você usa `?portfolioID={portfolio}.{ID}` em um filtro de campo de Projeto e um campo nativo do Portfolio está no formulário personalizado, o campo Projeto mostra somente os projetos que estão no portfólio selecionado. Se o campo Portfolio for deixado em branco, todos os projetos estarão disponíveis no campo Projeto.

Para obter informações, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Proteger nomes de campo contra renomeação acidental

>[!NOTE]
>
>Visualização: 7 de julho de 2026
>Versão rápida de produção: 15 de julho de 2026
>Produção para todos: 16 de julho de 2026

Para proteger as integrações e a integridade dos dados, atualizamos como os nomes de campo podem ser editados no painel de configurações de campo de um formulário personalizado.

Os nomes de campos no painel de configurações de campo agora são somente leitura por padrão. Você ainda pode editar o nome do campo, mas renomear requer uma etapa de confirmação explícita. O campo anteriormente chamado **Nome** também foi atualizado para **Nome da API** para refletir melhor seu significado técnico. O campo **Rótulo** permanece editável.

Para obter informações, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#notes-on-field-names-and-labels).

## Exibir histórico de alterações para objetos do Workfront

>[!NOTE]
>
>Visualização: 11 de junho de 2026
>Versão rápida de produção: 11 de junho de 2026
>Produção para todos: 16 de julho de 2026

Para facilitar a visualização das alterações que ocorreram em uma lista central, criamos a Lista do histórico de alterações. Essa lista exibe informações como o objeto, a operação e a origem da alteração (como um usuário ou o sistema Workfront).

Anteriormente, os logs de auditoria estavam disponíveis, mas não cobriam objetos.

Para obter mais informações, consulte [Exibir e gerenciar o histórico de alterações](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

## Nova preferência do sistema para converter portfólios de armazenamento herdados em armazenamento em nuvem Adobe

>[!NOTE]
>
>Visualização: 11 de junho de 2026
>Produção para todos: 11 de junho de 2026
>[!BADGE Fora do cronograma]{type=Neutral}

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
>Visualização: 28 de maio de 2026
>Versão rápida de produção: 11 de junho de 2026
>Produção para todos: 16 de julho de 2026

O novo tipo de campo **Rich text** em formulários personalizados é um editor de texto robusto, com opções de formatação como sobrescrito e subscrito, cabeçalhos e tabelas, além das opções tradicionais de negrito, itálico, sublinhado, marcadores, numeração, hiperlinks e aspas duplas. O limite de caracteres permanece de 15.000.

O tipo de campo Rich text está substituindo o texto pelo tipo de campo de formatação. Você pode converter rapidamente Texto existente com campos de formatação em Rich text, clicando no botão nas opções de campo à direita. Quando você converte, os dados históricos permanecem no campo e são usados da mesma maneira nos relatórios.

>[!IMPORTANT]
>
>Integrações externas, como cenários do Workfront Fusion ou automações baseadas em API, podem fazer referência a estruturas de campo herdadas e exigir atualizações após a conversão. Você deve verificar todas as integrações antes de converter campos em Rich text.

Para obter mais informações, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Campos financeiros nativos aceitos em formulários personalizados

>[!NOTE]
>
>Visualização: 28 de maio de 2026
>Versão rápida de produção: 11 de junho de 2026
>Produção para todos: 16 de julho de 2026

Agora é possível incluir campos financeiros nativos do Workfront em formulários personalizados. Anteriormente, os campos financeiros não eram compatíveis.

Os campos financeiros disponíveis que você pode referenciar dependem do tipo de formulário.

Para obter mais informações, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-workfront-native-fields).

## Os formulários personalizados podem ser compartilhados em todo o sistema com acesso para anexar

>[!NOTE]
>
>Visualização: 28 de maio de 2026
>Versão rápida de produção: 11 de junho de 2026
>Produção para todos: 16 de julho de 2026

Uma nova opção de compartilhamento, &quot;Todos no sistema podem visualizar e anexar&quot;, foi adicionada aos formulários personalizados. Ao selecionar essa opção, todos os usuários em todo o sistema podem anexar o formulário a outros objetos.

O compartilhamento em todo o sistema elimina a necessidade de compartilhar formulários manualmente e atualizar permissões entre grupos ou agências quando novos grupos são adicionados.

Para obter mais informações, consulte [Compartilhar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).

## Nova preferência do sistema para exigir campos obrigatórios na edição em massa

>[!NOTE]
>
>Visualização: 28 de maio de 2026
>Versão rápida de produção: 11 de junho de 2026
>Produção para todos: 16 de julho de 2026

Atualmente, ao editar objetos em massa, os campos obrigatórios só são aplicados quando um usuário modifica o campo. Se um campo não for modificado, será tratado como opcional e não validado.

Uma nova preferência do sistema agora permite aplicar campos obrigatórios na edição de itens em massa. Para não permitir que objetos editados em massa sejam salvos a menos que todos os campos obrigatórios tenham valores, selecione a opção **Sempre impor campos obrigatórios na edição em massa** na página Configuração > Sistema > Preferências.

Para obter mais informações, consulte [Configurar preferências do sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).
