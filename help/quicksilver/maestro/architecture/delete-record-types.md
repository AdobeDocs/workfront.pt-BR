---
title: Excluir tipos de registro
description: Você pode deletar tipos de registros operacionais ou tipos de registros de taxonomia quando eles não forem mais relevantes.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: ce015eba8291995eec1611917896a0e797f820cc
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav:
---
title: Delete record types
description: You can delete operational record types or taxonomy record types when they are no longer relevant. 
author: Alina
feature: Work Management
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->

# Excluir tipos de registro

>[!IMPORTANT]
>
>As informações neste artigo referem-se ao Adobe Maestro, que é uma nova oferta da Adobe Workfront.
>
>Atualmente, o Adobe Maestro faz parte de um programa beta aberto a um número limitado de clientes. Você deve ser um cliente do Workfront para usar os recursos do Maestro.
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro-overview.md).

Você pode deletar tipos de registros operacionais ou tipos de registros de taxonomia quando eles não forem mais relevantes.

Para obter informações sobre tipos de registros e taxonomias, consulte [Visão geral dos tipos de registro e taxonomias](../architecture/overview-of-record-types-and-taxonomies.md).

É recomendável recriar os campos e os registros associados ao tipo de registro ou taxonomia que você deseja excluir em outro tipo de registro antes de excluí-los.

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

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
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>Gerenciar permissões em um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>O administrador do Workfront ou do grupo deve adicionar a área Maestri no modelo de layout. Para obter informações, consulte <a href="../access/access-overview.md">Visão geral do Access</a>. </p>  
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

## Considerações ao excluir tipos de registro

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* Você pode excluir somente tipos de registro ou taxonomias de espaços de trabalho para os quais tenha Gerenciar permissões.
* A exclusão de tipos de registro remove todas as informações associadas a eles, incluindo campos e registros desse tipo. O tipo de registro é removido de todos os usuários que acessam o espaço de trabalho.
* Não é possível recuperar tipos de registros excluídos ou suas informações.

## Excluir tipos de registro

A exclusão de tipos de registro de taxonomia é idêntica à exclusão de tipos de registro operacionais.

{{step1-to-maestro}}

O espaço de trabalho acessado por último deve ser aberto por padrão.

1. (Opcional) Expanda a seta apontando para baixo à direita de um nome de espaço de trabalho existente e selecione o espaço de trabalho para o qual deseja excluir tipos de registro.

   O espaço de trabalho é aberto e os tipos de registro e taxonomias associadas a ele são exibidos.
1. Clique no cartão referente ao tipo de registro ou à taxonomia que deseja excluir.

   Essa ação abre a página do tipo de registro.
1. Clique em **Mais** menu ![](assets/more-menu.png) à direita do nome do tipo de registro e clique em **Excluir**.
1. Clique em **Excluir** para confirmar.

   O tipo ou a taxonomia de registro selecionada, juntamente com seus campos e registros associados, são excluídos.
