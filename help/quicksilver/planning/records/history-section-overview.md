---
title: Visão geral da seção Histórico
description: Você pode revisar as alterações feitas no registro e registradas pelo sistema no painel direito de um registro no Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 8258589f-a7c3-4d77-9abe-c99e9184bd21
source-git-commit: 6c50746c4c230d7f9fa2c73b66d13c8b02153b89
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 4%

---

# Visão geral da seção Histórico

{{planning-important-intro}}

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Workfront Planning records" should be there-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->

É possível colaborar em registros do Adobe Workfront Planning, adicionando comentários ou respostas no painel direito de um registro. Você também pode exibir outras alterações feitas no registro e registradas pelo sistema nessa área.

O painel direito de um registro exibe as seguintes seções:

* **Comentários**: exibe comentários e respostas que os usuários adicionam aos registros. Para obter mais informações sobre o gerenciamento de comentários em registros do Workfront Planning, consulte [Gerenciar comentários de registro](/help/quicksilver/planning/records/manage-record-comments.md).
* **Histórico**: exibe as alterações registradas pelo sistema que os usuários fazem nos campos de registro.

## Localizar a seção Histórico de um registro

{{step1-to-planning}}

O último espaço de trabalho acessado é aberto por padrão.

1. Escolha uma exibição de tabela na **Exibir** menu suspenso.
1. Clique no nome de um registro na exibição de tabela.

   A página do registro é aberta. A área Comentários é aberta por padrão no painel direito.
1. Clique em **Mostrar histórico** ícone ![](assets/show-history-icon.png). Todas as alterações feitas nos campos do registro são exibidas no painel direito, começando pela mais recente.
1. (Opcional) Clique no link **Ocultar histórico** ícone ![](assets/hide-history-icon.png) para fechar o painel direito.

## Considerações sobre a seção Histórico

Você pode revisar as alterações feitas nos campos de registro na seção History do painel direito da página de um registro.

![](assets/history-area-in-comments.png)

* O Workfront Planning registra as seguintes informações na seção Histórico:

   * Quaisquer alterações de campo

   * Os valores antigos e novos dos campos, quando os valores são alterados. Os valores antigos são exibidos em formato tachado.

   * O nome completo do usuário que fez a alteração

   * Uma data e carimbo de data e hora de quando a alteração ocorreu.

* Os campos dos seguintes tipos sempre exibem o valor antigo (em formato tachado) e o novo valor:

   * Texto
   * Parágrafo
   * Moeda
   * Data
   * Número
   * Percentagem
   * Seleção única

* Os campos dos seguintes tipos mostram o valor antigo no formato tachado somente se pelo menos um dos valores múltiplos tiver sido removido:

   * Seleção múltipla
   * Campos de registro vinculados
   * Pessoas

  Se a alteração adicionar apenas valores ao campo, o valor antigo não será exibido e somente o novo valor do campo será exibido.

* Os campos do tipo caixa de seleção nunca exibem o valor antigo no formato tachado. Se o campo for editado, somente o estado atual no momento em que a alteração foi feita será exibido.

  Para obter mais informações sobre campos do Workfront Planning, consulte [Criar campos](/help/quicksilver/planning/fields/create-fields.md).

* As alterações nos campos dos seguintes tipos não são exibidas na seção History:

   * Campos vinculados (pesquisa)
   * Fórmula
   * Criado por
   * Criado na data
   * Modificado pela última vez por
   * Data da última modificação

* Se um campo for removido do sistema, as atualizações feitas nesse campo permanecerão na seção Histórico. Não há nenhuma indicação de que o campo foi removido na seção Histórico de um registro.
