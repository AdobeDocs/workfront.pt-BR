---
title: Visão geral dos registros conectados
description: Depois de criar conexões entre tipos de registro, você pode conectar registros individuais uns aos outros. Este artigo descreve considerações que você deve considerar ao conectar registros no Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: be51023c-8e11-42e7-aa4f-34484c30eb03
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 0%

---

# Visão geral dos registros conectados

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>  -->

{{planning-important-intro}}

É possível conectar registros do Adobe Workfront Planning uns aos outros ou a objetos de outros aplicativos.

Este artigo descreve considerações que você deve considerar ao conectar registros no Adobe Workfront Planning.

Para obter informações sobre como conectar registros uns aos outros ou a outro objeto, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).


## Considerações sobre a conexão de registros

* Depois de conectar os tipos de registro, os tipos de registro conectados são exibidos como campos de registro vinculados na tabela dos tipos de registro a partir dos quais estão vinculados e nas páginas dos registros.
* Você pode procurar e adicionar registros e objetos do registro vinculado e tipos de objeto a partir dos campos de registro vinculados.
* É possível adicionar campos (campos de pesquisa) dos tipos de registro vinculados na tabela do tipo de registro a partir do qual você está vinculando.

  Além disso, é possível adicionar campos (campos de pesquisa) dos tipos de registro que você está vinculando na tabela do tipo de registro ao qual você está vinculando.

  Por exemplo, se você vincular o tipo de registro de Produto do tipo de registro de Campanha, será possível exibir campos de produto para campanhas, bem como campos de campanha para produtos.
* Não é possível atualizar manualmente os valores dos campos de pesquisa nos registros a partir dos quais você está vinculando.

  Os valores dos campos de pesquisa preenchem o registro do Workfront Planning que você está vinculando automaticamente depois de serem atualizados no registro ou objeto original.

* Todos os usuários com acesso ao Workfront Planning and View ou permissões mais altas para o espaço de trabalho e um tipo de registro podem ver as conexões que você faz entre registros ou entre registros e objetos de outros aplicativos. Eles podem exibir registros e objetos conectados independentemente de suas permissões nos aplicativos aos quais você está se conectando.
* Você poderá exibir e editar as conexões de todos os outros usuários se tiver permissões de Gerenciamento para o espaço de trabalho e o tipo de registro em que estão os registros conectados.
* É possível conectar um registro a um ou vários objetos de outro aplicativo., dependendo do tipo de conexão selecionado ao conectar os tipos de registro. Para obter mais informações, consulte a seção &quot;Tipos de conexões&quot; no artigo [Visão geral sobre tipos de registros conectados](/help/quicksilver/planning/architecture/connect-record-types-overview.md).
  <!--* <span class="preview">If connected record types are part of hierarchies, you can access any object type within the hierarchy from the records' pages. For information, see [Hierarchy and breadcrumb overview](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md). </span>-->

## Áreas em que é possível conectar registros

É possível conectar registros a outros registros ou a objetos de outro aplicativo nas seguintes áreas:

* Você pode conectar registros do Workfront Planning a objetos do Workfront, objetos do Experience Manager Assets ou Marcas da GenStudio nas seguintes áreas de um registro do Planning:

   * Os campos de registro conectados na exibição de tabela de um tipo de registro no Planning.
   * A página de visualização ou detalhes do registro nos campos de registro conectados na guia Detalhes.
   * A página de visualização ou de detalhes do registro na guia Conexões.
   * A página do registro em uma guia da página Registros conectados de um registro conectado.

* Você pode conectar objetos do Workfront a registros do Workfront Planning nas seguintes áreas do Workfront:

   * A seção Planejamento de um objeto do Workfront.
   * Um campo de conexão do Planning no formulário personalizado de um objeto do Workfront.

  Para obter informações, consulte [Gerenciar conexões de registro de objetos do Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md).
