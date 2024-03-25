---
title: Criar tipos de registro de taxonomia
description: Quando você usa um modelo para criar um espaço de trabalho, os tipos de registro são criados nas seções Tipos de Registro Operacionais e Taxonomias.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: e90a3ebe-fc02-4cce-8472-1ca5004ddde8
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 3%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Criar tipos de registro de taxonomia

{{maestro-important-intro}}

Quando você usa um modelo para criar um espaço de trabalho, os tipos de registro são criados nas seguintes seções:

* Tipos de registros operacionais
* Taxonomias

Os tipos de registro na seção Taxonomias de um espaço de trabalho capturam atributos sobre tipos de registro na seção Tipos de Registro Operacionais do mesmo espaço de trabalho.

Por exemplo, a campanha pode ser um tipo de registro operacional. A seguir estão taxonomias que capturam atributos sobre o tipo de registro do Campaign: Região, Público-alvo, País.

Para obter mais informações sobre tipos de registros, consulte [Visão geral dos tipos de registro](../architecture/overview-of-record-types-and-taxonomies.md).

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
   <p> Adobe Workfront</p> <p>Para conectar tipos de registro com o Experience Manager Assets, você deve ter uma licença do Adobe Experience Manager Assets e a instância da Workfront de sua organização deve ser integrada à Adobe Business Platform ou à Adobe Admin Console.</p> </td>
  </tr>  
 <td role="rowheader"><p>contrato do Adobe Workfront</p></td>
   <td>
<p>Sua organização deve estar inscrita no programa beta fechado de planejamento da Adobe Workfront. Entre em contato com seu representante de conta para obter mais informações sobre esta nova oferta. </p>
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
   <td> <p>Não há controles de nível de acesso para o planejamento do Adobe Workfront</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>O administrador do Workfront ou do grupo deve adicionar a área do Planning ao modelo de layout. Para obter informações, consulte <a href="../access/access-overview.md">Visão geral do Access</a>. </p>  
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

* Você deve criar um espaço de trabalho usando um modelo antes de criar tipos de registro na seção Taxonomias do espaço de trabalho.

  Para obter informações sobre espaços de trabalho, consulte [Criar espaços de trabalho](../architecture/create-workspaces.md).
* Você pode criar um tipo de registro na seção Taxonomias de um espaço de trabalho seguindo um destes procedimentos:
   * Crie-os automaticamente ao criar um espaço de trabalho usando um modelo. Para obter informações, consulte [Criar espaços de trabalho](../architecture/create-workspaces.md).
   * Crie-os manualmente, do zero, na seção Taxonomias de um espaço de trabalho.

* Todas as taxonomias recém-criadas têm os seguintes campos por padrão:

   * Nome
   * Descrição
   * Data de início
   * Data Final
   * Status

  Além disso, é possível adicionar campos personalizados a taxonomias. Para obter mais informações, consulte [Criar campos](../fields/create-fields.md).

  >[!NOTE]
  >
  >    Os tipos de registro de taxonomia criados ao usar um modelo de espaço de trabalho têm campos adicionais.

## Criar um tipo de registro de taxonomia

A criação de tipos de registro de taxonomia é semelhante à criação de tipos de registro.

Para obter informações, consulte [Criar tipos de registro](../architecture/create-record-types.md).
