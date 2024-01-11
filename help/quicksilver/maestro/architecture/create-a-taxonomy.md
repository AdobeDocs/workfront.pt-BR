---
title: Criar tipos de registro de taxonomia
description: Taxonomias são um tipo de registro reutilizável que captura atributos sobre um tipo de registro operacional no Adobe Workfront Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: e90a3ebe-fc02-4cce-8472-1ca5004ddde8
source-git-commit: ce015eba8291995eec1611917896a0e797f820cc
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Criar tipos de registro de taxonomia

>[!IMPORTANT]
>
>As informações neste artigo referem-se ao Adobe Maestro, que é uma nova oferta da Adobe Workfront.
>
>Atualmente, o Adobe Maestro faz parte de um programa beta aberto a um número limitado de clientes. Você deve ser um cliente do Workfront para usar os recursos do Maestro.
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro-overview.md).

Taxonomias são tipos de registro que capturam atributos sobre tipos de registro operacional no Adobe Maestro.

Por exemplo, a campanha pode ser um tipo de registro operacional. A seguir estão taxonomias que capturam atributos sobre o tipo de registro do Campaign: Região, Público-alvo, País.

Para obter mais informações sobre os tipos de registros do Maestro, consulte [Visão geral dos tipos de registro e taxonomias](../architecture/overview-of-record-types-and-taxonomies.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produto</p> </td>
   <td>
   <p> Adobe Workfront</p> <p>Para conectar tipos de registro Maestri com a Experience Manager Assets, você deve ter uma licença Adobe Experience Manager Assets e a instância da Workfront de sua organização deve ser integrada à Adobe Business Platform ou à Adobe Admin Console.</p> </td>
  </tr>  
 <td role="rowheader"><p>contrato do Adobe Workfront</p></td>
   <td>
<p>Sua organização deve estar inscrita no programa beta fechado do Adobe Maestro. Entre em contato com seu representante de conta para obter mais informações sobre esta nova oferta. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plano do Adobe Workfront</p></td>
   <td>
<p>Qualquer</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td>
   <td>
   <p>Qualquer</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurações de nível de acesso</p></td>
   <td> <p>Não há controles de nível de acesso para o Maestro</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>O administrador do Workfront ou do grupo deve adicionar a área Maestri no modelo de layout. Para obter informações, consulte <a href="../access/access-overview.md">Visão geral do Access</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>Gerenciar permissões em um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Considerações sobre a criação de taxonomias

* Você deve criar um espaço de trabalho antes de criar taxonomias no espaço de trabalho.

  Para obter informações sobre espaços de trabalho, consulte [Criar espaços de trabalho](../architecture/create-workspaces.md).
* Você pode criar um tipo de registro de taxonomia seguindo um destes procedimentos:
   * Crie-os automaticamente ao criar um espaço de trabalho usando um modelo. Para obter informações, consulte [Criar espaços de trabalho](../architecture/create-workspaces.md).
   * Crie-os manualmente, do zero.
   * Crie-os manualmente colando informações de uma lista externa.

  <!--this is not possible yet:
  * You can taxonomies to a workspace by doing one of the following:
    * Create a connection to object types from other systems, when adding fields to a taxnomy record type. This creates a read-only record type in Maestro.  - update this sentence when you can connect taxonomies as well as operational records to a third-party system.-->

* Todas as taxonomias recém-criadas vêm com os seguintes campos:

   * Nome <!--if there won't be any more fields, consider rephrasing this-->

  Além disso, é possível adicionar campos personalizados a taxonomias. Para obter mais informações, consulte [Criar campos](../fields/create-fields.md).

  >[!NOTE]
  >
  >    As taxonomias criadas ao usar um modelo de espaço de trabalho têm campos adicionais.

## Criar uma taxonomia

A criação de taxonomias é semelhante à criação de um tipo de registro operacional do zero ou de um modelo de espaço de trabalho.

Para obter informações, consulte a seção &quot;Criar um tipo de registro do zero&quot; no artigo [Criar tipos de registro](../architecture/create-record-types.md).

Para obter informações sobre como criar taxonomias automaticamente ao criar um espaço de trabalho a partir de um modelo, consulte [Criar espaços de trabalho](../architecture/create-workspaces.md).
