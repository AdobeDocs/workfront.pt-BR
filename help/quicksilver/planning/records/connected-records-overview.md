---
title: Visão geral dos registros conectados
description: Depois de criar conexões entre tipos de registro, você pode conectar registros individuais uns aos outros. Este artigo descreve considerações que você deve considerar ao conectar registros no Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: be51023c-8e11-42e7-aa4f-34484c30eb03
source-git-commit: 11d856aeee3bd9edcdc1dbca3964f37bdf83bd00
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---

# Visão geral dos registros conectados

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->

{{planning-important-intro}}

É possível conectar registros do Adobe Workfront Planning uns aos outros ou a objetos de outros aplicativos.

Este artigo descreve considerações que você deve considerar ao conectar registros no Workfront Planning.

Para obter informações sobre como conectar registros uns aos outros ou a outro objeto, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

## Pré-requisitos

Você deve conectar o seguinte antes de poder conectar registros no Workfront Planning:

* Dois tipos de registro
* Um tipo de registro com um objeto de outro aplicativo

Para obter mais informações, consulte [Visão geral dos tipos de registros conectados](/help/quicksilver/planning/architecture/connect-record-types-overview.md).


## Considerações sobre a conexão de registros

* Depois de conectar os tipos de registro, os tipos de registro conectados são exibidos como campos de conexão na tabela dos tipos de registro dos quais estão vinculados e nas páginas dos registros.
* Você pode procurar e adicionar registros e objetos do registro vinculado e tipos de objeto a partir dos campos de registro vinculados.
* É possível adicionar campos (campos de pesquisa) dos tipos de registro vinculados na tabela do tipo de registro a partir do qual você está vinculando.

  Além disso, é possível adicionar campos (campos de pesquisa) dos tipos de registro que você está vinculando na tabela do tipo de registro ao qual você está vinculando.

  Por exemplo, se você vincular o tipo de registro de Produto do tipo de registro de Campanha, será possível exibir campos de produto para campanhas, bem como campos de campanha para produtos.
* Não é possível atualizar manualmente os valores dos campos de pesquisa nos registros a partir dos quais você está vinculando.

  Os valores dos campos de pesquisa preenchem o registro do Workfront Planning que você está vinculando automaticamente depois de serem atualizados no registro ou objeto original.

* Todos os usuários com acesso ao Workfront Planning and View ou permissões mais altas para o espaço de trabalho e um tipo de registro podem ver as conexões que você faz entre registros ou entre registros e objetos de outros aplicativos. Eles podem exibir registros e objetos conectados independentemente de suas permissões nos aplicativos aos quais você está se conectando.
* Você poderá exibir e editar as conexões de todos os outros usuários se tiver permissões de Gerenciamento para o espaço de trabalho e o tipo de registro em que estão os registros conectados.
* É possível conectar um registro a um ou vários objetos de outro aplicativo., dependendo do tipo de conexão selecionado ao conectar os tipos de registro. Para obter mais informações, consulte a seção &quot;Tipos de conexões&quot; no artigo [Visão geral sobre tipos de registros conectados](/help/quicksilver/planning/architecture/connect-record-types-overview.md).
* Quando os tipos de registro conectados fazem parte de hierarquias, você pode acessar qualquer tipo de objeto dentro da hierarquia a partir das páginas dos registros. Para obter informações, consulte [Visão geral sobre hierarquia e navegação estrutural](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).
* Quando os tipos de registro conectados fazem parte de hierarquias, você pode conectar um registro de um tipo de registro-filho a até 10 registros de um tipo de registro-pai. Para obter informações, consulte [Visão geral sobre hierarquia e navegação estrutural](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

## Áreas em que é possível conectar registros

É possível conectar registros manual ou automaticamente no Workfront.

### Conectar registros manualmente

Você pode conectar registros manualmente a outros registros ou a objetos de outro aplicativo nas seguintes áreas:

* Você pode conectar registros do Workfront Planning a objetos do Workfront, objetos do Experience Manager Assets ou Marcas da GenStudio nas seguintes áreas de um registro do Planning:

   * Os campos de registro conectados na exibição de tabela de um tipo de registro no Planning.
   * Os campos de registro conectados na página de visualização ou de detalhes de um registro.
   * A página de visualização ou de detalhes do registro na página Registros conectados de um registro.

* Você pode conectar objetos do Workfront a registros do Workfront Planning nas seguintes áreas do Workfront:

   * A seção Planejamento de um objeto do Workfront.
   * Um campo de conexão do Planning no formulário personalizado de um objeto do Workfront.

  Para obter informações, consulte [Gerenciar conexões de registro de objetos do Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md).

### Conectar registros automaticamente

Depois de conectar tipos de registro uns aos outros ou um tipo de registro a um tipo de objeto de outro aplicativo, você pode conectar registros e objetos automaticamente das seguintes maneiras:

* Uso de automações

  Você pode criar registros ou objetos Workfront a partir de um registro do Planning no qual você configura automações.

  Quando uma condição definida é atendida, um registro ou um objeto é criado e é automaticamente conectado ao registro do qual você está acionando a automação.

  Para obter informações, consulte [Configurar automações do Adobe Workfront Planning](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

* Uso de formulários de solicitação para criar registros

  É possível criar registros ao submeter uma solicitação do Planning. A solicitação e o registro são conectados automaticamente.

  >[!NOTE]
  >
  >Não é possível desconectar um registro de sua solicitação original.

  Para obter informações, consulte [Enviar solicitações do Adobe Workfront Planning para criar registros](/help/quicksilver/planning/requests/submit-requests.md).
