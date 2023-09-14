---
title: Excluir tipos de registro
description: Você pode deletar tipos de registros operacionais ou tipos de registros de taxonomia quando eles não forem mais relevantes.
hidefromtoc: true
hide: true
source-git-commit: 14b456f32dd2c8735e0a5252387f25305efc7610
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 1%

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
>Atualmente, o Adobe Maestro faz parte de um programa beta fechado que está aberto a um número limitado de clientes.
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro-overview.md).

Você pode deletar tipos de registros operacionais ou tipos de registros de taxonomia quando eles não forem mais relevantes.

Para obter informações sobre tipos de registros e taxonomias, consulte [Visão geral dos tipos de registro e taxonomias](../architecture-and-fields/overview-of-record-types-and-taxonomies.md).

É recomendável recriar os campos e os registros associados ao tipo de registro ou taxonomia que você deseja excluir em outro tipo de registro antes de excluí-los.

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> produto Adobe</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>contrato do Adobe Workfront</p></td>
   <td>
<p>Sua organização deve estar inscrita no programa beta fechado do Adobe Maestro. Entre em contato com seu representante de conta para obter mais informações sobre esta nova oferta. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plano do Adobe Workfront</p></td>
   <td>
<p>Qualquer Um</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td>
   <td>
   <p>Qualquer Um</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Nível de acesso</td>
   <td> <p>Qualquer Um</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Modelo de layout</td>
   <td> <p>O administrador do sistema deve adicionar a área Maestro no modelo de layout. Para obter informações, consulte <a href="../access/grant-access.md">Conceder acesso ao Adobe Maestro</a>. </p>  
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

* É possível excluir qualquer tipo de registro ou taxonomia criada por você ou por qualquer pessoa da organização. <!--this will change with access levels and permissions-->
* A exclusão de tipos de registro remove todas as informações associadas a eles, incluindo campos e registros desse tipo.
* Não é possível recuperar tipos de registros excluídos ou suas informações.

## Excluir tipos de registro

A exclusão de tipos de registro de taxonomia é idêntica à exclusão de tipos de registro operacionais.

1. Clique em **Menu principal** ícone ![](assets/main-menu-workfront.png) no canto superior direito do Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> e clique em **Maestro** ![](assets/maestro-icon.png).

   O espaço de trabalho acessado por último deve ser aberto por padrão.

1. (Opcional) Expanda a seta apontando para baixo à direita de um nome de espaço de trabalho existente e selecione o espaço de trabalho para o qual deseja excluir tipos de registro.

   O espaço de trabalho é aberto e os tipos de registro e taxonomias associadas a ele são exibidos.
1. Clique no cartão referente ao tipo de registro ou à taxonomia que deseja excluir.

   Essa ação abre a página do tipo de registro.
1. Clique em **Mais** menu ![](assets/more-menu.png) à direita do nome do tipo de registro e clique em **Excluir**.
1. Clique em **Excluir** para confirmar.

   O tipo ou a taxonomia de registro selecionada, juntamente com seus campos e registros associados, são excluídos.