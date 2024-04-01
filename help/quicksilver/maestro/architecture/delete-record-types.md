---
title: Excluir tipos de registro
description: É possível excluir tipos de registro quando eles não forem mais relevantes. A exclusão de tipos de registro também exclui todas as informações associadas aos tipos de registro, como seus registros, campos e exibições.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: f4fb9d5c22ec6216a05e31cbcf80f1cf9add125f
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:
---
title: Delete record types
description: You can delete record types when they are no longer relevant. 
author: Alina
feature: Work Management
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->

# Excluir tipos de registro

{{maestro-important-intro}}

É possível excluir tipos de registro quando eles não forem mais relevantes.

No entanto, a exclusão de tipos de registro também exclui todas as informações associadas aos tipos de registro. Para obter mais informações, consulte [Considerações ao excluir tipos de registro](#considerations-when-deleting-record-types) neste artigo.

Para obter informações sobre tipos de registros, consulte [Visão geral dos tipos de registro](../architecture/overview-of-record-types-and-taxonomies.md).

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>contrato do Adobe Workfront</p></td>
   <td>
<p>Sua organização deve estar inscrita no programa beta de Planejamento do Adobe Workfront. Entre em contato com seu representante de conta para obter mais informações sobre esta nova oferta. </p>
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
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning</p>  
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
   <td> <p>O administrador do Workfront ou do grupo deve adicionar a área do Planning ao modelo de layout. Para obter informações, consulte <a href="../access/access-overview.md">Visão geral do Access</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Considerações ao excluir tipos de registro

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* Você pode excluir somente tipos de registro de espaços de trabalho para os quais tem permissões de gerenciamento.
* A exclusão de tipos de registro remove as seguintes informações associadas a eles:

   * Todos os registros desse tipo.
   * Todos os campos associados ao tipo de registro.
   * Todas as exibições (incluindo filtros, agrupamentos e critérios de classificação) do tipo de registro.
* O tipo de registro é removido de todos os usuários que acessam o espaço de trabalho.
* Não é possível recuperar tipos de registros excluídos ou suas informações.
* É recomendável recriar os campos e os registros associados ao tipo de registro que você deseja excluir em outro tipo de registro antes de excluí-los.

## Excluir tipos de registro

{{step1-to-maestro}}

O espaço de trabalho acessado por último deve ser aberto por padrão.

1. (Opcional) Expanda a seta apontando para baixo à direita de um nome de espaço de trabalho existente e selecione o espaço de trabalho para o qual deseja excluir tipos de registro.

   O espaço de trabalho é aberto e os tipos de registro são exibidos.
1. Clique no cartão do tipo de registro que deseja excluir.

   Essa ação abre a página do tipo de registro.
1. Clique em **Mais** menu ![](assets/more-menu.png) à direita do nome do tipo de registro e clique em **Excluir**. <!--add screen shot when they finalize the UI-->
1. Tipo **Excluir** na caixa de confirmação e clique em **Excluir permanentemente**.

   O tipo de registro selecionado, juntamente com seus campos, registros associados e exibições são excluídos.
