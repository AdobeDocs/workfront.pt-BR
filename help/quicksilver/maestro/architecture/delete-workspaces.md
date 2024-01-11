---
title: Excluir espaços de trabalho
description: É possível excluir espaços de trabalho quando eles não são mais relevantes.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: ce015eba8291995eec1611917896a0e797f820cc
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Excluir espaços de trabalho

>[!IMPORTANT]
>
>As informações neste artigo referem-se ao Adobe Maestro, que é uma nova oferta da Adobe Workfront.
>
>Atualmente, o Adobe Maestro faz parte de um programa beta aberto a um número limitado de clientes. Você deve ser um cliente do Workfront para usar os recursos do Maestro.
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro-overview.md).

No Adobe Maestri, os espaços de trabalho são locais centralizados para as equipes planejarem o trabalho. Para obter mais informações, consulte [Criar espaços de trabalho](../architecture/delete-workspaces.md).

É possível excluir espaços de trabalho que não são mais relevantes.

É recomendável recriar alguns ou todos os tipos de registros e taxonomias associados ao espaço de trabalho que você deseja excluir em outro espaço de trabalho antes de excluí-lo.

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
   <td role="rowheader"><p>Configuração do nível de acesso</p></td>
   <td> <p>Não há controles de nível de acesso para o Maestro</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>Gerenciar permissões em um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
   <p><b>Nota</b></p>
   Os usuários de licença de trabalhador e solicitação não podem criar um espaço de trabalho, mas podem excluí-lo se tiverem permissões de gerenciamento para ele. 
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

## Considerações sobre a exclusão de espaços de trabalho

* Quando você exclui espaços de trabalho, todos os tipos de registros, taxonomias, registros e seus campos também são excluídos.
* Os espaços de trabalho excluídos e as informações que eles contêm não podem ser recuperados.

## Excluir um espaço de trabalho

1. Clique em **Menu principal** ícone ![](assets/main-menu-workfront.png) no canto superior direito do Workfront ou na guia **Menu principal** ícone ![](assets/main-menu-shell.png)  no canto superior esquerdo, se disponível, clique em **Maestro** ![](assets/maestro-icon.png).

   Essa ação abre o último espaço de trabalho acessado.

1. (Opcional) Expanda a seta apontando para baixo à direita de um nome de espaço de trabalho existente e selecione o espaço de trabalho que deseja excluir.
1. Clique em **Mais** menu ![](assets/more-menu.png) ao lado do nome do espaço de trabalho, clique em **Excluir**.
1. Clique em **Excluir** para confirmar.

   O espaço de trabalho foi excluído e não pode ser recuperado. Quaisquer tipos de registro, taxonomias, seus registros e os campos associados a eles também serão excluídos. <!--ensure this is right after closed beta-->
