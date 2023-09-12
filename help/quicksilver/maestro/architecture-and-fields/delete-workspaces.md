---
title: Excluir espaços de trabalho
description: É possível excluir espaços de trabalho quando eles não são mais relevantes.
hidefromtoc: true
hide: true
source-git-commit: 71ce412ead1590b8511ec4219d3ba72fbf32b98d
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 1%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Excluir espaços de trabalho

>[!IMPORTANT]
>
>Atualmente, o Adobe Maestro faz parte de um programa beta fechado que está aberto a um número limitado de clientes.
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro-overview.md).

No Adobe Maestri, os espaços de trabalho são locais centralizados para as equipes planejarem o trabalho. Para obter mais informações, consulte [Criar espaços de trabalho](../architecture-and-fields/create-workspaces.md).

É possível excluir espaços de trabalho que não são mais relevantes.

É recomendável recriar alguns ou todos os tipos de registros e taxonomias associados ao espaço de trabalho que você deseja excluir em outro espaço de trabalho antes de excluí-lo.

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

## Considerações sobre a exclusão de espaços de trabalho

* Você pode excluir qualquer espaço de trabalho criado por você ou por qualquer pessoa em sua organização. <!--this will change with access levels and permissions-->
* Quando você exclui espaços de trabalho, todos os tipos de registro, taxonomias e seus campos também são excluídos. <!--asked Lilit because the confirmation says the records don't delete, but not sure how they can exist outside of a workspace?!-->
* Os espaços de trabalho excluídos e as informações que eles contêm não podem ser recuperados.

## Excluir um espaço de trabalho

1. Clique em **Menu principal** ícone ![](assets/main-menu-workfront.png) no canto superior direito do Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> e clique em **Maestro** ![](assets/maestro-icon.png).

   Essa ação abre o último espaço de trabalho acessado.

1. (Opcional) Expanda a seta apontando para baixo à direita de um nome de espaço de trabalho existente e selecione o espaço de trabalho que deseja excluir.
1. Clique em **Mais** menu ![](assets/more-menu.png) ao lado do nome do espaço de trabalho, clique em **Excluir**.
1. Clique em **Excluir** para confirmar.

   O espaço de trabalho foi excluído e não pode ser recuperado. Quaisquer tipos de registro, taxonomias, seus registros e os campos associados a eles também serão excluídos. <!--ensure this is right after closed beta-->
