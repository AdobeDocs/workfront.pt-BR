---
title: Excluir campos
description: No Adobe Workfront Planning, é possível excluir campos personalizados que não são mais relevantes.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: 5c7b60ac5b78bd065ffc270588ec72ab3eb2f41d
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Delete fields
description: In Adobe Planning, you can delete custom fields that are no longer relevant.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# Excluir campos

{{planning-important-intro}}

No Adobe Workfront Planning, é possível criar campos personalizados para armazenar informações sobre registros.

Para obter informações sobre como criar campos personalizados no Workfront Planning, consulte [Criar campos](/help/quicksilver/planning/fields/create-fields.md).

É possível excluir campos do Workfront Planning que não são mais relevantes.

## Considerações sobre a exclusão de campos do Workfront Planning:

* É possível excluir um campo somente na exibição de tabela do tipo de registro.
* Não é possível excluir o campo principal de um registro.
* As informações armazenadas no campo são excluídas e não podem ser recuperadas.
* Quando você exclui um campo de registro vinculado, todos os campos de pesquisa vinculados também são excluídos do tipo de registro que você vincula. Os campos de registro vinculados dos tipos de registro vinculados não são excluídos.

  Para obter mais informações, consulte [Tipos de registro de conexão](/help/quicksilver/planning/architecture/connect-record-types.md).

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

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
   <td role="rowheader"><p>Configurações de nível de acesso</p></td>
   <td> <p>Não há controles de nível de acesso para o Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>O administrador do Workfront ou do grupo deve adicionar a área do Planning ao modelo de layout. Para obter informações, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Visão geral sobre acesso</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>Gerenciar permissões para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
</td>
  </tr>
 </tbody>
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Excluir campos

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos campos de registro você deseja deletar.

   O espaço de trabalho é aberto e os tipos de registro são exibidos.

1. Clique no cartão de um tipo de registro.

1. (Condicional) Se ainda não estiver selecionada, clique na guia de uma **exibição de Tabela** na página de tipo de registro.

   Todos os registros existentes associados ao tipo de registro são exibidos nas linhas da exibição de tabela.

1. Localize o campo que deseja excluir nos cabeçalhos da coluna, passe o mouse sobre o cabeçalho da coluna e clique na seta para baixo após o nome do campo.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Clique em **Excluir**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Clique em **Excluir** para confirmar.

   O campo é excluído, não pode ser recuperado e não pode mais ser associado a nenhum registro.
