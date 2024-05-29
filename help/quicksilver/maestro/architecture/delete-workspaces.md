---
title: Excluir espaços de trabalho
description: É possível excluir espaços de trabalho quando eles não são mais relevantes.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: 44073ea242803e28ca00c82811ae2865747d11c3
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Excluir espaços de trabalho

{{maestro-important-intro}}

No Adobe Workfront Planning, os espaços de trabalho são locais centralizados para as equipes planejarem o trabalho. Para obter mais informações, consulte [Criar espaços de trabalho](../architecture/delete-workspaces.md).

É possível excluir espaços de trabalho que não são mais relevantes.

Recomendamos recriar alguns ou todos os tipos de registros, registros, campos e views associados ao espaço de trabalho que você deseja excluir em outro espaço de trabalho antes de excluí-lo.

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
<p>Sua organização deve estar inscrita no programa beta de planejamento do Adobe Workfront. Entre em contato com seu representante de conta para obter mais informações sobre esta nova oferta. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plano do Adobe Workfront</p></td>
   <td>
<p>Qualquer</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td>
   <td>
   <p>Novo: Padrão</p>
   <p>Atual: Plano</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuração do nível de acesso</p></td>
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>Gerenciar permissões em um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>

</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>O administrador do Workfront ou do grupo deve adicionar a área do Planning ao modelo de layout. Para obter informações, consulte <a href="../access/access-overview.md">Visão geral do Access</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Para obter mais informações sobre requisitos de acesso, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Considerações sobre a exclusão de espaços de trabalho

* Quando você exclui espaços de trabalho, todos os tipos de registro, registros, campos e exibições também são excluídos.
* Os espaços de trabalho excluídos e as informações que eles contêm não podem ser recuperados.

## Excluir um espaço de trabalho

{{step1-to-maestro}}

Essa ação abre o último espaço de trabalho acessado.

1. (Opcional) Expanda a seta apontando para baixo à direita de um nome de espaço de trabalho existente e selecione o espaço de trabalho que deseja excluir.
1. Clique em **Mais** menu ![](assets/more-menu.png) ao lado do nome do espaço de trabalho, clique em **Excluir**.
   <!--1. Type "**delete**" in the space provided, then click **Permanently delete**. **********AND DELETE THE STEP BELPW EXCEPT FOR THE LAST SENTENCE***********-->

1. Clique em **Excluir** para confirmar.

   O espaço de trabalho foi excluído e não pode ser recuperado. Quaisquer tipos de registro, registros, campos e exibições associados a eles também são excluídos. <!--ensure this is right after closed beta-->
