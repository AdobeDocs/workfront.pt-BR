---
title: Excluir espaços de trabalho
description: É possível excluir espaços de trabalho quando eles não são mais relevantes.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: ded6db27fa3fba9195e2133134f60bcadb0f897a
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Excluir espaços de trabalho

{{planning-important-intro}}

No Adobe Workfront Planning, os espaços de trabalho são locais centralizados para as equipes planejarem o trabalho. Para obter mais informações, consulte [Criar espaços de trabalho](/help/quicksilver/planning/architecture/create-workspaces.md).

É possível excluir espaços de trabalho que não são mais relevantes.

Recomendamos recriar alguns ou todos os tipos de registros, registros, campos e views associados ao espaço de trabalho que você deseja excluir em outro espaço de trabalho antes de excluí-lo.

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso do Workfront Planning.

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
<p>Sua organização deve estar inscrita no estágio de acesso antecipado do Workfront Planning </p>
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
   <td> <p>Gerenciar permissões para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>

</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>O administrador do Workfront ou do grupo deve adicionar a área do Planning ao modelo de layout. Para obter informações, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Visão geral sobre acesso</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Para obter mais informações sobre requisitos de acesso, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Considerações sobre a exclusão de espaços de trabalho

* Quando você exclui espaços de trabalho, todos os tipos de registro, registros, campos e exibições também são excluídos.
* Os espaços de trabalho excluídos e as informações que eles contêm não podem ser recuperados.

## Excluir um espaço de trabalho

{{step1-to-planning}}

1. (Condicional) Se você for um administrador do Workfront, clique em **Espaços de trabalho em que estou** para acessar os espaços de trabalho que você criou ou em **Outros espaços de trabalho** para acessar os espaços de trabalho que outras pessoas compartilharam com você.

1. (Opcional) Clique em **Mostrar tudo** para exibir espaços de trabalho adicionais. O link **Mostrar tudo** é exibido somente quando há mais de duas linhas de cartões de espaço de trabalho.
1. (Opcional) Clique em K **Mostrar menos** para limitar o número de espaços de trabalho exibidos na tela.
1. Para deletar um espaço de trabalho, siga um destes procedimentos:

   * Passe o mouse sobre o cartão de espaço de trabalho e clique no menu **Mais** ![](assets/more-menu.png), no canto superior direito do cartão
Ou
   * Clique em um cartão de espaço de trabalho para abrir o espaço de trabalho e no menu **Mais** ![](assets/more-menu.png) à direita do nome do espaço de trabalho.
1. Clique em **Excluir**.

   ![](assets/permanently-delete-workspace-confirmation.png)

1. Digite &quot;**delete**&quot; no espaço fornecido e clique em **Excluir permanentemente**. Isso não diferencia maiúsculas de minúsculas.

   O espaço de trabalho foi excluído e não pode ser recuperado. Quaisquer tipos de registro, registros, campos e exibições associados a eles também são excluídos. <!--ensure this is right at or before GA-->
